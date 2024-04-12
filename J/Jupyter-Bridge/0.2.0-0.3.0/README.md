# Comparing `tmp/jupyter_bridge-0.2.0.tar.gz` & `tmp/jupyter_bridge-0.3.0.tar.gz`

## Comparing `jupyter_bridge-0.2.0.tar` & `jupyter_bridge-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,46 @@
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.copier-answers.yml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.yarnrc.yml
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/RELEASE.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/babel.config.js
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/install.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/jest.config.js
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/package.json
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/tsconfig.json
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/tsconfig.test.json
--rw-r--r--   0        0        0   386385 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/yarn.lock
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/_version.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/package.json
--rw-r--r--   0        0        0   203030 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/373c04fd2418f5c77eea.eot
--rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/3f6d3488cf65374f6f67.woff
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js
--rw-r--r--   0        0        0    34034 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/79d088064beb3826054f.eot
--rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/821.05379ddf2d3d45468a67.js
--rw-r--r--   0        0        0    65844 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/898.49611806d94d0f697263.js
--rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/8ea8791754915a898a31.woff2
--rw-r--r--   0        0        0   918991 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/9674eb1bd55047179038.svg
--rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/9834b82ad26e2a37583d.woff2
--rw-r--r--   0        0        0   747927 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/a3b9817780214caf01e8.svg
--rw-r--r--   0        0        0   202744 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/af6397503fcefbd61397.ttf
--rw-r--r--   0        0        0   144714 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/be0a084962d8066884f7.svg
--rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/cb9e9e693192413cde2b.woff
--rw-r--r--   0        0        0   133988 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/cda59d6efffa685830fd.ttf
--rw-r--r--   0        0        0   134294 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e4299464e7b012968eed.eot
--rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e42a88444448ac3d6054.woff2
--rw-r--r--   0        0        0    33736 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/e8711bbb871afd8e9dea.ttf
--rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/f9217f66874b0c01cd8c.woff
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/remoteEntry.f2d6900c4d9c0155de96.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/style.js
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/src/index.ts
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/src/__tests__/Jupyter-Bridge.spec.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/base.css
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/style/index.js
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/README.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/package.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/ui-tests/tests/Jupyter-Bridge.spec.ts
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/LICENSE
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/README.md
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 jupyter_bridge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/.copier-answers.yml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/.yarnrc.yml
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/RELEASE.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/babel.config.js
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/install.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/jest.config.js
+-rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/package.json
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/tsconfig.json
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/tsconfig.test.json
+-rw-r--r--   0        0        0   386734 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/yarn.lock
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/_version.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/package.json
+-rw-r--r--   0        0        0   117852 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/232c6f6a7678304f9efa.woff2
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/821.05379ddf2d3d45468a67.js
+-rw-r--r--   0        0        0   109207 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/898.0cfca29af376f5db6d74.js
+-rw-r--r--   0        0        0    67860 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/9174757efc83e072436e.ttf
+-rw-r--r--   0        0        0   156400 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/ae17c16afbea216707b2.woff2
+-rw-r--r--   0        0        0   420332 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/b4990d0d0c5f5d38d62e.ttf
+-rw-r--r--   0        0        0    25392 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/c27da6f833431da5aa29.woff2
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/c7a869faca299d15be10.woff2
+-rw-r--r--   0        0        0   209128 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/e28096fa75a96ac77020.ttf
+-rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/ff8f525fb050c5d24519.ttf
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/remoteEntry.d22a1a7f4db5e8d0f62c.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/style.js
+-rw-r--r--   0        0        0    10233 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    15339 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/src/index.ts
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/src/__tests__/Jupyter-Bridge.spec.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/style/base.css
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/style/index.js
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/README.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/package.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/ui-tests/tests/Jupyter-Bridge.spec.ts
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/README.md
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6403 2020-02-02 00:00:00.000000 jupyter_bridge-0.3.0/PKG-INFO
```

### Comparing `jupyter_bridge-0.2.0/.copier-answers.yml` & `jupyter_bridge-0.3.0/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/RELEASE.md` & `jupyter_bridge-0.3.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/jest.config.js` & `jupyter_bridge-0.3.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/package.json` & `jupyter_bridge-0.3.0/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'dependencies'": "{'@fortawesome/fontawesome-free': '^6.5.2'}", "'version'": "'0.3.0'"}*

```diff
@@ -3,14 +3,15 @@
         "email": "lisamarie9006@gmail.com",
         "name": "Lisa Marie Meyers"
     },
     "bugs": {
         "url": "https://github.com/LtStarbuck1030/jupyter_bridge/issues"
     },
     "dependencies": {
+        "@fortawesome/fontawesome-free": "^6.5.2",
         "@jupyterlab/application": "^4.0.0"
     },
     "description": "Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
@@ -186,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyter_bridge-0.2.0/tsconfig.json` & `jupyter_bridge-0.3.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/yarn.lock` & `jupyter_bridge-0.3.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1724,14 +1724,21 @@
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
+"@fortawesome/fontawesome-free@npm:^6.5.2":
+  version: 6.5.2
+  resolution: "@fortawesome/fontawesome-free@npm:6.5.2"
+  checksum: b77c1751721f355edc3bbc5c305d3ae87130156846511dfd3f66d5e218e246a7b3b5c57839f7b57729864b9d8b166e76aba2a11472a3e2f2ff597c24d39999df
+  languageName: node
+  linkType: hard
+
 "@humanwhocodes/config-array@npm:^0.11.14":
   version: 0.11.14
   resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
     "@humanwhocodes/object-schema": ^2.0.2
     debug: ^4.3.1
     minimatch: ^3.0.5
@@ -3786,14 +3793,15 @@
   languageName: node
   linkType: hard
 
 "Jupyter-Bridge@workspace:.":
   version: 0.0.0-use.local
   resolution: "Jupyter-Bridge@workspace:."
   dependencies:
+    "@fortawesome/fontawesome-free": ^6.5.2
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/builder": ^4.0.0
     "@jupyterlab/testutils": ^4.0.0
     "@types/jest": ^29.2.0
     "@types/json-schema": ^7.0.11
     "@types/react": ^18.0.26
     "@types/react-addons-linked-state-mixin": ^0.14.22
```

### Comparing `jupyter_bridge-0.2.0/Jupyter-Bridge/__init__.py` & `jupyter_bridge-0.3.0/Jupyter-Bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/package.json` & `jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9681712962962963%*

 * *Differences: {"'dependencies'": "{'@fortawesome/fontawesome-free': '^6.5.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static\\\\remoteEntry.d22a1a7f4db5e8d0f62c.js'}}",*

 * * "'version'": "'0.3.0'"}*

```diff
@@ -3,14 +3,15 @@
         "email": "lisamarie9006@gmail.com",
         "name": "Lisa Marie Meyers"
     },
     "bugs": {
         "url": "https://github.com/LtStarbuck1030/jupyter_bridge/issues"
     },
     "dependencies": {
+        "@fortawesome/fontawesome-free": "^6.5.2",
         "@jupyterlab/application": "^4.0.0"
     },
     "description": "Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@jupyterlab/testutils": "^4.0.0",
         "@types/jest": "^29.2.0",
@@ -105,15 +106,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/LtStarbuck1030/jupyter_bridge",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static\\remoteEntry.f2d6900c4d9c0155de96.js",
+            "load": "static\\remoteEntry.d22a1a7f4db5e8d0f62c.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "Jupyter-Bridge/labextension"
     },
     "keywords": [
         "jupyter",
@@ -191,9 +192,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.0"
+    "version": "0.3.0"
 }
```

### Comparing `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js` & `jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/728.6c9624ae65fa2faeeb4d.js`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/821.05379ddf2d3d45468a67.js` & `jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/821.05379ddf2d3d45468a67.js`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/Jupyter-Bridge/labextension/static/remoteEntry.f2d6900c4d9c0155de96.js` & `jupyter_bridge-0.3.0/Jupyter-Bridge/labextension/static/remoteEntry.d22a1a7f4db5e8d0f62c.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, d, s, f, c, p, h, v, b, g, m, y, w, j, S, k = {
+    var e, r, t, n, o, a, i, u, l, d, s, f, p, c, h, v, b, g, m, y, w, j, S, k = {
             902: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(898), t.e(821)]).then((() => () => t(821))),
                         "./extension": () => Promise.all([t.e(898), t.e(821)]).then((() => () => t(821))),
                         "./style": () => t.e(728).then((() => () => t(728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -45,19 +45,19 @@
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         728: "6c9624ae65fa2faeeb4d",
         821: "05379ddf2d3d45468a67",
-        898: "49611806d94d0f697263"
+        898: "0cfca29af376f5db6d74"
     } [e] + ".js?v=" + {
         728: "6c9624ae65fa2faeeb4d",
         821: "05379ddf2d3d45468a67",
-        898: "49611806d94d0f697263"
+        898: "0cfca29af376f5db6d74"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -71,19 +71,19 @@
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
                         i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -108,15 +108,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => Promise.all([P.e(898), P.e(821)]).then((() => () => P(821))),
                         from: i,
                         eager: !1
                     })
-                })("Jupyter-Bridge", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("Jupyter-Bridge", "0.3.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -187,44 +187,44 @@
                     l = !1, u--
                 } else {
                     if (u <= n || s < f != o) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var p = [],
+            c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
-        return !!p()
+        return !!c()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || p(d(e, t, o, n)), v(e[t][o])
+        return a(n, o) || c(d(e, t, o, n)), v(e[t][o])
     }, f = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, c = (e, r, t, n) => {
+    }, p = (e, r, t, n) => {
         var a = e[t];
         return "No satisfying version (" + o(n) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(a).map((e => e + " from " + a[e].from)).join(", ")
-    }, p = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, n) => {
-        p(c(e, r, t, n))
+        c(p(e, r, t, n))
     }, v = e => (e.loaded = 1, e.get()), g = (b = e => function(r, t, n, o) {
         var a = P.I(r);
         return a && a.then ? a.then(e.bind(e, r, P.S[r], t, n, o)) : e(r, P.S[r], t, n, o)
     })(((e, r, t, n) => (i(e, t), v(f(r, t, n) || h(r, e, t, n) || u(r, t))))), m = b(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), y = {}, w = {
         71: () => m("default", "@jupyterlab/codeeditor", [1, 4, 1, 6]),
         302: () => g("default", "@jupyterlab/outputarea", [1, 4, 1, 6]),
         345: () => m("default", "react", [1, 18, 2, 0]),
```

### Comparing `jupyter_bridge-0.2.0/src/index.ts` & `jupyter_bridge-0.3.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/style/index.css` & `jupyter_bridge-0.3.0/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/ui-tests/README.md` & `jupyter_bridge-0.3.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/ui-tests/tests/Jupyter-Bridge.spec.ts` & `jupyter_bridge-0.3.0/ui-tests/tests/Jupyter-Bridge.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/.gitignore` & `jupyter_bridge-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/LICENSE` & `jupyter_bridge-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/README.md` & `jupyter_bridge-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/pyproject.toml` & `jupyter_bridge-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bridge-0.2.0/PKG-INFO` & `jupyter_bridge-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Jupyter-Bridge
-Version: 0.2.0
+Version: 0.3.0
 Dynamic: Keywords
 Summary: Enhances JupyterLab by adding customizable footer buttons to code cells for improved interactivity and visibility control, supporting operations like running cells, hiding/showing code, and managing output directly from the cell interface.
 Project-URL: Homepage, https://github.com/LtStarbuck1030/jupyter_bridge
 Project-URL: Bug Tracker, https://github.com/LtStarbuck1030/jupyter_bridge/issues
 Project-URL: Repository, https://github.com/LtStarbuck1030/jupyter_bridge.git
 Author-email: Lisa Marie Meyers <lisamarie9006@gmail.com>
 License: BSD 3-Clause License
```

