# Comparing `tmp/jupyter_bridge-0.1.0.tar.gz` & `tmp/jupyter_bridge-0.2.0.tar.gz`

## Comparing `jupyter_bridge-0.1.0.tar` & `jupyter_bridge-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,53 @@
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/babel.config.js
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/install.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/jest.config.js
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/package.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/tsconfig.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/tsconfig.test.json
--rw-r--r--   0        0        0   386385 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/yarn.lock
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/_version.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/package.json
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/509.746cae8da8be93da3179.js
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/remoteEntry.20976a8f3bc90c603f6d.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/src/index.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/src/__tests__/Jupyter-Bridge.spec.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/style/index.js
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/ui-tests/tests/Jupyter-Bridge.spec.ts
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/LICENSE
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/README.md
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 jupyter_bridge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/babel.config.js
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/install.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/jest.config.js
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/package.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/tsconfig.test.json
+-rw-r--r--   0        0        0   386385 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/yarn.lock
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/_version.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/package.json
+-rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/373c04fd2418f5c77eea.eot
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/3f6d3488cf65374f6f67.woff
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js
+-rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/79d088064beb3826054f.eot
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/821.05379ddf2d3d45468a67.js
+-rw-r--r--   0        0        0    65844 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/898.49611806d94d0f697263.js
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/8ea8791754915a898a31.woff2
+-rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/9674eb1bd55047179038.svg
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/9834b82ad26e2a37583d.woff2
+-rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/a3b9817780214caf01e8.svg
+-rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/af6397503fcefbd61397.ttf
+-rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/be0a084962d8066884f7.svg
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/cb9e9e693192413cde2b.woff
+-rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/cda59d6efffa685830fd.ttf
+-rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e4299464e7b012968eed.eot
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e42a88444448ac3d6054.woff2
+-rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e8711bbb871afd8e9dea.ttf
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/f9217f66874b0c01cd8c.woff
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/remoteEntry.f2d6900c4d9c0155de96.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/style.js
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/src/index.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/src/__tests__/Jupyter-Bridge.spec.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/base.css
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/index.js
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/README.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/package.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/tests/Jupyter-Bridge.spec.ts
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/README.md
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/PKG-INFO
```

### Comparing `jupyter_bridge-0.1.0/RELEASE.md` & `jupyter_bridge-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/jest.config.js` & `jupyter_bridge-0.2.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/package.json` & `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9513888888888888%*

 * *Differences: {"'description'": "'Enhances JupyterLab by adding customizable footer buttons to code cells for "*

 * *                  'improved interactivity and visibility control, supporting operations like '*

 * *                  'running cells, hiding/showing code, and managing output directly from the cell '*

 * *                  "interface.'",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', "*

 * *                 "'static\\\\remoteEntry.f2d6900c4d9c0155de96.js'), ('extension', './extension'), "*

 * *                 "('style', './st […]*

```diff
@@ -5,15 +5,15 @@
     },
     "bugs": {
         "url": "https://github.com/LtStarbuck1030/jupyter_bridge/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0"
     },
-    "description": "A JupyterLab extension.",
+    "description": "Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
@@ -103,14 +103,19 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/LtStarbuck1030/jupyter_bridge",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static\\remoteEntry.f2d6900c4d9c0155de96.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "Jupyter-Bridge/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -186,9 +191,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyter_bridge-0.1.0/tsconfig.json` & `jupyter_bridge-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/yarn.lock` & `jupyter_bridge-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/Jupyter-Bridge/__init__.py` & `jupyter_bridge-0.2.0/Jupyter-Bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/package.json` & `jupyter_bridge-0.2.0/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9513888888888888%*

 * *Differences: {"'description'": "'Enhances JupyterLab by adding customizable footer buttons to code cells for "*

 * *                  'improved interactivity and visibility control, supporting operations like '*

 * *                  'running cells, hiding/showing code, and managing output directly from the cell '*

 * *                  "interface.'",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -5,15 +5,15 @@
     },
     "bugs": {
         "url": "https://github.com/LtStarbuck1030/jupyter_bridge/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0"
     },
-    "description": "A JupyterLab extension.",
+    "description": "Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
@@ -103,19 +103,14 @@
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/LtStarbuck1030/jupyter_bridge",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static\\remoteEntry.20976a8f3bc90c603f6d.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "Jupyter-Bridge/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
@@ -191,9 +186,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyter_bridge-0.1.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js` & `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/ui-tests/README.md` & `jupyter_bridge-0.2.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/ui-tests/tests/Jupyter-Bridge.spec.ts` & `jupyter_bridge-0.2.0/ui-tests/tests/Jupyter-Bridge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/.gitignore` & `jupyter_bridge-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/LICENSE` & `jupyter_bridge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/README.md` & `jupyter_bridge-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Jupyter-Bridge
 
 [![Github Actions Status](https://github.com/LtStarbuck1030/jupyter_bridge/workflows/Build/badge.svg)](https://github.com/LtStarbuck1030/jupyter_bridge/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LtStarbuck1030/jupyter_bridge/main?urlpath=lab)
-A JupyterLab extension.
+Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
```

### Comparing `jupyter_bridge-0.1.0/pyproject.toml` & `jupyter_bridge-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.1.0/PKG-INFO` & `jupyter_bridge-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: Jupyter-Bridge
-Version: 0.1.0
+Version: 0.2.0
 Dynamic: Keywords
-Summary: A JupyterLab extension.
+Summary: Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.
 Project-URL: Homepage, https://github.com/LtStarbuck1030/jupyter_bridge
 Project-URL: Bug Tracker, https://github.com/LtStarbuck1030/jupyter_bridge/issues
 Project-URL: Repository, https://github.com/LtStarbuck1030/jupyter_bridge.git
 Author-email: Lisa Marie Meyers <lisamarie9006@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Lisa Marie Meyers
@@ -53,15 +53,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Jupyter-Bridge
 
 [![Github Actions Status](https://github.com/LtStarbuck1030/jupyter_bridge/workflows/Build/badge.svg)](https://github.com/LtStarbuck1030/jupyter_bridge/actions/workflows/build.yml)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/LtStarbuck1030/jupyter_bridge/main?urlpath=lab)
-A JupyterLab extension.
+Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.
 
 ## Requirements
 
 - JupyterLab >= 4.0.0
 
 ## Install
```

