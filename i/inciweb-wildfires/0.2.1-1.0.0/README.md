# Comparing `tmp/inciweb-wildfires-0.2.1.tar.gz` & `tmp/inciweb-wildfires-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inciweb-wildfires-0.2.1.tar", last modified: Sun Apr  2 10:54:46 2023, max compression
+gzip compressed data, was "inciweb-wildfires-1.0.0.tar", last modified: Fri Apr 12 10:19:37 2024, max compression
```

## Comparing `inciweb-wildfires-0.2.1.tar` & `inciweb-wildfires-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.447468 inciweb-wildfires-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.447468 inciweb-wildfires-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/.github/workflows/scrape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    46759 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.447468 inciweb-wildfires-0.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/data/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/data/timestamp.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.447468 inciweb-wildfires-0.2.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/_templates/nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/inciweb_wildfires/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/inciweb_wildfires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/inciweb_wildfires/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-02 10:54:46.000000 inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-02 10:54:46.451468 inciweb-wildfires-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-02 10:54:32.000000 inciweb-wildfires-0.2.1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.130078 inciweb-wildfires-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.github/workflows/scrape.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)    52150 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   110262 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/data/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/data/timestamp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.130078 inciweb-wildfires-1.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/_templates/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.134078 inciweb-wildfires-1.0.0/inciweb_wildfires/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/inciweb_wildfires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/inciweb_wildfires/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 10:19:37.000000 inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-12 10:19:37.138078 inciweb-wildfires-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 10:19:12.000000 inciweb-wildfires-1.0.0/test.py
```

### Comparing `inciweb-wildfires-0.2.1/.github/workflows/continuous-deployment.yml` & `inciweb-wildfires-1.0.0/.github/workflows/continuous-deployment.yml`

 * *Files 17% similar despite different names*

```diff
@@ -9,33 +9,62 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
       - name: Install pipenv
         run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
         shell: bash
 
       - id: pipenv-install
         name: Install Python dependencies
         run: pipenv sync --dev
 
       - id: run
         name: Run
         run: pipenv run flake8 inciweb_wildfires
 
+  mypy-python:
+    name: Static-types check
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+
+      - id: setup-python
+        name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+          cache: 'pipenv'
+
+      - id: install-pipenv
+        name: Install pipenv
+        run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
+        shell: bash
+
+      - id: install-python-dependencies
+        name: Install Python dependencies
+        run: pipenv sync --dev
+        shell: bash
+
+      - id: mypy
+        name: Run mypy
+        run: pipenv run mypy ./inciweb_wildfires --ignore-missing-imports --verbose
+        shell: bash
+
   test-python:
     strategy:
       matrix:
-        python: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python: ['3.8', '3.9', '3.10', '3.11']
     name: Test
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
@@ -63,15 +92,15 @@
     needs: [test-python]
     steps:
       - name: Checkout
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
       - name: Install pipenv
         run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
         shell: bash
 
       - id: pipenv-install
```

### Comparing `inciweb-wildfires-0.2.1/.github/workflows/docs.yml` & `inciweb-wildfires-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/.github/workflows/scrape.yml` & `inciweb-wildfires-1.0.0/.github/workflows/scrape.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     steps:
       - id: checkout
         name: Checkout
         uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: '3.9'
+          python-version: '3.10'
           cache: 'pipenv'
 
       - name: Install pipenv
         run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
         shell: bash
 
       - name: Run scrape command
```

### Comparing `inciweb-wildfires-0.2.1/.gitignore` & `inciweb-wildfires-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/.pre-commit-config.yaml` & `inciweb-wildfires-1.0.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
         args: ['--maxkb=10000']
     -   id: check-case-conflict
     -   id: mixed-line-ending
 
 -   repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 24.3.0
     hooks:
     -   id: black
 
 -   repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: 1.16.0
     hooks:
     -   id: blacken-docs
         additional_dependencies: [black]
 
 -   repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.13.2
     hooks:
     -   id: isort
         args: ["--profile", "black", "--filter-files"]
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.0.0
+    rev: 7.0.0
     hooks:
     - id: flake8
 
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
```

### Comparing `inciweb-wildfires-0.2.1/CODE_OF_CONDUCT.md` & `inciweb-wildfires-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/LICENSE` & `inciweb-wildfires-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/PKG-INFO` & `inciweb-wildfires-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inciweb-wildfires
-Version: 0.2.1
+Version: 1.0.0
 Summary: Download wildfire incidents data from InciWeb
 Home-page: http://www.github.com/datadesk/inciweb-wildfires
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/inciweb-wildfires
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: geojson
+Requires-Dist: click
 
 ### Links
 
 * Docs: [palewi.re/docs/inciweb-wildfires/](https://palewi.re/docs/inciweb-wildfires/)
 * Issues: [github.com/datadesk/inciweb-wildfires/issues](https://github.com/datadesk/inciweb-wildfires/issues)
 * Packaging: [pypi.python.org/pypi/inciweb-wildfires](https://pypi.python.org/pypi/inciweb-wildfires)
 * Testing: [github.com/datadesk/inciweb-wildfires/actions](https://github.com/datadesk/inciweb-wildfires/actions)
```

### Comparing `inciweb-wildfires-0.2.1/Pipfile.lock` & `inciweb-wildfires-1.0.0/Pipfile.lock`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8252933749257277%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'bccbc7eabc4a929b5563f4449b4afb86f460b30561e6ed0397c59eff69c00e31'}, 'requires': "*

 * *            "{'python_version': '3.10'}}",*

 * * "'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f', "*

 * *              "'sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1'], "*

 * *              '\'markers\': "python_version >= \'3.6\'", \'version\': \'==2024.2.2\'}, '*

 * *              "'charset […]*

```diff
@@ -1,833 +1,872 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "11cd5a8e003aac53f62e06d14b81ffa50c7b1d8c70dab2b5197970a957d184a2"
+            "sha256": "bccbc7eabc4a929b5563f4449b4afb86f460b30561e6ed0397c59eff69c00e31"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.9"
+            "python_version": "3.10"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "beautifulsoup4": {
-            "hashes": [
-                "sha256:0e79446b10b3ecb499c1556f7e228a53e64a2bfcebd455f370d8927cb5b59e39",
-                "sha256:bc4bdda6717de5a2987436fb8d72f45dc90dd856bdfd512a1314ce90349a0106"
-            ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==4.11.2"
-        },
-        "bs4": {
-            "hashes": [
-                "sha256:36ecea1fd7cc5c0c6e4a1ff075df26d50da647b75376626cc186e2212886dd3a"
-            ],
-            "index": "pypi",
-            "version": "==0.0.1"
-        },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==2022.12.7"
+            "markers": "python_version >= '3.6'",
+            "version": "==2024.2.2"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
-                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
+                "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
+                "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
+                "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
+                "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
+                "sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09",
+                "sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185",
+                "sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574",
+                "sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e",
+                "sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519",
+                "sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898",
+                "sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269",
+                "sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3",
+                "sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f",
+                "sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6",
+                "sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8",
+                "sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a",
+                "sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73",
+                "sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc",
+                "sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714",
+                "sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2",
+                "sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc",
+                "sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce",
+                "sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d",
+                "sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e",
+                "sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6",
+                "sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269",
+                "sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96",
+                "sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d",
+                "sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a",
+                "sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4",
+                "sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77",
+                "sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d",
+                "sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0",
+                "sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed",
+                "sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068",
+                "sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac",
+                "sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25",
+                "sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8",
+                "sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab",
+                "sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26",
+                "sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2",
+                "sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db",
+                "sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f",
+                "sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5",
+                "sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99",
+                "sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c",
+                "sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d",
+                "sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811",
+                "sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa",
+                "sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a",
+                "sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03",
+                "sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b",
+                "sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04",
+                "sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c",
+                "sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001",
+                "sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458",
+                "sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389",
+                "sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99",
+                "sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985",
+                "sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537",
+                "sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238",
+                "sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f",
+                "sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d",
+                "sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796",
+                "sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a",
+                "sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143",
+                "sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8",
+                "sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c",
+                "sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5",
+                "sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5",
+                "sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711",
+                "sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4",
+                "sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6",
+                "sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c",
+                "sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7",
+                "sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4",
+                "sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b",
+                "sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae",
+                "sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12",
+                "sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c",
+                "sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae",
+                "sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8",
+                "sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887",
+                "sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b",
+                "sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4",
+                "sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f",
+                "sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5",
+                "sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33",
+                "sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519",
+                "sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.3.2"
         },
         "click": {
             "hashes": [
-                "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
-                "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
+                "sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28",
+                "sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de"
             ],
             "index": "pypi",
-            "version": "==8.1.3"
+            "markers": "python_version >= '3.7'",
+            "version": "==8.1.7"
         },
         "geojson": {
             "hashes": [
-                "sha256:6e4bb7ace4226a45d9c8c8b1348b3fc43540658359f93c3f7e03efa9f15f658a",
-                "sha256:ccbd13368dd728f4e4f13ffe6aaf725b6e802c692ba0dde628be475040c534ba"
+                "sha256:58a7fa40727ea058efc28b0e9ff0099eadf6d0965e04690830208d3ef571adac",
+                "sha256:68a9771827237adb8c0c71f8527509c8f5bef61733aa434cefc9c9d4f0ebe8f3"
             ],
             "index": "pypi",
-            "version": "==2.5.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.0"
         },
         "idna": {
             "hashes": [
-                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
-                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.4"
-        },
-        "lxml": {
-            "hashes": [
-                "sha256:01d36c05f4afb8f7c20fd9ed5badca32a2029b93b1750f571ccc0b142531caf7",
-                "sha256:04876580c050a8c5341d706dd464ff04fd597095cc8c023252566a8826505726",
-                "sha256:05ca3f6abf5cf78fe053da9b1166e062ade3fa5d4f92b4ed688127ea7d7b1d03",
-                "sha256:090c6543d3696cbe15b4ac6e175e576bcc3f1ccfbba970061b7300b0c15a2140",
-                "sha256:0dc313ef231edf866912e9d8f5a042ddab56c752619e92dfd3a2c277e6a7299a",
-                "sha256:0f2b1e0d79180f344ff9f321327b005ca043a50ece8713de61d1cb383fb8ac05",
-                "sha256:13598ecfbd2e86ea7ae45ec28a2a54fb87ee9b9fdb0f6d343297d8e548392c03",
-                "sha256:16efd54337136e8cd72fb9485c368d91d77a47ee2d42b057564aae201257d419",
-                "sha256:1ab8f1f932e8f82355e75dda5413a57612c6ea448069d4fb2e217e9a4bed13d4",
-                "sha256:223f4232855ade399bd409331e6ca70fb5578efef22cf4069a6090acc0f53c0e",
-                "sha256:2455cfaeb7ac70338b3257f41e21f0724f4b5b0c0e7702da67ee6c3640835b67",
-                "sha256:2899456259589aa38bfb018c364d6ae7b53c5c22d8e27d0ec7609c2a1ff78b50",
-                "sha256:2a29ba94d065945944016b6b74e538bdb1751a1db6ffb80c9d3c2e40d6fa9894",
-                "sha256:2a87fa548561d2f4643c99cd13131acb607ddabb70682dcf1dff5f71f781a4bf",
-                "sha256:2e430cd2824f05f2d4f687701144556646bae8f249fd60aa1e4c768ba7018947",
-                "sha256:36c3c175d34652a35475a73762b545f4527aec044910a651d2bf50de9c3352b1",
-                "sha256:3818b8e2c4b5148567e1b09ce739006acfaa44ce3156f8cbbc11062994b8e8dd",
-                "sha256:3ab9fa9d6dc2a7f29d7affdf3edebf6ece6fb28a6d80b14c3b2fb9d39b9322c3",
-                "sha256:3efea981d956a6f7173b4659849f55081867cf897e719f57383698af6f618a92",
-                "sha256:4c8f293f14abc8fd3e8e01c5bd86e6ed0b6ef71936ded5bf10fe7a5efefbaca3",
-                "sha256:5344a43228767f53a9df6e5b253f8cdca7dfc7b7aeae52551958192f56d98457",
-                "sha256:58bfa3aa19ca4c0f28c5dde0ff56c520fbac6f0daf4fac66ed4c8d2fb7f22e74",
-                "sha256:5b4545b8a40478183ac06c073e81a5ce4cf01bf1734962577cf2bb569a5b3bbf",
-                "sha256:5f50a1c177e2fa3ee0667a5ab79fdc6b23086bc8b589d90b93b4bd17eb0e64d1",
-                "sha256:63da2ccc0857c311d764e7d3d90f429c252e83b52d1f8f1d1fe55be26827d1f4",
-                "sha256:6749649eecd6a9871cae297bffa4ee76f90b4504a2a2ab528d9ebe912b101975",
-                "sha256:6804daeb7ef69e7b36f76caddb85cccd63d0c56dedb47555d2fc969e2af6a1a5",
-                "sha256:689bb688a1db722485e4610a503e3e9210dcc20c520b45ac8f7533c837be76fe",
-                "sha256:699a9af7dffaf67deeae27b2112aa06b41c370d5e7633e0ee0aea2e0b6c211f7",
-                "sha256:6b418afe5df18233fc6b6093deb82a32895b6bb0b1155c2cdb05203f583053f1",
-                "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2",
-                "sha256:7b515674acfdcadb0eb5d00d8a709868173acece5cb0be3dd165950cbfdf5409",
-                "sha256:7b770ed79542ed52c519119473898198761d78beb24b107acf3ad65deae61f1f",
-                "sha256:7d2278d59425777cfcb19735018d897ca8303abe67cc735f9f97177ceff8027f",
-                "sha256:7e91ee82f4199af8c43d8158024cbdff3d931df350252288f0d4ce656df7f3b5",
-                "sha256:821b7f59b99551c69c85a6039c65b75f5683bdc63270fec660f75da67469ca24",
-                "sha256:822068f85e12a6e292803e112ab876bc03ed1f03dddb80154c395f891ca6b31e",
-                "sha256:8340225bd5e7a701c0fa98284c849c9b9fc9238abf53a0ebd90900f25d39a4e4",
-                "sha256:85cabf64adec449132e55616e7ca3e1000ab449d1d0f9d7f83146ed5bdcb6d8a",
-                "sha256:880bbbcbe2fca64e2f4d8e04db47bcdf504936fa2b33933efd945e1b429bea8c",
-                "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de",
-                "sha256:8e20cb5a47247e383cf4ff523205060991021233ebd6f924bca927fcf25cf86f",
-                "sha256:925073b2fe14ab9b87e73f9a5fde6ce6392da430f3004d8b72cc86f746f5163b",
-                "sha256:998c7c41910666d2976928c38ea96a70d1aa43be6fe502f21a651e17483a43c5",
-                "sha256:9b22c5c66f67ae00c0199f6055705bc3eb3fcb08d03d2ec4059a2b1b25ed48d7",
-                "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a",
-                "sha256:a08cff61517ee26cb56f1e949cca38caabe9ea9fbb4b1e10a805dc39844b7d5c",
-                "sha256:a0a336d6d3e8b234a3aae3c674873d8f0e720b76bc1d9416866c41cd9500ffb9",
-                "sha256:a35f8b7fa99f90dd2f5dc5a9fa12332642f087a7641289ca6c40d6e1a2637d8e",
-                "sha256:a38486985ca49cfa574a507e7a2215c0c780fd1778bb6290c21193b7211702ab",
-                "sha256:a5da296eb617d18e497bcf0a5c528f5d3b18dadb3619fbdadf4ed2356ef8d941",
-                "sha256:a6e441a86553c310258aca15d1c05903aaf4965b23f3bc2d55f200804e005ee5",
-                "sha256:a82d05da00a58b8e4c0008edbc8a4b6ec5a4bc1e2ee0fb6ed157cf634ed7fa45",
-                "sha256:ab323679b8b3030000f2be63e22cdeea5b47ee0abd2d6a1dc0c8103ddaa56cd7",
-                "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892",
-                "sha256:b23e19989c355ca854276178a0463951a653309fb8e57ce674497f2d9f208746",
-                "sha256:b264171e3143d842ded311b7dccd46ff9ef34247129ff5bf5066123c55c2431c",
-                "sha256:b26a29f0b7fc6f0897f043ca366142d2b609dc60756ee6e4e90b5f762c6adc53",
-                "sha256:b64d891da92e232c36976c80ed7ebb383e3f148489796d8d31a5b6a677825efe",
-                "sha256:b9cc34af337a97d470040f99ba4282f6e6bac88407d021688a5d585e44a23184",
-                "sha256:bc718cd47b765e790eecb74d044cc8d37d58562f6c314ee9484df26276d36a38",
-                "sha256:be7292c55101e22f2a3d4d8913944cbea71eea90792bf914add27454a13905df",
-                "sha256:c83203addf554215463b59f6399835201999b5e48019dc17f182ed5ad87205c9",
-                "sha256:c9ec3eaf616d67db0764b3bb983962b4f385a1f08304fd30c7283954e6a7869b",
-                "sha256:ca34efc80a29351897e18888c71c6aca4a359247c87e0b1c7ada14f0ab0c0fb2",
-                "sha256:ca989b91cf3a3ba28930a9fc1e9aeafc2a395448641df1f387a2d394638943b0",
-                "sha256:d02a5399126a53492415d4906ab0ad0375a5456cc05c3fc0fc4ca11771745cda",
-                "sha256:d17bc7c2ccf49c478c5bdd447594e82692c74222698cfc9b5daae7ae7e90743b",
-                "sha256:d5bf6545cd27aaa8a13033ce56354ed9e25ab0e4ac3b5392b763d8d04b08e0c5",
-                "sha256:d6b430a9938a5a5d85fc107d852262ddcd48602c120e3dbb02137c83d212b380",
-                "sha256:da248f93f0418a9e9d94b0080d7ebc407a9a5e6d0b57bb30db9b5cc28de1ad33",
-                "sha256:da4dd7c9c50c059aba52b3524f84d7de956f7fef88f0bafcf4ad7dde94a064e8",
-                "sha256:df0623dcf9668ad0445e0558a21211d4e9a149ea8f5666917c8eeec515f0a6d1",
-                "sha256:e5168986b90a8d1f2f9dc1b841467c74221bd752537b99761a93d2d981e04889",
-                "sha256:efa29c2fe6b4fdd32e8ef81c1528506895eca86e1d8c4657fda04c9b3786ddf9",
-                "sha256:f1496ea22ca2c830cbcbd473de8f114a320da308438ae65abad6bab7867fe38f",
-                "sha256:f49e52d174375a7def9915c9f06ec4e569d235ad428f70751765f48d5926678c"
-            ],
-            "index": "pypi",
-            "version": "==4.9.2"
+            "version": "==3.7"
         },
         "requests": {
             "hashes": [
-                "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
-                "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.28.1"
-        },
-        "soupsieve": {
-            "hashes": [
-                "sha256:3b2503d3c7084a42b1ebd08116e5f81aadfaea95863628c80a3b774a11b7c759",
-                "sha256:fc53893b3da2c33de295667a0e19f078c14bf86544af307354de5fcf12a3f30d"
-            ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.3.2.post1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.2.1"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
-                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
-                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
+                "sha256:75a8b99c28a5dad50dd7f8ccdd447a121ddb3892da9e53d1ca5cca3106d58d65",
+                "sha256:b46733c07dce03ae4e150330b975c75737fa60f0a7c591b6c8bf4928a28e2c92"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.7.13"
+            "markers": "python_version >= '3.9'",
+            "version": "==0.7.16"
         },
         "babel": {
             "hashes": [
-                "sha256:1ad3eca1c885218f6dce2ab67291178944f810a10a9b5f3cb8382a5a232b64fe",
-                "sha256:5ef4b3226b0180dedded4229651c8b0e1a3a6a2837d45a073272f313e4cf97f6"
+                "sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363",
+                "sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.11.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.14.0"
         },
-        "bleach": {
+        "backports.tarfile": {
             "hashes": [
-                "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
-                "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
+                "sha256:2688f159c21afd56a07b75f01306f9f52c79aebcc5f4a117fb8fbb4445352c75",
+                "sha256:bcd36290d9684beb524d3fe74f4a2db056824c47746583f090b8e55daf0776e4"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==6.0.0"
+            "markers": "python_version < '3.12'",
+            "version": "==1.0.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
-            ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==2022.12.7"
-        },
-        "cffi": {
-            "hashes": [
-                "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
-                "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
-                "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
-                "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
-                "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405",
-                "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375",
-                "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a",
-                "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e",
-                "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc",
-                "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf",
-                "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185",
-                "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497",
-                "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3",
-                "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35",
-                "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c",
-                "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83",
-                "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21",
-                "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca",
-                "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984",
-                "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac",
-                "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd",
-                "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee",
-                "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a",
-                "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2",
-                "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192",
-                "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7",
-                "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585",
-                "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f",
-                "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e",
-                "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27",
-                "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b",
-                "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e",
-                "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e",
-                "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d",
-                "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c",
-                "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415",
-                "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82",
-                "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02",
-                "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314",
-                "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325",
-                "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c",
-                "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3",
-                "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914",
-                "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045",
-                "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d",
-                "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9",
-                "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5",
-                "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2",
-                "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c",
-                "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3",
-                "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2",
-                "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8",
-                "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d",
-                "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d",
-                "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9",
-                "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162",
-                "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76",
-                "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4",
-                "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e",
-                "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9",
-                "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6",
-                "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b",
-                "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01",
-                "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"
+                "sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f",
+                "sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1"
             ],
-            "version": "==1.15.1"
+            "markers": "python_version >= '3.6'",
+            "version": "==2024.2.2"
         },
         "cfgv": {
             "hashes": [
-                "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
-                "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
+                "sha256:b7265b1f29fd3316bfcd2b330d63d024f2bfd8bcb8b0272f8e19a504856c48f9",
+                "sha256:e52591d4c5f5dead8e0f673fb16db7949d2cfb3f7da4582893288f0ded8fe560"
             ],
-            "markers": "python_full_version >= '3.6.1'",
-            "version": "==3.3.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.4.0"
         },
         "charset-normalizer": {
             "hashes": [
-                "sha256:5a3d016c7c547f69d6f81fb0db9449ce888b418b5b9952cc5e6e66843e9dd845",
-                "sha256:83e9a75d1911279afd89352c68b45348559d1fc0506b054b346651b5e7fee29f"
+                "sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027",
+                "sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087",
+                "sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786",
+                "sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8",
+                "sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09",
+                "sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185",
+                "sha256:1ceae2f17a9c33cb48e3263960dc5fc8005351ee19db217e9b1bb15d28c02574",
+                "sha256:1d3193f4a680c64b4b6a9115943538edb896edc190f0b222e73761716519268e",
+                "sha256:1f79682fbe303db92bc2b1136016a38a42e835d932bab5b3b1bfcfbf0640e519",
+                "sha256:2127566c664442652f024c837091890cb1942c30937add288223dc895793f898",
+                "sha256:22afcb9f253dac0696b5a4be4a1c0f8762f8239e21b99680099abd9b2b1b2269",
+                "sha256:25baf083bf6f6b341f4121c2f3c548875ee6f5339300e08be3f2b2ba1721cdd3",
+                "sha256:2e81c7b9c8979ce92ed306c249d46894776a909505d8f5a4ba55b14206e3222f",
+                "sha256:3287761bc4ee9e33561a7e058c72ac0938c4f57fe49a09eae428fd88aafe7bb6",
+                "sha256:34d1c8da1e78d2e001f363791c98a272bb734000fcef47a491c1e3b0505657a8",
+                "sha256:37e55c8e51c236f95b033f6fb391d7d7970ba5fe7ff453dad675e88cf303377a",
+                "sha256:3d47fa203a7bd9c5b6cee4736ee84ca03b8ef23193c0d1ca99b5089f72645c73",
+                "sha256:3e4d1f6587322d2788836a99c69062fbb091331ec940e02d12d179c1d53e25fc",
+                "sha256:42cb296636fcc8b0644486d15c12376cb9fa75443e00fb25de0b8602e64c1714",
+                "sha256:45485e01ff4d3630ec0d9617310448a8702f70e9c01906b0d0118bdf9d124cf2",
+                "sha256:4a78b2b446bd7c934f5dcedc588903fb2f5eec172f3d29e52a9096a43722adfc",
+                "sha256:4ab2fe47fae9e0f9dee8c04187ce5d09f48eabe611be8259444906793ab7cbce",
+                "sha256:4d0d1650369165a14e14e1e47b372cfcb31d6ab44e6e33cb2d4e57265290044d",
+                "sha256:549a3a73da901d5bc3ce8d24e0600d1fa85524c10287f6004fbab87672bf3e1e",
+                "sha256:55086ee1064215781fff39a1af09518bc9255b50d6333f2e4c74ca09fac6a8f6",
+                "sha256:572c3763a264ba47b3cf708a44ce965d98555f618ca42c926a9c1616d8f34269",
+                "sha256:573f6eac48f4769d667c4442081b1794f52919e7edada77495aaed9236d13a96",
+                "sha256:5b4c145409bef602a690e7cfad0a15a55c13320ff7a3ad7ca59c13bb8ba4d45d",
+                "sha256:6463effa3186ea09411d50efc7d85360b38d5f09b870c48e4600f63af490e56a",
+                "sha256:65f6f63034100ead094b8744b3b97965785388f308a64cf8d7c34f2f2e5be0c4",
+                "sha256:663946639d296df6a2bb2aa51b60a2454ca1cb29835324c640dafb5ff2131a77",
+                "sha256:6897af51655e3691ff853668779c7bad41579facacf5fd7253b0133308cf000d",
+                "sha256:68d1f8a9e9e37c1223b656399be5d6b448dea850bed7d0f87a8311f1ff3dabb0",
+                "sha256:6ac7ffc7ad6d040517be39eb591cac5ff87416c2537df6ba3cba3bae290c0fed",
+                "sha256:6b3251890fff30ee142c44144871185dbe13b11bab478a88887a639655be1068",
+                "sha256:6c4caeef8fa63d06bd437cd4bdcf3ffefe6738fb1b25951440d80dc7df8c03ac",
+                "sha256:6ef1d82a3af9d3eecdba2321dc1b3c238245d890843e040e41e470ffa64c3e25",
+                "sha256:753f10e867343b4511128c6ed8c82f7bec3bd026875576dfd88483c5c73b2fd8",
+                "sha256:7cd13a2e3ddeed6913a65e66e94b51d80a041145a026c27e6bb76c31a853c6ab",
+                "sha256:7ed9e526742851e8d5cc9e6cf41427dfc6068d4f5a3bb03659444b4cabf6bc26",
+                "sha256:7f04c839ed0b6b98b1a7501a002144b76c18fb1c1850c8b98d458ac269e26ed2",
+                "sha256:802fe99cca7457642125a8a88a084cef28ff0cf9407060f7b93dca5aa25480db",
+                "sha256:80402cd6ee291dcb72644d6eac93785fe2c8b9cb30893c1af5b8fdd753b9d40f",
+                "sha256:8465322196c8b4d7ab6d1e049e4c5cb460d0394da4a27d23cc242fbf0034b6b5",
+                "sha256:86216b5cee4b06df986d214f664305142d9c76df9b6512be2738aa72a2048f99",
+                "sha256:87d1351268731db79e0f8e745d92493ee2841c974128ef629dc518b937d9194c",
+                "sha256:8bdb58ff7ba23002a4c5808d608e4e6c687175724f54a5dade5fa8c67b604e4d",
+                "sha256:8c622a5fe39a48f78944a87d4fb8a53ee07344641b0562c540d840748571b811",
+                "sha256:8d756e44e94489e49571086ef83b2bb8ce311e730092d2c34ca8f7d925cb20aa",
+                "sha256:8f4a014bc36d3c57402e2977dada34f9c12300af536839dc38c0beab8878f38a",
+                "sha256:9063e24fdb1e498ab71cb7419e24622516c4a04476b17a2dab57e8baa30d6e03",
+                "sha256:90d558489962fd4918143277a773316e56c72da56ec7aa3dc3dbbe20fdfed15b",
+                "sha256:923c0c831b7cfcb071580d3f46c4baf50f174be571576556269530f4bbd79d04",
+                "sha256:95f2a5796329323b8f0512e09dbb7a1860c46a39da62ecb2324f116fa8fdc85c",
+                "sha256:96b02a3dc4381e5494fad39be677abcb5e6634bf7b4fa83a6dd3112607547001",
+                "sha256:9f96df6923e21816da7e0ad3fd47dd8f94b2a5ce594e00677c0013018b813458",
+                "sha256:a10af20b82360ab00827f916a6058451b723b4e65030c5a18577c8b2de5b3389",
+                "sha256:a50aebfa173e157099939b17f18600f72f84eed3049e743b68ad15bd69b6bf99",
+                "sha256:a981a536974bbc7a512cf44ed14938cf01030a99e9b3a06dd59578882f06f985",
+                "sha256:a9a8e9031d613fd2009c182b69c7b2c1ef8239a0efb1df3f7c8da66d5dd3d537",
+                "sha256:ae5f4161f18c61806f411a13b0310bea87f987c7d2ecdbdaad0e94eb2e404238",
+                "sha256:aed38f6e4fb3f5d6bf81bfa990a07806be9d83cf7bacef998ab1a9bd660a581f",
+                "sha256:b01b88d45a6fcb69667cd6d2f7a9aeb4bf53760d7fc536bf679ec94fe9f3ff3d",
+                "sha256:b261ccdec7821281dade748d088bb6e9b69e6d15b30652b74cbbac25e280b796",
+                "sha256:b2b0a0c0517616b6869869f8c581d4eb2dd83a4d79e0ebcb7d373ef9956aeb0a",
+                "sha256:b4a23f61ce87adf89be746c8a8974fe1c823c891d8f86eb218bb957c924bb143",
+                "sha256:bd8f7df7d12c2db9fab40bdd87a7c09b1530128315d047a086fa3ae3435cb3a8",
+                "sha256:beb58fe5cdb101e3a055192ac291b7a21e3b7ef4f67fa1d74e331a7f2124341c",
+                "sha256:c002b4ffc0be611f0d9da932eb0f704fe2602a9a949d1f738e4c34c75b0863d5",
+                "sha256:c083af607d2515612056a31f0a8d9e0fcb5876b7bfc0abad3ecd275bc4ebc2d5",
+                "sha256:c180f51afb394e165eafe4ac2936a14bee3eb10debc9d9e4db8958fe36afe711",
+                "sha256:c235ebd9baae02f1b77bcea61bce332cb4331dc3617d254df3323aa01ab47bd4",
+                "sha256:cd70574b12bb8a4d2aaa0094515df2463cb429d8536cfb6c7ce983246983e5a6",
+                "sha256:d0eccceffcb53201b5bfebb52600a5fb483a20b61da9dbc885f8b103cbe7598c",
+                "sha256:d965bba47ddeec8cd560687584e88cf699fd28f192ceb452d1d7ee807c5597b7",
+                "sha256:db364eca23f876da6f9e16c9da0df51aa4f104a972735574842618b8c6d999d4",
+                "sha256:ddbb2551d7e0102e7252db79ba445cdab71b26640817ab1e3e3648dad515003b",
+                "sha256:deb6be0ac38ece9ba87dea880e438f25ca3eddfac8b002a2ec3d9183a454e8ae",
+                "sha256:e06ed3eb3218bc64786f7db41917d4e686cc4856944f53d5bdf83a6884432e12",
+                "sha256:e27ad930a842b4c5eb8ac0016b0a54f5aebbe679340c26101df33424142c143c",
+                "sha256:e537484df0d8f426ce2afb2d0f8e1c3d0b114b83f8850e5f2fbea0e797bd82ae",
+                "sha256:eb00ed941194665c332bf8e078baf037d6c35d7c4f3102ea2d4f16ca94a26dc8",
+                "sha256:eb6904c354526e758fda7167b33005998fb68c46fbc10e013ca97f21ca5c8887",
+                "sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b",
+                "sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4",
+                "sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f",
+                "sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5",
+                "sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33",
+                "sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519",
+                "sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561"
             ],
-            "markers": "python_full_version >= '3.6.0'",
-            "version": "==2.1.1"
-        },
-        "cryptography": {
-            "hashes": [
-                "sha256:0f8da300b5c8af9f98111ffd512910bc792b4c77392a9523624680f7956a99d4",
-                "sha256:35f7c7d015d474f4011e859e93e789c87d21f6f4880ebdc29896a60403328f1f",
-                "sha256:5aa67414fcdfa22cf052e640cb5ddc461924a045cacf325cd164e65312d99502",
-                "sha256:5d2d8b87a490bfcd407ed9d49093793d0f75198a35e6eb1a923ce1ee86c62b41",
-                "sha256:6687ef6d0a6497e2b58e7c5b852b53f62142cfa7cd1555795758934da363a965",
-                "sha256:6f8ba7f0328b79f08bdacc3e4e66fb4d7aab0c3584e0bd41328dce5262e26b2e",
-                "sha256:706843b48f9a3f9b9911979761c91541e3d90db1ca905fd63fee540a217698bc",
-                "sha256:807ce09d4434881ca3a7594733669bd834f5b2c6d5c7e36f8c00f691887042ad",
-                "sha256:83e17b26de248c33f3acffb922748151d71827d6021d98c70e6c1a25ddd78505",
-                "sha256:96f1157a7c08b5b189b16b47bc9db2332269d6680a196341bf30046330d15388",
-                "sha256:aec5a6c9864be7df2240c382740fcf3b96928c46604eaa7f3091f58b878c0bb6",
-                "sha256:b0afd054cd42f3d213bf82c629efb1ee5f22eba35bf0eec88ea9ea7304f511a2",
-                "sha256:ced4e447ae29ca194449a3f1ce132ded8fcab06971ef5f618605aacaa612beac",
-                "sha256:d1f6198ee6d9148405e49887803907fe8962a23e6c6f83ea7d98f1c0de375695",
-                "sha256:e124352fd3db36a9d4a21c1aa27fd5d051e621845cb87fb851c08f4f75ce8be6",
-                "sha256:e422abdec8b5fa8462aa016786680720d78bdce7a30c652b7fadf83a4ba35336",
-                "sha256:ef8b72fa70b348724ff1218267e7f7375b8de4e8194d1636ee60510aae104cd0",
-                "sha256:f0c64d1bd842ca2633e74a1a28033d139368ad959872533b1bab8c80e8240a0c",
-                "sha256:f24077a3b5298a5a06a8e0536e3ea9ec60e4c7ac486755e5fb6e6ea9b3500106",
-                "sha256:fdd188c8a6ef8769f148f88f859884507b954cc64db6b52f66ef199bb9ad660a",
-                "sha256:fe913f20024eb2cb2f323e42a64bdf2911bb9738a15dba7d3cce48151034e3a8"
-            ],
-            "index": "pypi",
-            "version": "==39.0.1"
+            "markers": "python_full_version >= '3.7.0'",
+            "version": "==3.3.2"
         },
         "distlib": {
             "hashes": [
-                "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
-                "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
+                "sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784",
+                "sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64"
             ],
-            "version": "==0.3.6"
+            "version": "==0.3.8"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6",
+                "sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==0.19"
+            "markers": "python_version >= '3.7'",
+            "version": "==0.20.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:7b319f24340b51f55a2bf7a12ac0755a9b03e718311dac567a0f4f7fabd2f5de",
-                "sha256:f58d535af89bb9ad5cd4df046f741f8553a418c01a7856bf0d173bbc9f6bd16d"
+                "sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f",
+                "sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.9.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.13.4"
         },
         "flake8": {
             "hashes": [
-                "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
-                "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
+                "sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132",
+                "sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3"
             ],
             "index": "pypi",
-            "version": "==6.0.0"
+            "markers": "python_full_version >= '3.8.1'",
+            "version": "==7.0.0"
         },
         "identify": {
             "hashes": [
-                "sha256:7d526dd1283555aafcc91539acc061d8f6f59adb0a7bba462735b0a318bff7ed",
-                "sha256:93cc61a861052de9d4c541a7acb7e3dcc9c11b398a2144f6e52ae5285f5f4f06"
+                "sha256:10a7ca245cfcd756a554a7288159f72ff105ad233c7c4b9c6f0f4d108f5f6791",
+                "sha256:c4de0081837b211594f8e877a6b4fad7ca32bbfc1a9307fdd61c28bfe923f13e"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==2.5.17"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.5.35"
         },
         "idna": {
             "hashes": [
-                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
-                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
+                "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc",
+                "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"
             ],
             "markers": "python_version >= '3.5'",
-            "version": "==3.4"
+            "version": "==3.7"
         },
         "imagesize": {
             "hashes": [
                 "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:7efb448ec9a5e313a57655d35aa54cd3e01b7e1fbcf72dce1bf06119420f5bad",
-                "sha256:e354bedeb60efa6affdcc8ae121b73544a7aa74156d047311948f6d711cd378d"
+                "sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570",
+                "sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==6.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==7.1.0"
         },
         "jaraco.classes": {
             "hashes": [
-                "sha256:2353de3288bc6b82120752201c6b1c1a14b058267fa424ed5ce5984e3b922158",
-                "sha256:89559fa5c1d3c34eff6f631ad80bb21f378dbcbb35dd161fd2c6b93f5be2f98a"
+                "sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd",
+                "sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.2.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.4.0"
+        },
+        "jaraco.context": {
+            "hashes": [
+                "sha256:3e16388f7da43d384a1a7cd3452e72e14732ac9fe459678773a3608a812bf266",
+                "sha256:c2f67165ce1f9be20f32f650f25d8edfc1646a8aeee48ae06fb35f90763576d2"
+            ],
+            "markers": "python_version >= '3.8'",
+            "version": "==5.3.0"
         },
-        "jeepney": {
+        "jaraco.functools": {
             "hashes": [
-                "sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806",
-                "sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755"
+                "sha256:c279cb24c93d694ef7270f970d499cab4d3813f4e08273f95398651a634f0925",
+                "sha256:daf276ddf234bea897ef14f43c4e1bf9eefeac7b7a82a4dd69228ac20acff68d"
             ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==0.8.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.0.0"
         },
         "jinja2": {
             "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
+                "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa",
+                "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.1.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.1.3"
         },
         "keyring": {
             "hashes": [
-                "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
-                "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
+                "sha256:26fc12e6a329d61d24aa47b22a7c5c3f35753df7d8f2860973cf94f4e1fb3427",
+                "sha256:7230ea690525133f6ad536a9b5def74a4bd52642abe594761028fc044d7c7893"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==23.13.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==25.1.0"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27",
-                "sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==2.1.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf",
+                "sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff",
+                "sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f",
+                "sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3",
+                "sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532",
+                "sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f",
+                "sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617",
+                "sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df",
+                "sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4",
+                "sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906",
+                "sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f",
+                "sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4",
+                "sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8",
+                "sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371",
+                "sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2",
+                "sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465",
+                "sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52",
+                "sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6",
+                "sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169",
+                "sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad",
+                "sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2",
+                "sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0",
+                "sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029",
+                "sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f",
+                "sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a",
+                "sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced",
+                "sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5",
+                "sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c",
+                "sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf",
+                "sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9",
+                "sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb",
+                "sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad",
+                "sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3",
+                "sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1",
+                "sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46",
+                "sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc",
+                "sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a",
+                "sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee",
+                "sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900",
+                "sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5",
+                "sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea",
+                "sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f",
+                "sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5",
+                "sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e",
+                "sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a",
+                "sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f",
+                "sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50",
+                "sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a",
+                "sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b",
+                "sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4",
+                "sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff",
+                "sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2",
+                "sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46",
+                "sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b",
+                "sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf",
+                "sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5",
+                "sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5",
+                "sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab",
+                "sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd",
+                "sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==2.1.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.1.5"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "more-itertools": {
             "hashes": [
-                "sha256:250e83d7e81d0c87ca6bd942e6aeab8cc9daa6096d12c5308f3f92fa5e5c1f41",
-                "sha256:5a6257e40878ef0520b1803990e3e22303a41b5714006c32a3fd8304b26ea1ab"
+                "sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684",
+                "sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==9.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==10.2.0"
+        },
+        "mypy": {
+            "hashes": [
+                "sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6",
+                "sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913",
+                "sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129",
+                "sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc",
+                "sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974",
+                "sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374",
+                "sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150",
+                "sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03",
+                "sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9",
+                "sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02",
+                "sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89",
+                "sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2",
+                "sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d",
+                "sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3",
+                "sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612",
+                "sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e",
+                "sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3",
+                "sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e",
+                "sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd",
+                "sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04",
+                "sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed",
+                "sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185",
+                "sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf",
+                "sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b",
+                "sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4",
+                "sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f",
+                "sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==1.9.0"
+        },
+        "mypy-extensions": {
+            "hashes": [
+                "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
+                "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==1.0.0"
+        },
+        "nh3": {
+            "hashes": [
+                "sha256:0316c25b76289cf23be6b66c77d3608a4fdf537b35426280032f432f14291b9a",
+                "sha256:1a814dd7bba1cb0aba5bcb9bebcc88fd801b63e21e2450ae6c52d3b3336bc911",
+                "sha256:1aa52a7def528297f256de0844e8dd680ee279e79583c76d6fa73a978186ddfb",
+                "sha256:22c26e20acbb253a5bdd33d432a326d18508a910e4dcf9a3316179860d53345a",
+                "sha256:40015514022af31975c0b3bca4014634fa13cb5dc4dbcbc00570acc781316dcc",
+                "sha256:40d0741a19c3d645e54efba71cb0d8c475b59135c1e3c580f879ad5514cbf028",
+                "sha256:551672fd71d06cd828e282abdb810d1be24e1abb7ae2543a8fa36a71c1006fe9",
+                "sha256:66f17d78826096291bd264f260213d2b3905e3c7fae6dfc5337d49429f1dc9f3",
+                "sha256:85cdbcca8ef10733bd31f931956f7fbb85145a4d11ab9e6742bbf44d88b7e351",
+                "sha256:a3f55fabe29164ba6026b5ad5c3151c314d136fd67415a17660b4aaddacf1b10",
+                "sha256:b4427ef0d2dfdec10b641ed0bdaf17957eb625b2ec0ea9329b3d28806c153d71",
+                "sha256:ba73a2f8d3a1b966e9cdba7b211779ad8a2561d2dba9674b8a19ed817923f65f",
+                "sha256:c21bac1a7245cbd88c0b0e4a420221b7bfa838a2814ee5bb924e9c2f10a1120b",
+                "sha256:c551eb2a3876e8ff2ac63dff1585236ed5dfec5ffd82216a7a174f7c5082a78a",
+                "sha256:c790769152308421283679a142dbdb3d1c46c79c823008ecea8e8141db1a2062",
+                "sha256:d7a25fd8c86657f5d9d576268e3b3767c5cd4f42867c9383618be8517f0f022a"
+            ],
+            "version": "==0.2.17"
         },
         "nodeenv": {
             "hashes": [
-                "sha256:27083a7b96a25f2f5e1d8cb4b6317ee8aeda3bdd121394e5ac54e498028a042e",
-                "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
+                "sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2",
+                "sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==1.7.0"
+            "version": "==1.8.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
+                "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==23.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==24.0"
         },
         "pkginfo": {
             "hashes": [
-                "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
-                "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
+                "sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297",
+                "sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==1.9.6"
+            "version": "==1.10.0"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9",
-                "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"
+                "sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068",
+                "sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.0.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.2.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:51a5ba7c480ae8072ecdb6933df22d2f812dc897d5fe848778116129a681aac7",
-                "sha256:a978dac7bc9ec0bcee55c18a277d553b0f419d259dadb4b9418ff2d00eb43959"
+                "sha256:5eae9e10c2b5ac51577c3452ec0a490455c45a0533f7960f993a0d01e59decab",
+                "sha256:e209d61b8acdcf742404408531f0c37d49d2c734fd7cff2d6076083d191cb060"
             ],
             "index": "pypi",
-            "version": "==2.20.0"
+            "markers": "python_version >= '3.9'",
+            "version": "==3.7.0"
         },
         "pycodestyle": {
             "hashes": [
-                "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
-                "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.10.0"
-        },
-        "pycparser": {
-            "hashes": [
-                "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
-                "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
+                "sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f",
+                "sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67"
             ],
-            "version": "==2.21"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.11.1"
         },
         "pyflakes": {
             "hashes": [
-                "sha256:ec55bf7fe21fff7f1ad2f7da62363d749e2a470500eab1b555334b67aa1ef8cf",
-                "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
+                "sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f",
+                "sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==3.0.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.2.0"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
-        },
-        "pytz": {
-            "hashes": [
-                "sha256:01a0681c4b9684a28304615eba55d1ab31ae00bf68ec157ec3708a8182dbbcd0",
-                "sha256:78f4f37d8198e0627c5f1143240bb0206b8691d8d7ac6d78fee88b78733f8c4a"
+                "sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c",
+                "sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367"
             ],
-            "version": "==2022.7.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.17.2"
         },
         "pyyaml": {
             "hashes": [
-                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
-                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
-                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
-                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
-                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
-                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
-                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
-                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
-                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
-                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
-                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
-                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
-                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
-                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
-                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
-                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
-                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
-                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
-                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
-                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
-                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
-                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
-                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
-                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
-                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
-                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
-                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
-                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
-                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
-                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
-                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
-                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
-                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
-                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
-                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
-                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
-                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
-                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
-                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
-                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+                "sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5",
+                "sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc",
+                "sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df",
+                "sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741",
+                "sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206",
+                "sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27",
+                "sha256:1d4c7e777c441b20e32f52bd377e0c409713e8bb1386e1099c2415f26e479595",
+                "sha256:1e2722cc9fbb45d9b87631ac70924c11d3a401b2d7f410cc0e3bbf249f2dca62",
+                "sha256:1fe35611261b29bd1de0070f0b2f47cb6ff71fa6595c077e42bd0c419fa27b98",
+                "sha256:28c119d996beec18c05208a8bd78cbe4007878c6dd15091efb73a30e90539696",
+                "sha256:326c013efe8048858a6d312ddd31d56e468118ad4cdeda36c719bf5bb6192290",
+                "sha256:40df9b996c2b73138957fe23a16a4f0ba614f4c0efce1e9406a184b6d07fa3a9",
+                "sha256:42f8152b8dbc4fe7d96729ec2b99c7097d656dc1213a3229ca5383f973a5ed6d",
+                "sha256:49a183be227561de579b4a36efbb21b3eab9651dd81b1858589f796549873dd6",
+                "sha256:4fb147e7a67ef577a588a0e2c17b6db51dda102c71de36f8549b6816a96e1867",
+                "sha256:50550eb667afee136e9a77d6dc71ae76a44df8b3e51e41b77f6de2932bfe0f47",
+                "sha256:510c9deebc5c0225e8c96813043e62b680ba2f9c50a08d3724c7f28a747d1486",
+                "sha256:5773183b6446b2c99bb77e77595dd486303b4faab2b086e7b17bc6bef28865f6",
+                "sha256:596106435fa6ad000c2991a98fa58eeb8656ef2325d7e158344fb33864ed87e3",
+                "sha256:6965a7bc3cf88e5a1c3bd2e0b5c22f8d677dc88a455344035f03399034eb3007",
+                "sha256:69b023b2b4daa7548bcfbd4aa3da05b3a74b772db9e23b982788168117739938",
+                "sha256:6c22bec3fbe2524cde73d7ada88f6566758a8f7227bfbf93a408a9d86bcc12a0",
+                "sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c",
+                "sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735",
+                "sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d",
+                "sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28",
+                "sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4",
+                "sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba",
+                "sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8",
+                "sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef",
+                "sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5",
+                "sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd",
+                "sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3",
+                "sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0",
+                "sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515",
+                "sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c",
+                "sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c",
+                "sha256:bd4af7373a854424dabd882decdc5579653d7868b8fb26dc7d0e99f823aa5924",
+                "sha256:bf07ee2fef7014951eeb99f56f39c9bb4af143d8aa3c21b1677805985307da34",
+                "sha256:bfdf460b1736c775f2ba9f6a92bca30bc2095067b8a9d77876d1fad6cc3b4a43",
+                "sha256:c8098ddcc2a85b61647b2590f825f3db38891662cfc2fc776415143f599bb859",
+                "sha256:d2b04aac4d386b172d5b9692e2d2da8de7bfb6c387fa4f801fbf6fb2e6ba4673",
+                "sha256:d483d2cdf104e7c9fa60c544d92981f12ad66a457afae824d146093b8c294c54",
+                "sha256:d858aa552c999bc8a8d57426ed01e40bef403cd8ccdd0fc5f6f04a00414cac2a",
+                "sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b",
+                "sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab",
+                "sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa",
+                "sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c",
+                "sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585",
+                "sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d",
+                "sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==6.0"
+            "version": "==6.0.1"
         },
         "readme-renderer": {
             "hashes": [
-                "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
-                "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
+                "sha256:1818dd28140813509eeed8d62687f7cd4f7bad90d4db586001c5dc09d4fde311",
+                "sha256:19db308d86ecd60e5affa3b2a98f017af384678c63c88e5d4556a380e674f3f9"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==37.3"
+            "markers": "python_version >= '3.8'",
+            "version": "==43.0"
         },
         "requests": {
             "hashes": [
-                "sha256:7c5599b102feddaa661c826c56ab4fee28bfd17f5abca1ebbe3e7f19d7c97983",
-                "sha256:8fefa2a1a1365bf5520aac41836fbee479da67864514bdb821f31ce07ce65349"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
             "index": "pypi",
-            "version": "==2.28.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:125d96d20c92b946b983d0d392b84ff945461e5a06d3867e9f9e575f8697b67f",
-                "sha256:8aa57747f3fc3e977684f0176a88e789be314a99f99b43b75d1e9cb5dc6db9e9"
+                "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222",
+                "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.1"
-        },
-        "secretstorage": {
-            "hashes": [
-                "sha256:2403533ef369eca6d2ba81718576c5e0f564d5cca1b58f73a8b23e7d4eeebd77",
-                "sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99"
-            ],
-            "markers": "sys_platform == 'linux'",
-            "version": "==3.3.3"
+            "version": "==13.7.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:16ccf598aab3b506593c17378473978908a2734d7336755a8769b480906bec1c",
-                "sha256:b440ee5f7e607bb8c9de15259dba2583dd41a38879a7abc1d43a71c59524da48"
+                "sha256:0ff4183f8f42cd8fa3acea16c45205521a4ef28f73c6391d8a25e92893134f2e",
+                "sha256:c21c49fb1042386df081cb5d86759792ab89efca84cf114889191cd09aacc80c"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==67.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==69.2.0"
         },
         "setuptools-scm": {
             "hashes": [
-                "sha256:031e13af771d6f892b941adb6ea04545bbf91ebc5ce68c78aaf3fff6e1fb4844",
-                "sha256:7930f720905e03ccd1e1d821db521bff7ec2ac9cf0ceb6552dd73d24a45d3b02"
+                "sha256:b47844cd2a84b83b3187a5782c71128c28b4c94cad8bfb871da2784a5cb54c4f",
+                "sha256:b5f43ff6800669595193fd09891564ee9d1d7dcb196cab4b2506d53a2e1c95c7"
             ],
             "index": "pypi",
-            "version": "==7.0.5"
-        },
-        "six": {
-            "hashes": [
-                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
-                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.16.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==8.0.4"
         },
         "snowballstemmer": {
             "hashes": [
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:060ca5c9f7ba57a08a1219e547b269fadf125ae25b06b9fa7f66768efb652d6d",
-                "sha256:51026de0a9ff9fc13c05d74913ad66047e104f56a129ff73e174eb5c3ee794b5"
+                "sha256:1e09160a40b956dc623c910118fa636da93bd3ca0b9876a7b3df90f07d691560",
+                "sha256:9a5160e1ea90688d5963ba09a2dcd8bdd526620edbb65c328728f1b2228d5ab5"
             ],
             "index": "pypi",
-            "version": "==5.3.0"
+            "markers": "python_version >= '3.9'",
+            "version": "==7.2.6"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
-                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
-                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
+                "sha256:c40a4f96f3776c4393d933412053962fac2b84f4c99a7982ba42e09576a70619",
+                "sha256:cb61eb0ec1b61f349e5cc36b2028e9e7ca765be05e49641c97241274753067b4"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==1.0.4"
+            "markers": "python_version >= '3.9'",
+            "version": "==1.0.8"
         },
         "sphinxcontrib-devhelp": {
             "hashes": [
-                "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
-                "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
+                "sha256:6485d09629944511c893fa11355bda18b742b83a2b181f9a009f7e500595c90f",
+                "sha256:9893fd3f90506bc4b97bdb977ceb8fbd823989f4316b28c3841ec128544372d3"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
+            "markers": "python_version >= '3.9'",
+            "version": "==1.0.6"
         },
         "sphinxcontrib-htmlhelp": {
             "hashes": [
-                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
-                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
+                "sha256:0dc87637d5de53dd5eec3a6a01753b1ccf99494bd756aafecd74b4fa9e729015",
+                "sha256:393f04f112b4d2f53d93448d4bce35842f62b307ccdc549ec1585e950bc35e04"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==2.0.1"
+            "markers": "python_version >= '3.9'",
+            "version": "==2.0.5"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.0.1"
         },
         "sphinxcontrib-qthelp": {
             "hashes": [
-                "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72",
-                "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"
+                "sha256:053dedc38823a80a7209a80860b16b722e9e0209e32fea98c90e4e6624588ed6",
+                "sha256:e2ae3b5c492d58fcbd73281fbd27e34b8393ec34a073c792642cd8e529288182"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.3"
+            "markers": "python_version >= '3.9'",
+            "version": "==1.0.7"
         },
         "sphinxcontrib-serializinghtml": {
             "hashes": [
-                "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
-                "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
+                "sha256:326369b8df80a7d2d8d7f99aa5ac577f51ea51556ed974e7716cfd4fca3f6cb7",
+                "sha256:93f3f5dc458b91b192fe10c397e324f262cf163d79f3282c158e8436a2c4511f"
             ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.1.5"
-        },
-        "toml": {
-            "hashes": [
-                "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
-                "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
-            ],
-            "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.2"
+            "markers": "python_version >= '3.9'",
+            "version": "==1.1.10"
         },
         "tomli": {
             "hashes": [
                 "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
-            "markers": "python_full_version >= '3.7.0'",
+            "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "twine": {
             "hashes": [
-                "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
-                "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
+                "sha256:89b0cc7d370a4b66421cc6102f269aa910fe0f1861c124f573cf2ddedbc10cf4",
+                "sha256:a262933de0b484c53408f9edae2e7821c1c45a3314ff2df9bdd343aa7ab8edc0"
             ],
             "index": "pypi",
-            "version": "==4.0.2"
+            "markers": "python_version >= '3.8'",
+            "version": "==5.0.0"
         },
-        "typing-extensions": {
+        "types-requests": {
             "hashes": [
-                "sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa",
-                "sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e"
+                "sha256:4428df33c5503945c74b3f42e82b181e86ec7b724620419a2966e2de604ce1a1",
+                "sha256:6216cdac377c6b9a040ac1c0404f7284bd13199c0e1bb235f4324627e8898cf5"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==4.4.0"
+            "index": "pypi",
+            "markers": "python_version >= '3.8'",
+            "version": "==2.31.0.20240406"
         },
-        "urllib3": {
+        "typing-extensions": {
             "hashes": [
-                "sha256:076907bf8fd355cde77728471316625a4d2f7e713c125f51953bb5b3eecf4f72",
-                "sha256:75edcdc2f7d85b137124a6c3c9fc3933cdeaa12ecb9a6a959f22797a0feca7e1"
+                "sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0",
+                "sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.14"
+            "markers": "python_version >= '3.8'",
+            "version": "==4.11.0"
         },
-        "virtualenv": {
+        "urllib3": {
             "hashes": [
-                "sha256:37a640ba82ed40b226599c522d411e4be5edb339a0c0de030c0dc7b646d61590",
-                "sha256:54eb59e7352b573aa04d53f80fc9736ed0ad5143af445a1e539aada6eb947dd1"
+                "sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d",
+                "sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==20.19.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==2.2.1"
         },
-        "webencodings": {
+        "virtualenv": {
             "hashes": [
-                "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
-                "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
+                "sha256:961c026ac520bac5f69acb8ea063e8a4f071bcc9457b9c1f28f6b085c511583a",
+                "sha256:e08e13ecdca7a0bd53798f356d5831434afa5b07b93f0abdf0797b7a06ffe197"
             ],
-            "version": "==0.5.1"
+            "markers": "python_version >= '3.7'",
+            "version": "==20.25.1"
         },
         "zipp": {
             "hashes": [
-                "sha256:6c4fe274b8f85ec73c37a8e4e3fa00df9fb9335da96fb789e3b96b318e5097b3",
-                "sha256:a3cac813d40993596b39ea9e93a18e8a2076d5c378b8bc88ec32ab264e04ad02"
+                "sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b",
+                "sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715"
             ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.12.1"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.18.1"
         }
     }
 }
```

### Comparing `inciweb-wildfires-0.2.1/docs/Makefile` & `inciweb-wildfires-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/docs/_static/css/custom.css` & `inciweb-wildfires-1.0.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/docs/_templates/nav.html` & `inciweb-wildfires-1.0.0/docs/_templates/nav.html`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/docs/conf.py` & `inciweb-wildfires-1.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configure Sphinx configuration."""
+
 import os
 import sys
 from datetime import datetime
 
 # Insert the parent directory into the path
 sys.path.insert(0, os.path.abspath(".."))
```

### Comparing `inciweb-wildfires-0.2.1/docs/index.md` & `inciweb-wildfires-1.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/docs/make.bat` & `inciweb-wildfires-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/PKG-INFO` & `inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inciweb-wildfires
-Version: 0.2.1
+Version: 1.0.0
 Summary: Download wildfire incidents data from InciWeb
 Home-page: http://www.github.com/datadesk/inciweb-wildfires
 Author: Ben Welsh
 Author-email: b@palewi.re
 License: MIT
 Project-URL: Maintainer, https://github.com/datadesk
 Project-URL: Source, https://github.com/datadesk/inciweb-wildfires
@@ -14,14 +14,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: geojson
+Requires-Dist: click
 
 ### Links
 
 * Docs: [palewi.re/docs/inciweb-wildfires/](https://palewi.re/docs/inciweb-wildfires/)
 * Issues: [github.com/datadesk/inciweb-wildfires/issues](https://github.com/datadesk/inciweb-wildfires/issues)
 * Packaging: [pypi.python.org/pypi/inciweb-wildfires](https://pypi.python.org/pypi/inciweb-wildfires)
 * Testing: [github.com/datadesk/inciweb-wildfires/actions](https://github.com/datadesk/inciweb-wildfires/actions)
```

### Comparing `inciweb-wildfires-0.2.1/inciweb_wildfires.egg-info/SOURCES.txt` & `inciweb-wildfires-1.0.0/inciweb_wildfires.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inciweb-wildfires-0.2.1/setup.py` & `inciweb-wildfires-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="Ben Welsh",
     author_email="b@palewi.re",
     url="http://www.github.com/datadesk/inciweb-wildfires",
     license="MIT",
     packages=("inciweb_wildfires",),
-    install_requires=["requests", "geojson", "click", "bs4", "lxml"],
+    install_requires=["requests", "geojson", "click"],
     entry_points="""
         [console_scripts]
         inciwebwildfires=inciweb_wildfires.cli:cmd
         inciweb-wildfires=inciweb_wildfires.cli:cmd
     """,
     use_scm_version={"version_scheme": version_scheme, "local_scheme": local_version},
     classifiers=[
```

