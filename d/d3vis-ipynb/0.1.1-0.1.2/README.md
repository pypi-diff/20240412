# Comparing `tmp/d3vis_ipynb-0.1.1.tar.gz` & `tmp/d3vis_ipynb-0.1.2.tar.gz`

## Comparing `d3vis_ipynb-0.1.1.tar` & `d3vis_ipynb-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/D3vis_ipynb.json
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/RELEASE.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/install.json
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/setup.cfg
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/setup.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/__init__.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/_version.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/embedding.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/web.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/widgets.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/package.json
--rw-r--r--   0        0        0    22687 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/380.bce32fc1670ea497a572.js
--rw-r--r--   0        0        0    23295 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/493.e98395b66f4058ecc2a8.js
--rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/remoteEntry.7e42e6f84b582762349a.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/style.js
--rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    88462 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/d3vis_ipynb/nbextension/index.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/amd-public-path.js
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/package.json
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/webpack.config.js
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/webpack.exports.config.js
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/css/widget.css
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/extension.js
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/index.js
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/labplugin.js
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/web-dev.js
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/widgets.js
--rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/barplot.js
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/histogramplot.js
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/linearhistplot.js
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/graphs/scatterplot.js
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/tools/lasso.js
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/js/lib/wrappers/embedding.wrapper.js
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/.gitignore
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/README.md
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/D3vis_ipynb.json
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/RELEASE.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/install.json
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/setup.cfg
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/setup.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/__init__.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/_version.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/embedding.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/web.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/widgets.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/package.json
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/380.5f71b19ff5261cd2e5de.js
+-rw-r--r--   0        0        0    23626 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/493.6062c0a7b585f6ae1d22.js
+-rw-r--r--   0        0        0   282230 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/remoteEntry.bf58726a1c33e2ff91a1.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/style.js
+-rw-r--r--   0        0        0    35163 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/d3vis_ipynb/nbextension/index.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/amd-public-path.js
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/package.json
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/webpack.config.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/webpack.exports.config.js
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/css/widget.css
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/extension.js
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/index.js
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/labplugin.js
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/web-dev.js
+-rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/widgets.js
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/barplot.js
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/histogramplot.js
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/linearhistplot.js
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/graphs/scatterplot.js
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/tools/lasso.js
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/js/lib/wrappers/embedding.wrapper.js
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/README.md
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 d3vis_ipynb-0.1.2/PKG-INFO
```

### Comparing `d3vis_ipynb-0.1.1/RELEASE.md` & `d3vis_ipynb-0.1.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/setup.cfg` & `d3vis_ipynb-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/__init__.py` & `d3vis_ipynb-0.1.2/d3vis_ipynb/__init__.py`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/embedding.py` & `d3vis_ipynb-0.1.2/d3vis_ipynb/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,24 +115,24 @@
                     not_rects()
                 if rows[rows_keys[i]][-1] != rows[first_row][-1]:
                     not_rects()
 
     def add(self, widget, position: int):
         self._all_widgets.append(widget)
         if self._is_displayed:
-            widget.element = self.positions_hashs[position]
+            widget.elementId = self.positions_hashs[position]
             display(widget)
         else:
             self._widgets_to_display[position] = widget
 
     def _repr_html_(self):
         self._is_displayed = True
         for key in self._widgets_to_display.keys():
             widget = self._widgets_to_display[key]
-            widget.element = self.positions_hashs[key]
+            widget.elementId = self.positions_hashs[key]
             display(widget)
 
     def export(self):
         absolute_path = os.path.dirname(__file__)
         relative_js_path = "../js/lib/"
         js_path = os.path.abspath(os.path.join(absolute_path, relative_js_path))
         relative_data_path = "wrappers/data.json"
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/widgets.py` & `d3vis_ipynb-0.1.2/d3vis_ipynb/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 
     _name = "linearhistplot"
     _observing = []
 
     linearData_x = List([]).tag(sync=True)
     linearData_y = List([]).tag(sync=True)
     histogramData = List([]).tag(sync=True)
-    element = Unicode().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
     clickedValue = Unicode().tag(sync=True)
 
     def name(self):
         return self._name
 
     def export_data(self):
         data = {
             "linearData_x": self.linearData_x,
             "linearData_y": self.linearData_y,
             "histogramData": self.histogramData,
-            "element": self.element,
+            "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
 
 @widgets.register
@@ -50,28 +50,28 @@
     _name = "scatterplot"
     _observing = []
 
     data = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     y = Unicode().tag(sync=True)
     hue = Unicode().tag(sync=True)
-    element = Unicode().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
     clickedValue = Unicode().tag(sync=True)
     selectedValues = List([]).tag(sync=True)
 
     def name(self):
         return self._name
 
     def export_data(self):
         data = {
             "data": self.data,
             "x": self.x,
             "y": self.y,
             "hue": self.hue,
-            "element": self.element,
+            "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
 
 @widgets.register
@@ -86,26 +86,26 @@
     _name = "barplot"
     _observing = []
 
     data = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     y = Unicode().tag(sync=True)
     hue = Unicode().tag(sync=True)
-    element = Unicode().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
 
     def name(self):
         return self._name
 
     def export_data(self):
         data = {
             "data": self.data,
             "x": self.x,
             "y": self.y,
             "hue": self.hue,
-            "element": self.element,
+            "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
 
     def linkData(self, widget, widgetAttr):
         self._observing.append({"data": {widget.name(): widgetAttr}})
@@ -128,23 +128,23 @@
     _name = "histogramplot"
     _observing = []
 
     data = List([]).tag(sync=True)
     x = Unicode().tag(sync=True)
     start = Float().tag(sync=True)
     end = Float().tag(sync=True)
-    element = Unicode().tag(sync=True)
+    elementId = Unicode().tag(sync=True)
 
     def name(self):
         return self._name
 
     def export_data(self):
         data = {
             "data": self.data,
             "x": self.x,
             "start": self.start,
             "end": self.end,
-            "element": self.element,
+            "elementId": self.elementId,
             "observing": self._observing,
         }
 
         return {self._name: data}
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/package.json` & `d3vis_ipynb-0.1.2/js/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'0.1.2'"}*

```diff
@@ -14,18 +14,14 @@
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.7e42e6f84b582762349a.js"
-        },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -54,9 +50,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/380.bce32fc1670ea497a572.js` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/380.5f71b19ff5261cd2e5de.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,717 +1,730 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
     [380, 56], {
-        380: (e, t, a) => {
-            a.r(t), a.d(t, {
-                BarPlotModel: () => S,
-                BarPlotView: () => A,
-                EmbeddingModel: () => E,
-                EmbeddingView: () => V,
-                HistogramPlotModel: () => j,
-                HistogramPlotView: () => D,
-                LinearHistPlotModel: () => b,
-                LinearHistPlotView: () => w,
-                ScatterPlotModel: () => k,
-                ScatterPlotView: () => M,
-                author: () => L.author,
-                dependencies: () => L.dependencies,
-                description: () => L.description,
-                devDependencies: () => L.devDependencies,
-                files: () => L.files,
-                jupyterlab: () => L.jupyterlab,
-                keywords: () => L.keywords,
-                license: () => L.license,
-                main: () => L.main,
-                name: () => L.name,
-                repository: () => L.repository,
-                scripts: () => L.scripts,
-                version: () => L.version
+        380: (e, t, n) => {
+            n.r(t), n.d(t, {
+                BarPlotModel: () => L,
+                BarPlotView: () => j,
+                EmbeddingModel: () => O,
+                EmbeddingView: () => I,
+                HistogramPlotModel: () => D,
+                HistogramPlotView: () => V,
+                LinearHistPlotModel: () => M,
+                LinearHistPlotView: () => S,
+                ScatterPlotModel: () => A,
+                ScatterPlotView: () => E,
+                author: () => C.author,
+                dependencies: () => C.dependencies,
+                description: () => C.description,
+                devDependencies: () => C.devDependencies,
+                files: () => C.files,
+                jupyterlab: () => C.jupyterlab,
+                keywords: () => C.keywords,
+                license: () => C.license,
+                main: () => C.main,
+                name: () => C.name,
+                repository: () => C.repository,
+                scripts: () => C.scripts,
+                version: () => C.version
             });
-            var n = a(801),
-                r = a(840);
+            var a = n(801),
+                r = n(840);
 
             function i(e) {
-                const t = e.reduce(((e, t) => e + t), 0) / e.length;
-                let a = 1.96 * function(e, t) {
-                    let a = 0;
-                    return e.forEach((e => a += (e - t) ** 2)), a = Math.sqrt(a) / e.length, a
-                }(e, t);
-                return [t - a, t + a]
-            }
-            var o = a(72),
-                l = a.n(o),
-                s = a(825),
-                d = a.n(s),
-                c = a(659),
-                u = a.n(c),
-                m = a(56),
-                p = a.n(m),
-                h = a(540),
-                v = a.n(h),
-                g = a(113),
-                f = a.n(g),
-                _ = a(930),
+                const t = e.reduce(((e, t) => e + t), 0) / e.length,
+                    n = 1.96 * function(e, t) {
+                        let n = 0;
+                        return e.forEach((e => n += (e - t) ** 2)), n = Math.sqrt(n) / e.length, n
+                    }(e, t);
+                return [t - n, t + n]
+            }
+            var o = n(72),
+                s = n.n(o),
+                l = n(825),
+                d = n.n(l),
+                c = n(659),
+                m = n.n(c),
+                u = n(56),
+                p = n.n(u),
+                h = n(540),
+                f = n.n(h),
+                g = n(113),
+                v = n.n(g),
+                _ = n(930),
                 x = {};
-            x.styleTagTransform = f(), x.setAttributes = p(), x.insert = u().bind(null, "head"), x.domAPI = d(), x.insertStyleElement = v(), l()(_.A, x), _.A && _.A.locals && _.A.locals;
-            const y = a(330);
-            class b extends n.DOMWidgetModel {
+            x.styleTagTransform = v(), x.setAttributes = p(), x.insert = m().bind(null, "head"), x.domAPI = d(), x.insertStyleElement = f(), s()(_.A, x), _.A && _.A.locals && _.A.locals;
+            const y = n(330),
+                b = 400,
+                w = {
+                    top: 20,
+                    right: 20,
+                    bottom: 30,
+                    left: 40
+                };
+
+            function k(e) {
+                e.timeout && clearTimeout(e.timeout), e.timeout = setTimeout((() => {
+                    e.plot()
+                }), 100)
+            }
+            class M extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: b.model_name,
-                        _view_name: b.view_name,
-                        _model_module: b.model_module,
-                        _view_module: b.view_module,
-                        _model_module_version: b.model_module_version,
-                        _view_module_version: b.view_module_version,
+                        _model_name: M.model_name,
+                        _view_name: M.view_name,
+                        _model_module: M.model_module,
+                        _view_module: M.view_module,
+                        _model_module_version: M.model_module_version,
+                        _view_module_version: M.view_module_version,
                         linearData_x: [],
                         linearData_y: [],
                         histogramData: [],
-                        element: String,
+                        elementId: String,
                         clickedValue: String
                     }
                 }
                 static model_name = "LinearHistPlotModel";
                 static model_module = y.name;
                 static model_module_version = y.version;
                 static view_name = "LinearHistPlotView";
                 static view_module = y.name;
                 static view_module_version = y.version
             }
-            class w extends n.DOMWidgetView {
+            class S extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:linearData_x", this.value_changed, this)
+                    k(this), this.model.on("change:linearData_x", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("linearData_x"),
-                        a = this.model.get("linearData_y"),
+                plot() {
+                    const e = this.model.get("linearData_x"),
+                        t = this.model.get("linearData_y"),
                         n = this.model.get("histogramData"),
-                        i = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o) {
-                            var l = 375,
-                                s = 720;
-                            n ? (s = (n = document.getElementById(n)).clientWidth, l = n.clientHeight) : n = o.el, r.select(n).selectAll("*").remove();
-                            const d = s - 40 - 20,
-                                c = l - 20 - 30,
-                                u = l / 5 - 20 - 30,
-                                m = Math.min(r.min(e), r.min(a)),
-                                p = Math.max(r.max(e), r.max(a)),
-                                h = r.scaleLinear().range([0, d]),
-                                v = r.scaleLinear().range([c, 0]),
-                                g = r.scaleLinear().range([u, 0]),
-                                f = r.axisBottom(h),
-                                _ = r.axisLeft(v),
-                                x = r.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(a),
-                                y = r.select(n).append("svg").attr("width", d + 40 + 20).attr("height", c + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            h.domain([m, p]), v.domain(r.extent(t)), g.domain([0, r.max(x, (e => e.length))]);
-                            const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                            var w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                            y.append("g").attr("transform", "translate(0," + c + ")").call(f).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), y.append("g").call(_).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", r.line().x((e => h((e.x1 + e.x0) / 2))).y((e => g(e.length) + c - u)).curve(r.curveCatmullRom));
-                            var k = e.map(((e, a) => [e, t[a]])).map((([e, t]) => ({
-                                x: e,
-                                y: t
-                            })));
-                            y.append("path").datum(k).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", r.line().x((e => h(e.x))).y((e => v(e.y)))), y.selectAll("myCircles").data(k).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => h(e.x))).attr("cy", (e => v(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
-                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
-                            })).on("mouseout", (function() {
-                                b.style("opacity", 0), w.style("opacity", 0)
-                            })).on("click", (function(e, t) {
-                                const a = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
-                                void 0 !== i && i(a, o)
-                            }))
-                        }(t, a, n, i, this.setValue, e)
-                    }), 50)
+                        a = this.model.get("elementId");
+                    let i = b,
+                        o = this.el;
+                    a && (o = document.getElementById(a), i = o.clientHeight);
+                    let s = o.clientWidth;
+                    const l = w;
+                    ! function(e, t, n, a, i, o, s, l) {
+                        const d = o - l.left - l.right,
+                            c = s - l.top - l.bottom,
+                            m = c / 4;
+                        r.select(a).selectAll("*").remove();
+                        const u = Math.min(r.min(e), r.min(n)),
+                            p = Math.max(r.max(e), r.max(n)),
+                            h = r.scaleLinear().range([0, d]),
+                            f = r.scaleLinear().range([c, 0]),
+                            g = r.scaleLinear().range([m, 0]),
+                            v = r.axisBottom(h),
+                            _ = r.axisLeft(f),
+                            x = r.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
+                            y = r.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
+                        h.domain([u, p]), f.domain(r.extent(t)), g.domain([0, r.max(x, (e => e.length))]);
+                        const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                        y.append("g").attr("transform", "translate(0," + c + ")").call(v).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), y.append("g").call(_).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.append("path").datum(x).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", r.line().x((e => h((e.x1 + e.x0) / 2))).y((e => g(e.length) + c - m)).curve(r.curveCatmullRom));
+                        const k = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
+                            x: e,
+                            y: t
+                        })));
+                        y.append("path").datum(k).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", r.line().x((e => h(e.x))).y((e => f(e.y)))), y.selectAll("myCircles").data(k).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => h(e.x))).attr("cy", (e => f(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
+                            b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                        })).on("mouseout", (function() {
+                            b.style("opacity", 0), w.style("opacity", 0)
+                        })).on("click", (function(e, t) {
+                            const n = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
+                            void 0 !== i && i(n)
+                        }))
+                    }(e, t, n, o, this.setValue.bind(this), s, i, l)
                 }
-                setValue(e, t) {
-                    t.model.set({
+                setValue(e) {
+                    this.model.set({
                         clickedValue: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
             }
-            class k extends n.DOMWidgetModel {
+            class A extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: k.model_name,
-                        _view_name: k.view_name,
-                        _model_module: k.model_module,
-                        _view_module: k.view_module,
-                        _model_module_version: k.model_module_version,
-                        _view_module_version: k.view_module_version,
+                        _model_name: A.model_name,
+                        _view_name: A.view_name,
+                        _model_module: A.model_module,
+                        _view_module: A.view_module,
+                        _model_module_version: A.model_module_version,
+                        _view_module_version: A.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
-                        element: String,
+                        elementId: String,
                         clickedValue: String,
                         selectedValues: []
                     }
                 }
                 static model_name = "ScatterplotModel";
                 static model_module = y.name;
                 static model_module_version = y.version;
                 static view_name = "ScatterplotView";
                 static view_module = y.name;
                 static view_module_version = y.version
             }
-            class M extends n.DOMWidgetView {
+            class E extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("y"),
-                        i = this.model.get("hue"),
-                        o = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o, l, s) {
-                            for (let t = 0; t < e.length; t++) e[t].id = t;
-                            var d = Math.floor(Math.random() * Date.now() * 1e4).toString(36),
-                                c = 375,
-                                u = 720;
-                            i ? (u = (i = document.getElementById(i)).clientWidth, c = i.clientHeight) : i = s.el, r.select(i).selectAll("*").remove();
-                            const m = u - 40 - 20,
-                                p = c - 20 - 30;
-                            var h = r.scaleLinear().range([0, m]),
-                                v = r.scaleLinear().range([p, 0]),
-                                g = r.scaleOrdinal(r.schemeCategory10),
-                                f = r.axisBottom(h),
-                                _ = r.axisLeft(v),
-                                x = r.select(i).append("svg").attr("width", m + 40 + 20).attr("height", p + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            h.domain(r.extent(e, (function(e) {
-                                    return e[t]
-                                }))).nice(), v.domain(r.extent(e, (function(e) {
-                                    return e[a]
-                                }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + p + ")").call(f).append("text").attr("class", "label").attr("x", m).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(_).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
-                                    return "dot-" + d + e.id
-                                })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
-                                    return h(e[t])
-                                })).attr("cy", (function(e) {
-                                    return v(e[a])
-                                })).style("fill", (function(e) {
-                                    return g(e[n])
-                                })).on("mouseover", (function(e, n) {
-                                    b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * n[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * n[a]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
-                                })).on("mouseout", (function() {
-                                    b.style("opacity", 0), w.style("opacity", 0)
-                                })).on("click", (function(e, n) {
-                                    const r = "x:" + Math.round(10 * n[t]) / 10 + "    y:" + Math.round(10 * n[a]) / 10;
-                                    void 0 !== o && o(r, s)
-                                })),
-                                function(e, t, a, n, i, o, l, s, d, c) {
-                                    let u = [];
-                                    const m = r.line(),
-                                        p = r.select(e).selectAll(".dot"),
-                                        h = r.drag().on("start", (function() {
-                                            u = [], s(), r.select(e).select("svg").append("path").attr("id", "lasso" + c)
-                                        })).on("drag", (function(e) {
-                                            let t = e.sourceEvent.offsetX,
-                                                a = e.sourceEvent.offsetY;
-                                            u.push([t, a]), r.select("#lasso" + c).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(u))
-                                        })).on("end", (function() {
-                                            let e = [];
-                                            p.each(((s, d) => {
-                                                (function(e, t) {
-                                                    for (var a = e[0], n = e[1], r = !1, i = 0, o = t.length - 1; i < t.length; o = i++) {
-                                                        var l = t[i][0],
-                                                            s = t[i][1],
-                                                            d = t[o][0],
-                                                            c = t[o][1];
-                                                        s > n != c > n && a < (d - l) * (n - s) / (c - s) + l && (r = !r)
-                                                    }
-                                                    return r
-                                                })([t(s[n]) + o, a(s[i]) + l], u) && (r.select("#dot-" + c + s.id).style("fill", "red").attr("r", 6), e.push(s))
-                                            })), r.select("#lasso" + c).remove(), d(e)
-                                        }));
-                                    r.select(e).call(h)
-                                }(i, h, v, t, a, 40, 20, (function() {
-                                    x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
-                                        return g(e[n])
-                                    }))
-                                }), (function(e) {
-                                    void 0 !== l && l(e, s)
-                                }), d);
-                            var y = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
-                                return "translate(0," + 20 * t + ")"
-                            }));
-                            y.append("rect").attr("x", m - 18).attr("width", 18).attr("height", 18).style("fill", g), y.append("text").attr("x", m - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
-                                return e
-                            }));
-                            const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                            var w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
-                        }(t, a, n, i, o, this.setValue, this.setSelectedValues, e)
-                    }), 50)
+                        a = this.model.get("hue"),
+                        i = this.model.get("elementId");
+                    let o = b,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight);
+                    let l = s.clientWidth;
+                    const d = w;
+                    ! function(e, t, n, a, i, o, s, l, d, c) {
+                        const m = l - c.left - c.right,
+                            u = d - c.top - c.bottom;
+                        for (let t = 0; t < e.length; t++) e[t].id = t;
+                        const p = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        r.select(i).selectAll("*").remove();
+                        const h = r.scaleLinear().range([0, m]),
+                            f = r.scaleLinear().range([u, 0]),
+                            g = r.scaleOrdinal(r.schemeCategory10),
+                            v = r.axisBottom(h),
+                            _ = r.axisLeft(f),
+                            x = r.select(i).append("svg").attr("width", l).attr("height", d).append("g").attr("transform", "translate(" + c.left + "," + c.top + ")");
+                        h.domain(r.extent(e, (function(e) {
+                                return e[t]
+                            }))).nice(), f.domain(r.extent(e, (function(e) {
+                                return e[n]
+                            }))).nice(), x.append("g").attr("class", "x axis").attr("transform", "translate(0," + u + ")").call(v).append("text").attr("class", "label").attr("x", m).attr("y", -6).style("text-anchor", "end"), x.append("g").attr("class", "y axis").call(_).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                                return "dot-" + p + e.id
+                            })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
+                                return h(e[t])
+                            })).attr("cy", (function(e) {
+                                return f(e[n])
+                            })).style("fill", (function(e) {
+                                return g(e[a])
+                            })).on("mouseover", (function(e, a) {
+                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                            })).on("mouseout", (function() {
+                                b.style("opacity", 0), w.style("opacity", 0)
+                            })).on("click", (function(e, a) {
+                                const r = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
+                                void 0 !== o && o(r)
+                            })),
+                            function(e, t, n, a, i, o, s, l, d, c) {
+                                let m = [];
+                                const u = r.line(),
+                                    p = r.select(e).selectAll(".dot"),
+                                    h = r.drag().on("start", (function() {
+                                        m = [], l(), r.select(e).select("svg").append("path").attr("id", "lasso" + c)
+                                    })).on("drag", (function(e) {
+                                        let t = e.sourceEvent.offsetX,
+                                            n = e.sourceEvent.offsetY;
+                                        m.push([t, n]), r.select("#lasso" + c).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", u(m))
+                                    })).on("end", (function() {
+                                        let e = [];
+                                        p.each(((l, d) => {
+                                            (function(e, t) {
+                                                for (var n = e[0], a = e[1], r = !1, i = 0, o = t.length - 1; i < t.length; o = i++) {
+                                                    var s = t[i][0],
+                                                        l = t[i][1],
+                                                        d = t[o][0],
+                                                        c = t[o][1];
+                                                    l > a != c > a && n < (d - s) * (a - l) / (c - l) + s && (r = !r)
+                                                }
+                                                return r
+                                            })([t(l[a]) + o, n(l[i]) + s], m) && (r.select("#dot-" + c + l.id).style("fill", "red").attr("r", 6), e.push(l))
+                                        })), r.select("#lasso" + c).remove(), d(e)
+                                    }));
+                                r.select(e).call(h)
+                            }(i, h, f, t, n, c.left, c.top, (function() {
+                                x.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
+                                    return g(e[a])
+                                }))
+                            }), (function(e) {
+                                void 0 !== s && s(e)
+                            }), p);
+                        const y = x.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                            return "translate(0," + 20 * t + ")"
+                        }));
+                        y.append("rect").attr("x", m - 18).attr("width", 18).attr("height", 18).style("fill", g), y.append("text").attr("x", m - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                            return e
+                        }));
+                        const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
+                    }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), l, o, d)
                 }
-                setValue(e, t) {
-                    t.model.set({
+                setValue(e) {
+                    this.model.set({
                         clickedValue: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
-                setSelectedValues(e, t) {
-                    t.model.set({
+                setSelectedValues(e) {
+                    this.model.set({
                         selectedValues: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
             }
-            class S extends n.DOMWidgetModel {
+            class L extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: S.model_name,
-                        _view_name: S.view_name,
-                        _model_module: S.model_module,
-                        _view_module: S.view_module,
-                        _model_module_version: S.model_module_version,
-                        _view_module_version: S.view_module_version,
+                        _model_name: L.model_name,
+                        _view_name: L.view_name,
+                        _model_module: L.model_module,
+                        _view_module: L.view_module,
+                        _model_module_version: L.model_module_version,
+                        _view_module_version: L.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
-                        element: String
+                        elementId: String
                     }
                 }
                 static model_name = "BarplotModel";
                 static model_module = y.name;
                 static model_module_version = y.version;
                 static view_name = "BarplotView";
                 static view_module = y.name;
                 static view_module_version = y.version
             }
-            class A extends n.DOMWidgetView {
+            class j extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("y"),
-                        o = this.model.get("hue"),
-                        l = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, o, l) {
-                            var s = 375,
-                                d = 720;
-                            o ? (d = (o = document.getElementById(o)).clientWidth, s = o.clientHeight) : o = l.el, r.select(o).selectAll("*").remove();
-                            const c = d - 40 - 20,
-                                u = s - 20 - 30;
-                            var m = r.select(o).append("svg").attr("width", c + 40 + 20).attr("height", u + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            n || (n = t);
-                            const p = e.reduce(((e, t) => (e && -1 === e.indexOf(t[n]) && e.push(t[n]), e)), []);
-                            let h = {};
-                            var v = r.scaleOrdinal(r.schemeCategory10);
-                            n == t ? function() {
-                                let n = e.reduce(((e, n) => {
-                                    let r = n[t],
-                                        i = n[a];
-                                    if (r in e) e[r] += i, h[r].qt += 1, h[r][a].push(i);
+                        a = this.model.get("hue"),
+                        o = this.model.get("elementId");
+                    let s = b,
+                        l = this.el;
+                    o && (l = document.getElementById(o), s = l.clientHeight),
+                        function(e, t, n, a, o, s, l, d) {
+                            const c = s - d.left - d.right,
+                                m = l - d.top - d.bottom;
+                            r.select(o).selectAll("*").remove();
+                            const u = r.select(o).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
+                            a || (a = t);
+                            const p = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
+                                h = {},
+                                f = r.scaleOrdinal(r.schemeCategory10);
+                            a == t ? function() {
+                                let a = e.reduce(((e, a) => {
+                                    const r = a[t],
+                                        i = a[n];
+                                    if (r in e) e[r] += i, h[r].qt += 1, h[r][n].push(i);
                                     else {
-                                        var o = {
+                                        const t = {
                                             qt: 1
                                         };
-                                        o[a] = [], o[a].push(i), h[r] = o, e[r] = i
+                                        t[n] = [], t[n].push(i), h[r] = t, e[r] = i
                                     }
                                     return e
                                 }), {});
-                                n = Object.keys(n).map((e => {
-                                    let r = {};
-                                    return r[t] = e, r[a] = n[e], 0 != h[e].qt && (r[a] = r[a] / h[e].qt), r
+                                a = Object.keys(a).map((e => {
+                                    const r = {};
+                                    return r[t] = e, r[n] = a[e], 0 != h[e].qt && (r[n] = r[n] / h[e].qt), r
                                 })), Object.keys(h).forEach((e => {
-                                    let t = h[e][a],
-                                        [n, r] = i(t);
-                                    h[e].min = n, h[e].max = r
+                                    const t = h[e][n],
+                                        [a, r] = i(t);
+                                    h[e].min = a, h[e].max = r
                                 }));
-                                var o = n.map((e => e[t]));
-                                let l = [],
-                                    s = Object.keys(h).map((e => h[e]));
-                                l.push(r.min(s, (e => e.min))), l.push(r.max(s, (e => e.max))), l[0] > 0 && l[1] > 0 ? l[0] = 0 : l[0] < 0 && l[1] < 0 && (l[1] = 0);
-                                var d = r.scaleLinear().domain(l).range([u, 0]);
-                                m.append("g").call(r.axisLeft(d));
-                                var g = r.scaleBand().domain(o).range([0, c]).padding([.2]);
-                                m.append("g").selectAll("g").data(n).enter().append("rect").attr("x", (function(e) {
+                                const o = a.map((e => e[t])),
+                                    s = [],
+                                    l = Object.keys(h).map((e => h[e]));
+                                s.push(r.min(l, (e => e.min))), s.push(r.max(l, (e => e.max))), s[0] > 0 && s[1] > 0 ? s[0] = 0 : s[0] < 0 && s[1] < 0 && (s[1] = 0);
+                                const d = r.scaleLinear().domain(s).range([m, 0]);
+                                u.append("g").call(r.axisLeft(d));
+                                const g = r.scaleBand().domain(o).range([0, c]).padding([.2]);
+                                u.append("g").selectAll("g").data(a).enter().append("rect").attr("x", (function(e) {
                                     return g(e[t])
                                 })).attr("y", (function(e) {
-                                    return d(e[a]) < d(0) ? d(e[a]) : d(0)
+                                    return d(e[n]) < d(0) ? d(e[n]) : d(0)
                                 })).attr("width", g.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(d(0) - d(e[a]))
+                                    return Math.abs(d(0) - d(e[n]))
                                 })).data(p).attr("fill", (function(e) {
-                                    return v(e)
+                                    return f(e)
                                 }));
-                                const f = Object.keys(h).map((e => {
-                                    let a = {};
-                                    return a[t] = e, a.min = h[e].min, a.max = h[e].max, a
+                                const v = Object.keys(h).map((e => {
+                                    const n = {};
+                                    return n[t] = e, n.min = h[e].min, n.max = h[e].max, n
                                 }));
-                                m.append("g").selectAll("g").data(f).enter().append("rect").attr("x", (function(e) {
+                                u.append("g").selectAll("g").data(v).enter().append("rect").attr("x", (function(e) {
                                     return g(e[t]) + g.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
                                     return d(e.max)
                                 })).attr("width", 2).attr("height", (function(e) {
                                     return d(e.min) - d(e.max)
-                                })), m.append("g").style("font", "18px times").attr("transform", "translate(0," + d(0) + ")").call(r.axisBottom(g).tickSize(0))
+                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + d(0) + ")").call(r.axisBottom(g).tickSize(0))
                             }() : function() {
                                 let o = e.reduce(((e, r) => {
-                                    let i = r[t],
-                                        o = r[a],
-                                        l = r[n];
+                                    const i = r[t],
+                                        o = r[n],
+                                        s = r[a];
                                     if (i in e) {
-                                        h[i].qt[a + "-" + l] += 1, h[i][l][a].push(o);
-                                        for (let t of p) l == t && (e[i][a + "-" + t] += o)
+                                        h[i].qt[n + "-" + s] += 1, h[i][s][n].push(o);
+                                        for (const t of p) s == t && (e[i][n + "-" + t] += o)
                                     } else {
-                                        var s = {};
+                                        const t = {};
                                         p.forEach((e => {
-                                            s[e] = {}, s[e][a] = []
+                                            t[e] = {}, t[e][n] = []
                                         }));
-                                        var d = {};
-                                        for (let e of p) d[a + "-" + e] = 0;
-                                        d[a + "-" + l] = 1, s.qt = d, s[l][a].push(o), h[i] = s;
-                                        let t = {};
-                                        for (var c of p) t[a + "-" + c] = l == c ? o : 0;
-                                        e[i] = t
+                                        const a = {};
+                                        for (const e of p) a[n + "-" + e] = 0;
+                                        a[n + "-" + s] = 1, t.qt = a, t[s][n].push(o), h[i] = t;
+                                        const r = {};
+                                        for (const e of p) r[n + "-" + e] = s == e ? o : 0;
+                                        e[i] = r
                                     }
                                     return e
                                 }), {});
                                 o = Object.keys(o).map((e => {
-                                    let a = {};
-                                    a[t] = e;
-                                    for (let t of Object.keys(o[e])) 0 != h[e].qt[t] && (o[e][t] = o[e][t] / h[e].qt[t]);
-                                    return a = {
-                                        ...a,
+                                    let n = {};
+                                    n[t] = e;
+                                    for (const t of Object.keys(o[e])) 0 != h[e].qt[t] && (o[e][t] = o[e][t] / h[e].qt[t]);
+                                    return n = {
+                                        ...n,
                                         ...o[e]
-                                    }, a
+                                    }, n
                                 })), Object.keys(h).forEach((e => {
                                     p.forEach((t => {
-                                        let n = h[e][t][a],
-                                            [r, o] = i(n);
+                                        const a = h[e][t][n],
+                                            [r, o] = i(a);
                                         h[e][t].min = r, h[e][t].max = o
                                     }))
                                 }));
-                                var l = p.map((e => a + "-" + e)),
-                                    s = o.map((e => e[t]));
-                                let d = [];
+                                const s = p.map((e => n + "-" + e)),
+                                    l = o.map((e => e[t])),
+                                    d = [];
                                 Object.keys(h).map((e => {
                                     p.forEach((t => d.push(h[e][t])))
                                 }));
-                                let g = [];
+                                const g = [];
                                 g.push(r.min(d, (e => e.min))), g.push(r.max(d, (e => e.max))), g[0] > 0 && g[1] > 0 ? g[0] = 0 : g[0] < 0 && g[1] < 0 && (g[1] = 0);
-                                var f = r.scaleLinear().domain(g).range([u, 0]);
-                                m.append("g").call(r.axisLeft(f));
-                                var _ = r.scaleBand().domain(s).range([0, c]).padding([.2]),
-                                    x = r.scaleBand().domain(l).range([0, _.bandwidth()]).padding([.05]);
-                                m.append("g").selectAll("g").data(o).enter().append("g").attr("transform", (function(e) {
+                                const v = r.scaleLinear().domain(g).range([m, 0]);
+                                u.append("g").call(r.axisLeft(v));
+                                const _ = r.scaleBand().domain(l).range([0, c]).padding([.2]),
+                                    x = r.scaleBand().domain(s).range([0, _.bandwidth()]).padding([.05]);
+                                u.append("g").selectAll("g").data(o).enter().append("g").attr("transform", (function(e) {
                                     return "translate(" + _(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
-                                    return l.map((function(t) {
+                                    return s.map((function(t) {
                                         return {
                                             key: t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
                                     return x(e.key)
                                 })).attr("y", (function(e) {
-                                    return f(e.value) < f(0) ? f(e.value) : f(0)
+                                    return v(e.value) < v(0) ? v(e.value) : v(0)
                                 })).attr("width", x.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(f(0) - f(e.value))
+                                    return Math.abs(v(0) - v(e.value))
                                 })).data(p).attr("fill", (function(e) {
-                                    return v(e)
+                                    return f(e)
                                 }));
                                 const y = Object.keys(h).map((e => {
-                                    let a = {};
-                                    return a[t] = e, a = {
-                                        ...a,
+                                    let n = {};
+                                    return n[t] = e, n = {
+                                        ...n,
                                         ...h[e]
-                                    }, a
+                                    }, n
                                 }));
-                                m.append("g").selectAll("g").data(y).enter().append("g").attr("transform", (function(e) {
+                                u.append("g").selectAll("g").data(y).enter().append("g").attr("transform", (function(e) {
                                     return "translate(" + _(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
                                     return p.map((function(t) {
                                         return {
-                                            key: a + "-" + t,
+                                            key: n + "-" + t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
                                     return x(e.key) + x.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
-                                    return e.value.max ? f(e.value.max) : 0
+                                    return e.value.max ? v(e.value.max) : 0
                                 })).attr("width", 2).attr("height", (function(e) {
-                                    return e.value.min && e.value.max ? f(e.value.min) - f(e.value.max) : 0
+                                    return e.value.min && e.value.max ? v(e.value.min) - v(e.value.max) : 0
                                 }));
-                                var b = m.selectAll(".legend").data(v.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                const b = u.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                     return "translate(0," + 20 * t + ")"
                                 }));
-                                b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", v), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", f), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                     return e
-                                })), m.append("g").style("font", "18px times").attr("transform", "translate(0," + f(0) + ")").call(r.axisBottom(_).tickSize(0))
+                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + v(0) + ")").call(r.axisBottom(_).tickSize(0))
                             }()
-                        }(t, a, n, o, l, e)
-                    }), 50)
+                        }(e, t, n, a, l, l.clientWidth, s, w)
                 }
             }
-            class j extends n.DOMWidgetModel {
+            class D extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: j.model_name,
-                        _view_name: j.view_name,
-                        _model_module: j.model_module,
-                        _view_module: j.view_module,
-                        _model_module_version: j.model_module_version,
-                        _view_module_version: j.view_module_version,
+                        _model_name: D.model_name,
+                        _view_name: D.view_name,
+                        _model_module: D.model_module,
+                        _view_module: D.view_module,
+                        _model_module_version: D.model_module_version,
+                        _view_module_version: D.view_module_version,
                         data: [],
                         x: String,
                         start: Number,
                         end: Number,
-                        element: String
+                        elementId: String
                     }
                 }
                 static model_name = "HistogramplotModel";
                 static model_module = y.name;
                 static model_module_version = y.version;
                 static view_name = "HistogramplotView";
                 static view_module = y.name;
                 static view_module_version = y.version
             }
-            class D extends n.DOMWidgetView {
+            class V extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    k(this), this.model.on("change:data", (() => k(this)), this), window.addEventListener("resize", (() => k(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("start"),
-                        i = this.model.get("end"),
-                        o = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o) {
-                            var l = 375,
-                                s = 720;
-                            i ? (s = (i = document.getElementById(i)).clientWidth, l = i.clientHeight) : i = o.el, r.select(i).selectAll("*").remove();
-                            const d = s - 40 - 20,
-                                c = l - 20 - 30;
-                            let u = a;
-                            a || (u = r.min(e, (e => e[t])));
+                        a = this.model.get("end"),
+                        i = this.model.get("elementId");
+                    let o = b,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight),
+                        function(e, t, n, a, i, o, s, l) {
+                            const d = o - l.left - l.right,
+                                c = s - l.top - l.bottom;
+                            r.select(i).selectAll("*").remove();
                             let m = n;
-                            n || (m = r.max(e, (e => e[t])));
+                            n || (m = r.min(e, (e => e[t])));
+                            let u = a;
+                            a || (u = r.max(e, (e => e[t])));
                             const p = r.scaleLinear().range([0, d]),
                                 h = r.scaleLinear().range([c, 0]),
-                                v = r.axisBottom(p),
+                                f = r.axisBottom(p),
                                 g = r.axisLeft(h),
-                                f = r.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
-                                _ = r.select(i).append("svg").attr("width", d + 40 + 20).attr("height", c + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            p.domain([u, m]), h.domain([0, r.max(f, (e => e.length))]), _.append("g").attr("transform", "translate(0," + c + ")").call(v).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), _.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), _.append("g").attr("fill", "steelblue").selectAll().data(f).join("rect").attr("x", (e => p(e.x0) + 1)).attr("width", (e => p(e.x1) - p(e.x0) - 1)).attr("y", (e => h(e.length))).attr("height", (e => h(0) - h(e.length)))
-                        }(t, a, n, i, o, e)
-                    }), 50)
+                                v = r.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
+                                _ = r.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
+                            p.domain([m, u]), h.domain([0, r.max(v, (e => e.length))]), _.append("g").attr("transform", "translate(0," + c + ")").call(f).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), _.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), _.append("g").attr("fill", "steelblue").selectAll().data(v).join("rect").attr("x", (e => p(e.x0) + 1)).attr("width", (e => p(e.x1) - p(e.x0) - 1)).attr("y", (e => h(e.length))).attr("height", (e => h(0) - h(e.length)))
+                        }(e, t, n, a, s, s.clientWidth, o, w)
                 }
             }
-            class E extends n.DOMWidgetModel {
+            class O extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: E.model_name,
-                        _view_name: E.view_name,
-                        _model_module: E.model_module,
-                        _view_module: E.view_module,
-                        _model_module_version: E.model_module_version,
-                        _view_module_version: E.view_module_version,
+                        _model_name: O.model_name,
+                        _view_name: O.view_name,
+                        _model_module: O.model_module,
+                        _view_module: O.view_module,
+                        _model_module_version: O.model_module_version,
+                        _view_module_version: O.view_module_version,
                         matrix: [],
                         grid_areas: [],
                         grid_template_areas: String,
                         style: String
                     }
                 }
                 static model_name = "EmbeddingModel";
                 static model_module = y.name;
                 static model_module_version = y.version;
                 static view_name = "EmbeddingView";
                 static view_module = y.name;
                 static view_module_version = y.version
             }
-            class V extends n.DOMWidgetView {
+            class I extends a.DOMWidgetView {
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    this.value_changed()
                 }
                 value_changed() {
-                    var e = this.model.get("matrix"),
+                    const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
-                        a = this.model.get("grid_template_areas"),
-                        n = this.model.get("style");
-                    n || (n = "basic");
+                        n = this.model.get("grid_template_areas");
+                    let a = this.model.get("style");
+                    a || (a = "basic");
                     const r = document.createElement("div");
-                    r.classList.add(n), r.style.display = "grid", r.style.gridTemplateAreas = a, r.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", r.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", r.style.width = "100%", t.forEach((e => {
+                    r.classList.add(a), r.style.display = "grid", r.style.gridTemplateAreas = n, r.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", r.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", r.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), r.appendChild(t)
                     })), this.el.appendChild(r)
                 }
             }
-            var L = a(330)
+            var C = n(330)
         },
-        930: (e, t, a) => {
-            a.d(t, {
-                A: () => l
+        930: (e, t, n) => {
+            n.d(t, {
+                A: () => s
             });
-            var n = a(601),
-                r = a.n(n),
-                i = a(314),
-                o = a.n(i)()(r());
+            var a = n(601),
+                r = n.n(a),
+                i = n(314),
+                o = n.n(i)()(r());
             o.push([e.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
-            const l = o
+            const s = o
         },
         314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var a = "",
-                            n = void 0 !== t[5];
-                        return t[4] && (a += "@supports (".concat(t[4], ") {")), t[2] && (a += "@media ".concat(t[2], " {")), n && (a += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), a += e(t), n && (a += "}"), t[2] && (a += "}"), t[4] && (a += "}"), a
+                        var n = "",
+                            a = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), a && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), a && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, a, n, r, i) {
+                }, t.i = function(e, n, a, r, i) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
                     var o = {};
-                    if (n)
-                        for (var l = 0; l < this.length; l++) {
-                            var s = this[l][0];
-                            null != s && (o[s] = !0)
+                    if (a)
+                        for (var s = 0; s < this.length; s++) {
+                            var l = this[s][0];
+                            null != l && (o[l] = !0)
                         }
                     for (var d = 0; d < e.length; d++) {
                         var c = [].concat(e[d]);
-                        n && o[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), a && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = a) : c[2] = a), r && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = r) : c[4] = "".concat(r)), t.push(c))
+                        a && o[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), r && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = r) : c[4] = "".concat(r)), t.push(c))
                     }
                 }, t
             }
         },
         601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
         72: e => {
             var t = [];
 
-            function a(e) {
-                for (var a = -1, n = 0; n < t.length; n++)
-                    if (t[n].identifier === e) {
-                        a = n;
+            function n(e) {
+                for (var n = -1, a = 0; a < t.length; a++)
+                    if (t[a].identifier === e) {
+                        n = a;
                         break
-                    } return a
+                    } return n
             }
 
-            function n(e, n) {
-                for (var i = {}, o = [], l = 0; l < e.length; l++) {
-                    var s = e[l],
-                        d = n.base ? s[0] + n.base : s[0],
+            function a(e, a) {
+                for (var i = {}, o = [], s = 0; s < e.length; s++) {
+                    var l = e[s],
+                        d = a.base ? l[0] + a.base : l[0],
                         c = i[d] || 0,
-                        u = "".concat(d, " ").concat(c);
+                        m = "".concat(d, " ").concat(c);
                     i[d] = c + 1;
-                    var m = a(u),
+                    var u = n(m),
                         p = {
-                            css: s[1],
-                            media: s[2],
-                            sourceMap: s[3],
-                            supports: s[4],
-                            layer: s[5]
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
                         };
-                    if (-1 !== m) t[m].references++, t[m].updater(p);
+                    if (-1 !== u) t[u].references++, t[u].updater(p);
                     else {
-                        var h = r(p, n);
-                        n.byIndex = l, t.splice(l, 0, {
-                            identifier: u,
+                        var h = r(p, a);
+                        a.byIndex = s, t.splice(s, 0, {
+                            identifier: m,
                             updater: h,
                             references: 1
                         })
                     }
-                    o.push(u)
+                    o.push(m)
                 }
                 return o
             }
 
             function r(e, t) {
-                var a = t.domAPI(t);
-                return a.update(e),
+                var n = t.domAPI(t);
+                return n.update(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
-                            a.update(e = t)
-                        } else a.remove()
+                            n.update(e = t)
+                        } else n.remove()
                     }
             }
             e.exports = function(e, r) {
-                var i = n(e = e || [], r = r || {});
+                var i = a(e = e || [], r = r || {});
                 return function(e) {
                     e = e || [];
                     for (var o = 0; o < i.length; o++) {
-                        var l = a(i[o]);
-                        t[l].references--
+                        var s = n(i[o]);
+                        t[s].references--
                     }
-                    for (var s = n(e, r), d = 0; d < i.length; d++) {
-                        var c = a(i[d]);
+                    for (var l = a(e, r), d = 0; d < i.length; d++) {
+                        var c = n(i[d]);
                         0 === t[c].references && (t[c].updater(), t.splice(c, 1))
                     }
-                    i = s
+                    i = l
                 }
             }
         },
         659: e => {
             var t = {};
-            e.exports = function(e, a) {
-                var n = function(e) {
+            e.exports = function(e, n) {
+                var a = function(e) {
                     if (void 0 === t[e]) {
-                        var a = document.querySelector(e);
-                        if (window.HTMLIFrameElement && a instanceof window.HTMLIFrameElement) try {
-                            a = a.contentDocument.head
+                        var n = document.querySelector(e);
+                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                            n = n.contentDocument.head
                         } catch (e) {
-                            a = null
+                            n = null
                         }
-                        t[e] = a
+                        t[e] = n
                     }
                     return t[e]
                 }(e);
-                if (!n) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                n.appendChild(a)
+                if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                a.appendChild(n)
             }
         },
         540: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
-        56: (e, t, a) => {
+        56: (e, t, n) => {
             e.exports = function(e) {
-                var t = a.nc;
+                var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
         825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
-                    update: function(a) {
-                        ! function(e, t, a) {
-                            var n = "";
-                            a.supports && (n += "@supports (".concat(a.supports, ") {")), a.media && (n += "@media ".concat(a.media, " {"));
-                            var r = void 0 !== a.layer;
-                            r && (n += "@layer".concat(a.layer.length > 0 ? " ".concat(a.layer) : "", " {")), n += a.css, r && (n += "}"), a.media && (n += "}"), a.supports && (n += "}");
-                            var i = a.sourceMap;
-                            i && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(n, e, t.options)
-                        }(t, e, a)
+                    update: function(n) {
+                        ! function(e, t, n) {
+                            var a = "";
+                            n.supports && (a += "@supports (".concat(n.supports, ") {")), n.media && (a += "@media ".concat(n.media, " {"));
+                            var r = void 0 !== n.layer;
+                            r && (a += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), a += n.css, r && (a += "}"), n.media && (a += "}"), n.supports && (a += "}");
+                            var i = n.sourceMap;
+                            i && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(a, e, t.options)
+                        }(t, e, n)
                     },
                     remove: function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
@@ -724,11 +737,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/493.e98395b66f4058ecc2a8.js` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/493.6062c0a7b585f6ae1d22.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,748 +1,761 @@
 "use strict";
 (self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || []).push([
     [493], {
-        380: (e, t, a) => {
-            a.r(t), a.d(t, {
-                BarPlotModel: () => S,
-                BarPlotView: () => A,
-                EmbeddingModel: () => E,
-                EmbeddingView: () => L,
-                HistogramPlotModel: () => V,
-                HistogramPlotView: () => P,
-                LinearHistPlotModel: () => b,
-                LinearHistPlotView: () => w,
-                ScatterPlotModel: () => M,
-                ScatterPlotView: () => k,
-                author: () => j.author,
-                dependencies: () => j.dependencies,
-                description: () => j.description,
-                devDependencies: () => j.devDependencies,
-                files: () => j.files,
-                jupyterlab: () => j.jupyterlab,
-                keywords: () => j.keywords,
-                license: () => j.license,
-                main: () => j.main,
-                name: () => j.name,
-                repository: () => j.repository,
-                scripts: () => j.scripts,
-                version: () => j.version
+        380: (e, t, n) => {
+            n.r(t), n.d(t, {
+                BarPlotModel: () => E,
+                BarPlotView: () => L,
+                EmbeddingModel: () => D,
+                EmbeddingView: () => I,
+                HistogramPlotModel: () => P,
+                HistogramPlotView: () => j,
+                LinearHistPlotModel: () => k,
+                LinearHistPlotView: () => S,
+                ScatterPlotModel: () => A,
+                ScatterPlotView: () => V,
+                author: () => O.author,
+                dependencies: () => O.dependencies,
+                description: () => O.description,
+                devDependencies: () => O.devDependencies,
+                files: () => O.files,
+                jupyterlab: () => O.jupyterlab,
+                keywords: () => O.keywords,
+                license: () => O.license,
+                main: () => O.main,
+                name: () => O.name,
+                repository: () => O.repository,
+                scripts: () => O.scripts,
+                version: () => O.version
             });
-            var n = a(801),
-                r = a(840);
+            var a = n(801),
+                r = n(840);
 
             function i(e) {
-                const t = e.reduce(((e, t) => e + t), 0) / e.length;
-                let a = 1.96 * function(e, t) {
-                    let a = 0;
-                    return e.forEach((e => a += (e - t) ** 2)), a = Math.sqrt(a) / e.length, a
-                }(e, t);
-                return [t - a, t + a]
-            }
-            var o = a(72),
-                l = a.n(o),
-                s = a(825),
-                d = a.n(s),
-                c = a(659),
-                u = a.n(c),
-                m = a(56),
-                p = a.n(m),
-                h = a(540),
-                v = a.n(h),
-                g = a(113),
-                f = a.n(g),
-                _ = a(930),
-                y = {};
-            y.styleTagTransform = f(), y.setAttributes = p(), y.insert = u().bind(null, "head"), y.domAPI = d(), y.insertStyleElement = v(), l()(_.A, y), _.A && _.A.locals && _.A.locals;
-            const x = a(330);
-            class b extends n.DOMWidgetModel {
+                const t = e.reduce(((e, t) => e + t), 0) / e.length,
+                    n = 1.96 * function(e, t) {
+                        let n = 0;
+                        return e.forEach((e => n += (e - t) ** 2)), n = Math.sqrt(n) / e.length, n
+                    }(e, t);
+                return [t - n, t + n]
+            }
+            var o = n(72),
+                s = n.n(o),
+                l = n(825),
+                d = n.n(l),
+                c = n(659),
+                m = n.n(c),
+                u = n(56),
+                p = n.n(u),
+                h = n(540),
+                f = n.n(h),
+                g = n(113),
+                v = n.n(g),
+                y = n(930),
+                _ = {};
+            _.styleTagTransform = v(), _.setAttributes = p(), _.insert = m().bind(null, "head"), _.domAPI = d(), _.insertStyleElement = f(), s()(y.A, _), y.A && y.A.locals && y.A.locals;
+            const x = n(330),
+                b = 400,
+                w = {
+                    top: 20,
+                    right: 20,
+                    bottom: 30,
+                    left: 40
+                };
+
+            function M(e) {
+                e.timeout && clearTimeout(e.timeout), e.timeout = setTimeout((() => {
+                    e.plot()
+                }), 100)
+            }
+            class k extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: b.model_name,
-                        _view_name: b.view_name,
-                        _model_module: b.model_module,
-                        _view_module: b.view_module,
-                        _model_module_version: b.model_module_version,
-                        _view_module_version: b.view_module_version,
+                        _model_name: k.model_name,
+                        _view_name: k.view_name,
+                        _model_module: k.model_module,
+                        _view_module: k.view_module,
+                        _model_module_version: k.model_module_version,
+                        _view_module_version: k.view_module_version,
                         linearData_x: [],
                         linearData_y: [],
                         histogramData: [],
-                        element: String,
+                        elementId: String,
                         clickedValue: String
                     }
                 }
                 static model_name = "LinearHistPlotModel";
                 static model_module = x.name;
                 static model_module_version = x.version;
                 static view_name = "LinearHistPlotView";
                 static view_module = x.name;
                 static view_module_version = x.version
             }
-            class w extends n.DOMWidgetView {
+            class S extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:linearData_x", this.value_changed, this)
+                    M(this), this.model.on("change:linearData_x", (() => M(this)), this), window.addEventListener("resize", (() => M(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("linearData_x"),
-                        a = this.model.get("linearData_y"),
+                plot() {
+                    const e = this.model.get("linearData_x"),
+                        t = this.model.get("linearData_y"),
                         n = this.model.get("histogramData"),
-                        i = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o) {
-                            var l = 375,
-                                s = 720;
-                            n ? (s = (n = document.getElementById(n)).clientWidth, l = n.clientHeight) : n = o.el, r.select(n).selectAll("*").remove();
-                            const d = s - 40 - 20,
-                                c = l - 20 - 30,
-                                u = l / 5 - 20 - 30,
-                                m = Math.min(r.min(e), r.min(a)),
-                                p = Math.max(r.max(e), r.max(a)),
-                                h = r.scaleLinear().range([0, d]),
-                                v = r.scaleLinear().range([c, 0]),
-                                g = r.scaleLinear().range([u, 0]),
-                                f = r.axisBottom(h),
-                                _ = r.axisLeft(v),
-                                y = r.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(a),
-                                x = r.select(n).append("svg").attr("width", d + 40 + 20).attr("height", c + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            h.domain([m, p]), v.domain(r.extent(t)), g.domain([0, r.max(y, (e => e.length))]);
-                            const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                            var w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                            x.append("g").attr("transform", "translate(0," + c + ")").call(f).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), x.append("g").call(_).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", r.line().x((e => h((e.x1 + e.x0) / 2))).y((e => g(e.length) + c - u)).curve(r.curveCatmullRom));
-                            var M = e.map(((e, a) => [e, t[a]])).map((([e, t]) => ({
-                                x: e,
-                                y: t
-                            })));
-                            x.append("path").datum(M).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", r.line().x((e => h(e.x))).y((e => v(e.y)))), x.selectAll("myCircles").data(M).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => h(e.x))).attr("cy", (e => v(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
-                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
-                            })).on("mouseout", (function() {
-                                b.style("opacity", 0), w.style("opacity", 0)
-                            })).on("click", (function(e, t) {
-                                const a = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
-                                void 0 !== i && i(a, o)
-                            }))
-                        }(t, a, n, i, this.setValue, e)
-                    }), 50)
+                        a = this.model.get("elementId");
+                    let i = b,
+                        o = this.el;
+                    a && (o = document.getElementById(a), i = o.clientHeight);
+                    let s = o.clientWidth;
+                    const l = w;
+                    ! function(e, t, n, a, i, o, s, l) {
+                        const d = o - l.left - l.right,
+                            c = s - l.top - l.bottom,
+                            m = c / 4;
+                        r.select(a).selectAll("*").remove();
+                        const u = Math.min(r.min(e), r.min(n)),
+                            p = Math.max(r.max(e), r.max(n)),
+                            h = r.scaleLinear().range([0, d]),
+                            f = r.scaleLinear().range([c, 0]),
+                            g = r.scaleLinear().range([m, 0]),
+                            v = r.axisBottom(h),
+                            y = r.axisLeft(f),
+                            _ = r.bin().thresholds(20).value((e => Math.round(10 * e) / 10))(n),
+                            x = r.select(a).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
+                        h.domain([u, p]), f.domain(r.extent(t)), g.domain([0, r.max(_, (e => e.length))]);
+                        const b = x.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = x.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                        x.append("g").attr("transform", "translate(0," + c + ")").call(v).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), x.append("g").call(y).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), x.append("path").datum(_).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", r.line().x((e => h((e.x1 + e.x0) / 2))).y((e => g(e.length) + c - m)).curve(r.curveCatmullRom));
+                        const M = e.map(((e, n) => [e, t[n]])).map((([e, t]) => ({
+                            x: e,
+                            y: t
+                        })));
+                        x.append("path").datum(M).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", r.line().x((e => h(e.x))).y((e => f(e.y)))), x.selectAll("myCircles").data(M).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (e => h(e.x))).attr("cy", (e => f(e.y))).attr("r", 3).on("mouseover", (function(e, t) {
+                            b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                        })).on("mouseout", (function() {
+                            b.style("opacity", 0), w.style("opacity", 0)
+                        })).on("click", (function(e, t) {
+                            const n = "x:" + Math.round(10 * t.x) / 10 + "  -  y:" + Math.round(10 * t.y) / 10;
+                            void 0 !== i && i(n)
+                        }))
+                    }(e, t, n, o, this.setValue.bind(this), s, i, l)
                 }
-                setValue(e, t) {
-                    t.model.set({
+                setValue(e) {
+                    this.model.set({
                         clickedValue: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
             }
-            class M extends n.DOMWidgetModel {
+            class A extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: M.model_name,
-                        _view_name: M.view_name,
-                        _model_module: M.model_module,
-                        _view_module: M.view_module,
-                        _model_module_version: M.model_module_version,
-                        _view_module_version: M.view_module_version,
+                        _model_name: A.model_name,
+                        _view_name: A.view_name,
+                        _model_module: A.model_module,
+                        _view_module: A.view_module,
+                        _model_module_version: A.model_module_version,
+                        _view_module_version: A.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
-                        element: String,
+                        elementId: String,
                         clickedValue: String,
                         selectedValues: []
                     }
                 }
                 static model_name = "ScatterplotModel";
                 static model_module = x.name;
                 static model_module_version = x.version;
                 static view_name = "ScatterplotView";
                 static view_module = x.name;
                 static view_module_version = x.version
             }
-            class k extends n.DOMWidgetView {
+            class V extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    M(this), this.model.on("change:data", (() => M(this)), this), window.addEventListener("resize", (() => M(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("y"),
-                        i = this.model.get("hue"),
-                        o = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o, l, s) {
-                            for (let t = 0; t < e.length; t++) e[t].id = t;
-                            var d = Math.floor(Math.random() * Date.now() * 1e4).toString(36),
-                                c = 375,
-                                u = 720;
-                            i ? (u = (i = document.getElementById(i)).clientWidth, c = i.clientHeight) : i = s.el, r.select(i).selectAll("*").remove();
-                            const m = u - 40 - 20,
-                                p = c - 20 - 30;
-                            var h = r.scaleLinear().range([0, m]),
-                                v = r.scaleLinear().range([p, 0]),
-                                g = r.scaleOrdinal(r.schemeCategory10),
-                                f = r.axisBottom(h),
-                                _ = r.axisLeft(v),
-                                y = r.select(i).append("svg").attr("width", m + 40 + 20).attr("height", p + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            h.domain(r.extent(e, (function(e) {
-                                    return e[t]
-                                }))).nice(), v.domain(r.extent(e, (function(e) {
-                                    return e[a]
-                                }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + p + ")").call(f).append("text").attr("class", "label").attr("x", m).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(_).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
-                                    return "dot-" + d + e.id
-                                })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
-                                    return h(e[t])
-                                })).attr("cy", (function(e) {
-                                    return v(e[a])
-                                })).style("fill", (function(e) {
-                                    return g(e[n])
-                                })).on("mouseover", (function(e, n) {
-                                    b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * n[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * n[a]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
-                                })).on("mouseout", (function() {
-                                    b.style("opacity", 0), w.style("opacity", 0)
-                                })).on("click", (function(e, n) {
-                                    const r = "x:" + Math.round(10 * n[t]) / 10 + "    y:" + Math.round(10 * n[a]) / 10;
-                                    void 0 !== o && o(r, s)
-                                })),
-                                function(e, t, a, n, i, o, l, s, d, c) {
-                                    let u = [];
-                                    const m = r.line(),
-                                        p = r.select(e).selectAll(".dot"),
-                                        h = r.drag().on("start", (function() {
-                                            u = [], s(), r.select(e).select("svg").append("path").attr("id", "lasso" + c)
-                                        })).on("drag", (function(e) {
-                                            let t = e.sourceEvent.offsetX,
-                                                a = e.sourceEvent.offsetY;
-                                            u.push([t, a]), r.select("#lasso" + c).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", m(u))
-                                        })).on("end", (function() {
-                                            let e = [];
-                                            p.each(((s, d) => {
-                                                (function(e, t) {
-                                                    for (var a = e[0], n = e[1], r = !1, i = 0, o = t.length - 1; i < t.length; o = i++) {
-                                                        var l = t[i][0],
-                                                            s = t[i][1],
-                                                            d = t[o][0],
-                                                            c = t[o][1];
-                                                        s > n != c > n && a < (d - l) * (n - s) / (c - s) + l && (r = !r)
-                                                    }
-                                                    return r
-                                                })([t(s[n]) + o, a(s[i]) + l], u) && (r.select("#dot-" + c + s.id).style("fill", "red").attr("r", 6), e.push(s))
-                                            })), r.select("#lasso" + c).remove(), d(e)
-                                        }));
-                                    r.select(e).call(h)
-                                }(i, h, v, t, a, 40, 20, (function() {
-                                    y.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
-                                        return g(e[n])
-                                    }))
-                                }), (function(e) {
-                                    void 0 !== l && l(e, s)
-                                }), d);
-                            var x = y.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
-                                return "translate(0," + 20 * t + ")"
-                            }));
-                            x.append("rect").attr("x", m - 18).attr("width", 18).attr("height", 18).style("fill", g), x.append("text").attr("x", m - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
-                                return e
-                            }));
-                            const b = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                            var w = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
-                        }(t, a, n, i, o, this.setValue, this.setSelectedValues, e)
-                    }), 50)
+                        a = this.model.get("hue"),
+                        i = this.model.get("elementId");
+                    let o = b,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight);
+                    let l = s.clientWidth;
+                    const d = w;
+                    ! function(e, t, n, a, i, o, s, l, d, c) {
+                        const m = l - c.left - c.right,
+                            u = d - c.top - c.bottom;
+                        for (let t = 0; t < e.length; t++) e[t].id = t;
+                        const p = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                        r.select(i).selectAll("*").remove();
+                        const h = r.scaleLinear().range([0, m]),
+                            f = r.scaleLinear().range([u, 0]),
+                            g = r.scaleOrdinal(r.schemeCategory10),
+                            v = r.axisBottom(h),
+                            y = r.axisLeft(f),
+                            _ = r.select(i).append("svg").attr("width", l).attr("height", d).append("g").attr("transform", "translate(" + c.left + "," + c.top + ")");
+                        h.domain(r.extent(e, (function(e) {
+                                return e[t]
+                            }))).nice(), f.domain(r.extent(e, (function(e) {
+                                return e[n]
+                            }))).nice(), _.append("g").attr("class", "x axis").attr("transform", "translate(0," + u + ")").call(v).append("text").attr("class", "label").attr("x", m).attr("y", -6).style("text-anchor", "end"), _.append("g").attr("class", "y axis").call(y).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), _.selectAll(".dot").data(e).enter().append("circle").attr("id", (function(e, t) {
+                                return "dot-" + p + e.id
+                            })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(e) {
+                                return h(e[t])
+                            })).attr("cy", (function(e) {
+                                return f(e[n])
+                            })).style("fill", (function(e) {
+                                return g(e[a])
+                            })).on("mouseover", (function(e, a) {
+                                b.style("opacity", 1), w.style("opacity", 1), b.attr("x", e.offsetX - 30).attr("y", e.offsetY - 40), w.html("x: " + Math.round(10 * a[t]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * a[n]) / 10).attr("x", e.offsetX - 15).attr("y", e.offsetY - 20)
+                            })).on("mouseout", (function() {
+                                b.style("opacity", 0), w.style("opacity", 0)
+                            })).on("click", (function(e, a) {
+                                const r = "x:" + Math.round(10 * a[t]) / 10 + "    y:" + Math.round(10 * a[n]) / 10;
+                                void 0 !== o && o(r)
+                            })),
+                            function(e, t, n, a, i, o, s, l, d, c) {
+                                let m = [];
+                                const u = r.line(),
+                                    p = r.select(e).selectAll(".dot"),
+                                    h = r.drag().on("start", (function() {
+                                        m = [], l(), r.select(e).select("svg").append("path").attr("id", "lasso" + c)
+                                    })).on("drag", (function(e) {
+                                        let t = e.sourceEvent.offsetX,
+                                            n = e.sourceEvent.offsetY;
+                                        m.push([t, n]), r.select("#lasso" + c).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", u(m))
+                                    })).on("end", (function() {
+                                        let e = [];
+                                        p.each(((l, d) => {
+                                            (function(e, t) {
+                                                for (var n = e[0], a = e[1], r = !1, i = 0, o = t.length - 1; i < t.length; o = i++) {
+                                                    var s = t[i][0],
+                                                        l = t[i][1],
+                                                        d = t[o][0],
+                                                        c = t[o][1];
+                                                    l > a != c > a && n < (d - s) * (a - l) / (c - l) + s && (r = !r)
+                                                }
+                                                return r
+                                            })([t(l[a]) + o, n(l[i]) + s], m) && (r.select("#dot-" + c + l.id).style("fill", "red").attr("r", 6), e.push(l))
+                                        })), r.select("#lasso" + c).remove(), d(e)
+                                    }));
+                                r.select(e).call(h)
+                            }(i, h, f, t, n, c.left, c.top, (function() {
+                                _.selectAll(".dot").data(e).attr("r", 3.5).style("fill", (function(e) {
+                                    return g(e[a])
+                                }))
+                            }), (function(e) {
+                                void 0 !== s && s(e)
+                            }), p);
+                        const x = _.selectAll(".legend").data(g.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                            return "translate(0," + 20 * t + ")"
+                        }));
+                        x.append("rect").attr("x", m - 18).attr("width", 18).attr("height", 18).style("fill", g), x.append("text").attr("x", m - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                            return e
+                        }));
+                        const b = _.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                            w = _.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
+                    }(e, t, n, a, s, this.setValue.bind(this), this.setSelectedValues.bind(this), l, o, d)
                 }
-                setValue(e, t) {
-                    t.model.set({
+                setValue(e) {
+                    this.model.set({
                         clickedValue: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
-                setSelectedValues(e, t) {
-                    t.model.set({
+                setSelectedValues(e) {
+                    this.model.set({
                         selectedValues: e
-                    }), t.model.save_changes()
+                    }), this.model.save_changes()
                 }
             }
-            class S extends n.DOMWidgetModel {
+            class E extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: S.model_name,
-                        _view_name: S.view_name,
-                        _model_module: S.model_module,
-                        _view_module: S.view_module,
-                        _model_module_version: S.model_module_version,
-                        _view_module_version: S.view_module_version,
+                        _model_name: E.model_name,
+                        _view_name: E.view_name,
+                        _model_module: E.model_module,
+                        _view_module: E.view_module,
+                        _model_module_version: E.model_module_version,
+                        _view_module_version: E.view_module_version,
                         data: [],
                         x: String,
                         y: String,
                         hue: String,
-                        element: String
+                        elementId: String
                     }
                 }
                 static model_name = "BarplotModel";
                 static model_module = x.name;
                 static model_module_version = x.version;
                 static view_name = "BarplotView";
                 static view_module = x.name;
                 static view_module_version = x.version
             }
-            class A extends n.DOMWidgetView {
+            class L extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    M(this), this.model.on("change:data", (() => M(this)), this), window.addEventListener("resize", (() => M(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("y"),
-                        o = this.model.get("hue"),
-                        l = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, o, l) {
-                            var s = 375,
-                                d = 720;
-                            o ? (d = (o = document.getElementById(o)).clientWidth, s = o.clientHeight) : o = l.el, r.select(o).selectAll("*").remove();
-                            const c = d - 40 - 20,
-                                u = s - 20 - 30;
-                            var m = r.select(o).append("svg").attr("width", c + 40 + 20).attr("height", u + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            n || (n = t);
-                            const p = e.reduce(((e, t) => (e && -1 === e.indexOf(t[n]) && e.push(t[n]), e)), []);
-                            let h = {};
-                            var v = r.scaleOrdinal(r.schemeCategory10);
-                            n == t ? function() {
-                                let n = e.reduce(((e, n) => {
-                                    let r = n[t],
-                                        i = n[a];
-                                    if (r in e) e[r] += i, h[r].qt += 1, h[r][a].push(i);
+                        a = this.model.get("hue"),
+                        o = this.model.get("elementId");
+                    let s = b,
+                        l = this.el;
+                    o && (l = document.getElementById(o), s = l.clientHeight),
+                        function(e, t, n, a, o, s, l, d) {
+                            const c = s - d.left - d.right,
+                                m = l - d.top - d.bottom;
+                            r.select(o).selectAll("*").remove();
+                            const u = r.select(o).append("svg").attr("width", s).attr("height", l).append("g").attr("transform", "translate(" + d.left + "," + d.top + ")");
+                            a || (a = t);
+                            const p = e.reduce(((e, t) => (e && -1 === e.indexOf(t[a]) && e.push(t[a]), e)), []),
+                                h = {},
+                                f = r.scaleOrdinal(r.schemeCategory10);
+                            a == t ? function() {
+                                let a = e.reduce(((e, a) => {
+                                    const r = a[t],
+                                        i = a[n];
+                                    if (r in e) e[r] += i, h[r].qt += 1, h[r][n].push(i);
                                     else {
-                                        var o = {
+                                        const t = {
                                             qt: 1
                                         };
-                                        o[a] = [], o[a].push(i), h[r] = o, e[r] = i
+                                        t[n] = [], t[n].push(i), h[r] = t, e[r] = i
                                     }
                                     return e
                                 }), {});
-                                n = Object.keys(n).map((e => {
-                                    let r = {};
-                                    return r[t] = e, r[a] = n[e], 0 != h[e].qt && (r[a] = r[a] / h[e].qt), r
+                                a = Object.keys(a).map((e => {
+                                    const r = {};
+                                    return r[t] = e, r[n] = a[e], 0 != h[e].qt && (r[n] = r[n] / h[e].qt), r
                                 })), Object.keys(h).forEach((e => {
-                                    let t = h[e][a],
-                                        [n, r] = i(t);
-                                    h[e].min = n, h[e].max = r
+                                    const t = h[e][n],
+                                        [a, r] = i(t);
+                                    h[e].min = a, h[e].max = r
                                 }));
-                                var o = n.map((e => e[t]));
-                                let l = [],
-                                    s = Object.keys(h).map((e => h[e]));
-                                l.push(r.min(s, (e => e.min))), l.push(r.max(s, (e => e.max))), l[0] > 0 && l[1] > 0 ? l[0] = 0 : l[0] < 0 && l[1] < 0 && (l[1] = 0);
-                                var d = r.scaleLinear().domain(l).range([u, 0]);
-                                m.append("g").call(r.axisLeft(d));
-                                var g = r.scaleBand().domain(o).range([0, c]).padding([.2]);
-                                m.append("g").selectAll("g").data(n).enter().append("rect").attr("x", (function(e) {
+                                const o = a.map((e => e[t])),
+                                    s = [],
+                                    l = Object.keys(h).map((e => h[e]));
+                                s.push(r.min(l, (e => e.min))), s.push(r.max(l, (e => e.max))), s[0] > 0 && s[1] > 0 ? s[0] = 0 : s[0] < 0 && s[1] < 0 && (s[1] = 0);
+                                const d = r.scaleLinear().domain(s).range([m, 0]);
+                                u.append("g").call(r.axisLeft(d));
+                                const g = r.scaleBand().domain(o).range([0, c]).padding([.2]);
+                                u.append("g").selectAll("g").data(a).enter().append("rect").attr("x", (function(e) {
                                     return g(e[t])
                                 })).attr("y", (function(e) {
-                                    return d(e[a]) < d(0) ? d(e[a]) : d(0)
+                                    return d(e[n]) < d(0) ? d(e[n]) : d(0)
                                 })).attr("width", g.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(d(0) - d(e[a]))
+                                    return Math.abs(d(0) - d(e[n]))
                                 })).data(p).attr("fill", (function(e) {
-                                    return v(e)
+                                    return f(e)
                                 }));
-                                const f = Object.keys(h).map((e => {
-                                    let a = {};
-                                    return a[t] = e, a.min = h[e].min, a.max = h[e].max, a
+                                const v = Object.keys(h).map((e => {
+                                    const n = {};
+                                    return n[t] = e, n.min = h[e].min, n.max = h[e].max, n
                                 }));
-                                m.append("g").selectAll("g").data(f).enter().append("rect").attr("x", (function(e) {
+                                u.append("g").selectAll("g").data(v).enter().append("rect").attr("x", (function(e) {
                                     return g(e[t]) + g.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
                                     return d(e.max)
                                 })).attr("width", 2).attr("height", (function(e) {
                                     return d(e.min) - d(e.max)
-                                })), m.append("g").style("font", "18px times").attr("transform", "translate(0," + d(0) + ")").call(r.axisBottom(g).tickSize(0))
+                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + d(0) + ")").call(r.axisBottom(g).tickSize(0))
                             }() : function() {
                                 let o = e.reduce(((e, r) => {
-                                    let i = r[t],
-                                        o = r[a],
-                                        l = r[n];
+                                    const i = r[t],
+                                        o = r[n],
+                                        s = r[a];
                                     if (i in e) {
-                                        h[i].qt[a + "-" + l] += 1, h[i][l][a].push(o);
-                                        for (let t of p) l == t && (e[i][a + "-" + t] += o)
+                                        h[i].qt[n + "-" + s] += 1, h[i][s][n].push(o);
+                                        for (const t of p) s == t && (e[i][n + "-" + t] += o)
                                     } else {
-                                        var s = {};
+                                        const t = {};
                                         p.forEach((e => {
-                                            s[e] = {}, s[e][a] = []
+                                            t[e] = {}, t[e][n] = []
                                         }));
-                                        var d = {};
-                                        for (let e of p) d[a + "-" + e] = 0;
-                                        d[a + "-" + l] = 1, s.qt = d, s[l][a].push(o), h[i] = s;
-                                        let t = {};
-                                        for (var c of p) t[a + "-" + c] = l == c ? o : 0;
-                                        e[i] = t
+                                        const a = {};
+                                        for (const e of p) a[n + "-" + e] = 0;
+                                        a[n + "-" + s] = 1, t.qt = a, t[s][n].push(o), h[i] = t;
+                                        const r = {};
+                                        for (const e of p) r[n + "-" + e] = s == e ? o : 0;
+                                        e[i] = r
                                     }
                                     return e
                                 }), {});
                                 o = Object.keys(o).map((e => {
-                                    let a = {};
-                                    a[t] = e;
-                                    for (let t of Object.keys(o[e])) 0 != h[e].qt[t] && (o[e][t] = o[e][t] / h[e].qt[t]);
-                                    return a = {
-                                        ...a,
+                                    let n = {};
+                                    n[t] = e;
+                                    for (const t of Object.keys(o[e])) 0 != h[e].qt[t] && (o[e][t] = o[e][t] / h[e].qt[t]);
+                                    return n = {
+                                        ...n,
                                         ...o[e]
-                                    }, a
+                                    }, n
                                 })), Object.keys(h).forEach((e => {
                                     p.forEach((t => {
-                                        let n = h[e][t][a],
-                                            [r, o] = i(n);
+                                        const a = h[e][t][n],
+                                            [r, o] = i(a);
                                         h[e][t].min = r, h[e][t].max = o
                                     }))
                                 }));
-                                var l = p.map((e => a + "-" + e)),
-                                    s = o.map((e => e[t]));
-                                let d = [];
+                                const s = p.map((e => n + "-" + e)),
+                                    l = o.map((e => e[t])),
+                                    d = [];
                                 Object.keys(h).map((e => {
                                     p.forEach((t => d.push(h[e][t])))
                                 }));
-                                let g = [];
+                                const g = [];
                                 g.push(r.min(d, (e => e.min))), g.push(r.max(d, (e => e.max))), g[0] > 0 && g[1] > 0 ? g[0] = 0 : g[0] < 0 && g[1] < 0 && (g[1] = 0);
-                                var f = r.scaleLinear().domain(g).range([u, 0]);
-                                m.append("g").call(r.axisLeft(f));
-                                var _ = r.scaleBand().domain(s).range([0, c]).padding([.2]),
-                                    y = r.scaleBand().domain(l).range([0, _.bandwidth()]).padding([.05]);
-                                m.append("g").selectAll("g").data(o).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + _(e[t]) + ",0)"
+                                const v = r.scaleLinear().domain(g).range([m, 0]);
+                                u.append("g").call(r.axisLeft(v));
+                                const y = r.scaleBand().domain(l).range([0, c]).padding([.2]),
+                                    _ = r.scaleBand().domain(s).range([0, y.bandwidth()]).padding([.05]);
+                                u.append("g").selectAll("g").data(o).enter().append("g").attr("transform", (function(e) {
+                                    return "translate(" + y(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
-                                    return l.map((function(t) {
+                                    return s.map((function(t) {
                                         return {
                                             key: t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return y(e.key)
+                                    return _(e.key)
                                 })).attr("y", (function(e) {
-                                    return f(e.value) < f(0) ? f(e.value) : f(0)
-                                })).attr("width", y.bandwidth()).attr("height", (function(e) {
-                                    return Math.abs(f(0) - f(e.value))
+                                    return v(e.value) < v(0) ? v(e.value) : v(0)
+                                })).attr("width", _.bandwidth()).attr("height", (function(e) {
+                                    return Math.abs(v(0) - v(e.value))
                                 })).data(p).attr("fill", (function(e) {
-                                    return v(e)
+                                    return f(e)
                                 }));
                                 const x = Object.keys(h).map((e => {
-                                    let a = {};
-                                    return a[t] = e, a = {
-                                        ...a,
+                                    let n = {};
+                                    return n[t] = e, n = {
+                                        ...n,
                                         ...h[e]
-                                    }, a
+                                    }, n
                                 }));
-                                m.append("g").selectAll("g").data(x).enter().append("g").attr("transform", (function(e) {
-                                    return "translate(" + _(e[t]) + ",0)"
+                                u.append("g").selectAll("g").data(x).enter().append("g").attr("transform", (function(e) {
+                                    return "translate(" + y(e[t]) + ",0)"
                                 })).selectAll("rect").data((function(e) {
                                     return p.map((function(t) {
                                         return {
-                                            key: a + "-" + t,
+                                            key: n + "-" + t,
                                             value: e[t]
                                         }
                                     }))
                                 })).enter().append("rect").attr("x", (function(e) {
-                                    return y(e.key) + y.bandwidth() / 2 - 1
+                                    return _(e.key) + _.bandwidth() / 2 - 1
                                 })).attr("y", (function(e) {
-                                    return e.value.max ? f(e.value.max) : 0
+                                    return e.value.max ? v(e.value.max) : 0
                                 })).attr("width", 2).attr("height", (function(e) {
-                                    return e.value.min && e.value.max ? f(e.value.min) - f(e.value.max) : 0
+                                    return e.value.min && e.value.max ? v(e.value.min) - v(e.value.max) : 0
                                 }));
-                                var b = m.selectAll(".legend").data(v.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
+                                const b = u.selectAll(".legend").data(f.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(e, t) {
                                     return "translate(0," + 20 * t + ")"
                                 }));
-                                b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", v), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
+                                b.append("rect").attr("x", c - 18).attr("width", 18).attr("height", 18).style("fill", f), b.append("text").attr("x", c - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(e) {
                                     return e
-                                })), m.append("g").style("font", "18px times").attr("transform", "translate(0," + f(0) + ")").call(r.axisBottom(_).tickSize(0))
+                                })), u.append("g").style("font", "18px times").attr("transform", "translate(0," + v(0) + ")").call(r.axisBottom(y).tickSize(0))
                             }()
-                        }(t, a, n, o, l, e)
-                    }), 50)
+                        }(e, t, n, a, l, l.clientWidth, s, w)
                 }
             }
-            class V extends n.DOMWidgetModel {
+            class P extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: V.model_name,
-                        _view_name: V.view_name,
-                        _model_module: V.model_module,
-                        _view_module: V.view_module,
-                        _model_module_version: V.model_module_version,
-                        _view_module_version: V.view_module_version,
+                        _model_name: P.model_name,
+                        _view_name: P.view_name,
+                        _model_module: P.model_module,
+                        _view_module: P.view_module,
+                        _model_module_version: P.model_module_version,
+                        _view_module_version: P.view_module_version,
                         data: [],
                         x: String,
                         start: Number,
                         end: Number,
-                        element: String
+                        elementId: String
                     }
                 }
                 static model_name = "HistogramplotModel";
                 static model_module = x.name;
                 static model_module_version = x.version;
                 static view_name = "HistogramplotView";
                 static view_module = x.name;
                 static view_module_version = x.version
             }
-            class P extends n.DOMWidgetView {
+            class j extends a.DOMWidgetView {
+                timeout;
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    M(this), this.model.on("change:data", (() => M(this)), this), window.addEventListener("resize", (() => M(this).bind(this)))
                 }
-                value_changed() {
-                    let e = this;
-                    var t = this.model.get("data"),
-                        a = this.model.get("x"),
+                plot() {
+                    const e = this.model.get("data"),
+                        t = this.model.get("x"),
                         n = this.model.get("start"),
-                        i = this.model.get("end"),
-                        o = this.model.get("element");
-                    setTimeout((() => {
-                        ! function(e, t, a, n, i, o) {
-                            var l = 375,
-                                s = 720;
-                            i ? (s = (i = document.getElementById(i)).clientWidth, l = i.clientHeight) : i = o.el, r.select(i).selectAll("*").remove();
-                            const d = s - 40 - 20,
-                                c = l - 20 - 30;
-                            let u = a;
-                            a || (u = r.min(e, (e => e[t])));
+                        a = this.model.get("end"),
+                        i = this.model.get("elementId");
+                    let o = b,
+                        s = this.el;
+                    i && (s = document.getElementById(i), o = s.clientHeight),
+                        function(e, t, n, a, i, o, s, l) {
+                            const d = o - l.left - l.right,
+                                c = s - l.top - l.bottom;
+                            r.select(i).selectAll("*").remove();
                             let m = n;
-                            n || (m = r.max(e, (e => e[t])));
+                            n || (m = r.min(e, (e => e[t])));
+                            let u = a;
+                            a || (u = r.max(e, (e => e[t])));
                             const p = r.scaleLinear().range([0, d]),
                                 h = r.scaleLinear().range([c, 0]),
-                                v = r.axisBottom(p),
+                                f = r.axisBottom(p),
                                 g = r.axisLeft(h),
-                                f = r.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
-                                _ = r.select(i).append("svg").attr("width", d + 40 + 20).attr("height", c + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                            p.domain([u, m]), h.domain([0, r.max(f, (e => e.length))]), _.append("g").attr("transform", "translate(0," + c + ")").call(v).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), _.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), _.append("g").attr("fill", "steelblue").selectAll().data(f).join("rect").attr("x", (e => p(e.x0) + 1)).attr("width", (e => p(e.x1) - p(e.x0) - 1)).attr("y", (e => h(e.length))).attr("height", (e => h(0) - h(e.length)))
-                        }(t, a, n, i, o, e)
-                    }), 50)
+                                v = r.bin().thresholds(40).value((e => Math.round(10 * e[t]) / 10))(e),
+                                y = r.select(i).append("svg").attr("width", o).attr("height", s).append("g").attr("transform", "translate(" + l.left + "," + l.top + ")");
+                            p.domain([m, u]), h.domain([0, r.max(v, (e => e.length))]), y.append("g").attr("transform", "translate(0," + c + ")").call(f).append("text").attr("x", d).attr("y", -6).style("text-anchor", "end"), y.append("g").call(g).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.append("g").attr("fill", "steelblue").selectAll().data(v).join("rect").attr("x", (e => p(e.x0) + 1)).attr("width", (e => p(e.x1) - p(e.x0) - 1)).attr("y", (e => h(e.length))).attr("height", (e => h(0) - h(e.length)))
+                        }(e, t, n, a, s, s.clientWidth, o, w)
                 }
             }
-            class E extends n.DOMWidgetModel {
+            class D extends a.DOMWidgetModel {
                 defaults() {
                     return {
                         ...super.defaults(),
-                        _model_name: E.model_name,
-                        _view_name: E.view_name,
-                        _model_module: E.model_module,
-                        _view_module: E.view_module,
-                        _model_module_version: E.model_module_version,
-                        _view_module_version: E.view_module_version,
+                        _model_name: D.model_name,
+                        _view_name: D.view_name,
+                        _model_module: D.model_module,
+                        _view_module: D.view_module,
+                        _model_module_version: D.model_module_version,
+                        _view_module_version: D.view_module_version,
                         matrix: [],
                         grid_areas: [],
                         grid_template_areas: String,
                         style: String
                     }
                 }
                 static model_name = "EmbeddingModel";
                 static model_module = x.name;
                 static model_module_version = x.version;
                 static view_name = "EmbeddingView";
                 static view_module = x.name;
                 static view_module_version = x.version
             }
-            class L extends n.DOMWidgetView {
+            class I extends a.DOMWidgetView {
                 render() {
-                    this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                    this.value_changed()
                 }
                 value_changed() {
-                    var e = this.model.get("matrix"),
+                    const e = this.model.get("matrix"),
                         t = this.model.get("grid_areas"),
-                        a = this.model.get("grid_template_areas"),
-                        n = this.model.get("style");
-                    n || (n = "basic");
+                        n = this.model.get("grid_template_areas");
+                    let a = this.model.get("style");
+                    a || (a = "basic");
                     const r = document.createElement("div");
-                    r.classList.add(n), r.style.display = "grid", r.style.gridTemplateAreas = a, r.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", r.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", r.style.width = "100%", t.forEach((e => {
+                    r.classList.add(a), r.style.display = "grid", r.style.gridTemplateAreas = n, r.style.gridTemplateRows = "repeat(" + e.length + ", 20vh)", r.style.gridTemplateColumns = "repeat(" + e[0].length + ", 1fr)", r.style.width = "100%", t.forEach((e => {
                         const t = document.createElement("div");
                         t.setAttribute("id", e), t.style.gridArea = e, t.classList.add("dashboard-div"), r.appendChild(t)
                     })), this.el.appendChild(r)
                 }
             }
-            var j = a(330)
+            var O = n(330)
         },
-        493: (e, t, a) => {
-            a.r(t), a.d(t, {
+        493: (e, t, n) => {
+            n.r(t), n.d(t, {
                 default: () => i,
                 helloWidgetPlugin: () => r
             });
-            var n = a(380);
+            var a = n(380);
             const r = {
                     id: "d3vis_ipynb:plugin",
-                    requires: [a(801).IJupyterWidgetRegistry],
+                    requires: [n(801).IJupyterWidgetRegistry],
                     activate: function(e, t) {
                         t.registerWidget({
                             name: "d3vis_ipynb",
-                            version: n.version,
+                            version: a.version,
                             exports: {
-                                LinearHistPlotModel: n.LinearHistPlotModel,
-                                LinearHistPlotView: n.LinearHistPlotView,
-                                ScatterPlotModel: n.ScatterPlotModel,
-                                ScatterPlotView: n.ScatterPlotView,
-                                BarPlotModel: n.BarPlotModel,
-                                BarPlotView: n.BarPlotView,
-                                HistogramPlotModel: n.HistogramPlotModel,
-                                HistogramPlotView: n.HistogramPlotView,
-                                EmbeddingModel: n.EmbeddingModel,
-                                EmbeddingView: n.EmbeddingView
+                                LinearHistPlotModel: a.LinearHistPlotModel,
+                                LinearHistPlotView: a.LinearHistPlotView,
+                                ScatterPlotModel: a.ScatterPlotModel,
+                                ScatterPlotView: a.ScatterPlotView,
+                                BarPlotModel: a.BarPlotModel,
+                                BarPlotView: a.BarPlotView,
+                                HistogramPlotModel: a.HistogramPlotModel,
+                                HistogramPlotView: a.HistogramPlotView,
+                                EmbeddingModel: a.EmbeddingModel,
+                                EmbeddingView: a.EmbeddingView
                             }
                         })
                     },
                     autoStart: !0
                 },
                 i = r
         },
-        930: (e, t, a) => {
-            a.d(t, {
-                A: () => l
+        930: (e, t, n) => {
+            n.d(t, {
+                A: () => s
             });
-            var n = a(601),
-                r = a.n(n),
-                i = a(314),
-                o = a.n(i)()(r());
+            var a = n(601),
+                r = n.n(a),
+                i = n(314),
+                o = n.n(i)()(r());
             o.push([e.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
-            const l = o
+            const s = o
         },
         314: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var a = "",
-                            n = void 0 !== t[5];
-                        return t[4] && (a += "@supports (".concat(t[4], ") {")), t[2] && (a += "@media ".concat(t[2], " {")), n && (a += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), a += e(t), n && (a += "}"), t[2] && (a += "}"), t[4] && (a += "}"), a
+                        var n = "",
+                            a = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), a && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), a && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, a, n, r, i) {
+                }, t.i = function(e, n, a, r, i) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
                     var o = {};
-                    if (n)
-                        for (var l = 0; l < this.length; l++) {
-                            var s = this[l][0];
-                            null != s && (o[s] = !0)
+                    if (a)
+                        for (var s = 0; s < this.length; s++) {
+                            var l = this[s][0];
+                            null != l && (o[l] = !0)
                         }
                     for (var d = 0; d < e.length; d++) {
                         var c = [].concat(e[d]);
-                        n && o[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), a && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = a) : c[2] = a), r && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = r) : c[4] = "".concat(r)), t.push(c))
+                        a && o[c[0]] || (void 0 !== i && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = i), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), r && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = r) : c[4] = "".concat(r)), t.push(c))
                     }
                 }, t
             }
         },
         601: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
         72: e => {
             var t = [];
 
-            function a(e) {
-                for (var a = -1, n = 0; n < t.length; n++)
-                    if (t[n].identifier === e) {
-                        a = n;
+            function n(e) {
+                for (var n = -1, a = 0; a < t.length; a++)
+                    if (t[a].identifier === e) {
+                        n = a;
                         break
-                    } return a
+                    } return n
             }
 
-            function n(e, n) {
-                for (var i = {}, o = [], l = 0; l < e.length; l++) {
-                    var s = e[l],
-                        d = n.base ? s[0] + n.base : s[0],
+            function a(e, a) {
+                for (var i = {}, o = [], s = 0; s < e.length; s++) {
+                    var l = e[s],
+                        d = a.base ? l[0] + a.base : l[0],
                         c = i[d] || 0,
-                        u = "".concat(d, " ").concat(c);
+                        m = "".concat(d, " ").concat(c);
                     i[d] = c + 1;
-                    var m = a(u),
+                    var u = n(m),
                         p = {
-                            css: s[1],
-                            media: s[2],
-                            sourceMap: s[3],
-                            supports: s[4],
-                            layer: s[5]
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3],
+                            supports: l[4],
+                            layer: l[5]
                         };
-                    if (-1 !== m) t[m].references++, t[m].updater(p);
+                    if (-1 !== u) t[u].references++, t[u].updater(p);
                     else {
-                        var h = r(p, n);
-                        n.byIndex = l, t.splice(l, 0, {
-                            identifier: u,
+                        var h = r(p, a);
+                        a.byIndex = s, t.splice(s, 0, {
+                            identifier: m,
                             updater: h,
                             references: 1
                         })
                     }
-                    o.push(u)
+                    o.push(m)
                 }
                 return o
             }
 
             function r(e, t) {
-                var a = t.domAPI(t);
-                return a.update(e),
+                var n = t.domAPI(t);
+                return n.update(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
-                            a.update(e = t)
-                        } else a.remove()
+                            n.update(e = t)
+                        } else n.remove()
                     }
             }
             e.exports = function(e, r) {
-                var i = n(e = e || [], r = r || {});
+                var i = a(e = e || [], r = r || {});
                 return function(e) {
                     e = e || [];
                     for (var o = 0; o < i.length; o++) {
-                        var l = a(i[o]);
-                        t[l].references--
+                        var s = n(i[o]);
+                        t[s].references--
                     }
-                    for (var s = n(e, r), d = 0; d < i.length; d++) {
-                        var c = a(i[d]);
+                    for (var l = a(e, r), d = 0; d < i.length; d++) {
+                        var c = n(i[d]);
                         0 === t[c].references && (t[c].updater(), t.splice(c, 1))
                     }
-                    i = s
+                    i = l
                 }
             }
         },
         659: e => {
             var t = {};
-            e.exports = function(e, a) {
-                var n = function(e) {
+            e.exports = function(e, n) {
+                var a = function(e) {
                     if (void 0 === t[e]) {
-                        var a = document.querySelector(e);
-                        if (window.HTMLIFrameElement && a instanceof window.HTMLIFrameElement) try {
-                            a = a.contentDocument.head
+                        var n = document.querySelector(e);
+                        if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                            n = n.contentDocument.head
                         } catch (e) {
-                            a = null
+                            n = null
                         }
-                        t[e] = a
+                        t[e] = n
                     }
                     return t[e]
                 }(e);
-                if (!n) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                n.appendChild(a)
+                if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                a.appendChild(n)
             }
         },
         540: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
-        56: (e, t, a) => {
+        56: (e, t, n) => {
             e.exports = function(e) {
-                var t = a.nc;
+                var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
         825: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
-                    update: function(a) {
-                        ! function(e, t, a) {
-                            var n = "";
-                            a.supports && (n += "@supports (".concat(a.supports, ") {")), a.media && (n += "@media ".concat(a.media, " {"));
-                            var r = void 0 !== a.layer;
-                            r && (n += "@layer".concat(a.layer.length > 0 ? " ".concat(a.layer) : "", " {")), n += a.css, r && (n += "}"), a.media && (n += "}"), a.supports && (n += "}");
-                            var i = a.sourceMap;
-                            i && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(n, e, t.options)
-                        }(t, e, a)
+                    update: function(n) {
+                        ! function(e, t, n) {
+                            var a = "";
+                            n.supports && (a += "@supports (".concat(n.supports, ") {")), n.media && (a += "@media ".concat(n.media, " {"));
+                            var r = void 0 !== n.layer;
+                            r && (a += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), a += n.css, r && (a += "}"), n.media && (a += "}"), n.supports && (a += "}");
+                            var i = n.sourceMap;
+                            i && "undefined" != typeof btoa && (a += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(a, e, t.options)
+                        }(t, e, n)
                     },
                     remove: function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
@@ -755,11 +768,11 @@
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
         330: e => {
-            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/693.c8409ce8329f6703470f.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/remoteEntry.7e42e6f84b582762349a.js` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/remoteEntry.bf58726a1c33e2ff91a1.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, d, u, s, l, f, p, c, h, v, b, g, m, y, w = {
+    var e, r, t, n, o, i, a, d, u, f, s, l, p, c, h, v, b, g, m, y, w = {
             772: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(380).then((() => () => t(380))),
                         "./extension": () => Promise.all([t.e(56), t.e(493)]).then((() => () => t(493)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    o = (e, r) => {
+                    i = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => o
+                    get: () => o,
+                    init: () => i
                 })
             }
         },
         S = {};
 
     function E(e) {
         var r = S[e];
@@ -43,82 +43,82 @@
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         56: "2d1dea0ba8f2782da6dd",
-        380: "bce32fc1670ea497a572",
-        493: "e98395b66f4058ecc2a8",
+        380: "5f71b19ff5261cd2e5de",
+        493: "6062c0a7b585f6ae1d22",
         693: "c8409ce8329f6703470f"
     } [e] + ".js?v=" + {
         56: "2d1dea0ba8f2782da6dd",
-        380: "bce32fc1670ea497a572",
-        493: "e98395b66f4058ecc2a8",
+        380: "5f71b19ff5261cd2e5de",
+        493: "6062c0a7b585f6ae1d22",
         693: "c8409ce8329f6703470f"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, a, o) => {
+    }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "d3vis_ipynb:", E.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var i, d;
-            if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
-                    var l = u[s];
-                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + a) {
-                        i = l;
+            var a, d;
+            if (void 0 !== o)
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        a = s;
                         break
                     }
                 }
-            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var f = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+            a || (d = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, E.nc && a.setAttribute("nonce", E.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            var l = (r, n) => {
+                    a.onerror = a.onload = null, clearTimeout(p);
+                    var o = e[t];
+                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(l.bind(null, void 0, {
                     type: "timeout",
-                    target: i
+                    target: a
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), d && document.head.appendChild(i)
+            a.onerror = l.bind(null, a.onerror), a.onload = l.bind(null, a.onload), d && document.head.appendChild(a)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         E.S = {};
         var e = {},
             r = {};
         E.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 E.o(E.S, t) || (E.S[t] = {});
-                var o = E.S[t],
-                    i = "d3vis_ipynb",
+                var i = E.S[t],
+                    a = "d3vis_ipynb",
                     d = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            d = a[r];
-                        (!d || !d.loaded && (!n != !d.eager ? n : i > d.from)) && (a[r] = {
+                        var o = i[e] = i[e] || {},
+                            d = o[r];
+                        (!d || !d.loaded && (!n != !d.eager ? n : a > d.from)) && (o[r] = {
                             get: t,
-                            from: i,
+                            from: a,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.1", (() => E.e(380).then((() => () => E(380)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("d3", "7.9.0", (() => E.e(693).then((() => () => E(693))))), d("d3vis_ipynb", "0.1.2", (() => E.e(380).then((() => () => E(380)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -133,98 +133,98 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
-            var i = r[n],
-                d = (typeof i)[0];
-            if (o != d) return "o" == o && "n" == d || "s" == d || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
+            var o = e[n],
+                i = (typeof o)[0];
+            if (n >= r.length) return "u" == i;
+            var a = r[n],
+                d = (typeof a)[0];
+            if (i != d) return "o" == i && "n" == d || "s" == d || "u" == i;
+            if ("o" != i && "u" != i && o != a) return o < a;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(d = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, d);
             return t
         }
-        var i = [];
-        for (o = 1; o < e.length; o++) {
-            var d = e[o];
-            i.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? i.pop() + " " + i.pop() : a(d))
+        var a = [];
+        for (i = 1; i < e.length; i++) {
+            var d = e[i];
+            a.push(0 === d ? "not(" + u() + ")" : 1 === d ? "(" + u() + " || " + u() + ")" : 2 === d ? a.pop() + " " + a.pop() : o(d))
         }
         return u();
 
         function u() {
-            return i.pop().replace(/^\((.+)\)$/, "$1")
+            return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, o = (e, r) => {
+    }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
-            for (var i = 0, d = 1, u = !0;; d++, i++) {
-                var s, l, f = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (l = (typeof(s = r[i]))[0])) return !u || ("u" == f ? d > n && !a : "" == f != a);
-                if ("u" == l) {
-                    if (!u || "u" != f) return !1
+                o = n < 0;
+            o && (n = -n - 1);
+            for (var a = 0, d = 1, u = !0;; d++, a++) {
+                var f, s, l = d < e.length ? (typeof e[d])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == l ? d > n && !o : "" == l != o);
+                if ("u" == s) {
+                    if (!u || "u" != l) return !1
                 } else if (u)
-                    if (f == l)
+                    if (l == s)
                         if (d <= n) {
-                            if (s != e[d]) return !1
+                            if (f != e[d]) return !1
                         } else {
-                            if (a ? s > e[d] : s < e[d]) return !1;
-                            s != e[d] && (u = !1)
+                            if (o ? f > e[d] : f < e[d]) return !1;
+                            f != e[d] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (a || d <= n) return !1;
+                else if ("s" != l && "n" != l) {
+                    if (o || d <= n) return !1;
                     u = !1, d--
                 } else {
-                    if (d <= n || l < f != a) return !1;
+                    if (d <= n || s < l != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, d--)
+                } else "s" != l && "n" != l && (u = !1, d--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (i = 1; i < e.length; i++) {
-            var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+        for (a = 1; a < e.length; a++) {
+            var h = e[a];
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
         return !!c()
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", s = (e, r, t, n) => {
-        var a = d(e, t);
-        return o(n, a) || f(u(e, t, a, n)), p(e[t][a])
-    }, l = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, f = e => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+        var o = d(e, t);
+        return i(n, o) || l(u(e, t, o, n)), p(e[t][o])
+    }, s = (e, r, t) => {
+        var o = e[r];
+        return (r = Object.keys(o).reduce(((e, r) => !i(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+    }, l = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, a) {
-        var o = E.I(r);
-        return o && o.then ? o.then(e.bind(e, r, E.S[r], t, n, a)) : e(r, E.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = c(((e, r, t, n, a) => {
-        var o = r && E.o(r, t) && l(r, t, n);
-        return o ? p(o) : a()
+    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
+        var i = E.I(r);
+        return i && i.then ? i.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
+    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n, o) => {
+        var i = r && E.o(r, t) && s(r, t, n);
+        return i ? p(i) : o()
     })), b = {}, g = {
         801: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
@@ -244,51 +244,51 @@
                 y[e] = !0;
                 var n = r => {
                     delete b[e], E.m[e] = t => {
                         throw delete E.c[e], r
                     }
                 };
                 try {
-                    var a = g[e]();
-                    a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
+                    var o = g[e]();
+                    o.then ? r.push(b[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
             71: 0
         };
         E.f.j = (r, t) => {
             var n = E.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (56 != r) {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
-                var o = E.p + E.u(r),
-                    i = new Error;
-                E.l(o, (t => {
+                var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                t.push(n[2] = o);
+                var i = E.p + E.u(r),
+                    a = new Error;
+                E.l(i, (t => {
                     if (E.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        var o = t && ("load" === t.type ? "missing" : t.type),
+                            i = t && t.target && t.target.src;
+                        a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, a, [o, i, d] = t,
+                var n, o, [i, a, d] = t,
                     u = 0;
-                if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) E.o(i, n) && (E.m[n] = i[n]);
+                if (i.some((r => 0 !== e[r]))) {
+                    for (n in a) E.o(a, n) && (E.m[n] = a[n]);
                     d && d(E)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], E.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < i.length; u++) o = i[u], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkd3vis_ipynb = self.webpackChunkd3vis_ipynb || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(772);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).d3vis_ipynb = P
 })();
```

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/labextension/static/third-party-licenses.json` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/d3vis_ipynb/nbextension/index.js` & `d3vis_ipynb-0.1.2/d3vis_ipynb/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,41 +3,41 @@
     var n = {
             930: (t, e, n) => {
                 n.d(e, {
                     A: () => s
                 });
                 var r = n(601),
                     i = n.n(r),
-                    a = n(314),
-                    o = n.n(a)()(i());
-                o.push([t.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
-                const s = o
+                    o = n(314),
+                    a = n.n(o)()(i());
+                a.push([t.id, "/***** BASIC *****/\n.basic .dashboard-div {\n  border: 1px solid black;\n  text-align: center;\n}\n\n/***** DARK *****/\n.dark .dashboard-div {\n  margin: 2px;\n  border-radius: 10px;\n  background-color: #262626;\n  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.5);\n}\n\n/***** GLASSMORPHISM *****/\n.glassmorphism .dashboard-div {\n  margin: 5px;\n  border-radius: 10px;\n  background: rgb(255, 254, 254);\n  border: 1px solid rgb(255, 255, 255);\n  backdrop-filter: blur(10px);\n  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);\n}\n\n/***** NEUMORPHISM *****/\n.neumorphism .dashboard-div {\n  margin: 10px;\n  border-radius: 15px;\n  background-color: #e0e0e0;\n  box-shadow: 5px 5px 10px #bebebe, -5px -5px 10px #ffffff;\n}\n\n/***** MINIMALISM *****/\n.minimalism .dashboard-div {\n  margin-bottom: 5px;\n}\n", ""]);
+                const s = a
             },
             314: t => {
                 t.exports = function(t) {
                     var e = [];
                     return e.toString = function() {
                         return this.map((function(e) {
                             var n = "",
                                 r = void 0 !== e[5];
                             return e[4] && (n += "@supports (".concat(e[4], ") {")), e[2] && (n += "@media ".concat(e[2], " {")), r && (n += "@layer".concat(e[5].length > 0 ? " ".concat(e[5]) : "", " {")), n += t(e), r && (n += "}"), e[2] && (n += "}"), e[4] && (n += "}"), n
                         })).join("")
-                    }, e.i = function(t, n, r, i, a) {
+                    }, e.i = function(t, n, r, i, o) {
                         "string" == typeof t && (t = [
                             [null, t, void 0]
                         ]);
-                        var o = {};
+                        var a = {};
                         if (r)
                             for (var s = 0; s < this.length; s++) {
                                 var u = this[s][0];
-                                null != u && (o[u] = !0)
+                                null != u && (a[u] = !0)
                             }
                         for (var l = 0; l < t.length; l++) {
                             var c = [].concat(t[l]);
-                            r && o[c[0]] || (void 0 !== a && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = a), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), e.push(c))
+                            r && a[c[0]] || (void 0 !== o && (void 0 === c[5] || (c[1] = "@layer".concat(c[5].length > 0 ? " ".concat(c[5]) : "", " {").concat(c[1], "}")), c[5] = o), n && (c[2] ? (c[1] = "@media ".concat(c[2], " {").concat(c[1], "}"), c[2] = n) : c[2] = n), i && (c[4] ? (c[1] = "@supports (".concat(c[4], ") {").concat(c[1], "}"), c[4] = i) : c[4] = "".concat(i)), e.push(c))
                         }
                     }, e
                 }
             },
             601: t => {
                 t.exports = function(t) {
                     return t[1]
@@ -51,20 +51,20 @@
                         if (e[r].identifier === t) {
                             n = r;
                             break
                         } return n
                 }
 
                 function r(t, r) {
-                    for (var a = {}, o = [], s = 0; s < t.length; s++) {
+                    for (var o = {}, a = [], s = 0; s < t.length; s++) {
                         var u = t[s],
                             l = r.base ? u[0] + r.base : u[0],
-                            c = a[l] || 0,
+                            c = o[l] || 0,
                             h = "".concat(l, " ").concat(c);
-                        a[l] = c + 1;
+                        o[l] = c + 1;
                         var f = n(h),
                             d = {
                                 css: u[1],
                                 media: u[2],
                                 sourceMap: u[3],
                                 supports: u[4],
                                 layer: u[5]
@@ -74,42 +74,42 @@
                             var p = i(d, r);
                             r.byIndex = s, e.splice(s, 0, {
                                 identifier: h,
                                 updater: p,
                                 references: 1
                             })
                         }
-                        o.push(h)
+                        a.push(h)
                     }
-                    return o
+                    return a
                 }
 
                 function i(t, e) {
                     var n = e.domAPI(e);
                     return n.update(t),
                         function(e) {
                             if (e) {
                                 if (e.css === t.css && e.media === t.media && e.sourceMap === t.sourceMap && e.supports === t.supports && e.layer === t.layer) return;
                                 n.update(t = e)
                             } else n.remove()
                         }
                 }
                 t.exports = function(t, i) {
-                    var a = r(t = t || [], i = i || {});
+                    var o = r(t = t || [], i = i || {});
                     return function(t) {
                         t = t || [];
-                        for (var o = 0; o < a.length; o++) {
-                            var s = n(a[o]);
+                        for (var a = 0; a < o.length; a++) {
+                            var s = n(o[a]);
                             e[s].references--
                         }
-                        for (var u = r(t, i), l = 0; l < a.length; l++) {
-                            var c = n(a[l]);
+                        for (var u = r(t, i), l = 0; l < o.length; l++) {
+                            var c = n(o[l]);
                             0 === e[c].references && (e[c].updater(), e.splice(c, 1))
                         }
-                        a = u
+                        o = u
                     }
                 }
             },
             659: t => {
                 var e = {};
                 t.exports = function(t, n) {
                     var r = function(t) {
@@ -150,16 +150,16 @@
                     return {
                         update: function(n) {
                             ! function(t, e, n) {
                                 var r = "";
                                 n.supports && (r += "@supports (".concat(n.supports, ") {")), n.media && (r += "@media ".concat(n.media, " {"));
                                 var i = void 0 !== n.layer;
                                 i && (r += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), r += n.css, i && (r += "}"), n.media && (r += "}"), n.supports && (r += "}");
-                                var a = n.sourceMap;
-                                a && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleTagTransform(r, t, e.options)
+                                var o = n.sourceMap;
+                                o && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(o)))), " */")), e.styleTagTransform(r, t, e.options)
                             }(e, t, n)
                         },
                         remove: function() {
                             ! function(t) {
                                 if (null === t.parentNode) return !1;
                                 t.parentNode.removeChild(t)
                             }(e)
@@ -179,27 +179,27 @@
             55: t => {
                 t.exports = e
             },
             308: e => {
                 e.exports = t
             },
             330: t => {
-                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.1","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                t.exports = JSON.parse('{"name":"d3vis_ipynb","version":"0.1.2","description":"A Custom Jupyter Widget Library with visualizations created with D3.js.","author":"Daniel Adam Miranda","license":"BSD-3-Clause","main":"lib/index.js","repository":{"type":"git","url":"https://github.com/H-IAAC/d3vis_ipynb.git"},"keywords":["jupyter","widgets","ipython","ipywidgets","jupyterlab-extension"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"scripts":{"clean":"rimraf dist/ && rimraf ../d3vis_ipynb/labextension/ && rimraf ../d3vis_ipynb/nbextension","prepublish":"yarn run clean && yarn run build:prod","build":"webpack --mode=development && yarn run build:labextension:dev","build:prod":"webpack --mode=production && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","watch":"webpack --watch --mode=development","start":"webpack serve --open --config webpack.exports.config.js","start:export":"webpack serve --open --config webpack.exports.config.js --env export","export":"webpack --env export --config webpack.exports.config.js","test":"echo \\"Error: no test specified\\" && exit 1"},"devDependencies":{"@jupyterlab/builder":"^4.0.6","html-webpack-plugin":"^5.6.0","rimraf":"^2.6.1","webpack":"^5","webpack-dev-server":"^5.0.2"},"dependencies":{"@jupyter-widgets/base":"^1.1 || ^2 || ^3 || ^4 || ^6","d3":"^7.9.0"},"jupyterlab":{"extension":"lib/labplugin","outputDir":"../d3vis_ipynb/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         r = {};
 
     function i(t) {
         var e = r[t];
         if (void 0 !== e) return e.exports;
-        var a = r[t] = {
+        var o = r[t] = {
             id: t,
             exports: {}
         };
-        return n[t](a, a.exports, i), a.exports
+        return n[t](o, o.exports, i), o.exports
     }
     i.n = t => {
         var e = t && t.__esModule ? () => t.default : () => t;
         return i.d(e, {
             a: e
         }), e
     }, i.d = (t, e) => {
@@ -210,105 +210,105 @@
     }, i.o = (t, e) => Object.prototype.hasOwnProperty.call(t, e), i.r = t => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(t, "__esModule", {
             value: !0
         })
     }, i.p = "", i.nc = void 0;
-    var a = {};
+    var o = {};
     return (() => {
         var t = i(308);
         const e = new URL(t.uri, document.location);
         e.pathname = e.pathname.slice(0, e.pathname.lastIndexOf("/") + 1), i.p = `${e.origin}${e.pathname}`
     })(), (() => {
-        i.r(a), i.d(a, {
-            BarPlotModel: () => Pi,
-            BarPlotView: () => Ci,
-            EmbeddingModel: () => Di,
-            EmbeddingView: () => qi,
-            HistogramPlotModel: () => Oi,
-            HistogramPlotView: () => Vi,
-            LinearHistPlotModel: () => Si,
-            LinearHistPlotView: () => Ei,
-            ScatterPlotModel: () => Ti,
-            ScatterPlotView: () => ji,
-            author: () => Ii.author,
-            dependencies: () => Ii.dependencies,
-            description: () => Ii.description,
-            devDependencies: () => Ii.devDependencies,
-            files: () => Ii.files,
-            jupyterlab: () => Ii.jupyterlab,
-            keywords: () => Ii.keywords,
-            license: () => Ii.license,
-            main: () => Ii.main,
-            name: () => Ii.name,
-            repository: () => Ii.repository,
-            scripts: () => Ii.scripts,
-            version: () => Ii.version
+        i.r(o), i.d(o, {
+            BarPlotModel: () => Ii,
+            BarPlotView: () => Vi,
+            EmbeddingModel: () => Li,
+            EmbeddingView: () => Hi,
+            HistogramPlotModel: () => Di,
+            HistogramPlotView: () => qi,
+            LinearHistPlotModel: () => Ti,
+            LinearHistPlotView: () => Pi,
+            ScatterPlotModel: () => Ci,
+            ScatterPlotView: () => Oi,
+            author: () => Xi.author,
+            dependencies: () => Xi.dependencies,
+            description: () => Xi.description,
+            devDependencies: () => Xi.devDependencies,
+            files: () => Xi.files,
+            jupyterlab: () => Xi.jupyterlab,
+            keywords: () => Xi.keywords,
+            license: () => Xi.license,
+            main: () => Xi.main,
+            name: () => Xi.name,
+            repository: () => Xi.repository,
+            scripts: () => Xi.scripts,
+            version: () => Xi.version
         });
         var t = i(55);
 
         function e(t, e) {
             let n, r;
             if (void 0 === e)
                 for (const e of t) null != e && (void 0 === n ? e >= e && (n = r = e) : (n > e && (n = e), r < e && (r = e)));
             else {
                 let i = -1;
-                for (let a of t) null != (a = e(a, ++i, t)) && (void 0 === n ? a >= a && (n = r = a) : (n > a && (n = a), r < a && (r = a)))
+                for (let o of t) null != (o = e(o, ++i, t)) && (void 0 === n ? o >= o && (n = r = o) : (n > o && (n = o), r < o && (r = o)))
             }
             return [n, r]
         }
         var n = Array.prototype,
             r = n.slice;
 
-        function o(t, e) {
+        function a(t, e) {
             return null == t || null == e ? NaN : t < e ? -1 : t > e ? 1 : t >= e ? 0 : NaN
         }
 
         function s(t, e) {
             return null == t || null == e ? NaN : e < t ? -1 : e > t ? 1 : e >= t ? 0 : NaN
         }
 
         function u(t) {
             let e, n, r;
 
-            function i(t, r, i = 0, a = t.length) {
-                if (i < a) {
-                    if (0 !== e(r, r)) return a;
+            function i(t, r, i = 0, o = t.length) {
+                if (i < o) {
+                    if (0 !== e(r, r)) return o;
                     do {
-                        const e = i + a >>> 1;
-                        n(t[e], r) < 0 ? i = e + 1 : a = e
-                    } while (i < a)
+                        const e = i + o >>> 1;
+                        n(t[e], r) < 0 ? i = e + 1 : o = e
+                    } while (i < o)
                 }
                 return i
             }
-            return 2 !== t.length ? (e = o, n = (e, n) => o(t(e), n), r = (e, n) => t(e) - n) : (e = t === o || t === s ? t : l, n = t, r = t), {
+            return 2 !== t.length ? (e = a, n = (e, n) => a(t(e), n), r = (e, n) => t(e) - n) : (e = t === a || t === s ? t : l, n = t, r = t), {
                 left: i,
-                center: function(t, e, n = 0, a = t.length) {
-                    const o = i(t, e, n, a - 1);
-                    return o > n && r(t[o - 1], e) > -r(t[o], e) ? o - 1 : o
+                center: function(t, e, n = 0, o = t.length) {
+                    const a = i(t, e, n, o - 1);
+                    return a > n && r(t[a - 1], e) > -r(t[a], e) ? a - 1 : a
                 },
-                right: function(t, r, i = 0, a = t.length) {
-                    if (i < a) {
-                        if (0 !== e(r, r)) return a;
+                right: function(t, r, i = 0, o = t.length) {
+                    if (i < o) {
+                        if (0 !== e(r, r)) return o;
                         do {
-                            const e = i + a >>> 1;
-                            n(t[e], r) <= 0 ? i = e + 1 : a = e
-                        } while (i < a)
+                            const e = i + o >>> 1;
+                            n(t[e], r) <= 0 ? i = e + 1 : o = e
+                        } while (i < o)
                     }
                     return i
                 }
             }
         }
 
         function l() {
             return 0
         }
         n.map;
-        const c = u(o),
+        const c = u(a),
             h = c.right,
             f = (c.left, u((function(t) {
                 return null === t ? NaN : +t
             })).center, h);
 
         function d(t) {
             return () => t
@@ -320,37 +320,37 @@
         const m = Math.sqrt(50),
             _ = Math.sqrt(10),
             g = Math.sqrt(2);
 
         function v(t, e, n) {
             const r = (e - t) / Math.max(0, n),
                 i = Math.floor(Math.log10(r)),
-                a = r / Math.pow(10, i),
-                o = a >= m ? 10 : a >= _ ? 5 : a >= g ? 2 : 1;
+                o = r / Math.pow(10, i),
+                a = o >= m ? 10 : o >= _ ? 5 : o >= g ? 2 : 1;
             let s, u, l;
-            return i < 0 ? (l = Math.pow(10, -i) / o, s = Math.round(t * l), u = Math.round(e * l), s / l < t && ++s, u / l > e && --u, l = -l) : (l = Math.pow(10, i) * o, s = Math.round(t / l), u = Math.round(e / l), s * l < t && ++s, u * l > e && --u), u < s && .5 <= n && n < 2 ? v(t, e, 2 * n) : [s, u, l]
+            return i < 0 ? (l = Math.pow(10, -i) / a, s = Math.round(t * l), u = Math.round(e * l), s / l < t && ++s, u / l > e && --u, l = -l) : (l = Math.pow(10, i) * a, s = Math.round(t / l), u = Math.round(e / l), s * l < t && ++s, u * l > e && --u), u < s && .5 <= n && n < 2 ? v(t, e, 2 * n) : [s, u, l]
         }
 
         function y(t, e, n) {
             if (!((n = +n) > 0)) return [];
             if ((t = +t) == (e = +e)) return [t];
             const r = e < t,
-                [i, a, o] = r ? v(e, t, n) : v(t, e, n);
-            if (!(a >= i)) return [];
-            const s = a - i + 1,
+                [i, o, a] = r ? v(e, t, n) : v(t, e, n);
+            if (!(o >= i)) return [];
+            const s = o - i + 1,
                 u = new Array(s);
             if (r)
-                if (o < 0)
-                    for (let t = 0; t < s; ++t) u[t] = (a - t) / -o;
+                if (a < 0)
+                    for (let t = 0; t < s; ++t) u[t] = (o - t) / -a;
                 else
-                    for (let t = 0; t < s; ++t) u[t] = (a - t) * o;
-            else if (o < 0)
-                for (let t = 0; t < s; ++t) u[t] = (i + t) / -o;
+                    for (let t = 0; t < s; ++t) u[t] = (o - t) * a;
+            else if (a < 0)
+                for (let t = 0; t < s; ++t) u[t] = (i + t) / -a;
             else
-                for (let t = 0; t < s; ++t) u[t] = (i + t) * o;
+                for (let t = 0; t < s; ++t) u[t] = (i + t) * a;
             return u
         }
 
         function w(t, e, n) {
             return v(t = +t, e = +e, n = +n)[2]
         }
 
@@ -363,19 +363,19 @@
         }
 
         function b() {
             var t = p,
                 n = e,
                 i = x;
 
-            function a(r) {
+            function o(r) {
                 Array.isArray(r) || (r = Array.from(r));
-                var a, o, s, u = r.length,
+                var o, a, s, u = r.length,
                     l = new Array(u);
-                for (a = 0; a < u; ++a) l[a] = t(r[a], a, r);
+                for (o = 0; o < u; ++o) l[o] = t(r[o], o, r);
                 var c = n(l),
                     h = c[0],
                     d = c[1],
                     p = i(l, h, d);
                 if (!Array.isArray(p)) {
                     const t = d,
                         r = +p;
@@ -392,35 +392,35 @@
                             isFinite(t) && (t > 0 ? d = (Math.floor(d / t) + 1) * t : t < 0 && (d = (Math.ceil(d * -t) + 1) / -t))
                         } else p.pop()
                 }
                 for (var m = p.length, _ = 0, g = m; p[_] <= h;) ++_;
                 for (; p[g - 1] > d;) --g;
                 (_ || g < m) && (p = p.slice(_, g), m = g - _);
                 var v, x = new Array(m + 1);
-                for (a = 0; a <= m; ++a)(v = x[a] = []).x0 = a > 0 ? p[a - 1] : h, v.x1 = a < m ? p[a] : d;
+                for (o = 0; o <= m; ++o)(v = x[o] = []).x0 = o > 0 ? p[o - 1] : h, v.x1 = o < m ? p[o] : d;
                 if (isFinite(s)) {
                     if (s > 0)
-                        for (a = 0; a < u; ++a) null != (o = l[a]) && h <= o && o <= d && x[Math.min(m, Math.floor((o - h) / s))].push(r[a]);
+                        for (o = 0; o < u; ++o) null != (a = l[o]) && h <= a && a <= d && x[Math.min(m, Math.floor((a - h) / s))].push(r[o]);
                     else if (s < 0)
-                        for (a = 0; a < u; ++a)
-                            if (null != (o = l[a]) && h <= o && o <= d) {
-                                const t = Math.floor((h - o) * s);
-                                x[Math.min(m, t + (p[t] <= o))].push(r[a])
+                        for (o = 0; o < u; ++o)
+                            if (null != (a = l[o]) && h <= a && a <= d) {
+                                const t = Math.floor((h - a) * s);
+                                x[Math.min(m, t + (p[t] <= a))].push(r[o])
                             }
                 } else
-                    for (a = 0; a < u; ++a) null != (o = l[a]) && h <= o && o <= d && x[f(p, o, 0, m)].push(r[a]);
+                    for (o = 0; o < u; ++o) null != (a = l[o]) && h <= a && a <= d && x[f(p, a, 0, m)].push(r[o]);
                 return x
             }
-            return a.value = function(e) {
-                return arguments.length ? (t = "function" == typeof e ? e : d(e), a) : t
-            }, a.domain = function(t) {
-                return arguments.length ? (n = "function" == typeof t ? t : d([t[0], t[1]]), a) : n
-            }, a.thresholds = function(t) {
-                return arguments.length ? (i = "function" == typeof t ? t : d(Array.isArray(t) ? r.call(t) : t), a) : i
-            }, a
+            return o.value = function(e) {
+                return arguments.length ? (t = "function" == typeof e ? e : d(e), o) : t
+            }, o.domain = function(t) {
+                return arguments.length ? (n = "function" == typeof t ? t : d([t[0], t[1]]), o) : n
+            }, o.thresholds = function(t) {
+                return arguments.length ? (i = "function" == typeof t ? t : d(Array.isArray(t) ? r.call(t) : t), o) : i
+            }, o
         }
 
         function M(t, e) {
             let n;
             if (void 0 === e)
                 for (const e of t) null != e && (n < e || void 0 === n && e >= e) && (n = e);
             else {
@@ -444,17 +444,17 @@
         function A(t) {
             return t
         }
         var N = 1,
             $ = 2,
             S = 3,
             E = 4,
-            T = 1e-6;
+            j = 1e-6;
 
-        function j(t) {
+        function T(t) {
             return "translate(" + t + ",0)"
         }
 
         function P(t) {
             return "translate(0," + t + ")"
         }
 
@@ -462,106 +462,106 @@
             return e => +t(e)
         }
 
         function O(t, e) {
             return e = Math.max(0, t.bandwidth() - 2 * e) / 2, t.round() && (e = Math.round(e)), n => +t(n) + e
         }
 
-        function V() {
+        function I() {
             return !this.__axis
         }
 
-        function D(t, e) {
+        function V(t, e) {
             var n = [],
                 r = null,
                 i = null,
-                a = 6,
                 o = 6,
+                a = 6,
                 s = 3,
                 u = "undefined" != typeof window && window.devicePixelRatio > 1 ? 0 : .5,
                 l = t === N || t === E ? -1 : 1,
                 c = t === E || t === $ ? "x" : "y",
-                h = t === N || t === S ? j : P;
+                h = t === N || t === S ? T : P;
 
             function f(f) {
                 var d = null == r ? e.ticks ? e.ticks.apply(e, n) : e.domain() : r,
                     p = null == i ? e.tickFormat ? e.tickFormat.apply(e, n) : A : i,
-                    m = Math.max(a, 0) + s,
+                    m = Math.max(o, 0) + s,
                     _ = e.range(),
                     g = +_[0] + u,
                     v = +_[_.length - 1] + u,
                     y = (e.bandwidth ? O : C)(e.copy(), u),
                     w = f.selection ? f.selection() : f,
                     x = w.selectAll(".domain").data([null]),
                     b = w.selectAll(".tick").data(d, e).order(),
                     M = b.exit(),
                     k = b.enter().append("g").attr("class", "tick"),
-                    j = b.select("line"),
+                    T = b.select("line"),
                     P = b.select("text");
-                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), j = j.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", l * a)), P = P.merge(k.append("text").attr("fill", "currentColor").attr(c, l * m).attr("dy", t === N ? "0em" : t === S ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), j = j.transition(f), P = P.transition(f), M = M.transition(f).attr("opacity", T).attr("transform", (function(t) {
+                x = x.merge(x.enter().insert("path", ".tick").attr("class", "domain").attr("stroke", "currentColor")), b = b.merge(k), T = T.merge(k.append("line").attr("stroke", "currentColor").attr(c + "2", l * o)), P = P.merge(k.append("text").attr("fill", "currentColor").attr(c, l * m).attr("dy", t === N ? "0em" : t === S ? "0.71em" : "0.32em")), f !== w && (x = x.transition(f), b = b.transition(f), T = T.transition(f), P = P.transition(f), M = M.transition(f).attr("opacity", j).attr("transform", (function(t) {
                     return isFinite(t = y(t)) ? h(t + u) : this.getAttribute("transform")
-                })), k.attr("opacity", T).attr("transform", (function(t) {
+                })), k.attr("opacity", j).attr("transform", (function(t) {
                     var e = this.parentNode.__axis;
                     return h((e && isFinite(e = e(t)) ? e : y(t)) + u)
-                }))), M.remove(), x.attr("d", t === E || t === $ ? o ? "M" + l * o + "," + g + "H" + u + "V" + v + "H" + l * o : "M" + u + "," + g + "V" + v : o ? "M" + g + "," + l * o + "V" + u + "H" + v + "V" + l * o : "M" + g + "," + u + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
+                }))), M.remove(), x.attr("d", t === E || t === $ ? a ? "M" + l * a + "," + g + "H" + u + "V" + v + "H" + l * a : "M" + u + "," + g + "V" + v : a ? "M" + g + "," + l * a + "V" + u + "H" + v + "V" + l * a : "M" + g + "," + u + "H" + v), b.attr("opacity", 1).attr("transform", (function(t) {
                     return h(y(t) + u)
-                })), j.attr(c + "2", l * a), P.attr(c, l * m).text(p), w.filter(V).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === $ ? "start" : t === E ? "end" : "middle"), w.each((function() {
+                })), T.attr(c + "2", l * o), P.attr(c, l * m).text(p), w.filter(I).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", t === $ ? "start" : t === E ? "end" : "middle"), w.each((function() {
                     this.__axis = y
                 }))
             }
             return f.scale = function(t) {
                 return arguments.length ? (e = t, f) : e
             }, f.ticks = function() {
                 return n = Array.from(arguments), f
             }, f.tickArguments = function(t) {
                 return arguments.length ? (n = null == t ? [] : Array.from(t), f) : n.slice()
             }, f.tickValues = function(t) {
                 return arguments.length ? (r = null == t ? null : Array.from(t), f) : r && r.slice()
             }, f.tickFormat = function(t) {
                 return arguments.length ? (i = t, f) : i
             }, f.tickSize = function(t) {
-                return arguments.length ? (a = o = +t, f) : a
+                return arguments.length ? (o = a = +t, f) : o
             }, f.tickSizeInner = function(t) {
-                return arguments.length ? (a = +t, f) : a
-            }, f.tickSizeOuter = function(t) {
                 return arguments.length ? (o = +t, f) : o
+            }, f.tickSizeOuter = function(t) {
+                return arguments.length ? (a = +t, f) : a
             }, f.tickPadding = function(t) {
                 return arguments.length ? (s = +t, f) : s
             }, f.offset = function(t) {
                 return arguments.length ? (u = +t, f) : u
             }, f
         }
 
-        function q(t) {
-            return D(S, t)
+        function D(t) {
+            return V(S, t)
         }
 
-        function I(t) {
-            return D(E, t)
+        function q(t) {
+            return V(E, t)
         }
 
-        function H() {}
+        function L() {}
 
-        function L(t) {
-            return null == t ? H : function() {
+        function H(t) {
+            return null == t ? L : function() {
                 return this.querySelector(t)
             }
         }
 
         function X() {
             return []
         }
 
-        function R(t) {
+        function z(t) {
             return null == t ? X : function() {
                 return this.querySelectorAll(t)
             }
         }
 
-        function z(t) {
+        function R(t) {
             return function() {
                 return this.matches(t)
             }
         }
 
         function Y(t) {
             return function(e) {
@@ -583,26 +583,26 @@
             return new Array(t.length)
         }
 
         function J(t, e) {
             this.ownerDocument = t.ownerDocument, this.namespaceURI = t.namespaceURI, this._next = null, this._parent = t, this.__data__ = e
         }
 
-        function K(t, e, n, r, i, a) {
-            for (var o, s = 0, u = e.length, l = a.length; s < l; ++s)(o = e[s]) ? (o.__data__ = a[s], r[s] = o) : n[s] = new J(t, a[s]);
-            for (; s < u; ++s)(o = e[s]) && (i[s] = o)
+        function K(t, e, n, r, i, o) {
+            for (var a, s = 0, u = e.length, l = o.length; s < l; ++s)(a = e[s]) ? (a.__data__ = o[s], r[s] = a) : n[s] = new J(t, o[s]);
+            for (; s < u; ++s)(a = e[s]) && (i[s] = a)
         }
 
-        function Z(t, e, n, r, i, a, o) {
+        function Z(t, e, n, r, i, o, a) {
             var s, u, l, c = new Map,
                 h = e.length,
-                f = a.length,
+                f = o.length,
                 d = new Array(h);
-            for (s = 0; s < h; ++s)(u = e[s]) && (d[s] = l = o.call(u, u.__data__, s, e) + "", c.has(l) ? i[s] = u : c.set(l, u));
-            for (s = 0; s < f; ++s) l = o.call(t, a[s], s, a) + "", (u = c.get(l)) ? (r[s] = u, u.__data__ = a[s], c.delete(l)) : n[s] = new J(t, a[s]);
+            for (s = 0; s < h; ++s)(u = e[s]) && (d[s] = l = a.call(u, u.__data__, s, e) + "", c.has(l) ? i[s] = u : c.set(l, u));
+            for (s = 0; s < f; ++s) l = a.call(t, o[s], s, o) + "", (u = c.get(l)) ? (r[s] = u, u.__data__ = o[s], c.delete(l)) : n[s] = new J(t, o[s]);
             for (s = 0; s < h; ++s)(u = e[s]) && c.get(d[s]) === u && (i[s] = u)
         }
 
         function Q(t) {
             return t.__data__
         }
 
@@ -642,21 +642,21 @@
                 n = e.indexOf(":");
             return n >= 0 && "xmlns" !== (e = t.slice(0, n)) && (t = t.slice(n + 1)), rt.hasOwnProperty(e) ? {
                 space: rt[e],
                 local: t
             } : t
         }
 
-        function at(t) {
+        function ot(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
 
-        function ot(t) {
+        function at(t) {
             return function() {
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
         function st(t, e) {
             return function() {
@@ -781,19 +781,19 @@
         function Et(t) {
             return function() {
                 var e = t.apply(this, arguments);
                 this.textContent = null == e ? "" : e
             }
         }
 
-        function Tt() {
+        function jt() {
             this.innerHTML = ""
         }
 
-        function jt(t) {
+        function Tt(t) {
             return function() {
                 this.innerHTML = t
             }
         }
 
         function Pt(t) {
             return function() {
@@ -806,80 +806,80 @@
             this.nextSibling && this.parentNode.appendChild(this)
         }
 
         function Ot() {
             this.previousSibling && this.parentNode.insertBefore(this, this.parentNode.firstChild)
         }
 
-        function Vt(t) {
+        function It(t) {
             return function() {
                 var e = this.ownerDocument,
                     n = this.namespaceURI;
                 return n === nt && e.documentElement.namespaceURI === nt ? e.createElement(t) : e.createElementNS(n, t)
             }
         }
 
-        function Dt(t) {
+        function Vt(t) {
             return function() {
                 return this.ownerDocument.createElementNS(t.space, t.local)
             }
         }
 
-        function qt(t) {
+        function Dt(t) {
             var e = it(t);
-            return (e.local ? Dt : Vt)(e)
+            return (e.local ? Vt : It)(e)
         }
 
-        function It() {
+        function qt() {
             return null
         }
 
-        function Ht() {
+        function Lt() {
             var t = this.parentNode;
             t && t.removeChild(this)
         }
 
-        function Lt() {
+        function Ht() {
             var t = this.cloneNode(!1),
                 e = this.parentNode;
             return e ? e.insertBefore(t, this.nextSibling) : t
         }
 
         function Xt() {
             var t = this.cloneNode(!0),
                 e = this.parentNode;
             return e ? e.insertBefore(t, this.nextSibling) : t
         }
 
-        function Rt(t) {
+        function zt(t) {
             return function() {
                 var e = this.__on;
                 if (e) {
-                    for (var n, r = 0, i = -1, a = e.length; r < a; ++r) n = e[r], t.type && n.type !== t.type || n.name !== t.name ? e[++i] = n : this.removeEventListener(n.type, n.listener, n.options);
+                    for (var n, r = 0, i = -1, o = e.length; r < o; ++r) n = e[r], t.type && n.type !== t.type || n.name !== t.name ? e[++i] = n : this.removeEventListener(n.type, n.listener, n.options);
                     ++i ? e.length = i : delete this.__on
                 }
             }
         }
 
-        function zt(t, e, n) {
+        function Rt(t, e, n) {
             return function() {
                 var r, i = this.__on,
-                    a = function(t) {
+                    o = function(t) {
                         return function(e) {
                             t.call(this, e, this.__data__)
                         }
                     }(e);
                 if (i)
-                    for (var o = 0, s = i.length; o < s; ++o)
-                        if ((r = i[o]).type === t.type && r.name === t.name) return this.removeEventListener(r.type, r.listener, r.options), this.addEventListener(r.type, r.listener = a, r.options = n), void(r.value = e);
-                this.addEventListener(t.type, a, n), r = {
+                    for (var a = 0, s = i.length; a < s; ++a)
+                        if ((r = i[a]).type === t.type && r.name === t.name) return this.removeEventListener(r.type, r.listener, r.options), this.addEventListener(r.type, r.listener = o, r.options = n), void(r.value = e);
+                this.addEventListener(t.type, o, n), r = {
                     type: t.type,
                     name: t.name,
                     value: e,
-                    listener: a,
+                    listener: o,
                     options: n
                 }, i ? i.push(r) : this.__on = [r]
             }
         }
 
         function Yt(t, e, n) {
             var r = ht(t),
@@ -920,28 +920,28 @@
             return new Ut([
                 [document.documentElement]
             ], Ft)
         }
         Ut.prototype = Gt.prototype = {
             constructor: Ut,
             select: function(t) {
-                "function" != typeof t && (t = L(t));
+                "function" != typeof t && (t = H(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var a, o, s = e[i], u = s.length, l = r[i] = new Array(u), c = 0; c < u; ++c)(a = s[c]) && (o = t.call(a, a.__data__, c, s)) && ("__data__" in a && (o.__data__ = a.__data__), l[c] = o);
+                    for (var o, a, s = e[i], u = s.length, l = r[i] = new Array(u), c = 0; c < u; ++c)(o = s[c]) && (a = t.call(o, o.__data__, c, s)) && ("__data__" in o && (a.__data__ = o.__data__), l[c] = a);
                 return new Ut(r, this._parents)
             },
             selectAll: function(t) {
                 t = "function" == typeof t ? function(t) {
                     return function() {
                         return null == (e = t.apply(this, arguments)) ? [] : Array.isArray(e) ? e : Array.from(e);
                         var e
                     }
-                }(t) : R(t);
-                for (var e = this._groups, n = e.length, r = [], i = [], a = 0; a < n; ++a)
-                    for (var o, s = e[a], u = s.length, l = 0; l < u; ++l)(o = s[l]) && (r.push(t.call(o, o.__data__, l, s)), i.push(o));
+                }(t) : z(t);
+                for (var e = this._groups, n = e.length, r = [], i = [], o = 0; o < n; ++o)
+                    for (var a, s = e[o], u = s.length, l = 0; l < u; ++l)(a = s[l]) && (r.push(t.call(a, a.__data__, l, s)), i.push(a));
                 return new Ut(r, i)
             },
             selectChild: function(t) {
                 return this.select(null == t ? W : function(t) {
                     return function() {
                         return B.call(this.children, t)
                     }
@@ -951,30 +951,30 @@
                 return this.selectAll(null == t ? U : function(t) {
                     return function() {
                         return F.call(this.children, t)
                     }
                 }("function" == typeof t ? t : Y(t)))
             },
             filter: function(t) {
-                "function" != typeof t && (t = z(t));
+                "function" != typeof t && (t = R(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var a, o = e[i], s = o.length, u = r[i] = [], l = 0; l < s; ++l)(a = o[l]) && t.call(a, a.__data__, l, o) && u.push(a);
+                    for (var o, a = e[i], s = a.length, u = r[i] = [], l = 0; l < s; ++l)(o = a[l]) && t.call(o, o.__data__, l, a) && u.push(o);
                 return new Ut(r, this._parents)
             },
             data: function(t, e) {
                 if (!arguments.length) return Array.from(this, Q);
                 var n, r = e ? Z : K,
                     i = this._parents,
-                    a = this._groups;
+                    o = this._groups;
                 "function" != typeof t && (n = t, t = function() {
                     return n
                 });
-                for (var o = a.length, s = new Array(o), u = new Array(o), l = new Array(o), c = 0; c < o; ++c) {
+                for (var a = o.length, s = new Array(a), u = new Array(a), l = new Array(a), c = 0; c < a; ++c) {
                     var h = i[c],
-                        f = a[c],
+                        f = o[c],
                         d = f.length,
                         p = tt(t.call(h, h && h.__data__, c, i)),
                         m = p.length,
                         _ = u[c] = new Array(m),
                         g = s[c] = new Array(m);
                     r(h, f, _, g, l[c] = new Array(d), p, e);
                     for (var v, y, w = 0, x = 0; w < m; ++w)
@@ -990,155 +990,155 @@
             },
             exit: function() {
                 return new Ut(this._exit || this._groups.map(G), this._parents)
             },
             join: function(t, e, n) {
                 var r = this.enter(),
                     i = this,
-                    a = this.exit();
-                return "function" == typeof t ? (r = t(r)) && (r = r.selection()) : r = r.append(t + ""), null != e && (i = e(i)) && (i = i.selection()), null == n ? a.remove() : n(a), r && i ? r.merge(i).order() : i
+                    o = this.exit();
+                return "function" == typeof t ? (r = t(r)) && (r = r.selection()) : r = r.append(t + ""), null != e && (i = e(i)) && (i = i.selection()), null == n ? o.remove() : n(o), r && i ? r.merge(i).order() : i
             },
             merge: function(t) {
-                for (var e = t.selection ? t.selection() : t, n = this._groups, r = e._groups, i = n.length, a = r.length, o = Math.min(i, a), s = new Array(i), u = 0; u < o; ++u)
+                for (var e = t.selection ? t.selection() : t, n = this._groups, r = e._groups, i = n.length, o = r.length, a = Math.min(i, o), s = new Array(i), u = 0; u < a; ++u)
                     for (var l, c = n[u], h = r[u], f = c.length, d = s[u] = new Array(f), p = 0; p < f; ++p)(l = c[p] || h[p]) && (d[p] = l);
                 for (; u < i; ++u) s[u] = n[u];
                 return new Ut(s, this._parents)
             },
             selection: function() {
                 return this
             },
             order: function() {
                 for (var t = this._groups, e = -1, n = t.length; ++e < n;)
-                    for (var r, i = t[e], a = i.length - 1, o = i[a]; --a >= 0;)(r = i[a]) && (o && 4 ^ r.compareDocumentPosition(o) && o.parentNode.insertBefore(r, o), o = r);
+                    for (var r, i = t[e], o = i.length - 1, a = i[o]; --o >= 0;)(r = i[o]) && (a && 4 ^ r.compareDocumentPosition(a) && a.parentNode.insertBefore(r, a), a = r);
                 return this
             },
             sort: function(t) {
                 function e(e, n) {
                     return e && n ? t(e.__data__, n.__data__) : !e - !n
                 }
                 t || (t = et);
-                for (var n = this._groups, r = n.length, i = new Array(r), a = 0; a < r; ++a) {
-                    for (var o, s = n[a], u = s.length, l = i[a] = new Array(u), c = 0; c < u; ++c)(o = s[c]) && (l[c] = o);
+                for (var n = this._groups, r = n.length, i = new Array(r), o = 0; o < r; ++o) {
+                    for (var a, s = n[o], u = s.length, l = i[o] = new Array(u), c = 0; c < u; ++c)(a = s[c]) && (l[c] = a);
                     l.sort(e)
                 }
                 return new Ut(i, this._parents).order()
             },
             call: function() {
                 var t = arguments[0];
                 return arguments[0] = this, t.apply(null, arguments), this
             },
             nodes: function() {
                 return Array.from(this)
             },
             node: function() {
                 for (var t = this._groups, e = 0, n = t.length; e < n; ++e)
-                    for (var r = t[e], i = 0, a = r.length; i < a; ++i) {
-                        var o = r[i];
-                        if (o) return o
+                    for (var r = t[e], i = 0, o = r.length; i < o; ++i) {
+                        var a = r[i];
+                        if (a) return a
                     }
                 return null
             },
             size: function() {
                 let t = 0;
                 for (const e of this) ++t;
                 return t
             },
             empty: function() {
                 return !this.node()
             },
             each: function(t) {
                 for (var e = this._groups, n = 0, r = e.length; n < r; ++n)
-                    for (var i, a = e[n], o = 0, s = a.length; o < s; ++o)(i = a[o]) && t.call(i, i.__data__, o, a);
+                    for (var i, o = e[n], a = 0, s = o.length; a < s; ++a)(i = o[a]) && t.call(i, i.__data__, a, o);
                 return this
             },
             attr: function(t, e) {
                 var n = it(t);
                 if (arguments.length < 2) {
                     var r = this.node();
                     return n.local ? r.getAttributeNS(n.space, n.local) : r.getAttribute(n)
                 }
-                return this.each((null == e ? n.local ? ot : at : "function" == typeof e ? n.local ? ct : lt : n.local ? ut : st)(n, e))
+                return this.each((null == e ? n.local ? at : ot : "function" == typeof e ? n.local ? ct : lt : n.local ? ut : st)(n, e))
             },
             style: function(t, e, n) {
                 return arguments.length > 1 ? this.each((null == e ? ft : "function" == typeof e ? pt : dt)(t, e, null == n ? "" : n)) : mt(this.node(), t)
             },
             property: function(t, e) {
                 return arguments.length > 1 ? this.each((null == e ? _t : "function" == typeof e ? vt : gt)(t, e)) : this.node()[t]
             },
             classed: function(t, e) {
                 var n = yt(t + "");
                 if (arguments.length < 2) {
-                    for (var r = wt(this.node()), i = -1, a = n.length; ++i < a;)
+                    for (var r = wt(this.node()), i = -1, o = n.length; ++i < o;)
                         if (!r.contains(n[i])) return !1;
                     return !0
                 }
                 return this.each(("function" == typeof e ? Nt : e ? kt : At)(n, e))
             },
             text: function(t) {
                 return arguments.length ? this.each(null == t ? $t : ("function" == typeof t ? Et : St)(t)) : this.node().textContent
             },
             html: function(t) {
-                return arguments.length ? this.each(null == t ? Tt : ("function" == typeof t ? Pt : jt)(t)) : this.node().innerHTML
+                return arguments.length ? this.each(null == t ? jt : ("function" == typeof t ? Pt : Tt)(t)) : this.node().innerHTML
             },
             raise: function() {
                 return this.each(Ct)
             },
             lower: function() {
                 return this.each(Ot)
             },
             append: function(t) {
-                var e = "function" == typeof t ? t : qt(t);
+                var e = "function" == typeof t ? t : Dt(t);
                 return this.select((function() {
                     return this.appendChild(e.apply(this, arguments))
                 }))
             },
             insert: function(t, e) {
-                var n = "function" == typeof t ? t : qt(t),
-                    r = null == e ? It : "function" == typeof e ? e : L(e);
+                var n = "function" == typeof t ? t : Dt(t),
+                    r = null == e ? qt : "function" == typeof e ? e : H(e);
                 return this.select((function() {
                     return this.insertBefore(n.apply(this, arguments), r.apply(this, arguments) || null)
                 }))
             },
             remove: function() {
-                return this.each(Ht)
+                return this.each(Lt)
             },
             clone: function(t) {
-                return this.select(t ? Xt : Lt)
+                return this.select(t ? Xt : Ht)
             },
             datum: function(t) {
                 return arguments.length ? this.property("__data__", t) : this.node().__data__
             },
             on: function(t, e, n) {
-                var r, i, a = function(t) {
+                var r, i, o = function(t) {
                         return t.trim().split(/^|\s+/).map((function(t) {
                             var e = "",
                                 n = t.indexOf(".");
                             return n >= 0 && (e = t.slice(n + 1), t = t.slice(0, n)), {
                                 type: t,
                                 name: e
                             }
                         }))
                     }(t + ""),
-                    o = a.length;
+                    a = o.length;
                 if (!(arguments.length < 2)) {
-                    for (s = e ? zt : Rt, r = 0; r < o; ++r) this.each(s(a[r], e, n));
+                    for (s = e ? Rt : zt, r = 0; r < a; ++r) this.each(s(o[r], e, n));
                     return this
                 }
                 var s = this.node().__on;
                 if (s)
                     for (var u, l = 0, c = s.length; l < c; ++l)
-                        for (r = 0, u = s[l]; r < o; ++r)
-                            if ((i = a[r]).type === u.type && i.name === u.name) return u.value
+                        for (r = 0, u = s[l]; r < a; ++r)
+                            if ((i = o[r]).type === u.type && i.name === u.name) return u.value
             },
             dispatch: function(t, e) {
                 return this.each(("function" == typeof e ? Wt : Bt)(t, e))
             },
             [Symbol.iterator]: function*() {
                 for (var t = this._groups, e = 0, n = t.length; e < n; ++e)
-                    for (var r, i = t[e], a = 0, o = i.length; a < o; ++a)(r = i[a]) && (yield r)
+                    for (var r, i = t[e], o = 0, a = i.length; o < a; ++o)(r = i[o]) && (yield r)
             }
         };
         const Jt = Gt;
         var Kt = {
             value: () => {}
         };
 
@@ -1169,56 +1169,56 @@
                 value: n
             }), t
         }
         Qt.prototype = Zt.prototype = {
             constructor: Qt,
             on: function(t, e) {
                 var n, r, i = this._,
-                    a = (r = i, (t + "").trim().split(/^|\s+/).map((function(t) {
+                    o = (r = i, (t + "").trim().split(/^|\s+/).map((function(t) {
                         var e = "",
                             n = t.indexOf(".");
                         if (n >= 0 && (e = t.slice(n + 1), t = t.slice(0, n)), t && !r.hasOwnProperty(t)) throw new Error("unknown type: " + t);
                         return {
                             type: t,
                             name: e
                         }
                     }))),
-                    o = -1,
-                    s = a.length;
+                    a = -1,
+                    s = o.length;
                 if (!(arguments.length < 2)) {
                     if (null != e && "function" != typeof e) throw new Error("invalid callback: " + e);
-                    for (; ++o < s;)
-                        if (n = (t = a[o]).type) i[n] = ee(i[n], t.name, e);
+                    for (; ++a < s;)
+                        if (n = (t = o[a]).type) i[n] = ee(i[n], t.name, e);
                         else if (null == e)
                         for (n in i) i[n] = ee(i[n], t.name, null);
                     return this
                 }
-                for (; ++o < s;)
-                    if ((n = (t = a[o]).type) && (n = te(i[n], t.name))) return n
+                for (; ++a < s;)
+                    if ((n = (t = o[a]).type) && (n = te(i[n], t.name))) return n
             },
             copy: function() {
                 var t = {},
                     e = this._;
                 for (var n in e) t[n] = e[n].slice();
                 return new Qt(t)
             },
             call: function(t, e) {
                 if ((n = arguments.length - 2) > 0)
-                    for (var n, r, i = new Array(n), a = 0; a < n; ++a) i[a] = arguments[a + 2];
+                    for (var n, r, i = new Array(n), o = 0; o < n; ++o) i[o] = arguments[o + 2];
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
-                for (a = 0, n = (r = this._[t]).length; a < n; ++a) r[a].value.apply(e, i)
+                for (o = 0, n = (r = this._[t]).length; o < n; ++o) r[o].value.apply(e, i)
             },
             apply: function(t, e, n) {
                 if (!this._.hasOwnProperty(t)) throw new Error("unknown type: " + t);
-                for (var r = this._[t], i = 0, a = r.length; i < a; ++i) r[i].value.apply(e, n)
+                for (var r = this._[t], i = 0, o = r.length; i < o; ++i) r[i].value.apply(e, n)
             }
         };
         const ne = Zt;
-        var re, ie, ae = 0,
-            oe = 0,
+        var re, ie, oe = 0,
+            ae = 0,
             se = 0,
             ue = 1e3,
             le = 0,
             ce = 0,
             he = 0,
             fe = "object" == typeof performance && performance.now ? performance : Date,
             de = "object" == typeof window && window.requestAnimationFrame ? window.requestAnimationFrame.bind(window) : function(t) {
@@ -1239,38 +1239,38 @@
 
         function ge(t, e, n) {
             var r = new _e;
             return r.restart(t, e, n), r
         }
 
         function ve() {
-            ce = (le = fe.now()) + he, ae = oe = 0;
+            ce = (le = fe.now()) + he, oe = ae = 0;
             try {
                 ! function() {
-                    pe(), ++ae;
+                    pe(), ++oe;
                     for (var t, e = re; e;)(t = ce - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
-                    --ae
+                    --oe
                 }()
             } finally {
-                ae = 0,
+                oe = 0,
                     function() {
                         for (var t, e, n = re, r = 1 / 0; n;) n._call ? (r > n._time && (r = n._time), t = n, n = n._next) : (e = n._next, n._next = null, n = t ? t._next = e : re = e);
                         ie = t, we(r)
                     }(), ce = 0
             }
         }
 
         function ye() {
             var t = fe.now(),
                 e = t - le;
             e > ue && (he -= e, le = t)
         }
 
         function we(t) {
-            ae || (oe && (oe = clearTimeout(oe)), t - ce > 24 ? (t < 1 / 0 && (oe = setTimeout(ve, t - fe.now() - he)), se && (se = clearInterval(se))) : (se || (le = fe.now(), se = setInterval(ye, ue)), ae = 1, de(ve)))
+            oe || (ae && (ae = clearTimeout(ae)), t - ce > 24 ? (t < 1 / 0 && (ae = setTimeout(ve, t - fe.now() - he)), se && (se = clearInterval(se))) : (se || (le = fe.now(), se = setInterval(ye, ue)), oe = 1, de(ve)))
         }
 
         function xe(t, e, n) {
             var r = new _e;
             return e = null == e ? 0 : +e, r.restart((n => {
                 r.stop(), t(n + e)
             }), e, n), r
@@ -1286,59 +1286,59 @@
             }
         };
         var be = ne("start", "end", "cancel", "interrupt"),
             Me = [],
             ke = 0,
             Ae = 3;
 
-        function Ne(t, e, n, r, i, a) {
-            var o = t.__transition;
-            if (o) {
-                if (n in o) return
+        function Ne(t, e, n, r, i, o) {
+            var a = t.__transition;
+            if (a) {
+                if (n in a) return
             } else t.__transition = {};
             ! function(t, e, n) {
                 var r, i = t.__transition;
 
-                function a(u) {
+                function o(u) {
                     var l, c, h, f;
                     if (1 !== n.state) return s();
                     for (l in i)
                         if ((f = i[l]).name === n.name) {
-                            if (f.state === Ae) return xe(a);
+                            if (f.state === Ae) return xe(o);
                             4 === f.state ? (f.state = 6, f.timer.stop(), f.on.call("interrupt", t, t.__data__, f.index, f.group), delete i[l]) : +l < e && (f.state = 6, f.timer.stop(), f.on.call("cancel", t, t.__data__, f.index, f.group), delete i[l])
                         } if (xe((function() {
-                            n.state === Ae && (n.state = 4, n.timer.restart(o, n.delay, n.time), o(u))
+                            n.state === Ae && (n.state = 4, n.timer.restart(a, n.delay, n.time), a(u))
                         })), n.state = 2, n.on.call("start", t, t.__data__, n.index, n.group), 2 === n.state) {
                         for (n.state = Ae, r = new Array(h = n.tween.length), l = 0, c = -1; l < h; ++l)(f = n.tween[l].value.call(t, t.__data__, n.index, n.group)) && (r[++c] = f);
                         r.length = c + 1
                     }
                 }
 
-                function o(e) {
-                    for (var i = e < n.duration ? n.ease.call(null, e / n.duration) : (n.timer.restart(s), n.state = 5, 1), a = -1, o = r.length; ++a < o;) r[a].call(t, i);
+                function a(e) {
+                    for (var i = e < n.duration ? n.ease.call(null, e / n.duration) : (n.timer.restart(s), n.state = 5, 1), o = -1, a = r.length; ++o < a;) r[o].call(t, i);
                     5 === n.state && (n.on.call("end", t, t.__data__, n.index, n.group), s())
                 }
 
                 function s() {
                     for (var r in n.state = 6, n.timer.stop(), delete i[e], i) return;
                     delete t.__transition
                 }
                 i[e] = n, n.timer = ge((function(t) {
-                    n.state = 1, n.timer.restart(a, n.delay, n.time), n.delay <= t && a(t - n.delay)
+                    n.state = 1, n.timer.restart(o, n.delay, n.time), n.delay <= t && o(t - n.delay)
                 }), 0, n.time)
             }(t, n, {
                 name: e,
                 index: r,
                 group: i,
                 on: be,
                 tween: Me,
-                time: a.time,
-                delay: a.delay,
-                duration: a.duration,
-                ease: a.ease,
+                time: o.time,
+                delay: o.delay,
+                duration: o.duration,
+                ease: o.ease,
                 timer: null,
                 state: ke
             })
         }
 
         function $e(t, e) {
             var n = Ee(t, e);
@@ -1354,157 +1354,157 @@
 
         function Ee(t, e) {
             var n = t.__transition;
             if (!n || !(n = n[e])) throw new Error("transition not found");
             return n
         }
 
-        function Te(t, e) {
+        function je(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return t * (1 - n) + e * n
                 }
         }
-        var je, Pe = 180 / Math.PI,
+        var Te, Pe = 180 / Math.PI,
             Ce = {
                 translateX: 0,
                 translateY: 0,
                 rotate: 0,
                 skewX: 0,
                 scaleX: 1,
                 scaleY: 1
             };
 
-        function Oe(t, e, n, r, i, a) {
-            var o, s, u;
-            return (o = Math.sqrt(t * t + e * e)) && (t /= o, e /= o), (u = t * n + e * r) && (n -= t * u, r -= e * u), (s = Math.sqrt(n * n + r * r)) && (n /= s, r /= s, u /= s), t * r < e * n && (t = -t, e = -e, u = -u, o = -o), {
+        function Oe(t, e, n, r, i, o) {
+            var a, s, u;
+            return (a = Math.sqrt(t * t + e * e)) && (t /= a, e /= a), (u = t * n + e * r) && (n -= t * u, r -= e * u), (s = Math.sqrt(n * n + r * r)) && (n /= s, r /= s, u /= s), t * r < e * n && (t = -t, e = -e, u = -u, a = -a), {
                 translateX: i,
-                translateY: a,
+                translateY: o,
                 rotate: Math.atan2(e, t) * Pe,
                 skewX: Math.atan(u) * Pe,
-                scaleX: o,
+                scaleX: a,
                 scaleY: s
             }
         }
 
-        function Ve(t, e, n, r) {
+        function Ie(t, e, n, r) {
             function i(t) {
                 return t.length ? t.pop() + " " : ""
             }
-            return function(a, o) {
+            return function(o, a) {
                 var s = [],
                     u = [];
-                return a = t(a), o = t(o),
-                    function(t, r, i, a, o, s) {
-                        if (t !== i || r !== a) {
-                            var u = o.push("translate(", null, e, null, n);
+                return o = t(o), a = t(a),
+                    function(t, r, i, o, a, s) {
+                        if (t !== i || r !== o) {
+                            var u = a.push("translate(", null, e, null, n);
                             s.push({
                                 i: u - 4,
-                                x: Te(t, i)
+                                x: je(t, i)
                             }, {
                                 i: u - 2,
-                                x: Te(r, a)
+                                x: je(r, o)
                             })
-                        } else(i || a) && o.push("translate(" + i + e + a + n)
-                    }(a.translateX, a.translateY, o.translateX, o.translateY, s, u),
-                    function(t, e, n, a) {
-                        t !== e ? (t - e > 180 ? e += 360 : e - t > 180 && (t += 360), a.push({
+                        } else(i || o) && a.push("translate(" + i + e + o + n)
+                    }(o.translateX, o.translateY, a.translateX, a.translateY, s, u),
+                    function(t, e, n, o) {
+                        t !== e ? (t - e > 180 ? e += 360 : e - t > 180 && (t += 360), o.push({
                             i: n.push(i(n) + "rotate(", null, r) - 2,
-                            x: Te(t, e)
+                            x: je(t, e)
                         })) : e && n.push(i(n) + "rotate(" + e + r)
-                    }(a.rotate, o.rotate, s, u),
-                    function(t, e, n, a) {
-                        t !== e ? a.push({
+                    }(o.rotate, a.rotate, s, u),
+                    function(t, e, n, o) {
+                        t !== e ? o.push({
                             i: n.push(i(n) + "skewX(", null, r) - 2,
-                            x: Te(t, e)
+                            x: je(t, e)
                         }) : e && n.push(i(n) + "skewX(" + e + r)
-                    }(a.skewX, o.skewX, s, u),
-                    function(t, e, n, r, a, o) {
+                    }(o.skewX, a.skewX, s, u),
+                    function(t, e, n, r, o, a) {
                         if (t !== n || e !== r) {
-                            var s = a.push(i(a) + "scale(", null, ",", null, ")");
-                            o.push({
+                            var s = o.push(i(o) + "scale(", null, ",", null, ")");
+                            a.push({
                                 i: s - 4,
-                                x: Te(t, n)
+                                x: je(t, n)
                             }, {
                                 i: s - 2,
-                                x: Te(e, r)
+                                x: je(e, r)
                             })
-                        } else 1 === n && 1 === r || a.push(i(a) + "scale(" + n + "," + r + ")")
-                    }(a.scaleX, a.scaleY, o.scaleX, o.scaleY, s, u), a = o = null,
+                        } else 1 === n && 1 === r || o.push(i(o) + "scale(" + n + "," + r + ")")
+                    }(o.scaleX, o.scaleY, a.scaleX, a.scaleY, s, u), o = a = null,
                     function(t) {
                         for (var e, n = -1, r = u.length; ++n < r;) s[(e = u[n]).i] = e.x(t);
                         return s.join("")
                     }
             }
         }
-        var De = Ve((function(t) {
+        var Ve = Ie((function(t) {
                 const e = new("function" == typeof DOMMatrix ? DOMMatrix : WebKitCSSMatrix)(t + "");
                 return e.isIdentity ? Ce : Oe(e.a, e.b, e.c, e.d, e.e, e.f)
             }), "px, ", "px)", "deg)"),
-            qe = Ve((function(t) {
-                return null == t ? Ce : (je || (je = document.createElementNS("http://www.w3.org/2000/svg", "g")), je.setAttribute("transform", t), (t = je.transform.baseVal.consolidate()) ? Oe((t = t.matrix).a, t.b, t.c, t.d, t.e, t.f) : Ce)
+            De = Ie((function(t) {
+                return null == t ? Ce : (Te || (Te = document.createElementNS("http://www.w3.org/2000/svg", "g")), Te.setAttribute("transform", t), (t = Te.transform.baseVal.consolidate()) ? Oe((t = t.matrix).a, t.b, t.c, t.d, t.e, t.f) : Ce)
             }), ", ", ")", ")");
 
-        function Ie(t, e) {
+        function qe(t, e) {
             var n, r;
             return function() {
                 var i = Se(this, t),
-                    a = i.tween;
-                if (a !== n)
-                    for (var o = 0, s = (r = n = a).length; o < s; ++o)
-                        if (r[o].name === e) {
-                            (r = r.slice()).splice(o, 1);
+                    o = i.tween;
+                if (o !== n)
+                    for (var a = 0, s = (r = n = o).length; a < s; ++a)
+                        if (r[a].name === e) {
+                            (r = r.slice()).splice(a, 1);
                             break
                         } i.tween = r
             }
         }
 
-        function He(t, e, n) {
+        function Le(t, e, n) {
             var r, i;
             if ("function" != typeof n) throw new Error;
             return function() {
-                var a = Se(this, t),
-                    o = a.tween;
-                if (o !== r) {
-                    i = (r = o).slice();
+                var o = Se(this, t),
+                    a = o.tween;
+                if (a !== r) {
+                    i = (r = a).slice();
                     for (var s = {
                             name: e,
                             value: n
                         }, u = 0, l = i.length; u < l; ++u)
                         if (i[u].name === e) {
                             i[u] = s;
                             break
                         } u === l && i.push(s)
                 }
-                a.tween = i
+                o.tween = i
             }
         }
 
-        function Le(t, e, n) {
+        function He(t, e, n) {
             var r = t._id;
             return t.each((function() {
                     var t = Se(this, r);
                     (t.value || (t.value = {}))[e] = n.apply(this, arguments)
                 })),
                 function(t) {
                     return Ee(t, r).value[e]
                 }
         }
 
         function Xe(t, e, n) {
             t.prototype = e.prototype = n, n.constructor = t
         }
 
-        function Re(t, e) {
+        function ze(t, e) {
             var n = Object.create(t.prototype);
             for (var r in e) n[r] = e[r];
             return n
         }
 
-        function ze() {}
+        function Re() {}
         var Ye = .7,
             Be = 1 / Ye,
             We = "\\s*([+-]?\\d+)\\s*",
             Fe = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
             Ue = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
             Ge = /^#([0-9a-f]{3,8})$/,
             Je = new RegExp(`^rgb\\(${We},${We},${We}\\)$`),
@@ -1664,33 +1664,33 @@
                 yellowgreen: 10145074
             };
 
         function rn() {
             return this.rgb().formatHex()
         }
 
-        function an() {
+        function on() {
             return this.rgb().formatRgb()
         }
 
-        function on(t) {
+        function an(t) {
             var e, n;
             return t = (t + "").trim().toLowerCase(), (e = Ge.exec(t)) ? (n = e[1].length, e = parseInt(e[1], 16), 6 === n ? sn(e) : 3 === n ? new cn(e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, (15 & e) << 4 | 15 & e, 1) : 8 === n ? un(e >> 24 & 255, e >> 16 & 255, e >> 8 & 255, (255 & e) / 255) : 4 === n ? un(e >> 12 & 15 | e >> 8 & 240, e >> 8 & 15 | e >> 4 & 240, e >> 4 & 15 | 240 & e, ((15 & e) << 4 | 15 & e) / 255) : null) : (e = Je.exec(t)) ? new cn(e[1], e[2], e[3], 1) : (e = Ke.exec(t)) ? new cn(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, 1) : (e = Ze.exec(t)) ? un(e[1], e[2], e[3], e[4]) : (e = Qe.exec(t)) ? un(255 * e[1] / 100, 255 * e[2] / 100, 255 * e[3] / 100, e[4]) : (e = tn.exec(t)) ? _n(e[1], e[2] / 100, e[3] / 100, 1) : (e = en.exec(t)) ? _n(e[1], e[2] / 100, e[3] / 100, e[4]) : nn.hasOwnProperty(t) ? sn(nn[t]) : "transparent" === t ? new cn(NaN, NaN, NaN, 0) : null
         }
 
         function sn(t) {
             return new cn(t >> 16 & 255, t >> 8 & 255, 255 & t, 1)
         }
 
         function un(t, e, n, r) {
             return r <= 0 && (t = e = n = NaN), new cn(t, e, n, r)
         }
 
         function ln(t, e, n, r) {
-            return 1 === arguments.length ? ((i = t) instanceof ze || (i = on(i)), i ? new cn((i = i.rgb()).r, i.g, i.b, i.opacity) : new cn) : new cn(t, e, n, null == r ? 1 : r);
+            return 1 === arguments.length ? ((i = t) instanceof Re || (i = an(i)), i ? new cn((i = i.rgb()).r, i.g, i.b, i.opacity) : new cn) : new cn(t, e, n, null == r ? 1 : r);
             var i
         }
 
         function cn(t, e, n, r) {
             this.r = +t, this.g = +e, this.b = +n, this.opacity = +r
         }
 
@@ -1717,25 +1717,25 @@
 
         function _n(t, e, n, r) {
             return r <= 0 ? t = e = n = NaN : n <= 0 || n >= 1 ? t = e = NaN : e <= 0 && (t = NaN), new vn(t, e, n, r)
         }
 
         function gn(t) {
             if (t instanceof vn) return new vn(t.h, t.s, t.l, t.opacity);
-            if (t instanceof ze || (t = on(t)), !t) return new vn;
+            if (t instanceof Re || (t = an(t)), !t) return new vn;
             if (t instanceof vn) return t;
             var e = (t = t.rgb()).r / 255,
                 n = t.g / 255,
                 r = t.b / 255,
                 i = Math.min(e, n, r),
-                a = Math.max(e, n, r),
-                o = NaN,
-                s = a - i,
-                u = (a + i) / 2;
-            return s ? (o = e === a ? (n - r) / s + 6 * (n < r) : n === a ? (r - e) / s + 2 : (e - n) / s + 4, s /= u < .5 ? a + i : 2 - a - i, o *= 60) : s = u > 0 && u < 1 ? 0 : o, new vn(o, s, u, t.opacity)
+                o = Math.max(e, n, r),
+                a = NaN,
+                s = o - i,
+                u = (o + i) / 2;
+            return s ? (a = e === o ? (n - r) / s + 6 * (n < r) : n === o ? (r - e) / s + 2 : (e - n) / s + 4, s /= u < .5 ? o + i : 2 - o - i, a *= 60) : s = u > 0 && u < 1 ? 0 : a, new vn(a, s, u, t.opacity)
         }
 
         function vn(t, e, n, r) {
             this.h = +t, this.s = +e, this.l = +n, this.opacity = +r
         }
 
         function yn(t) {
@@ -1747,36 +1747,36 @@
         }
 
         function xn(t, e, n) {
             return 255 * (t < 60 ? e + (n - e) * t / 60 : t < 180 ? n : t < 240 ? e + (n - e) * (240 - t) / 60 : e)
         }
 
         function bn(t, e, n, r, i) {
-            var a = t * t,
-                o = a * t;
-            return ((1 - 3 * t + 3 * a - o) * e + (4 - 6 * a + 3 * o) * n + (1 + 3 * t + 3 * a - 3 * o) * r + o * i) / 6
+            var o = t * t,
+                a = o * t;
+            return ((1 - 3 * t + 3 * o - a) * e + (4 - 6 * o + 3 * a) * n + (1 + 3 * t + 3 * o - 3 * a) * r + a * i) / 6
         }
-        Xe(ze, on, {
+        Xe(Re, an, {
             copy(t) {
                 return Object.assign(new this.constructor, this, t)
             },
             displayable() {
                 return this.rgb().displayable()
             },
             hex: rn,
             formatHex: rn,
             formatHex8: function() {
                 return this.rgb().formatHex8()
             },
             formatHsl: function() {
                 return gn(this).formatHsl()
             },
-            formatRgb: an,
-            toString: an
-        }), Xe(cn, ln, Re(ze, {
+            formatRgb: on,
+            toString: on
+        }), Xe(cn, ln, ze(Re, {
             brighter(t) {
                 return t = null == t ? Be : Math.pow(Be, t), new cn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             darker(t) {
                 return t = null == t ? Ye : Math.pow(Ye, t), new cn(this.r * t, this.g * t, this.b * t, this.opacity)
             },
             rgb() {
@@ -1793,15 +1793,15 @@
             formatHex8: function() {
                 return `#${mn(this.r)}${mn(this.g)}${mn(this.b)}${mn(255*(isNaN(this.opacity)?1:this.opacity))}`
             },
             formatRgb: fn,
             toString: fn
         })), Xe(vn, (function(t, e, n, r) {
             return 1 === arguments.length ? gn(t) : new vn(t, e, n, null == r ? 1 : r)
-        }), Re(ze, {
+        }), ze(Re, {
             brighter(t) {
                 return t = null == t ? Be : Math.pow(Be, t), new vn(this.h, this.s, this.l * t, this.opacity)
             },
             darker(t) {
                 return t = null == t ? Ye : Math.pow(Ye, t), new vn(this.h, this.s, this.l * t, this.opacity)
             },
             rgb() {
@@ -1844,189 +1844,189 @@
                     }(e, n, t) : Mn(isNaN(e) ? n : e)
                 }
             }(e);
 
             function r(t, e) {
                 var r = n((t = ln(t)).r, (e = ln(e)).r),
                     i = n(t.g, e.g),
-                    a = n(t.b, e.b),
-                    o = kn(t.opacity, e.opacity);
+                    o = n(t.b, e.b),
+                    a = kn(t.opacity, e.opacity);
                 return function(e) {
-                    return t.r = r(e), t.g = i(e), t.b = a(e), t.opacity = o(e), t + ""
+                    return t.r = r(e), t.g = i(e), t.b = o(e), t.opacity = a(e), t + ""
                 }
             }
             return r.gamma = t, r
         }(1);
 
         function Nn(t) {
             return function(e) {
                 var n, r, i = e.length,
-                    a = new Array(i),
                     o = new Array(i),
+                    a = new Array(i),
                     s = new Array(i);
-                for (n = 0; n < i; ++n) r = ln(e[n]), a[n] = r.r || 0, o[n] = r.g || 0, s[n] = r.b || 0;
-                return a = t(a), o = t(o), s = t(s), r.opacity = 1,
+                for (n = 0; n < i; ++n) r = ln(e[n]), o[n] = r.r || 0, a[n] = r.g || 0, s[n] = r.b || 0;
+                return o = t(o), a = t(a), s = t(s), r.opacity = 1,
                     function(t) {
-                        return r.r = a(t), r.g = o(t), r.b = s(t), r + ""
+                        return r.r = o(t), r.g = a(t), r.b = s(t), r + ""
                     }
             }
         }
         Nn((function(t) {
             var e = t.length - 1;
             return function(n) {
                 var r = n <= 0 ? n = 0 : n >= 1 ? (n = 1, e - 1) : Math.floor(n * e),
                     i = t[r],
-                    a = t[r + 1],
-                    o = r > 0 ? t[r - 1] : 2 * i - a,
-                    s = r < e - 1 ? t[r + 2] : 2 * a - i;
-                return bn((n - r / e) * e, o, i, a, s)
+                    o = t[r + 1],
+                    a = r > 0 ? t[r - 1] : 2 * i - o,
+                    s = r < e - 1 ? t[r + 2] : 2 * o - i;
+                return bn((n - r / e) * e, a, i, o, s)
             }
         })), Nn((function(t) {
             var e = t.length;
             return function(n) {
                 var r = Math.floor(((n %= 1) < 0 ? ++n : n) * e),
                     i = t[(r + e - 1) % e],
-                    a = t[r % e],
-                    o = t[(r + 1) % e],
+                    o = t[r % e],
+                    a = t[(r + 1) % e],
                     s = t[(r + 2) % e];
-                return bn((n - r / e) * e, i, a, o, s)
+                return bn((n - r / e) * e, i, o, a, s)
             }
         }));
         var $n = /[-+]?(?:\d+\.?\d*|\.?\d+)(?:[eE][-+]?\d+)?/g,
             Sn = new RegExp($n.source, "g");
 
         function En(t, e) {
-            var n, r, i, a = $n.lastIndex = Sn.lastIndex = 0,
-                o = -1,
+            var n, r, i, o = $n.lastIndex = Sn.lastIndex = 0,
+                a = -1,
                 s = [],
                 u = [];
             for (t += "", e += "";
-                (n = $n.exec(t)) && (r = Sn.exec(e));)(i = r.index) > a && (i = e.slice(a, i), s[o] ? s[o] += i : s[++o] = i), (n = n[0]) === (r = r[0]) ? s[o] ? s[o] += r : s[++o] = r : (s[++o] = null, u.push({
-                i: o,
-                x: Te(n, r)
-            })), a = Sn.lastIndex;
-            return a < e.length && (i = e.slice(a), s[o] ? s[o] += i : s[++o] = i), s.length < 2 ? u[0] ? function(t) {
+                (n = $n.exec(t)) && (r = Sn.exec(e));)(i = r.index) > o && (i = e.slice(o, i), s[a] ? s[a] += i : s[++a] = i), (n = n[0]) === (r = r[0]) ? s[a] ? s[a] += r : s[++a] = r : (s[++a] = null, u.push({
+                i: a,
+                x: je(n, r)
+            })), o = Sn.lastIndex;
+            return o < e.length && (i = e.slice(o), s[a] ? s[a] += i : s[++a] = i), s.length < 2 ? u[0] ? function(t) {
                 return function(e) {
                     return t(e) + ""
                 }
             }(u[0].x) : function(t) {
                 return function() {
                     return t
                 }
             }(e) : (e = u.length, function(t) {
                 for (var n, r = 0; r < e; ++r) s[(n = u[r]).i] = n.x(t);
                 return s.join("")
             })
         }
 
-        function Tn(t, e) {
+        function jn(t, e) {
             var n;
-            return ("number" == typeof e ? Te : e instanceof on ? An : (n = on(e)) ? (e = n, An) : En)(t, e)
+            return ("number" == typeof e ? je : e instanceof an ? An : (n = an(e)) ? (e = n, An) : En)(t, e)
         }
 
-        function jn(t) {
+        function Tn(t) {
             return function() {
                 this.removeAttribute(t)
             }
         }
 
         function Pn(t) {
             return function() {
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
         function Cn(t, e, n) {
-            var r, i, a = n + "";
+            var r, i, o = n + "";
             return function() {
-                var o = this.getAttribute(t);
-                return o === a ? null : o === r ? i : i = e(r = o, n)
+                var a = this.getAttribute(t);
+                return a === o ? null : a === r ? i : i = e(r = a, n)
             }
         }
 
         function On(t, e, n) {
-            var r, i, a = n + "";
+            var r, i, o = n + "";
             return function() {
-                var o = this.getAttributeNS(t.space, t.local);
-                return o === a ? null : o === r ? i : i = e(r = o, n)
+                var a = this.getAttributeNS(t.space, t.local);
+                return a === o ? null : a === r ? i : i = e(r = a, n)
             }
         }
 
-        function Vn(t, e, n) {
-            var r, i, a;
+        function In(t, e, n) {
+            var r, i, o;
             return function() {
-                var o, s, u = n(this);
-                if (null != u) return (o = this.getAttribute(t)) === (s = u + "") ? null : o === r && s === i ? a : (i = s, a = e(r = o, u));
+                var a, s, u = n(this);
+                if (null != u) return (a = this.getAttribute(t)) === (s = u + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, u));
                 this.removeAttribute(t)
             }
         }
 
-        function Dn(t, e, n) {
-            var r, i, a;
+        function Vn(t, e, n) {
+            var r, i, o;
             return function() {
-                var o, s, u = n(this);
-                if (null != u) return (o = this.getAttributeNS(t.space, t.local)) === (s = u + "") ? null : o === r && s === i ? a : (i = s, a = e(r = o, u));
+                var a, s, u = n(this);
+                if (null != u) return (a = this.getAttributeNS(t.space, t.local)) === (s = u + "") ? null : a === r && s === i ? o : (i = s, o = e(r = a, u));
                 this.removeAttributeNS(t.space, t.local)
             }
         }
 
-        function qn(t, e) {
+        function Dn(t, e) {
             var n, r;
 
             function i() {
                 var i = e.apply(this, arguments);
                 return i !== r && (n = (r = i) && function(t, e) {
                     return function(n) {
                         this.setAttributeNS(t.space, t.local, e.call(this, n))
                     }
                 }(t, i)), n
             }
             return i._value = e, i
         }
 
-        function In(t, e) {
+        function qn(t, e) {
             var n, r;
 
             function i() {
                 var i = e.apply(this, arguments);
                 return i !== r && (n = (r = i) && function(t, e) {
                     return function(n) {
                         this.setAttribute(t, e.call(this, n))
                     }
                 }(t, i)), n
             }
             return i._value = e, i
         }
 
-        function Hn(t, e) {
+        function Ln(t, e) {
             return function() {
                 $e(this, t).delay = +e.apply(this, arguments)
             }
         }
 
-        function Ln(t, e) {
+        function Hn(t, e) {
             return e = +e,
                 function() {
                     $e(this, t).delay = e
                 }
         }
 
         function Xn(t, e) {
             return function() {
                 Se(this, t).duration = +e.apply(this, arguments)
             }
         }
 
-        function Rn(t, e) {
+        function zn(t, e) {
             return e = +e,
                 function() {
                     Se(this, t).duration = e
                 }
         }
-        var zn = Jt.prototype.constructor;
+        var Rn = Jt.prototype.constructor;
 
         function Yn(t) {
             return function() {
                 this.style.removeProperty(t)
             }
         }
         var Bn = 0;
@@ -2042,54 +2042,54 @@
         Wn.prototype = function(t) {
             return Jt().transition(t)
         }.prototype = {
             constructor: Wn,
             select: function(t) {
                 var e = this._name,
                     n = this._id;
-                "function" != typeof t && (t = L(t));
-                for (var r = this._groups, i = r.length, a = new Array(i), o = 0; o < i; ++o)
-                    for (var s, u, l = r[o], c = l.length, h = a[o] = new Array(c), f = 0; f < c; ++f)(s = l[f]) && (u = t.call(s, s.__data__, f, l)) && ("__data__" in s && (u.__data__ = s.__data__), h[f] = u, Ne(h[f], e, n, f, h, Ee(s, n)));
-                return new Wn(a, this._parents, e, n)
+                "function" != typeof t && (t = H(t));
+                for (var r = this._groups, i = r.length, o = new Array(i), a = 0; a < i; ++a)
+                    for (var s, u, l = r[a], c = l.length, h = o[a] = new Array(c), f = 0; f < c; ++f)(s = l[f]) && (u = t.call(s, s.__data__, f, l)) && ("__data__" in s && (u.__data__ = s.__data__), h[f] = u, Ne(h[f], e, n, f, h, Ee(s, n)));
+                return new Wn(o, this._parents, e, n)
             },
             selectAll: function(t) {
                 var e = this._name,
                     n = this._id;
-                "function" != typeof t && (t = R(t));
-                for (var r = this._groups, i = r.length, a = [], o = [], s = 0; s < i; ++s)
+                "function" != typeof t && (t = z(t));
+                for (var r = this._groups, i = r.length, o = [], a = [], s = 0; s < i; ++s)
                     for (var u, l = r[s], c = l.length, h = 0; h < c; ++h)
                         if (u = l[h]) {
                             for (var f, d = t.call(u, u.__data__, h, l), p = Ee(u, n), m = 0, _ = d.length; m < _; ++m)(f = d[m]) && Ne(f, e, n, m, d, p);
-                            a.push(d), o.push(u)
-                        } return new Wn(a, o, e, n)
+                            o.push(d), a.push(u)
+                        } return new Wn(o, a, e, n)
             },
             selectChild: Un.selectChild,
             selectChildren: Un.selectChildren,
             filter: function(t) {
-                "function" != typeof t && (t = z(t));
+                "function" != typeof t && (t = R(t));
                 for (var e = this._groups, n = e.length, r = new Array(n), i = 0; i < n; ++i)
-                    for (var a, o = e[i], s = o.length, u = r[i] = [], l = 0; l < s; ++l)(a = o[l]) && t.call(a, a.__data__, l, o) && u.push(a);
+                    for (var o, a = e[i], s = a.length, u = r[i] = [], l = 0; l < s; ++l)(o = a[l]) && t.call(o, o.__data__, l, a) && u.push(o);
                 return new Wn(r, this._parents, this._name, this._id)
             },
             merge: function(t) {
                 if (t._id !== this._id) throw new Error;
-                for (var e = this._groups, n = t._groups, r = e.length, i = n.length, a = Math.min(r, i), o = new Array(r), s = 0; s < a; ++s)
-                    for (var u, l = e[s], c = n[s], h = l.length, f = o[s] = new Array(h), d = 0; d < h; ++d)(u = l[d] || c[d]) && (f[d] = u);
-                for (; s < r; ++s) o[s] = e[s];
-                return new Wn(o, this._parents, this._name, this._id)
+                for (var e = this._groups, n = t._groups, r = e.length, i = n.length, o = Math.min(r, i), a = new Array(r), s = 0; s < o; ++s)
+                    for (var u, l = e[s], c = n[s], h = l.length, f = a[s] = new Array(h), d = 0; d < h; ++d)(u = l[d] || c[d]) && (f[d] = u);
+                for (; s < r; ++s) a[s] = e[s];
+                return new Wn(a, this._parents, this._name, this._id)
             },
             selection: function() {
-                return new zn(this._groups, this._parents)
+                return new Rn(this._groups, this._parents)
             },
             transition: function() {
-                for (var t = this._name, e = this._id, n = Fn(), r = this._groups, i = r.length, a = 0; a < i; ++a)
-                    for (var o, s = r[a], u = s.length, l = 0; l < u; ++l)
-                        if (o = s[l]) {
-                            var c = Ee(o, e);
-                            Ne(o, t, n, l, s, {
+                for (var t = this._name, e = this._id, n = Fn(), r = this._groups, i = r.length, o = 0; o < i; ++o)
+                    for (var a, s = r[o], u = s.length, l = 0; l < u; ++l)
+                        if (a = s[l]) {
+                            var c = Ee(a, e);
+                            Ne(a, t, n, l, s, {
                                 time: c.time + c.delay + c.duration,
                                 delay: 0,
                                 duration: c.duration,
                                 ease: c.ease
                             })
                         } return new Wn(r, this._parents, t, n)
             },
@@ -2098,100 +2098,100 @@
             node: Un.node,
             size: Un.size,
             empty: Un.empty,
             each: Un.each,
             on: function(t, e) {
                 var n = this._id;
                 return arguments.length < 2 ? Ee(this.node(), n).on.on(t) : this.each(function(t, e, n) {
-                    var r, i, a = function(t) {
+                    var r, i, o = function(t) {
                         return (t + "").trim().split(/^|\s+/).every((function(t) {
                             var e = t.indexOf(".");
                             return e >= 0 && (t = t.slice(0, e)), !t || "start" === t
                         }))
                     }(e) ? $e : Se;
                     return function() {
-                        var o = a(this, t),
-                            s = o.on;
-                        s !== r && (i = (r = s).copy()).on(e, n), o.on = i
+                        var a = o(this, t),
+                            s = a.on;
+                        s !== r && (i = (r = s).copy()).on(e, n), a.on = i
                     }
                 }(n, t, e))
             },
             attr: function(t, e) {
                 var n = it(t),
-                    r = "transform" === n ? qe : Tn;
-                return this.attrTween(t, "function" == typeof e ? (n.local ? Dn : Vn)(n, r, Le(this, "attr." + t, e)) : null == e ? (n.local ? Pn : jn)(n) : (n.local ? On : Cn)(n, r, e))
+                    r = "transform" === n ? De : jn;
+                return this.attrTween(t, "function" == typeof e ? (n.local ? Vn : In)(n, r, He(this, "attr." + t, e)) : null == e ? (n.local ? Pn : Tn)(n) : (n.local ? On : Cn)(n, r, e))
             },
             attrTween: function(t, e) {
                 var n = "attr." + t;
                 if (arguments.length < 2) return (n = this.tween(n)) && n._value;
                 if (null == e) return this.tween(n, null);
                 if ("function" != typeof e) throw new Error;
                 var r = it(t);
-                return this.tween(n, (r.local ? qn : In)(r, e))
+                return this.tween(n, (r.local ? Dn : qn)(r, e))
             },
             style: function(t, e, n) {
-                var r = "transform" == (t += "") ? De : Tn;
+                var r = "transform" == (t += "") ? Ve : jn;
                 return null == e ? this.styleTween(t, function(t, e) {
                     var n, r, i;
                     return function() {
-                        var a = mt(this, t),
-                            o = (this.style.removeProperty(t), mt(this, t));
-                        return a === o ? null : a === n && o === r ? i : i = e(n = a, r = o)
+                        var o = mt(this, t),
+                            a = (this.style.removeProperty(t), mt(this, t));
+                        return o === a ? null : o === n && a === r ? i : i = e(n = o, r = a)
                     }
                 }(t, r)).on("end.style." + t, Yn(t)) : "function" == typeof e ? this.styleTween(t, function(t, e, n) {
-                    var r, i, a;
+                    var r, i, o;
                     return function() {
-                        var o = mt(this, t),
+                        var a = mt(this, t),
                             s = n(this),
                             u = s + "";
-                        return null == s && (this.style.removeProperty(t), u = s = mt(this, t)), o === u ? null : o === r && u === i ? a : (i = u, a = e(r = o, s))
+                        return null == s && (this.style.removeProperty(t), u = s = mt(this, t)), a === u ? null : a === r && u === i ? o : (i = u, o = e(r = a, s))
                     }
-                }(t, r, Le(this, "style." + t, e))).each(function(t, e) {
-                    var n, r, i, a, o = "style." + e,
-                        s = "end." + o;
+                }(t, r, He(this, "style." + t, e))).each(function(t, e) {
+                    var n, r, i, o, a = "style." + e,
+                        s = "end." + a;
                     return function() {
                         var u = Se(this, t),
                             l = u.on,
-                            c = null == u.value[o] ? a || (a = Yn(e)) : void 0;
+                            c = null == u.value[a] ? o || (o = Yn(e)) : void 0;
                         l === n && i === c || (r = (n = l).copy()).on(s, i = c), u.on = r
                     }
                 }(this._id, t)) : this.styleTween(t, function(t, e, n) {
-                    var r, i, a = n + "";
+                    var r, i, o = n + "";
                     return function() {
-                        var o = mt(this, t);
-                        return o === a ? null : o === r ? i : i = e(r = o, n)
+                        var a = mt(this, t);
+                        return a === o ? null : a === r ? i : i = e(r = a, n)
                     }
                 }(t, r, e), n).on("end.style." + t, null)
             },
             styleTween: function(t, e, n) {
                 var r = "style." + (t += "");
                 if (arguments.length < 2) return (r = this.tween(r)) && r._value;
                 if (null == e) return this.tween(r, null);
                 if ("function" != typeof e) throw new Error;
                 return this.tween(r, function(t, e, n) {
                     var r, i;
 
-                    function a() {
-                        var a = e.apply(this, arguments);
-                        return a !== i && (r = (i = a) && function(t, e, n) {
+                    function o() {
+                        var o = e.apply(this, arguments);
+                        return o !== i && (r = (i = o) && function(t, e, n) {
                             return function(r) {
                                 this.style.setProperty(t, e.call(this, r), n)
                             }
-                        }(t, a, n)), r
+                        }(t, o, n)), r
                     }
-                    return a._value = e, a
+                    return o._value = e, o
                 }(t, e, null == n ? "" : n))
             },
             text: function(t) {
                 return this.tween("text", "function" == typeof t ? function(t) {
                     return function() {
                         var e = t(this);
                         this.textContent = null == e ? "" : e
                     }
-                }(Le(this, "text", t)) : function(t) {
+                }(He(this, "text", t)) : function(t) {
                     return function() {
                         this.textContent = t
                     }
                 }(null == t ? "" : t + ""))
             },
             textTween: function(t) {
                 var e = "text";
@@ -2221,27 +2221,27 @@
                         e && e.removeChild(this)
                     }
                 }(this._id))
             },
             tween: function(t, e) {
                 var n = this._id;
                 if (t += "", arguments.length < 2) {
-                    for (var r, i = Ee(this.node(), n).tween, a = 0, o = i.length; a < o; ++a)
-                        if ((r = i[a]).name === t) return r.value;
+                    for (var r, i = Ee(this.node(), n).tween, o = 0, a = i.length; o < a; ++o)
+                        if ((r = i[o]).name === t) return r.value;
                     return null
                 }
-                return this.each((null == e ? Ie : He)(n, t, e))
+                return this.each((null == e ? qe : Le)(n, t, e))
             },
             delay: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? Hn : Ln)(e, t)) : Ee(this.node(), e).delay
+                return arguments.length ? this.each(("function" == typeof t ? Ln : Hn)(e, t)) : Ee(this.node(), e).delay
             },
             duration: function(t) {
                 var e = this._id;
-                return arguments.length ? this.each(("function" == typeof t ? Xn : Rn)(e, t)) : Ee(this.node(), e).duration
+                return arguments.length ? this.each(("function" == typeof t ? Xn : zn)(e, t)) : Ee(this.node(), e).duration
             },
             ease: function(t) {
                 var e = this._id;
                 return arguments.length ? this.each(function(t, e) {
                     if ("function" != typeof e) throw new Error;
                     return function() {
                         Se(this, t).ease = e
@@ -2258,28 +2258,28 @@
                     }
                 }(this._id, t))
             },
             end: function() {
                 var t, e, n = this,
                     r = n._id,
                     i = n.size();
-                return new Promise((function(a, o) {
+                return new Promise((function(o, a) {
                     var s = {
-                            value: o
+                            value: a
                         },
                         u = {
                             value: function() {
-                                0 == --i && a()
+                                0 == --i && o()
                             }
                         };
                     n.each((function() {
                         var n = Se(this, r),
                             i = n.on;
                         i !== t && ((e = (t = i).copy())._.cancel.push(s), e._.interrupt.push(s), e._.end.push(u)), n.on = e
-                    })), 0 === i && a()
+                    })), 0 === i && o()
                 }))
             },
             [Symbol.iterator]: Un[Symbol.iterator]
         };
         var Gn = {
             time: null,
             delay: 0,
@@ -2293,27 +2293,27 @@
             for (var n; !(n = t.__transition) || !(n = n[e]);)
                 if (!(t = t.parentNode)) throw new Error(`transition ${e} not found`);
             return n
         }
         Jt.prototype.interrupt = function(t) {
             return this.each((function() {
                 ! function(t, e) {
-                    var n, r, i, a = t.__transition,
-                        o = !0;
-                    if (a) {
-                        for (i in e = null == e ? null : e + "", a)(n = a[i]).name === e ? (r = n.state > 2 && n.state < 5, n.state = 6, n.timer.stop(), n.on.call(r ? "interrupt" : "cancel", t, t.__data__, n.index, n.group), delete a[i]) : o = !1;
-                        o && delete t.__transition
+                    var n, r, i, o = t.__transition,
+                        a = !0;
+                    if (o) {
+                        for (i in e = null == e ? null : e + "", o)(n = o[i]).name === e ? (r = n.state > 2 && n.state < 5, n.state = 6, n.timer.stop(), n.on.call(r ? "interrupt" : "cancel", t, t.__data__, n.index, n.group), delete o[i]) : a = !1;
+                        a && delete t.__transition
                     }
                 }(this, t)
             }))
         }, Jt.prototype.transition = function(t) {
             var e, n;
             t instanceof Wn ? (e = t._id, t = t._name) : (e = Fn(), (n = Gn).time = pe(), t = null == t ? null : t + "");
-            for (var r = this._groups, i = r.length, a = 0; a < i; ++a)
-                for (var o, s = r[a], u = s.length, l = 0; l < u; ++l)(o = s[l]) && Ne(o, t, e, l, s, n || Jn(o, e));
+            for (var r = this._groups, i = r.length, o = 0; o < i; ++o)
+                for (var a, s = r[o], u = s.length, l = 0; l < u; ++l)(a = s[l]) && Ne(a, t, e, l, s, n || Jn(a, e));
             return new Wn(r, this._parents, t, e)
         };
         const {
             abs: Kn,
             max: Zn,
             min: Qn
         } = Math;
@@ -2354,30 +2354,30 @@
                 passive: !1
             },
             ir = {
                 capture: !0,
                 passive: !1
             };
 
-        function ar(t) {
+        function or(t) {
             t.stopImmediatePropagation()
         }
 
-        function or(t) {
+        function ar(t) {
             t.preventDefault(), t.stopImmediatePropagation()
         }
         const sr = t => () => t;
 
         function ur(t, {
             sourceEvent: e,
             subject: n,
             target: r,
             identifier: i,
-            active: a,
-            x: o,
+            active: o,
+            x: a,
             y: s,
             dx: u,
             dy: l,
             dispatch: c
         }) {
             Object.defineProperties(this, {
                 type: {
@@ -2402,20 +2402,20 @@
                 },
                 identifier: {
                     value: i,
                     enumerable: !0,
                     configurable: !0
                 },
                 active: {
-                    value: a,
+                    value: o,
                     enumerable: !0,
                     configurable: !0
                 },
                 x: {
-                    value: o,
+                    value: a,
                     enumerable: !0,
                     configurable: !0
                 },
                 y: {
                     value: s,
                     enumerable: !0,
                     configurable: !0
@@ -2526,20 +2526,20 @@
         function vr() {
             var t = new pr,
                 e = [],
                 n = [],
                 r = gr;
 
             function i(i) {
-                let a = t.get(i);
-                if (void 0 === a) {
+                let o = t.get(i);
+                if (void 0 === o) {
                     if (r !== gr) return r;
-                    t.set(i, a = e.push(i) - 1)
+                    t.set(i, o = e.push(i) - 1)
                 }
-                return n[a % n.length]
+                return n[o % n.length]
             }
             return i.domain = function(n) {
                 if (!arguments.length) return e.slice();
                 e = [], t = new pr;
                 for (const r of n) t.has(r) || t.set(r, e.push(r) - 1);
                 return i
             }, i.range = function(t) {
@@ -2551,42 +2551,42 @@
             }, dr.apply(i, arguments), i
         }
 
         function yr() {
             var t, e, n = vr().unknown(void 0),
                 r = n.domain,
                 i = n.range,
-                a = 0,
-                o = 1,
+                o = 0,
+                a = 1,
                 s = !1,
                 u = 0,
                 l = 0,
                 c = .5;
 
             function h() {
                 var n = r().length,
-                    h = o < a,
-                    f = h ? o : a,
-                    d = h ? a : o;
+                    h = a < o,
+                    f = h ? a : o,
+                    d = h ? o : a;
                 t = (d - f) / Math.max(1, n - u + 2 * l), s && (t = Math.floor(t)), f += (d - f - t * (n - u)) * c, e = t * (1 - u), s && (f = Math.round(f), e = Math.round(e));
                 var p = function(t, e, n) {
                     t = +t, e = +e, n = (i = arguments.length) < 2 ? (e = t, t = 0, 1) : i < 3 ? 1 : +n;
-                    for (var r = -1, i = 0 | Math.max(0, Math.ceil((e - t) / n)), a = new Array(i); ++r < i;) a[r] = t + r * n;
-                    return a
+                    for (var r = -1, i = 0 | Math.max(0, Math.ceil((e - t) / n)), o = new Array(i); ++r < i;) o[r] = t + r * n;
+                    return o
                 }(n).map((function(e) {
                     return f + t * e
                 }));
                 return i(h ? p.reverse() : p)
             }
             return delete n.unknown, n.domain = function(t) {
                 return arguments.length ? (r(t), h()) : r()
             }, n.range = function(t) {
-                return arguments.length ? ([a, o] = t, a = +a, o = +o, h()) : [a, o]
+                return arguments.length ? ([o, a] = t, o = +o, a = +a, h()) : [o, a]
             }, n.rangeRound = function(t) {
-                return [a, o] = t, a = +a, o = +o, s = !0, h()
+                return [o, a] = t, o = +o, a = +a, s = !0, h()
             }, n.bandwidth = function() {
                 return e
             }, n.step = function() {
                 return t
             }, n.round = function(t) {
                 return arguments.length ? (s = !!t, h()) : s
             }, n.padding = function(t) {
@@ -2594,28 +2594,28 @@
             }, n.paddingInner = function(t) {
                 return arguments.length ? (u = Math.min(1, t), h()) : u
             }, n.paddingOuter = function(t) {
                 return arguments.length ? (l = +t, h()) : l
             }, n.align = function(t) {
                 return arguments.length ? (c = Math.max(0, Math.min(1, t)), h()) : c
             }, n.copy = function() {
-                return yr(r(), [a, o]).round(s).paddingInner(u).paddingOuter(l).align(c)
+                return yr(r(), [o, a]).round(s).paddingInner(u).paddingOuter(l).align(c)
             }, dr.apply(h(), arguments)
         }
 
         function wr(t, e) {
             var n, r = e ? e.length : 0,
                 i = t ? Math.min(r, t.length) : 0,
-                a = new Array(i),
-                o = new Array(r);
-            for (n = 0; n < i; ++n) a[n] = kr(t[n], e[n]);
-            for (; n < r; ++n) o[n] = e[n];
+                o = new Array(i),
+                a = new Array(r);
+            for (n = 0; n < i; ++n) o[n] = kr(t[n], e[n]);
+            for (; n < r; ++n) a[n] = e[n];
             return function(t) {
-                for (n = 0; n < i; ++n) o[n] = a[n](t);
-                return o
+                for (n = 0; n < i; ++n) a[n] = o[n](t);
+                return a
             }
         }
 
         function xr(t, e) {
             var n = new Date;
             return t = +t, e = +e,
                 function(r) {
@@ -2633,23 +2633,23 @@
             }
         }
 
         function Mr(t, e) {
             e || (e = []);
             var n, r = t ? Math.min(e.length, t.length) : 0,
                 i = e.slice();
-            return function(a) {
-                for (n = 0; n < r; ++n) i[n] = t[n] * (1 - a) + e[n] * a;
+            return function(o) {
+                for (n = 0; n < r; ++n) i[n] = t[n] * (1 - o) + e[n] * o;
                 return i
             }
         }
 
         function kr(t, e) {
             var n, r, i = typeof e;
-            return null == e || "boolean" === i ? Mn(e) : ("number" === i ? Te : "string" === i ? (n = on(e)) ? (e = n, An) : En : e instanceof on ? An : e instanceof Date ? xr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? wr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? br : Te : Mr))(t, e)
+            return null == e || "boolean" === i ? Mn(e) : ("number" === i ? je : "string" === i ? (n = an(e)) ? (e = n, An) : En : e instanceof an ? An : e instanceof Date ? xr : (r = e, !ArrayBuffer.isView(r) || r instanceof DataView ? Array.isArray(e) ? wr : "function" != typeof e.valueOf && "function" != typeof e.toString || isNaN(e) ? br : je : Mr))(t, e)
         }
 
         function Ar(t, e) {
             return t = +t, e = +e,
                 function(n) {
                     return Math.round(t * (1 - n) + e * n)
                 }
@@ -2669,132 +2669,132 @@
                 return (n - t) / e
             } : (n = isNaN(e) ? NaN : .5, function() {
                 return n
             });
             var n
         }
 
-        function Tr(t, e, n) {
+        function jr(t, e, n) {
             var r = t[0],
                 i = t[1],
-                a = e[0],
-                o = e[1];
-            return i < r ? (r = Er(i, r), a = n(o, a)) : (r = Er(r, i), a = n(a, o)),
+                o = e[0],
+                a = e[1];
+            return i < r ? (r = Er(i, r), o = n(a, o)) : (r = Er(r, i), o = n(o, a)),
                 function(t) {
-                    return a(r(t))
+                    return o(r(t))
                 }
         }
 
-        function jr(t, e, n) {
+        function Tr(t, e, n) {
             var r = Math.min(t.length, e.length) - 1,
                 i = new Array(r),
-                a = new Array(r),
-                o = -1;
-            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++o < r;) i[o] = Er(t[o], t[o + 1]), a[o] = n(e[o], e[o + 1]);
+                o = new Array(r),
+                a = -1;
+            for (t[r] < t[0] && (t = t.slice().reverse(), e = e.slice().reverse()); ++a < r;) i[a] = Er(t[a], t[a + 1]), o[a] = n(e[a], e[a + 1]);
             return function(e) {
                 var n = f(t, e, 1, r) - 1;
-                return a[n](i[n](e))
+                return o[n](i[n](e))
             }
         }
         var Pr, Cr = /^(?:(.)?([<>=^]))?([+\-( ])?([$#])?(0)?(\d+)?(,)?(\.\d+)?(~)?([a-z%])?$/i;
 
         function Or(t) {
             if (!(e = Cr.exec(t))) throw new Error("invalid format: " + t);
             var e;
-            return new Vr({
+            return new Ir({
                 fill: e[1],
                 align: e[2],
                 sign: e[3],
                 symbol: e[4],
                 zero: e[5],
                 width: e[6],
                 comma: e[7],
                 precision: e[8] && e[8].slice(1),
                 trim: e[9],
                 type: e[10]
             })
         }
 
-        function Vr(t) {
+        function Ir(t) {
             this.fill = void 0 === t.fill ? " " : t.fill + "", this.align = void 0 === t.align ? ">" : t.align + "", this.sign = void 0 === t.sign ? "-" : t.sign + "", this.symbol = void 0 === t.symbol ? "" : t.symbol + "", this.zero = !!t.zero, this.width = void 0 === t.width ? void 0 : +t.width, this.comma = !!t.comma, this.precision = void 0 === t.precision ? void 0 : +t.precision, this.trim = !!t.trim, this.type = void 0 === t.type ? "" : t.type + ""
         }
 
-        function Dr(t, e) {
+        function Vr(t, e) {
             if ((n = (t = e ? t.toExponential(e - 1) : t.toExponential()).indexOf("e")) < 0) return null;
             var n, r = t.slice(0, n);
             return [r.length > 1 ? r[0] + r.slice(2) : r, +t.slice(n + 1)]
         }
 
-        function qr(t) {
-            return (t = Dr(Math.abs(t))) ? t[1] : NaN
+        function Dr(t) {
+            return (t = Vr(Math.abs(t))) ? t[1] : NaN
         }
 
-        function Ir(t, e) {
-            var n = Dr(t, e);
+        function qr(t, e) {
+            var n = Vr(t, e);
             if (!n) return t + "";
             var r = n[0],
                 i = n[1];
             return i < 0 ? "0." + new Array(-i).join("0") + r : r.length > i + 1 ? r.slice(0, i + 1) + "." + r.slice(i + 1) : r + new Array(i - r.length + 2).join("0")
         }
-        Or.prototype = Vr.prototype, Vr.prototype.toString = function() {
+        Or.prototype = Ir.prototype, Ir.prototype.toString = function() {
             return this.fill + this.align + this.sign + this.symbol + (this.zero ? "0" : "") + (void 0 === this.width ? "" : Math.max(1, 0 | this.width)) + (this.comma ? "," : "") + (void 0 === this.precision ? "" : "." + Math.max(0, 0 | this.precision)) + (this.trim ? "~" : "") + this.type
         };
-        const Hr = {
+        const Lr = {
             "%": (t, e) => (100 * t).toFixed(e),
             b: t => Math.round(t).toString(2),
             c: t => t + "",
             d: function(t) {
                 return Math.abs(t = Math.round(t)) >= 1e21 ? t.toLocaleString("en").replace(/,/g, "") : t.toString(10)
             },
             e: (t, e) => t.toExponential(e),
             f: (t, e) => t.toFixed(e),
             g: (t, e) => t.toPrecision(e),
             o: t => Math.round(t).toString(8),
-            p: (t, e) => Ir(100 * t, e),
-            r: Ir,
+            p: (t, e) => qr(100 * t, e),
+            r: qr,
             s: function(t, e) {
-                var n = Dr(t, e);
+                var n = Vr(t, e);
                 if (!n) return t + "";
                 var r = n[0],
                     i = n[1],
-                    a = i - (Pr = 3 * Math.max(-8, Math.min(8, Math.floor(i / 3)))) + 1,
-                    o = r.length;
-                return a === o ? r : a > o ? r + new Array(a - o + 1).join("0") : a > 0 ? r.slice(0, a) + "." + r.slice(a) : "0." + new Array(1 - a).join("0") + Dr(t, Math.max(0, e + a - 1))[0]
+                    o = i - (Pr = 3 * Math.max(-8, Math.min(8, Math.floor(i / 3)))) + 1,
+                    a = r.length;
+                return o === a ? r : o > a ? r + new Array(o - a + 1).join("0") : o > 0 ? r.slice(0, o) + "." + r.slice(o) : "0." + new Array(1 - o).join("0") + Vr(t, Math.max(0, e + o - 1))[0]
             },
             X: t => Math.round(t).toString(16).toUpperCase(),
             x: t => Math.round(t).toString(16)
         };
 
-        function Lr(t) {
+        function Hr(t) {
             return t
         }
-        var Xr, Rr, zr, Yr = Array.prototype.map,
+        var Xr, zr, Rr, Yr = Array.prototype.map,
             Br = ["y", "z", "a", "f", "p", "n", "µ", "m", "", "k", "M", "G", "T", "P", "E", "Z", "Y"];
 
         function Wr() {
             var t = function() {
-                var t, e, n, r, i, a, o = $r,
+                var t, e, n, r, i, o, a = $r,
                     s = $r,
                     u = kr,
                     l = Sr;
 
                 function c() {
-                    var t, e, n, u = Math.min(o.length, s.length);
-                    return l !== Sr && (t = o[0], e = o[u - 1], t > e && (n = t, t = e, e = n), l = function(n) {
+                    var t, e, n, u = Math.min(a.length, s.length);
+                    return l !== Sr && (t = a[0], e = a[u - 1], t > e && (n = t, t = e, e = n), l = function(n) {
                         return Math.max(t, Math.min(e, n))
-                    }), r = u > 2 ? jr : Tr, i = a = null, h
+                    }), r = u > 2 ? Tr : jr, i = o = null, h
                 }
 
                 function h(e) {
-                    return null == e || isNaN(e = +e) ? n : (i || (i = r(o.map(t), s, u)))(t(l(e)))
+                    return null == e || isNaN(e = +e) ? n : (i || (i = r(a.map(t), s, u)))(t(l(e)))
                 }
                 return h.invert = function(n) {
-                        return l(e((a || (a = r(s, o.map(t), Te)))(n)))
+                        return l(e((o || (o = r(s, a.map(t), je)))(n)))
                     }, h.domain = function(t) {
-                        return arguments.length ? (o = Array.from(t, Nr), c()) : o.slice()
+                        return arguments.length ? (a = Array.from(t, Nr), c()) : a.slice()
                     }, h.range = function(t) {
                         return arguments.length ? (s = Array.from(t), c()) : s.slice()
                     }, h.rangeRound = function(t) {
                         return s = Array.from(t), u = Ar, c()
                     }, h.clamp = function(t) {
                         return arguments.length ? (l = !!t || Sr, c()) : l !== Sr
                     }, h.interpolate = function(t) {
@@ -2814,73 +2814,73 @@
                     var e = t.domain;
                     return t.ticks = function(t) {
                         var n = e();
                         return y(n[0], n[n.length - 1], null == t ? 10 : t)
                     }, t.tickFormat = function(t, n) {
                         var r = e();
                         return function(t, e, n, r) {
-                            var i, a = function(t, e, n) {
+                            var i, o = function(t, e, n) {
                                 n = +n;
                                 const r = (e = +e) < (t = +t),
                                     i = r ? w(e, t, n) : w(t, e, n);
                                 return (r ? -1 : 1) * (i < 0 ? 1 / -i : i)
                             }(t, e, n);
                             switch ((r = Or(null == r ? ",f" : r)).type) {
                                 case "s":
-                                    var o = Math.max(Math.abs(t), Math.abs(e));
+                                    var a = Math.max(Math.abs(t), Math.abs(e));
                                     return null != r.precision || isNaN(i = function(t, e) {
-                                        return Math.max(0, 3 * Math.max(-8, Math.min(8, Math.floor(qr(e) / 3))) - qr(Math.abs(t)))
-                                    }(a, o)) || (r.precision = i), zr(r, o);
+                                        return Math.max(0, 3 * Math.max(-8, Math.min(8, Math.floor(Dr(e) / 3))) - Dr(Math.abs(t)))
+                                    }(o, a)) || (r.precision = i), Rr(r, a);
                                 case "":
                                 case "e":
                                 case "g":
                                 case "p":
                                 case "r":
                                     null != r.precision || isNaN(i = function(t, e) {
-                                        return t = Math.abs(t), e = Math.abs(e) - t, Math.max(0, qr(e) - qr(t)) + 1
-                                    }(a, Math.max(Math.abs(t), Math.abs(e)))) || (r.precision = i - ("e" === r.type));
+                                        return t = Math.abs(t), e = Math.abs(e) - t, Math.max(0, Dr(e) - Dr(t)) + 1
+                                    }(o, Math.max(Math.abs(t), Math.abs(e)))) || (r.precision = i - ("e" === r.type));
                                     break;
                                 case "f":
                                 case "%":
                                     null != r.precision || isNaN(i = function(t) {
-                                        return Math.max(0, -qr(Math.abs(t)))
-                                    }(a)) || (r.precision = i - 2 * ("%" === r.type))
+                                        return Math.max(0, -Dr(Math.abs(t)))
+                                    }(o)) || (r.precision = i - 2 * ("%" === r.type))
                             }
-                            return Rr(r)
+                            return zr(r)
                         }(r[0], r[r.length - 1], null == t ? 10 : t, n)
                     }, t.nice = function(n) {
                         null == n && (n = 10);
-                        var r, i, a = e(),
-                            o = 0,
-                            s = a.length - 1,
-                            u = a[o],
-                            l = a[s],
+                        var r, i, o = e(),
+                            a = 0,
+                            s = o.length - 1,
+                            u = o[a],
+                            l = o[s],
                             c = 10;
-                        for (l < u && (i = u, u = l, l = i, i = o, o = s, s = i); c-- > 0;) {
-                            if ((i = w(u, l, n)) === r) return a[o] = u, a[s] = l, e(a);
+                        for (l < u && (i = u, u = l, l = i, i = a, a = s, s = i); c-- > 0;) {
+                            if ((i = w(u, l, n)) === r) return o[a] = u, o[s] = l, e(o);
                             if (i > 0) u = Math.floor(u / i) * i, l = Math.ceil(l / i) * i;
                             else {
                                 if (!(i < 0)) break;
                                 u = Math.ceil(u * i) / i, l = Math.floor(l * i) / i
                             }
                             r = i
                         }
                         return t
                     }, t
                 }(t)
         }
         Xr = function(t) {
-            var e, n, r = void 0 === t.grouping || void 0 === t.thousands ? Lr : (e = Yr.call(t.grouping, Number), n = t.thousands + "", function(t, r) {
-                    for (var i = t.length, a = [], o = 0, s = e[0], u = 0; i > 0 && s > 0 && (u + s + 1 > r && (s = Math.max(1, r - u)), a.push(t.substring(i -= s, i + s)), !((u += s + 1) > r));) s = e[o = (o + 1) % e.length];
-                    return a.reverse().join(n)
+            var e, n, r = void 0 === t.grouping || void 0 === t.thousands ? Hr : (e = Yr.call(t.grouping, Number), n = t.thousands + "", function(t, r) {
+                    for (var i = t.length, o = [], a = 0, s = e[0], u = 0; i > 0 && s > 0 && (u + s + 1 > r && (s = Math.max(1, r - u)), o.push(t.substring(i -= s, i + s)), !((u += s + 1) > r));) s = e[a = (a + 1) % e.length];
+                    return o.reverse().join(n)
                 }),
                 i = void 0 === t.currency ? "" : t.currency[0] + "",
-                a = void 0 === t.currency ? "" : t.currency[1] + "",
-                o = void 0 === t.decimal ? "." : t.decimal + "",
-                s = void 0 === t.numerals ? Lr : function(t) {
+                o = void 0 === t.currency ? "" : t.currency[1] + "",
+                a = void 0 === t.decimal ? "." : t.decimal + "",
+                s = void 0 === t.numerals ? Hr : function(t) {
                     return function(e) {
                         return e.replace(/[0-9]/g, (function(e) {
                             return t[+e]
                         }))
                     }
                 }(Yr.call(t.numerals, String)),
                 u = void 0 === t.percent ? "%" : t.percent + "",
@@ -2894,22 +2894,22 @@
                     f = t.symbol,
                     d = t.zero,
                     p = t.width,
                     m = t.comma,
                     _ = t.precision,
                     g = t.trim,
                     v = t.type;
-                "n" === v ? (m = !0, v = "g") : Hr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (d || "0" === e && "=" === n) && (d = !0, e = "0", n = "=");
+                "n" === v ? (m = !0, v = "g") : Lr[v] || (void 0 === _ && (_ = 12), g = !0, v = "g"), (d || "0" === e && "=" === n) && (d = !0, e = "0", n = "=");
                 var y = "$" === f ? i : "#" === f && /[boxX]/.test(v) ? "0" + v.toLowerCase() : "",
-                    w = "$" === f ? a : /[%p]/.test(v) ? u : "",
-                    x = Hr[v],
+                    w = "$" === f ? o : /[%p]/.test(v) ? u : "",
+                    x = Lr[v],
                     b = /[defgprs%]/.test(v);
 
                 function M(t) {
-                    var i, a, u, f = y,
+                    var i, o, u, f = y,
                         M = w;
                     if ("c" === v) M = x(t) + M, t = "";
                     else {
                         var k = (t = +t) < 0 || 1 / t < 0;
                         if (t = isNaN(t) ? c : x(Math.abs(t), _), g && (t = function(t) {
                                 t: for (var e, n = t.length, r = 1, i = -1; r < n; ++r) switch (t[r]) {
                                     case ".":
@@ -2920,17 +2920,17 @@
                                         break;
                                     default:
                                         if (!+t[r]) break t;
                                         i > 0 && (i = 0)
                                 }
                                 return i > 0 ? t.slice(0, i) + t.slice(e + 1) : t
                             }(t)), k && 0 == +t && "+" !== h && (k = !1), f = (k ? "(" === h ? h : l : "-" === h || "(" === h ? "" : h) + f, M = ("s" === v ? Br[8 + Pr / 3] : "") + M + (k && "(" === h ? ")" : ""), b)
-                            for (i = -1, a = t.length; ++i < a;)
+                            for (i = -1, o = t.length; ++i < o;)
                                 if (48 > (u = t.charCodeAt(i)) || u > 57) {
-                                    M = (46 === u ? o + t.slice(i + 1) : t.slice(i)) + M, t = t.slice(0, i);
+                                    M = (46 === u ? a + t.slice(i + 1) : t.slice(i)) + M, t = t.slice(0, i);
                                     break
                                 }
                     }
                     m && !d && (t = r(t, 1 / 0));
                     var A = f.length + t.length + M.length,
                         N = A < p ? new Array(p - A + 1).join(e) : "";
                     switch (m && d && (t = r(N + t, N.length ? p - M.length : 1 / 0), N = ""), n) {
@@ -2952,27 +2952,27 @@
                     return t + ""
                 }, M
             }
             return {
                 format: h,
                 formatPrefix: function(t, e) {
                     var n = h(((t = Or(t)).type = "f", t)),
-                        r = 3 * Math.max(-8, Math.min(8, Math.floor(qr(e) / 3))),
+                        r = 3 * Math.max(-8, Math.min(8, Math.floor(Dr(e) / 3))),
                         i = Math.pow(10, -r),
-                        a = Br[8 + r / 3];
+                        o = Br[8 + r / 3];
                     return function(t) {
-                        return n(i * t) + a
+                        return n(i * t) + o
                     }
                 }
             }
         }({
             thousands: ",",
             grouping: [3],
             currency: ["$", ""]
-        }), Rr = Xr.format, zr = Xr.formatPrefix;
+        }), zr = Xr.format, Rr = Xr.formatPrefix;
         const Fr = function(t) {
             for (var e = new Array(10), n = 0; n < 10;) e[n] = "#" + t.slice(6 * n, 6 * ++n);
             return e
         }("1f77b4ff7f0e2ca02cd627289467bd8c564be377c27f7f7fbcbd2217becf");
 
         function Ur(t) {
             return function() {
@@ -3042,50 +3042,50 @@
             }
             lineTo(t, e) {
                 this._append`L${this._x1=+t},${this._y1=+e}`
             }
             quadraticCurveTo(t, e, n, r) {
                 this._append`Q${+t},${+e},${this._x1=+n},${this._y1=+r}`
             }
-            bezierCurveTo(t, e, n, r, i, a) {
-                this._append`C${+t},${+e},${+n},${+r},${this._x1=+i},${this._y1=+a}`
+            bezierCurveTo(t, e, n, r, i, o) {
+                this._append`C${+t},${+e},${+n},${+r},${this._x1=+i},${this._y1=+o}`
             }
             arcTo(t, e, n, r, i) {
                 if (t = +t, e = +e, n = +n, r = +r, (i = +i) < 0) throw new Error(`negative radius: ${i}`);
-                let a = this._x1,
-                    o = this._y1,
+                let o = this._x1,
+                    a = this._y1,
                     s = n - t,
                     u = r - e,
-                    l = a - t,
-                    c = o - e,
+                    l = o - t,
+                    c = a - e,
                     h = l * l + c * c;
                 if (null === this._x1) this._append`M${this._x1=t},${this._y1=e}`;
                 else if (h > Qr)
                     if (Math.abs(c * s - u * l) > Qr && i) {
-                        let f = n - a,
-                            d = r - o,
+                        let f = n - o,
+                            d = r - a,
                             p = s * s + u * u,
                             m = f * f + d * d,
                             _ = Math.sqrt(p),
                             g = Math.sqrt(h),
                             v = i * Math.tan((Kr - Math.acos((p + h - m) / (2 * _ * g))) / 2),
                             y = v / g,
                             w = v / _;
                         Math.abs(y - 1) > Qr && this._append`L${t+y*l},${e+y*c}`, this._append`A${i},${i},0,0,${+(c*f>l*d)},${this._x1=t+w*s},${this._y1=e+w*u}`
                     } else this._append`L${this._x1=t},${this._y1=e}`
             }
-            arc(t, e, n, r, i, a) {
-                if (t = +t, e = +e, a = !!a, (n = +n) < 0) throw new Error(`negative radius: ${n}`);
-                let o = n * Math.cos(r),
+            arc(t, e, n, r, i, o) {
+                if (t = +t, e = +e, o = !!o, (n = +n) < 0) throw new Error(`negative radius: ${n}`);
+                let a = n * Math.cos(r),
                     s = n * Math.sin(r),
-                    u = t + o,
+                    u = t + a,
                     l = e + s,
-                    c = 1 ^ a,
-                    h = a ? r - i : i - r;
-                null === this._x1 ? this._append`M${u},${l}` : (Math.abs(this._x1 - u) > Qr || Math.abs(this._y1 - l) > Qr) && this._append`L${u},${l}`, n && (h < 0 && (h = h % Zr + Zr), h > ti ? this._append`A${n},${n},0,1,${c},${t-o},${e-s}A${n},${n},0,1,${c},${this._x1=u},${this._y1=l}` : h > Qr && this._append`A${n},${n},0,${+(h>=Kr)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
+                    c = 1 ^ o,
+                    h = o ? r - i : i - r;
+                null === this._x1 ? this._append`M${u},${l}` : (Math.abs(this._x1 - u) > Qr || Math.abs(this._y1 - l) > Qr) && this._append`L${u},${l}`, n && (h < 0 && (h = h % Zr + Zr), h > ti ? this._append`A${n},${n},0,1,${c},${t-a},${e-s}A${n},${n},0,1,${c},${this._x1=u},${this._y1=l}` : h > Qr && this._append`A${n},${n},0,${+(h>=Kr)},${c},${this._x1=t+n*Math.cos(i)},${this._y1=e+n*Math.sin(i)}`)
             }
             rect(t, e, n, r) {
                 this._append`M${this._x0=this._x1=+t},${this._y0=this._y1=+e}h${n=+n}v${+r}h${-n}Z`
             }
             toString() {
                 return this._
             }
@@ -3095,20 +3095,20 @@
             return t[0]
         }
 
         function ii(t) {
             return t[1]
         }
 
-        function ai(t, e) {
+        function oi(t, e) {
             var n = Ur(!0),
                 r = null,
                 i = Jr,
-                a = null,
-                o = function(t) {
+                o = null,
+                a = function(t) {
                     let e = 3;
                     return t.digits = function(n) {
                         if (!arguments.length) return e;
                         if (null == n) e = null;
                         else {
                             const t = Math.floor(n);
                             if (!(t >= 0)) throw new RangeError(`invalid digits: ${n}`);
@@ -3119,31 +3119,31 @@
                 }(s);
 
             function s(s) {
                 var u, l, c, h = (s = function(t) {
                         return "object" == typeof t && "length" in t ? t : Array.from(t)
                     }(s)).length,
                     f = !1;
-                for (null == r && (a = i(c = o())), u = 0; u <= h; ++u) !(u < h && n(l = s[u], u, s)) === f && ((f = !f) ? a.lineStart() : a.lineEnd()), f && a.point(+t(l, u, s), +e(l, u, s));
-                if (c) return a = null, c + "" || null
+                for (null == r && (o = i(c = a())), u = 0; u <= h; ++u) !(u < h && n(l = s[u], u, s)) === f && ((f = !f) ? o.lineStart() : o.lineEnd()), f && o.point(+t(l, u, s), +e(l, u, s));
+                if (c) return o = null, c + "" || null
             }
             return t = "function" == typeof t ? t : void 0 === t ? ri : Ur(t), e = "function" == typeof e ? e : void 0 === e ? ii : Ur(e), s.x = function(e) {
                 return arguments.length ? (t = "function" == typeof e ? e : Ur(+e), s) : t
             }, s.y = function(t) {
                 return arguments.length ? (e = "function" == typeof t ? t : Ur(+t), s) : e
             }, s.defined = function(t) {
                 return arguments.length ? (n = "function" == typeof t ? t : Ur(!!t), s) : n
             }, s.curve = function(t) {
-                return arguments.length ? (i = t, null != r && (a = i(r)), s) : i
+                return arguments.length ? (i = t, null != r && (o = i(r)), s) : i
             }, s.context = function(t) {
-                return arguments.length ? (null == t ? r = a = null : a = i(r = t), s) : r
+                return arguments.length ? (null == t ? r = o = null : o = i(r = t), s) : r
             }, s
         }
 
-        function oi(t, e, n) {
+        function ai(t, e, n) {
             t._context.bezierCurveTo(t._x1 + t._k * (t._x2 - t._x0), t._y1 + t._k * (t._y2 - t._y0), t._x2 + t._k * (t._x1 - e), t._y2 + t._k * (t._y1 - n), t._x2, t._y2)
         }
 
         function si(t, e) {
             this._context = t, this._k = (1 - e) / 6
         }
 
@@ -3162,29 +3162,29 @@
                 },
                 lineEnd: function() {
                     switch (this._point) {
                         case 2:
                             this._context.lineTo(this._x2, this._y2);
                             break;
                         case 3:
-                            oi(this, this._x1, this._y1)
+                            ai(this, this._x1, this._y1)
                     }(this._line || 0 !== this._line && 1 === this._point) && this._context.closePath(), this._line = 1 - this._line
                 },
                 point: function(t, e) {
                     switch (t = +t, e = +e, this._point) {
                         case 0:
                             this._point = 1, this._line ? this._context.lineTo(t, e) : this._context.moveTo(t, e);
                             break;
                         case 1:
                             this._point = 2, this._x1 = t, this._y1 = e;
                             break;
                         case 2:
                             this._point = 3;
                         default:
-                            oi(this, t, e)
+                            ai(this, t, e)
                     }
                     this._x0 = this._x1, this._x1 = this._x2, this._x2 = t, this._y0 = this._y1, this._y1 = this._y2, this._y2 = e
                 }
             },
             function t(e) {
                 function n(t) {
                     return new si(t, e)
@@ -3226,27 +3226,27 @@
                             break;
                         case 2:
                             this._point = 3;
                         default:
                             ! function(t, e, n) {
                                 var r = t._x1,
                                     i = t._y1,
-                                    a = t._x2,
-                                    o = t._y2;
+                                    o = t._x2,
+                                    a = t._y2;
                                 if (t._l01_a > 1e-12) {
                                     var s = 2 * t._l01_2a + 3 * t._l01_a * t._l12_a + t._l12_2a,
                                         u = 3 * t._l01_a * (t._l01_a + t._l12_a);
                                     r = (r * s - t._x0 * t._l12_2a + t._x2 * t._l01_2a) / u, i = (i * s - t._y0 * t._l12_2a + t._y2 * t._l01_2a) / u
                                 }
                                 if (t._l23_a > 1e-12) {
                                     var l = 2 * t._l23_2a + 3 * t._l23_a * t._l12_a + t._l12_2a,
                                         c = 3 * t._l23_a * (t._l23_a + t._l12_a);
-                                    a = (a * l + t._x1 * t._l23_2a - e * t._l12_2a) / c, o = (o * l + t._y1 * t._l23_2a - n * t._l12_2a) / c
+                                    o = (o * l + t._x1 * t._l23_2a - e * t._l12_2a) / c, a = (a * l + t._y1 * t._l23_2a - n * t._l12_2a) / c
                                 }
-                                t._context.bezierCurveTo(r, i, a, o, t._x2, t._y2)
+                                t._context.bezierCurveTo(r, i, o, a, t._x2, t._y2)
                             }(this, t, e)
                     }
                     this._l01_a = this._l12_a, this._l12_a = this._l23_a, this._l01_2a = this._l12_2a, this._l12_2a = this._l23_2a, this._x0 = this._x1, this._x1 = this._x2, this._x2 = t, this._y0 = this._y1, this._y1 = this._y2, this._y2 = e
                 }
             };
         const li = function t(e) {
             function n(t) {
@@ -3257,113 +3257,113 @@
             }, n
         }(.5);
 
         function ci(t, e, n) {
             this.k = t, this.x = e, this.y = n
         }
 
-        function hi(t, e, n, r, i, a, o, s, u, l) {
+        function hi(t, e, n, r, i, o, a, s, u, l) {
             let c = [];
-            const h = ai(),
+            const h = oi(),
                 f = er(t).selectAll(".dot"),
                 d = function() {
                     var t, e, n, r, i = lr,
-                        a = cr,
-                        o = hr,
+                        o = cr,
+                        a = hr,
                         s = fr,
                         u = {},
                         l = ne("start", "drag", "end"),
                         c = 0,
                         h = 0;
 
                     function f(t) {
                         t.on("mousedown.drag", d).filter(s).on("touchstart.drag", _).on("touchmove.drag", g, rr).on("touchend.drag touchcancel.drag", v).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
                     }
 
-                    function d(o, s) {
-                        if (!r && i.call(this, o, s)) {
-                            var u = y(this, a.call(this, o, s), o, s, "mouse");
-                            u && (er(o.view).on("mousemove.drag", p, ir).on("mouseup.drag", m, ir), function(t) {
+                    function d(a, s) {
+                        if (!r && i.call(this, a, s)) {
+                            var u = y(this, o.call(this, a, s), a, s, "mouse");
+                            u && (er(a.view).on("mousemove.drag", p, ir).on("mouseup.drag", m, ir), function(t) {
                                 var e = t.document.documentElement,
-                                    n = er(t).on("dragstart.drag", or, ir);
-                                "onselectstart" in e ? n.on("selectstart.drag", or, ir) : (e.__noselect = e.style.MozUserSelect, e.style.MozUserSelect = "none")
-                            }(o.view), ar(o), n = !1, t = o.clientX, e = o.clientY, u("start", o))
+                                    n = er(t).on("dragstart.drag", ar, ir);
+                                "onselectstart" in e ? n.on("selectstart.drag", ar, ir) : (e.__noselect = e.style.MozUserSelect, e.style.MozUserSelect = "none")
+                            }(a.view), or(a), n = !1, t = a.clientX, e = a.clientY, u("start", a))
                         }
                     }
 
                     function p(r) {
-                        if (or(r), !n) {
+                        if (ar(r), !n) {
                             var i = r.clientX - t,
-                                a = r.clientY - e;
-                            n = i * i + a * a > h
+                                o = r.clientY - e;
+                            n = i * i + o * o > h
                         }
                         u.mouse("drag", r)
                     }
 
                     function m(t) {
                         er(t.view).on("mousemove.drag mouseup.drag", null),
                             function(t, e) {
                                 var n = t.document.documentElement,
                                     r = er(t).on("dragstart.drag", null);
-                                e && (r.on("click.drag", or, ir), setTimeout((function() {
+                                e && (r.on("click.drag", ar, ir), setTimeout((function() {
                                     r.on("click.drag", null)
                                 }), 0)), "onselectstart" in n ? r.on("selectstart.drag", null) : (n.style.MozUserSelect = n.__noselect, delete n.__noselect)
-                            }(t.view, n), or(t), u.mouse("end", t)
+                            }(t.view, n), ar(t), u.mouse("end", t)
                     }
 
                     function _(t, e) {
                         if (i.call(this, t, e)) {
-                            var n, r, o = t.changedTouches,
-                                s = a.call(this, t, e),
-                                u = o.length;
-                            for (n = 0; n < u; ++n)(r = y(this, s, t, e, o[n].identifier, o[n])) && (ar(t), r("start", t, o[n]))
+                            var n, r, a = t.changedTouches,
+                                s = o.call(this, t, e),
+                                u = a.length;
+                            for (n = 0; n < u; ++n)(r = y(this, s, t, e, a[n].identifier, a[n])) && (or(t), r("start", t, a[n]))
                         }
                     }
 
                     function g(t) {
                         var e, n, r = t.changedTouches,
                             i = r.length;
-                        for (e = 0; e < i; ++e)(n = u[r[e].identifier]) && (or(t), n("drag", t, r[e]))
+                        for (e = 0; e < i; ++e)(n = u[r[e].identifier]) && (ar(t), n("drag", t, r[e]))
                     }
 
                     function v(t) {
                         var e, n, i = t.changedTouches,
-                            a = i.length;
+                            o = i.length;
                         for (r && clearTimeout(r), r = setTimeout((function() {
                                 r = null
-                            }), 500), e = 0; e < a; ++e)(n = u[i[e].identifier]) && (ar(t), n("end", t, i[e]))
+                            }), 500), e = 0; e < o; ++e)(n = u[i[e].identifier]) && (or(t), n("end", t, i[e]))
                     }
 
-                    function y(t, e, n, r, i, a) {
+                    function y(t, e, n, r, i, o) {
                         var s, h, d, p = l.copy(),
-                            m = nr(a || n, e);
-                        if (null != (d = o.call(t, new ur("beforestart", {
+                            m = nr(o || n, e);
+                        if (null != (d = a.call(t, new ur("beforestart", {
                                 sourceEvent: n,
                                 target: f,
                                 identifier: i,
                                 active: c,
                                 x: m[0],
                                 y: m[1],
                                 dx: 0,
                                 dy: 0,
                                 dispatch: p
                             }), r))) return s = d.x - m[0] || 0, h = d.y - m[1] || 0,
-                            function n(a, o, l) {
+                            function n(o, a, l) {
                                 var _, g = m;
-                                switch (a) {
+                                switch (o) {
                                     case "start":
                                         u[i] = n, _ = c++;
                                         break;
                                     case "end":
                                         delete u[i], --c;
                                     case "drag":
-                                        m = nr(l || o, e), _ = c
+                                        m = nr(l || a, e), _ = c
                                 }
-                                p.call(a, t, new ur(a, {
-                                    sourceEvent: o,
+                                p.call(o, t, new ur(o, {
+                                    sourceEvent: a,
                                     subject: d,
                                     target: f,
                                     identifier: i,
                                     active: _,
                                     x: m[0] + s,
                                     y: m[1] + h,
                                     dx: m[0] - g[0],
@@ -3371,17 +3371,17 @@
                                     dispatch: p
                                 }), r)
                             }
                     }
                     return f.filter = function(t) {
                         return arguments.length ? (i = "function" == typeof t ? t : sr(!!t), f) : i
                     }, f.container = function(t) {
-                        return arguments.length ? (a = "function" == typeof t ? t : sr(t), f) : a
-                    }, f.subject = function(t) {
                         return arguments.length ? (o = "function" == typeof t ? t : sr(t), f) : o
+                    }, f.subject = function(t) {
+                        return arguments.length ? (a = "function" == typeof t ? t : sr(t), f) : a
                     }, f.touchable = function(t) {
                         return arguments.length ? (s = "function" == typeof t ? t : sr(!!t), f) : s
                     }, f.on = function() {
                         var t = l.on.apply(l, arguments);
                         return t === l ? f : t
                     }, f.clickDistance = function(t) {
                         return arguments.length ? (h = (t = +t) * t, f) : Math.sqrt(h)
@@ -3392,34 +3392,34 @@
                     let e = t.sourceEvent.offsetX,
                         n = t.sourceEvent.offsetY;
                     c.push([e, n]), er("#lasso" + l).style("stroke", "blue").style("stroke-width", 2).style("fill", "#00008854").attr("d", h(c))
                 })).on("end", (function() {
                     let t = [];
                     f.each(((s, u) => {
                         (function(t, e) {
-                            for (var n = t[0], r = t[1], i = !1, a = 0, o = e.length - 1; a < e.length; o = a++) {
-                                var s = e[a][0],
-                                    u = e[a][1],
-                                    l = e[o][0],
-                                    c = e[o][1];
+                            for (var n = t[0], r = t[1], i = !1, o = 0, a = e.length - 1; o < e.length; a = o++) {
+                                var s = e[o][0],
+                                    u = e[o][1],
+                                    l = e[a][0],
+                                    c = e[a][1];
                                 u > r != c > r && n < (l - s) * (r - u) / (c - u) + s && (i = !i)
                             }
                             return i
-                        })([e(s[r]) + a, n(s[i]) + o], c) && (er("#dot-" + l + s.id).style("fill", "red").attr("r", 6), t.push(s))
+                        })([e(s[r]) + o, n(s[i]) + a], c) && (er("#dot-" + l + s.id).style("fill", "red").attr("r", 6), t.push(s))
                     })), er("#lasso" + l).remove(), u(t)
                 }));
             er(t).call(d)
         }
 
         function fi(t) {
-            const e = t.reduce(((t, e) => t + e), 0) / t.length;
-            let n = 1.96 * function(t, e) {
-                let n = 0;
-                return t.forEach((t => n += (t - e) ** 2)), n = Math.sqrt(n) / t.length, n
-            }(t, e);
+            const e = t.reduce(((t, e) => t + e), 0) / t.length,
+                n = 1.96 * function(t, e) {
+                    let n = 0;
+                    return t.forEach((t => n += (t - e) ** 2)), n = Math.sqrt(n) / t.length, n
+                }(t, e);
             return [e - n, e + n]
         }
         ci.prototype = {
             constructor: ci,
             scale: function(t) {
                 return 1 === t ? this : new ci(this.k * t, this.x, this.y)
             },
@@ -3465,339 +3465,354 @@
             xi = i(540),
             bi = i.n(xi),
             Mi = i(113),
             ki = i.n(Mi),
             Ai = i(930),
             Ni = {};
         Ni.styleTagTransform = ki(), Ni.setAttributes = wi(), Ni.insert = vi().bind(null, "head"), Ni.domAPI = _i(), Ni.insertStyleElement = bi(), pi()(Ai.A, Ni), Ai.A && Ai.A.locals && Ai.A.locals;
-        const $i = i(330);
-        class Si extends t.DOMWidgetModel {
+        const $i = i(330),
+            Si = 400,
+            Ei = {
+                top: 20,
+                right: 20,
+                bottom: 30,
+                left: 40
+            };
+
+        function ji(t) {
+            t.timeout && clearTimeout(t.timeout), t.timeout = setTimeout((() => {
+                t.plot()
+            }), 100)
+        }
+        class Ti extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Si.model_name,
-                    _view_name: Si.view_name,
-                    _model_module: Si.model_module,
-                    _view_module: Si.view_module,
-                    _model_module_version: Si.model_module_version,
-                    _view_module_version: Si.view_module_version,
+                    _model_name: Ti.model_name,
+                    _view_name: Ti.view_name,
+                    _model_module: Ti.model_module,
+                    _view_module: Ti.view_module,
+                    _model_module_version: Ti.model_module_version,
+                    _view_module_version: Ti.view_module_version,
                     linearData_x: [],
                     linearData_y: [],
                     histogramData: [],
-                    element: String,
+                    elementId: String,
                     clickedValue: String
                 }
             }
             static model_name = "LinearHistPlotModel";
             static model_module = $i.name;
             static model_module_version = $i.version;
             static view_name = "LinearHistPlotView";
             static view_module = $i.name;
             static view_module_version = $i.version
         }
-        class Ei extends t.DOMWidgetView {
+        class Pi extends t.DOMWidgetView {
+            timeout;
             render() {
-                this.value_changed(), this.model.on("change:linearData_x", this.value_changed, this)
+                ji(this), this.model.on("change:linearData_x", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
             }
-            value_changed() {
-                let t = this;
-                var n = this.model.get("linearData_x"),
-                    r = this.model.get("linearData_y"),
-                    i = this.model.get("histogramData"),
-                    a = this.model.get("element");
-                setTimeout((() => {
-                    ! function(t, n, r, i, a, o) {
-                        var s = 375,
-                            u = 720;
-                        i ? (u = (i = document.getElementById(i)).clientWidth, s = i.clientHeight) : i = o.el, er(i).selectAll("*").remove();
-                        const l = u - 40 - 20,
-                            c = s - 20 - 30,
-                            h = s / 5 - 20 - 30,
-                            f = Math.min(k(t), k(r)),
-                            d = Math.max(M(t), M(r)),
-                            p = Wr().range([0, l]),
-                            m = Wr().range([c, 0]),
-                            _ = Wr().range([h, 0]),
-                            g = q(p),
-                            v = I(m),
-                            y = b().thresholds(20).value((t => Math.round(10 * t) / 10))(r),
-                            w = er(i).append("svg").attr("width", l + 40 + 20).attr("height", c + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                        p.domain([f, d]), m.domain(e(n)), _.domain([0, M(y, (t => t.length))]);
-                        const x = w.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                        var A = w.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
-                        w.append("g").attr("transform", "translate(0," + c + ")").call(g).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), w.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", ai().x((t => p((t.x1 + t.x0) / 2))).y((t => _(t.length) + c - h)).curve(li));
-                        var N = t.map(((t, e) => [t, n[e]])).map((([t, e]) => ({
-                            x: t,
-                            y: e
-                        })));
-                        w.append("path").datum(N).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", ai().x((t => p(t.x))).y((t => m(t.y)))), w.selectAll("myCircles").data(N).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => p(t.x))).attr("cy", (t => m(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
-                            x.style("opacity", 1), A.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), A.html("x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
-                        })).on("mouseout", (function() {
-                            x.style("opacity", 0), A.style("opacity", 0)
-                        })).on("click", (function(t, e) {
-                            const n = "x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10;
-                            void 0 !== a && a(n, o)
-                        }))
-                    }(n, r, i, a, this.setValue, t)
-                }), 50)
+            plot() {
+                const t = this.model.get("linearData_x"),
+                    n = this.model.get("linearData_y"),
+                    r = this.model.get("histogramData"),
+                    i = this.model.get("elementId");
+                let o = Si,
+                    a = this.el;
+                i && (a = document.getElementById(i), o = a.clientHeight);
+                let s = a.clientWidth;
+                const u = Ei;
+                ! function(t, n, r, i, o, a, s, u) {
+                    const l = a - u.left - u.right,
+                        c = s - u.top - u.bottom,
+                        h = c / 4;
+                    er(i).selectAll("*").remove();
+                    const f = Math.min(k(t), k(r)),
+                        d = Math.max(M(t), M(r)),
+                        p = Wr().range([0, l]),
+                        m = Wr().range([c, 0]),
+                        _ = Wr().range([h, 0]),
+                        g = D(p),
+                        v = q(m),
+                        y = b().thresholds(20).value((t => Math.round(10 * t) / 10))(r),
+                        w = er(i).append("svg").attr("width", a).attr("height", s).append("g").attr("transform", "translate(" + u.left + "," + u.top + ")");
+                    p.domain([f, d]), m.domain(e(n)), _.domain([0, M(y, (t => t.length))]);
+                    const x = w.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                        A = w.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle");
+                    w.append("g").attr("transform", "translate(0," + c + ")").call(g).append("text").attr("x", l).attr("y", -6).style("text-anchor", "end"), w.append("g").call(v).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), w.append("path").datum(y).attr("fill", "paleturquoise").attr("stroke", "steelblue").attr("stroke-width", 1).attr("d", oi().x((t => p((t.x1 + t.x0) / 2))).y((t => _(t.length) + c - h)).curve(li));
+                    const N = t.map(((t, e) => [t, n[e]])).map((([t, e]) => ({
+                        x: t,
+                        y: e
+                    })));
+                    w.append("path").datum(N).attr("fill", "none").attr("stroke", "steelblue").attr("stroke-width", 1.5).attr("d", oi().x((t => p(t.x))).y((t => m(t.y)))), w.selectAll("myCircles").data(N).enter().append("circle").attr("fill", "red").attr("stroke", "none").attr("cx", (t => p(t.x))).attr("cy", (t => m(t.y))).attr("r", 3).on("mouseover", (function(t, e) {
+                        x.style("opacity", 1), A.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), A.html("x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                    })).on("mouseout", (function() {
+                        x.style("opacity", 0), A.style("opacity", 0)
+                    })).on("click", (function(t, e) {
+                        const n = "x:" + Math.round(10 * e.x) / 10 + "  -  y:" + Math.round(10 * e.y) / 10;
+                        void 0 !== o && o(n)
+                    }))
+                }(t, n, r, a, this.setValue.bind(this), s, o, u)
             }
-            setValue(t, e) {
-                e.model.set({
+            setValue(t) {
+                this.model.set({
                     clickedValue: t
-                }), e.model.save_changes()
+                }), this.model.save_changes()
             }
         }
-        class Ti extends t.DOMWidgetModel {
+        class Ci extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Ti.model_name,
-                    _view_name: Ti.view_name,
-                    _model_module: Ti.model_module,
-                    _view_module: Ti.view_module,
-                    _model_module_version: Ti.model_module_version,
-                    _view_module_version: Ti.view_module_version,
+                    _model_name: Ci.model_name,
+                    _view_name: Ci.view_name,
+                    _model_module: Ci.model_module,
+                    _view_module: Ci.view_module,
+                    _model_module_version: Ci.model_module_version,
+                    _view_module_version: Ci.view_module_version,
                     data: [],
                     x: String,
                     y: String,
                     hue: String,
-                    element: String,
+                    elementId: String,
                     clickedValue: String,
                     selectedValues: []
                 }
             }
             static model_name = "ScatterplotModel";
             static model_module = $i.name;
             static model_module_version = $i.version;
             static view_name = "ScatterplotView";
             static view_module = $i.name;
             static view_module_version = $i.version
         }
-        class ji extends t.DOMWidgetView {
+        class Oi extends t.DOMWidgetView {
+            timeout;
             render() {
-                this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
             }
-            value_changed() {
-                let t = this;
-                var n = this.model.get("data"),
-                    r = this.model.get("x"),
-                    i = this.model.get("y"),
-                    a = this.model.get("hue"),
-                    o = this.model.get("element");
-                setTimeout((() => {
-                    ! function(t, n, r, i, a, o, s, u) {
-                        for (let e = 0; e < t.length; e++) t[e].id = e;
-                        var l = Math.floor(Math.random() * Date.now() * 1e4).toString(36),
-                            c = 375,
-                            h = 720;
-                        a ? (h = (a = document.getElementById(a)).clientWidth, c = a.clientHeight) : a = u.el, er(a).selectAll("*").remove();
-                        const f = h - 40 - 20,
-                            d = c - 20 - 30;
-                        var p = Wr().range([0, f]),
-                            m = Wr().range([d, 0]),
-                            _ = vr(Fr),
-                            g = q(p),
-                            v = I(m),
-                            y = er(a).append("svg").attr("width", f + 40 + 20).attr("height", d + 20 + 30).append("g").attr("transform", "translate(40,20)");
-                        p.domain(e(t, (function(t) {
-                            return t[n]
-                        }))).nice(), m.domain(e(t, (function(t) {
-                            return t[r]
-                        }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + d + ")").call(g).append("text").attr("class", "label").attr("x", f).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
-                            return "dot-" + l + t.id
-                        })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
-                            return p(t[n])
-                        })).attr("cy", (function(t) {
-                            return m(t[r])
-                        })).style("fill", (function(t) {
+            plot() {
+                const t = this.model.get("data"),
+                    n = this.model.get("x"),
+                    r = this.model.get("y"),
+                    i = this.model.get("hue"),
+                    o = this.model.get("elementId");
+                let a = Si,
+                    s = this.el;
+                o && (s = document.getElementById(o), a = s.clientHeight);
+                let u = s.clientWidth;
+                const l = Ei;
+                ! function(t, n, r, i, o, a, s, u, l, c) {
+                    const h = u - c.left - c.right,
+                        f = l - c.top - c.bottom;
+                    for (let e = 0; e < t.length; e++) t[e].id = e;
+                    const d = Math.floor(Math.random() * Date.now() * 1e4).toString(36);
+                    er(o).selectAll("*").remove();
+                    const p = Wr().range([0, h]),
+                        m = Wr().range([f, 0]),
+                        _ = vr(Fr),
+                        g = D(p),
+                        v = q(m),
+                        y = er(o).append("svg").attr("width", u).attr("height", l).append("g").attr("transform", "translate(" + c.left + "," + c.top + ")");
+                    p.domain(e(t, (function(t) {
+                        return t[n]
+                    }))).nice(), m.domain(e(t, (function(t) {
+                        return t[r]
+                    }))).nice(), y.append("g").attr("class", "x axis").attr("transform", "translate(0," + f + ")").call(g).append("text").attr("class", "label").attr("x", h).attr("y", -6).style("text-anchor", "end"), y.append("g").attr("class", "y axis").call(v).append("text").attr("class", "label").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), y.selectAll(".dot").data(t).enter().append("circle").attr("id", (function(t, e) {
+                        return "dot-" + d + t.id
+                    })).attr("class", "dot").attr("r", 3.5).attr("cx", (function(t) {
+                        return p(t[n])
+                    })).attr("cy", (function(t) {
+                        return m(t[r])
+                    })).style("fill", (function(t) {
+                        return _(t[i])
+                    })).on("mouseover", (function(t, e) {
+                        x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * e[n]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * e[r]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
+                    })).on("mouseout", (function() {
+                        x.style("opacity", 0), b.style("opacity", 0)
+                    })).on("click", (function(t, e) {
+                        const i = "x:" + Math.round(10 * e[n]) / 10 + "    y:" + Math.round(10 * e[r]) / 10;
+                        void 0 !== a && a(i)
+                    })), hi(o, p, m, n, r, c.left, c.top, (function() {
+                        y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
                             return _(t[i])
-                        })).on("mouseover", (function(t, e) {
-                            x.style("opacity", 1), b.style("opacity", 1), x.attr("x", t.offsetX - 30).attr("y", t.offsetY - 40), b.html("x: " + Math.round(10 * e[n]) / 10 + "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;y: " + Math.round(10 * e[r]) / 10).attr("x", t.offsetX - 15).attr("y", t.offsetY - 20)
-                        })).on("mouseout", (function() {
-                            x.style("opacity", 0), b.style("opacity", 0)
-                        })).on("click", (function(t, e) {
-                            const i = "x:" + Math.round(10 * e[n]) / 10 + "    y:" + Math.round(10 * e[r]) / 10;
-                            void 0 !== o && o(i, u)
-                        })), hi(a, p, m, n, r, 40, 20, (function() {
-                            y.selectAll(".dot").data(t).attr("r", 3.5).style("fill", (function(t) {
-                                return _(t[i])
-                            }))
-                        }), (function(t) {
-                            void 0 !== s && s(t, u)
-                        }), l);
-                        var w = y.selectAll(".legend").data(_.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
-                            return "translate(0," + 20 * e + ")"
-                        }));
-                        w.append("rect").attr("x", f - 18).attr("width", 18).attr("height", 18).style("fill", _), w.append("text").attr("x", f - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
-                            return t
-                        }));
-                        const x = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0);
-                        var b = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
-                    }(n, r, i, a, o, this.setValue, this.setSelectedValues, t)
-                }), 50)
+                        }))
+                    }), (function(t) {
+                        void 0 !== s && s(t)
+                    }), d);
+                    const w = y.selectAll(".legend").data(_.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                        return "translate(0," + 20 * e + ")"
+                    }));
+                    w.append("rect").attr("x", h - 18).attr("width", 18).attr("height", 18).style("fill", _), w.append("text").attr("x", h - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
+                        return t
+                    }));
+                    const x = y.append("g").append("rect").style("fill", "none").attr("width", 160).attr("height", 40).attr("stroke", "#69b3a2").attr("stroke-width", 4).style("opacity", 0),
+                        b = y.append("g").append("text").style("opacity", 0).attr("text-anchor", "left").attr("alignment-baseline", "middle")
+                }(t, n, r, i, s, this.setValue.bind(this), this.setSelectedValues.bind(this), u, a, l)
             }
-            setValue(t, e) {
-                e.model.set({
+            setValue(t) {
+                this.model.set({
                     clickedValue: t
-                }), e.model.save_changes()
+                }), this.model.save_changes()
             }
-            setSelectedValues(t, e) {
-                e.model.set({
+            setSelectedValues(t) {
+                this.model.set({
                     selectedValues: t
-                }), e.model.save_changes()
+                }), this.model.save_changes()
             }
         }
-        class Pi extends t.DOMWidgetModel {
+        class Ii extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Pi.model_name,
-                    _view_name: Pi.view_name,
-                    _model_module: Pi.model_module,
-                    _view_module: Pi.view_module,
-                    _model_module_version: Pi.model_module_version,
-                    _view_module_version: Pi.view_module_version,
+                    _model_name: Ii.model_name,
+                    _view_name: Ii.view_name,
+                    _model_module: Ii.model_module,
+                    _view_module: Ii.view_module,
+                    _model_module_version: Ii.model_module_version,
+                    _view_module_version: Ii.view_module_version,
                     data: [],
                     x: String,
                     y: String,
                     hue: String,
-                    element: String
+                    elementId: String
                 }
             }
             static model_name = "BarplotModel";
             static model_module = $i.name;
             static model_module_version = $i.version;
             static view_name = "BarplotView";
             static view_module = $i.name;
             static view_module_version = $i.version
         }
-        class Ci extends t.DOMWidgetView {
+        class Vi extends t.DOMWidgetView {
+            timeout;
             render() {
-                this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
             }
-            value_changed() {
-                let t = this;
-                var e = this.model.get("data"),
-                    n = this.model.get("x"),
-                    r = this.model.get("y"),
-                    i = this.model.get("hue"),
-                    a = this.model.get("element");
-                setTimeout((() => {
-                    ! function(t, e, n, r, i, a) {
-                        var o = 375,
-                            s = 720;
-                        i ? (s = (i = document.getElementById(i)).clientWidth, o = i.clientHeight) : i = a.el, er(i).selectAll("*").remove();
-                        const u = s - 40 - 20,
-                            l = o - 20 - 30;
-                        var c = er(i).append("svg").attr("width", u + 40 + 20).attr("height", l + 20 + 30).append("g").attr("transform", "translate(40,20)");
+            plot() {
+                const t = this.model.get("data"),
+                    e = this.model.get("x"),
+                    n = this.model.get("y"),
+                    r = this.model.get("hue"),
+                    i = this.model.get("elementId");
+                let o = Si,
+                    a = this.el;
+                i && (a = document.getElementById(i), o = a.clientHeight),
+                    function(t, e, n, r, i, o, a, s) {
+                        const u = o - s.left - s.right,
+                            l = a - s.top - s.bottom;
+                        er(i).selectAll("*").remove();
+                        const c = er(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         r || (r = e);
-                        const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []);
-                        let f = {};
-                        var d = vr(Fr);
+                        const h = t.reduce(((t, e) => (t && -1 === t.indexOf(e[r]) && t.push(e[r]), t)), []),
+                            f = {},
+                            d = vr(Fr);
                         r == e ? function() {
                             let r = t.reduce(((t, r) => {
-                                let i = r[e],
-                                    a = r[n];
-                                if (i in t) t[i] += a, f[i].qt += 1, f[i][n].push(a);
+                                const i = r[e],
+                                    o = r[n];
+                                if (i in t) t[i] += o, f[i].qt += 1, f[i][n].push(o);
                                 else {
-                                    var o = {
+                                    const e = {
                                         qt: 1
                                     };
-                                    o[n] = [], o[n].push(a), f[i] = o, t[i] = a
+                                    e[n] = [], e[n].push(o), f[i] = e, t[i] = o
                                 }
                                 return t
                             }), {});
                             r = Object.keys(r).map((t => {
-                                let i = {};
+                                const i = {};
                                 return i[e] = t, i[n] = r[t], 0 != f[t].qt && (i[n] = i[n] / f[t].qt), i
                             })), Object.keys(f).forEach((t => {
-                                let e = f[t][n],
+                                const e = f[t][n],
                                     [r, i] = fi(e);
                                 f[t].min = r, f[t].max = i
                             }));
-                            var i = r.map((t => t[e]));
-                            let a = [],
-                                o = Object.keys(f).map((t => f[t]));
-                            a.push(k(o, (t => t.min))), a.push(M(o, (t => t.max))), a[0] > 0 && a[1] > 0 ? a[0] = 0 : a[0] < 0 && a[1] < 0 && (a[1] = 0);
-                            var s = Wr().domain(a).range([l, 0]);
-                            c.append("g").call(I(s));
-                            var p = yr().domain(i).range([0, u]).padding([.2]);
+                            const i = r.map((t => t[e])),
+                                o = [],
+                                a = Object.keys(f).map((t => f[t]));
+                            o.push(k(a, (t => t.min))), o.push(M(a, (t => t.max))), o[0] > 0 && o[1] > 0 ? o[0] = 0 : o[0] < 0 && o[1] < 0 && (o[1] = 0);
+                            const s = Wr().domain(o).range([l, 0]);
+                            c.append("g").call(q(s));
+                            const p = yr().domain(i).range([0, u]).padding([.2]);
                             c.append("g").selectAll("g").data(r).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e])
                             })).attr("y", (function(t) {
                                 return s(t[n]) < s(0) ? s(t[n]) : s(0)
                             })).attr("width", p.bandwidth()).attr("height", (function(t) {
                                 return Math.abs(s(0) - s(t[n]))
                             })).data(h).attr("fill", (function(t) {
                                 return d(t)
                             }));
                             const m = Object.keys(f).map((t => {
-                                let n = {};
+                                const n = {};
                                 return n[e] = t, n.min = f[t].min, n.max = f[t].max, n
                             }));
                             c.append("g").selectAll("g").data(m).enter().append("rect").attr("x", (function(t) {
                                 return p(t[e]) + p.bandwidth() / 2 - 1
                             })).attr("y", (function(t) {
                                 return s(t.max)
                             })).attr("width", 2).attr("height", (function(t) {
                                 return s(t.min) - s(t.max)
-                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + s(0) + ")").call(q(p).tickSize(0))
+                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + s(0) + ")").call(D(p).tickSize(0))
                         }() : function() {
                             let i = t.reduce(((t, i) => {
-                                let a = i[e],
-                                    o = i[n],
+                                const o = i[e],
+                                    a = i[n],
                                     s = i[r];
-                                if (a in t) {
-                                    f[a].qt[n + "-" + s] += 1, f[a][s][n].push(o);
-                                    for (let e of h) s == e && (t[a][n + "-" + e] += o)
+                                if (o in t) {
+                                    f[o].qt[n + "-" + s] += 1, f[o][s][n].push(a);
+                                    for (const e of h) s == e && (t[o][n + "-" + e] += a)
                                 } else {
-                                    var u = {};
+                                    const e = {};
                                     h.forEach((t => {
-                                        u[t] = {}, u[t][n] = []
+                                        e[t] = {}, e[t][n] = []
                                     }));
-                                    var l = {};
-                                    for (let t of h) l[n + "-" + t] = 0;
-                                    l[n + "-" + s] = 1, u.qt = l, u[s][n].push(o), f[a] = u;
-                                    let e = {};
-                                    for (var c of h) e[n + "-" + c] = s == c ? o : 0;
-                                    t[a] = e
+                                    const r = {};
+                                    for (const t of h) r[n + "-" + t] = 0;
+                                    r[n + "-" + s] = 1, e.qt = r, e[s][n].push(a), f[o] = e;
+                                    const i = {};
+                                    for (const t of h) i[n + "-" + t] = s == t ? a : 0;
+                                    t[o] = i
                                 }
                                 return t
                             }), {});
                             i = Object.keys(i).map((t => {
                                 let n = {};
                                 n[e] = t;
-                                for (let e of Object.keys(i[t])) 0 != f[t].qt[e] && (i[t][e] = i[t][e] / f[t].qt[e]);
+                                for (const e of Object.keys(i[t])) 0 != f[t].qt[e] && (i[t][e] = i[t][e] / f[t].qt[e]);
                                 return n = {
                                     ...n,
                                     ...i[t]
                                 }, n
                             })), Object.keys(f).forEach((t => {
                                 h.forEach((e => {
-                                    let r = f[t][e][n],
-                                        [i, a] = fi(r);
-                                    f[t][e].min = i, f[t][e].max = a
+                                    const r = f[t][e][n],
+                                        [i, o] = fi(r);
+                                    f[t][e].min = i, f[t][e].max = o
                                 }))
                             }));
-                            var a = h.map((t => n + "-" + t)),
-                                o = i.map((t => t[e]));
-                            let s = [];
+                            const o = h.map((t => n + "-" + t)),
+                                a = i.map((t => t[e])),
+                                s = [];
                             Object.keys(f).map((t => {
                                 h.forEach((e => s.push(f[t][e])))
                             }));
-                            let p = [];
+                            const p = [];
                             p.push(k(s, (t => t.min))), p.push(M(s, (t => t.max))), p[0] > 0 && p[1] > 0 ? p[0] = 0 : p[0] < 0 && p[1] < 0 && (p[1] = 0);
-                            var m = Wr().domain(p).range([l, 0]);
-                            c.append("g").call(I(m));
-                            var _ = yr().domain(o).range([0, u]).padding([.2]),
-                                g = yr().domain(a).range([0, _.bandwidth()]).padding([.05]);
+                            const m = Wr().domain(p).range([l, 0]);
+                            c.append("g").call(q(m));
+                            const _ = yr().domain(a).range([0, u]).padding([.2]),
+                                g = yr().domain(o).range([0, _.bandwidth()]).padding([.05]);
                             c.append("g").selectAll("g").data(i).enter().append("g").attr("transform", (function(t) {
                                 return "translate(" + _(t[e]) + ",0)"
                             })).selectAll("rect").data((function(t) {
-                                return a.map((function(e) {
+                                return o.map((function(e) {
                                     return {
                                         key: e,
                                         value: t[e]
                                     }
                                 }))
                             })).enter().append("rect").attr("x", (function(t) {
                                 return g(t.key)
@@ -3827,118 +3842,116 @@
                             })).enter().append("rect").attr("x", (function(t) {
                                 return g(t.key) + g.bandwidth() / 2 - 1
                             })).attr("y", (function(t) {
                                 return t.value.max ? m(t.value.max) : 0
                             })).attr("width", 2).attr("height", (function(t) {
                                 return t.value.min && t.value.max ? m(t.value.min) - m(t.value.max) : 0
                             }));
-                            var y = c.selectAll(".legend").data(d.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
+                            const y = c.selectAll(".legend").data(d.domain()).enter().append("g").attr("class", "legend").attr("transform", (function(t, e) {
                                 return "translate(0," + 20 * e + ")"
                             }));
                             y.append("rect").attr("x", u - 18).attr("width", 18).attr("height", 18).style("fill", d), y.append("text").attr("x", u - 24).attr("y", 9).attr("dy", ".35em").style("text-anchor", "end").text((function(t) {
                                 return t
-                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + m(0) + ")").call(q(_).tickSize(0))
+                            })), c.append("g").style("font", "18px times").attr("transform", "translate(0," + m(0) + ")").call(D(_).tickSize(0))
                         }()
-                    }(e, n, r, i, a, t)
-                }), 50)
+                    }(t, e, n, r, a, a.clientWidth, o, Ei)
             }
         }
-        class Oi extends t.DOMWidgetModel {
+        class Di extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Oi.model_name,
-                    _view_name: Oi.view_name,
-                    _model_module: Oi.model_module,
-                    _view_module: Oi.view_module,
-                    _model_module_version: Oi.model_module_version,
-                    _view_module_version: Oi.view_module_version,
+                    _model_name: Di.model_name,
+                    _view_name: Di.view_name,
+                    _model_module: Di.model_module,
+                    _view_module: Di.view_module,
+                    _model_module_version: Di.model_module_version,
+                    _view_module_version: Di.view_module_version,
                     data: [],
                     x: String,
                     start: Number,
                     end: Number,
-                    element: String
+                    elementId: String
                 }
             }
             static model_name = "HistogramplotModel";
             static model_module = $i.name;
             static model_module_version = $i.version;
             static view_name = "HistogramplotView";
             static view_module = $i.name;
             static view_module_version = $i.version
         }
-        class Vi extends t.DOMWidgetView {
+        class qi extends t.DOMWidgetView {
+            timeout;
             render() {
-                this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                ji(this), this.model.on("change:data", (() => ji(this)), this), window.addEventListener("resize", (() => ji(this).bind(this)))
             }
-            value_changed() {
-                let t = this;
-                var e = this.model.get("data"),
-                    n = this.model.get("x"),
-                    r = this.model.get("start"),
-                    i = this.model.get("end"),
-                    a = this.model.get("element");
-                setTimeout((() => {
-                    ! function(t, e, n, r, i, a) {
-                        var o = 375,
-                            s = 720;
-                        i ? (s = (i = document.getElementById(i)).clientWidth, o = i.clientHeight) : i = a.el, er(i).selectAll("*").remove();
-                        const u = s - 40 - 20,
-                            l = o - 20 - 30;
+            plot() {
+                const t = this.model.get("data"),
+                    e = this.model.get("x"),
+                    n = this.model.get("start"),
+                    r = this.model.get("end"),
+                    i = this.model.get("elementId");
+                let o = Si,
+                    a = this.el;
+                i && (a = document.getElementById(i), o = a.clientHeight),
+                    function(t, e, n, r, i, o, a, s) {
+                        const u = o - s.left - s.right,
+                            l = a - s.top - s.bottom;
+                        er(i).selectAll("*").remove();
                         let c = n;
                         n || (c = k(t, (t => t[e])));
                         let h = r;
                         r || (h = M(t, (t => t[e])));
                         const f = Wr().range([0, u]),
                             d = Wr().range([l, 0]),
-                            p = q(f),
-                            m = I(d),
+                            p = D(f),
+                            m = q(d),
                             _ = b().thresholds(40).value((t => Math.round(10 * t[e]) / 10))(t),
-                            g = er(i).append("svg").attr("width", u + 40 + 20).attr("height", l + 20 + 30).append("g").attr("transform", "translate(40,20)");
+                            g = er(i).append("svg").attr("width", o).attr("height", a).append("g").attr("transform", "translate(" + s.left + "," + s.top + ")");
                         f.domain([c, h]), d.domain([0, M(_, (t => t.length))]), g.append("g").attr("transform", "translate(0," + l + ")").call(p).append("text").attr("x", u).attr("y", -6).style("text-anchor", "end"), g.append("g").call(m).append("text").attr("transform", "rotate(-90)").attr("y", 6).attr("dy", ".71em").style("text-anchor", "end"), g.append("g").attr("fill", "steelblue").selectAll().data(_).join("rect").attr("x", (t => f(t.x0) + 1)).attr("width", (t => f(t.x1) - f(t.x0) - 1)).attr("y", (t => d(t.length))).attr("height", (t => d(0) - d(t.length)))
-                    }(e, n, r, i, a, t)
-                }), 50)
+                    }(t, e, n, r, a, a.clientWidth, o, Ei)
             }
         }
-        class Di extends t.DOMWidgetModel {
+        class Li extends t.DOMWidgetModel {
             defaults() {
                 return {
                     ...super.defaults(),
-                    _model_name: Di.model_name,
-                    _view_name: Di.view_name,
-                    _model_module: Di.model_module,
-                    _view_module: Di.view_module,
-                    _model_module_version: Di.model_module_version,
-                    _view_module_version: Di.view_module_version,
+                    _model_name: Li.model_name,
+                    _view_name: Li.view_name,
+                    _model_module: Li.model_module,
+                    _view_module: Li.view_module,
+                    _model_module_version: Li.model_module_version,
+                    _view_module_version: Li.view_module_version,
                     matrix: [],
                     grid_areas: [],
                     grid_template_areas: String,
                     style: String
                 }
             }
             static model_name = "EmbeddingModel";
             static model_module = $i.name;
             static model_module_version = $i.version;
             static view_name = "EmbeddingView";
             static view_module = $i.name;
             static view_module_version = $i.version
         }
-        class qi extends t.DOMWidgetView {
+        class Hi extends t.DOMWidgetView {
             render() {
-                this.value_changed(), this.model.on("change:data", this.value_changed, this)
+                this.value_changed()
             }
             value_changed() {
-                var t = this.model.get("matrix"),
+                const t = this.model.get("matrix"),
                     e = this.model.get("grid_areas"),
-                    n = this.model.get("grid_template_areas"),
-                    r = this.model.get("style");
+                    n = this.model.get("grid_template_areas");
+                let r = this.model.get("style");
                 r || (r = "basic");
                 const i = document.createElement("div");
                 i.classList.add(r), i.style.display = "grid", i.style.gridTemplateAreas = n, i.style.gridTemplateRows = "repeat(" + t.length + ", 20vh)", i.style.gridTemplateColumns = "repeat(" + t[0].length + ", 1fr)", i.style.width = "100%", e.forEach((t => {
                     const e = document.createElement("div");
                     e.setAttribute("id", t), e.style.gridArea = t, e.classList.add("dashboard-div"), i.appendChild(e)
                 })), this.el.appendChild(i)
             }
         }
-        var Ii = i(330)
-    })(), a
+        var Xi = i(330)
+    })(), o
 })()));
```

### Comparing `d3vis_ipynb-0.1.1/js/amd-public-path.js` & `d3vis_ipynb-0.1.2/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/package.json` & `d3vis_ipynb-0.1.2/d3vis_ipynb/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.bf58726a1c33e2ff91a1.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -14,14 +14,18 @@
     },
     "files": [
         "lib/**/*.js",
         "dist/*.js",
         "css/*.css"
     ],
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.bf58726a1c33e2ff91a1.js"
+        },
         "extension": "lib/labplugin",
         "outputDir": "../d3vis_ipynb/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
             }
@@ -50,9 +54,9 @@
         "export": "webpack --env export --config webpack.exports.config.js",
         "prepublish": "yarn run clean && yarn run build:prod",
         "start": "webpack serve --open --config webpack.exports.config.js",
         "start:export": "webpack serve --open --config webpack.exports.config.js --env export",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `d3vis_ipynb-0.1.1/js/webpack.config.js` & `d3vis_ipynb-0.1.2/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/webpack.exports.config.js` & `d3vis_ipynb-0.1.2/js/webpack.exports.config.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/css/widget.css` & `d3vis_ipynb-0.1.2/js/css/widget.css`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/lib/labplugin.js` & `d3vis_ipynb-0.1.2/js/lib/labplugin.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/lib/web-dev.js` & `d3vis_ipynb-0.1.2/js/lib/web-dev.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/lib/widgets.js` & `d3vis_ipynb-0.1.2/js/lib/widgets.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -13,74 +13,101 @@
 } from "./graphs/barplot";
 import {
     histogramplot
 } from "./graphs/histogramplot";
 import "../css/widget.css";
 const data = require("../package.json");
 
+const WIDGET_HEIGHT = 400;
+const WIDGET_MARGIN = {
+    top: 20,
+    right: 20,
+    bottom: 30,
+    left: 40
+};
+const RENDER_INTERVAL = 100;
+
+function plotAfterInterval(that) {
+    if (that.timeout) {
+        clearTimeout(that.timeout);
+    }
+    that.timeout = setTimeout(() => {
+        that.plot();
+    }, RENDER_INTERVAL);
+}
+
 export class LinearHistPlotModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
             _model_name: LinearHistPlotModel.model_name,
             _view_name: LinearHistPlotModel.view_name,
             _model_module: LinearHistPlotModel.model_module,
             _view_module: LinearHistPlotModel.view_module,
             _model_module_version: LinearHistPlotModel.model_module_version,
             _view_module_version: LinearHistPlotModel.view_module_version,
 
             linearData_x: [],
             linearData_y: [],
             histogramData: [],
-            element: String,
+            elementId: String,
             clickedValue: String,
         };
     }
 
     static model_name = "LinearHistPlotModel";
     static model_module = data.name;
     static model_module_version = data.version;
     static view_name = "LinearHistPlotView"; // Set to null if no view
     static view_module = data.name; // Set to null if no view
     static view_module_version = data.version;
 }
 
 export class LinearHistPlotView extends DOMWidgetView {
+    timeout;
+
     render() {
-        this.value_changed();
+        plotAfterInterval(this);
 
-        // Observe and act on future changes to the value attribute
-        this.model.on("change:linearData_x", this.value_changed, this);
+        this.model.on("change:linearData_x", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
     }
 
-    value_changed() {
-        let that = this;
+    plot() {
+        const linearData_x = this.model.get("linearData_x");
+        const linearData_y = this.model.get("linearData_y");
+        const histogramData = this.model.get("histogramData");
+        const elementId = this.model.get("elementId");
+
+        let height = WIDGET_HEIGHT;
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+            height = element.clientHeight;
+        }
+        let width = element.clientWidth;
+        const margin = WIDGET_MARGIN;
 
-        var linearData_x = this.model.get("linearData_x");
-        var linearData_y = this.model.get("linearData_y");
-        var histogramData = this.model.get("histogramData");
-        var element = this.model.get("element");
-
-        setTimeout(() => {
-            linearhistplot(
-                linearData_x,
-                linearData_y,
-                histogramData,
-                element,
-                this.setValue,
-                that
-            );
-        }, 50);
+        linearhistplot(
+            linearData_x,
+            linearData_y,
+            histogramData,
+            element,
+            this.setValue.bind(this),
+            width,
+            height,
+            margin
+        );
     }
 
-    setValue(text, that) {
-        that.model.set({
+    setValue(text) {
+        this.model.set({
             clickedValue: text
         });
-        that.model.save_changes();
+        this.model.save_changes();
     }
 }
 
 export class ScatterPlotModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
@@ -91,71 +118,80 @@
             _model_module_version: ScatterPlotModel.model_module_version,
             _view_module_version: ScatterPlotModel.view_module_version,
 
             data: [],
             x: String,
             y: String,
             hue: String,
-            element: String,
+            elementId: String,
             clickedValue: String,
             selectedValues: [],
         };
     }
 
     static model_name = "ScatterplotModel";
     static model_module = data.name;
     static model_module_version = data.version;
     static view_name = "ScatterplotView"; // Set to null if no view
     static view_module = data.name; // Set to null if no view
     static view_module_version = data.version;
 }
 
 export class ScatterPlotView extends DOMWidgetView {
+    timeout;
+
     render() {
-        this.value_changed();
+        plotAfterInterval(this);
 
-        // Observe and act on future changes to the value attribute
-        this.model.on("change:data", this.value_changed, this);
+        this.model.on("change:data", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
     }
 
-    value_changed() {
-        let that = this;
+    plot() {
+        const data = this.model.get("data");
+        const x = this.model.get("x");
+        const y = this.model.get("y");
+        const hue = this.model.get("hue");
+        const elementId = this.model.get("elementId");
+
+        let height = WIDGET_HEIGHT;
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+            height = element.clientHeight;
+        }
+        let width = element.clientWidth;
+        const margin = WIDGET_MARGIN;
 
-        var data = this.model.get("data");
-        var x = this.model.get("x");
-        var y = this.model.get("y");
-        var hue = this.model.get("hue");
-        var element = this.model.get("element");
-
-        setTimeout(() => {
-            scatterplot(
-                data,
-                x,
-                y,
-                hue,
-                element,
-                this.setValue,
-                this.setSelectedValues,
-                that
-            );
-        }, 50);
+        scatterplot(
+            data,
+            x,
+            y,
+            hue,
+            element,
+            this.setValue.bind(this),
+            this.setSelectedValues.bind(this),
+            width,
+            height,
+            margin
+        );
     }
 
-    setValue(text, that) {
-        that.model.set({
+    setValue(text) {
+        this.model.set({
             clickedValue: text
         });
-        that.model.save_changes();
+        this.model.save_changes();
     }
 
-    setSelectedValues(values, that) {
-        that.model.set({
+    setSelectedValues(values) {
+        this.model.set({
             selectedValues: values
         });
-        that.model.save_changes();
+        this.model.save_changes();
     }
 }
 
 export class BarPlotModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
@@ -166,46 +202,53 @@
             _model_module_version: BarPlotModel.model_module_version,
             _view_module_version: BarPlotModel.view_module_version,
 
             data: [],
             x: String,
             y: String,
             hue: String,
-            element: String,
+            elementId: String,
         };
     }
 
     static model_name = "BarplotModel";
     static model_module = data.name;
     static model_module_version = data.version;
     static view_name = "BarplotView"; // Set to null if no view
     static view_module = data.name; // Set to null if no view
     static view_module_version = data.version;
 }
 
 export class BarPlotView extends DOMWidgetView {
+    timeout;
+
     render() {
-        this.value_changed();
+        plotAfterInterval(this);
 
-        // Observe and act on future changes to the value attribute
-        this.model.on("change:data", this.value_changed, this);
+        this.model.on("change:data", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
     }
 
-    value_changed() {
-        let that = this;
+    plot() {
+        const data = this.model.get("data");
+        const x = this.model.get("x");
+        const y = this.model.get("y");
+        const hue = this.model.get("hue");
+        const elementId = this.model.get("elementId");
+
+        let height = WIDGET_HEIGHT;
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+            height = element.clientHeight;
+        }
+        let width = element.clientWidth;
+        const margin = WIDGET_MARGIN;
 
-        var data = this.model.get("data");
-        var x = this.model.get("x");
-        var y = this.model.get("y");
-        var hue = this.model.get("hue");
-        var element = this.model.get("element");
-
-        setTimeout(() => {
-            barplot(data, x, y, hue, element, that);
-        }, 50);
+        barplot(data, x, y, hue, element, width, height, margin);
     }
 }
 
 export class HistogramPlotModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
@@ -216,46 +259,53 @@
             _model_module_version: HistogramPlotModel.model_module_version,
             _view_module_version: HistogramPlotModel.view_module_version,
 
             data: [],
             x: String,
             start: Number,
             end: Number,
-            element: String,
+            elementId: String,
         };
     }
 
     static model_name = "HistogramplotModel";
     static model_module = data.name;
     static model_module_version = data.version;
     static view_name = "HistogramplotView"; // Set to null if no view
     static view_module = data.name; // Set to null if no view
     static view_module_version = data.version;
 }
 
 export class HistogramPlotView extends DOMWidgetView {
+    timeout;
+
     render() {
-        this.value_changed();
+        plotAfterInterval(this);
 
-        // Observe and act on future changes to the value attribute
-        this.model.on("change:data", this.value_changed, this);
+        this.model.on("change:data", () => plotAfterInterval(this), this);
+        window.addEventListener("resize", () => plotAfterInterval(this).bind(this));
     }
 
-    value_changed() {
-        let that = this;
+    plot() {
+        const data = this.model.get("data");
+        const x = this.model.get("x");
+        const start = this.model.get("start");
+        const end = this.model.get("end");
+        const elementId = this.model.get("elementId");
+
+        let height = WIDGET_HEIGHT;
+        let element = this.el;
+        if (elementId) {
+            element = document.getElementById(elementId);
+            height = element.clientHeight;
+        }
+        let width = element.clientWidth;
+        const margin = WIDGET_MARGIN;
 
-        var data = this.model.get("data");
-        var x = this.model.get("x");
-        var start = this.model.get("start");
-        var end = this.model.get("end");
-        var element = this.model.get("element");
-
-        setTimeout(() => {
-            histogramplot(data, x, start, end, element, that);
-        }, 50);
+        histogramplot(data, x, start, end, element, width, height, margin);
     }
 }
 
 export class EmbeddingModel extends DOMWidgetModel {
     defaults() {
         return {
             ...super.defaults(),
@@ -280,44 +330,39 @@
     static view_module = data.name; // Set to null if no view
     static view_module_version = data.version;
 }
 
 export class EmbeddingView extends DOMWidgetView {
     render() {
         this.value_changed();
-
-        // Observe and act on future changes to the value attribute
-        this.model.on("change:data", this.value_changed, this);
     }
 
     value_changed() {
-        let that = this;
-
-        var matrix = this.model.get("matrix");
-        var grid_areas = this.model.get("grid_areas");
-        var grid_template_areas = this.model.get("grid_template_areas");
-        var style = this.model.get("style");
+        const matrix = this.model.get("matrix");
+        const grid_areas = this.model.get("grid_areas");
+        const grid_template_areas = this.model.get("grid_template_areas");
+        let style = this.model.get("style");
 
         if (!style) {
-            style = "basic"
+            style = "basic";
         }
 
         const node = document.createElement("div");
 
-        node.classList.add(style)
+        node.classList.add(style);
         node.style.display = "grid";
         node.style.gridTemplateAreas = grid_template_areas;
         node.style.gridTemplateRows = "repeat(" + matrix.length + ", 20vh)";
         node.style.gridTemplateColumns = "repeat(" + matrix[0].length + ", 1fr)";
         node.style.width = "100%";
 
         grid_areas.forEach((area) => {
             const grid_area = document.createElement("div");
             grid_area.setAttribute("id", area);
             grid_area.style.gridArea = area;
-            grid_area.classList.add("dashboard-div")
+            grid_area.classList.add("dashboard-div");
             node.appendChild(grid_area);
         });
 
-        that.el.appendChild(node);
+        this.el.appendChild(node);
     }
 }
```

### Comparing `d3vis_ipynb-0.1.1/js/lib/graphs/barplot.js` & `d3vis_ipynb-0.1.2/js/lib/graphs/barplot.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,108 +1,93 @@
 import * as d3 from "d3";
 
-export function barplot(data, x_axis, y_axis, hue_axis, element, that) {
-    var customHeight = 375;
-    var customWidth = 720;
-    if (element) {
-        element = document.getElementById(element)
-        customWidth = element.clientWidth;
-        customHeight = element.clientHeight;
-    } else {
-        element = that.el;
-    }
-    d3.select(element).selectAll("*").remove();
+export function barplot(data, x_axis, y_axis, hue_axis, element, width, height, margin) {
+    const innerWidth = width - margin.left - margin.right
+    const innerHeight = height - margin.top - margin.bottom
 
-    const margin = {
-        top: 20,
-        right: 20,
-        bottom: 30,
-        left: 40
-    };
-    const width = customWidth - margin.left - margin.right;
-    const height = customHeight - margin.top - margin.bottom;
+    d3.select(element).selectAll("*").remove();
 
-    var svg = d3
+    const svg = d3
         .select(element)
         .append("svg")
-        .attr("width", width + margin.left + margin.right)
-        .attr("height", height + margin.top + margin.bottom)
+        .attr("width", width)
+        .attr("height", height)
         .append("g")
         .attr("transform", "translate(" + margin.left + "," + margin.top + ")");
 
     if (!hue_axis) hue_axis = x_axis;
 
     const allHues = data.reduce((all, row) => {
         if (all && all.indexOf(row[hue_axis]) === -1) {
             all.push(row[hue_axis]);
         }
         return all;
     }, []);
-    let values = {};
+    const values = {};
 
-    var color = d3.scaleOrdinal(d3.schemeCategory10);
+    const color = d3.scaleOrdinal(d3.schemeCategory10);
 
     if (hue_axis == x_axis) {
         createSingleBars();
     } else {
         createGroupBars();
     }
 
     function createSingleBars() {
         let result = data.reduce((res, row) => {
-            let x = row[x_axis];
-            let y = row[y_axis];
+            const x = row[x_axis];
+            const y = row[y_axis];
 
             if (x in res) {
                 res[x] += y;
                 values[x]["qt"] += 1;
                 values[x][y_axis].push(y);
             } else {
-                var newValues = {};
+                const newValues = {};
                 newValues["qt"] = 1;
                 newValues[y_axis] = [];
                 newValues[y_axis].push(y);
                 values[x] = newValues;
                 res[x] = y;
             }
 
             return res;
         }, {});
 
         result = Object.keys(result).map((key) => {
-            let newRow = {};
+            const newRow = {};
             newRow[x_axis] = key;
             newRow[y_axis] = result[key];
             if (values[key]["qt"] != 0) {
                 newRow[y_axis] = newRow[y_axis] / values[key]["qt"];
             }
             return newRow;
         });
 
         Object.keys(values).forEach((key) => {
-            let array = values[key][y_axis];
-            let [min, max] = getCI(array);
+            const array = values[key][y_axis];
+            const [min, max] = getCI(array);
             values[key]["min"] = min;
             values[key]["max"] = max;
         });
 
-        var groups = result.map((r) => r[x_axis]);
+        const groups = result.map((r) => r[x_axis]);
 
-        let y_domain = [];
-        let all_min_max = Object.keys(values).map((key) => values[key]);
+        const y_domain = [];
+        const all_min_max = Object.keys(values).map((key) => values[key]);
         y_domain.push(d3.min(all_min_max, (v) => v.min));
         y_domain.push(d3.max(all_min_max, (v) => v.max));
         if (y_domain[0] > 0 && y_domain[1] > 0) y_domain[0] = 0;
         else if (y_domain[0] < 0 && y_domain[1] < 0) y_domain[1] = 0;
 
-        var y = d3.scaleLinear().domain(y_domain).range([height, 0]);
+        const y = d3.scaleLinear().domain(y_domain).range([innerHeight, 0]);
 
         svg.append("g").call(d3.axisLeft(y));
 
-        var x = d3.scaleBand().domain(groups).range([0, width]).padding([0.2]);
+        const x = d3.scaleBand().domain(groups).range([0, innerWidth]).padding([0.2]);
 
         svg
             .append("g")
             .selectAll("g")
             .data(result)
             .enter()
             .append("rect")
@@ -118,15 +103,15 @@
             })
             .data(allHues)
             .attr("fill", function(d) {
                 return color(d);
             });
 
         const itrValues = Object.keys(values).map((key) => {
-            let newRow = {};
+            const newRow = {};
             newRow[x_axis] = key;
             newRow["min"] = values[key]["min"];
             newRow["max"] = values[key]["max"];
             return newRow;
         });
 
         svg
@@ -151,96 +136,96 @@
             .style("font", "18px times")
             .attr("transform", "translate(0," + y(0) + ")")
             .call(d3.axisBottom(x).tickSize(0));
     }
 
     function createGroupBars() {
         let result = data.reduce((res, row) => {
-            let x = row[x_axis];
-            let y = row[y_axis];
-            let hue = row[hue_axis];
+            const x = row[x_axis];
+            const y = row[y_axis];
+            const hue = row[hue_axis];
 
             if (x in res) {
                 values[x]["qt"][y_axis + "-" + hue] += 1;
                 values[x][hue][y_axis].push(y);
-                for (let h of allHues) {
+                for (const h of allHues) {
                     if (hue == h) res[x][y_axis + "-" + h] += y;
                 }
             } else {
-                var newValues = {};
+                const newValues = {};
                 allHues.forEach((hue) => {
                     newValues[hue] = {};
                     newValues[hue][y_axis] = [];
                 });
 
-                var qt = {};
-                for (let h of allHues) {
+                const qt = {};
+                for (const h of allHues) {
                     qt[y_axis + "-" + h] = 0;
                 }
                 qt[y_axis + "-" + hue] = 1;
 
                 newValues["qt"] = qt;
                 newValues[hue][y_axis].push(y);
                 values[x] = newValues;
-                let newRow = {};
-                for (var h of allHues) {
+                const newRow = {};
+                for (const h of allHues) {
                     if (hue == h) newRow[y_axis + "-" + h] = y;
                     else newRow[y_axis + "-" + h] = 0;
                 }
                 res[x] = newRow;
             }
 
             return res;
         }, {});
 
         result = Object.keys(result).map((key) => {
             let newRow = {};
             newRow[x_axis] = key;
-            for (let i of Object.keys(result[key])) {
+            for (const i of Object.keys(result[key])) {
                 if (values[key]["qt"][i] != 0) {
                     result[key][i] = result[key][i] / values[key]["qt"][i];
                 }
             }
             newRow = {
                 ...newRow,
                 ...result[key]
             };
             return newRow;
         });
 
         Object.keys(values).forEach((key) => {
             allHues.forEach((h) => {
-                let array = values[key][h][y_axis];
-                let [min, max] = getCI(array);
+                const array = values[key][h][y_axis];
+                const [min, max] = getCI(array);
                 values[key][h]["min"] = min;
                 values[key][h]["max"] = max;
             });
         });
 
-        var subgroups = allHues.map((value) => y_axis + "-" + value);
-        var groups = result.map((r) => r[x_axis]);
+        const subgroups = allHues.map((value) => y_axis + "-" + value);
+        const groups = result.map((r) => r[x_axis]);
 
-        let all_min_max = [];
+        const all_min_max = [];
         Object.keys(values).map((key) => {
             allHues.forEach((h) => all_min_max.push(values[key][h]));
         });
 
-        let y_domain = [];
+        const y_domain = [];
         y_domain.push(d3.min(all_min_max, (v) => v.min));
         y_domain.push(d3.max(all_min_max, (v) => v.max));
         if (y_domain[0] > 0 && y_domain[1] > 0) y_domain[0] = 0;
         else if (y_domain[0] < 0 && y_domain[1] < 0) y_domain[1] = 0;
 
-        var y = d3.scaleLinear().domain(y_domain).range([height, 0]);
+        const y = d3.scaleLinear().domain(y_domain).range([innerHeight, 0]);
 
         svg.append("g").call(d3.axisLeft(y));
 
-        var x = d3.scaleBand().domain(groups).range([0, width]).padding([0.2]);
+        const x = d3.scaleBand().domain(groups).range([0, innerWidth]).padding([0.2]);
 
-        var xSubgroup = d3
+        const xSubgroup = d3
             .scaleBand()
             .domain(subgroups)
             .range([0, x.bandwidth()])
             .padding([0.05]);
 
         svg
             .append("g")
@@ -316,34 +301,34 @@
             })
             .attr("width", 2)
             .attr("height", function(d) {
                 if (!d.value.min || !d.value.max) return 0;
                 return y(d.value["min"]) - y(d.value["max"]);
             });
 
-        var legend = svg
+        const legend = svg
             .selectAll(".legend")
             .data(color.domain())
             .enter()
             .append("g")
             .attr("class", "legend")
             .attr("transform", function(d, i) {
                 return "translate(0," + i * 20 + ")";
             });
 
         legend
             .append("rect")
-            .attr("x", width - 18)
+            .attr("x", innerWidth - 18)
             .attr("width", 18)
             .attr("height", 18)
             .style("fill", color);
 
         legend
             .append("text")
-            .attr("x", width - 24)
+            .attr("x", innerWidth - 24)
             .attr("y", 9)
             .attr("dy", ".35em")
             .style("text-anchor", "end")
             .text(function(d) {
                 return d;
             });
 
@@ -360,10 +345,10 @@
     array.forEach((num) => (sd = sd + (num - mean) ** 2));
     sd = Math.sqrt(sd) / array.length;
     return sd;
 }
 
 function getCI(array) {
     const mean = array.reduce((a, b) => a + b, 0) / array.length;
-    let complement = 1.96 * standardDeviationPerSquareRootedSize(array, mean);
+    const complement = 1.96 * standardDeviationPerSquareRootedSize(array, mean);
     return [mean - complement, mean + complement];
 }
```

### Comparing `d3vis_ipynb-0.1.1/js/lib/graphs/histogramplot.js` & `d3vis_ipynb-0.1.2/js/lib/graphs/histogramplot.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,69 +1,63 @@
 import * as d3 from "d3";
 
-export function histogramplot(data, x_axis, xStart, xEnd, element, that) {
-    var customHeight = 375;
-    var customWidth = 720;
-    if (element) {
-        element = document.getElementById(element)
-        customWidth = element.clientWidth;
-        customHeight = element.clientHeight;
-    } else {
-        element = that.el;
-    }
-    d3.select(element).selectAll("*").remove();
+export function histogramplot(
+    data,
+    x_axis,
+    xStart,
+    xEnd,
+    element,
+    width,
+    height,
+    margin
+) {
+    const innerWidth = width - margin.left - margin.right;
+    const innerHeight = height - margin.top - margin.bottom;
 
-    const margin = {
-        top: 20,
-        right: 20,
-        bottom: 30,
-        left: 40
-    };
-    const width = customWidth - margin.left - margin.right;
-    const height = customHeight - margin.top - margin.bottom;
+    d3.select(element).selectAll("*").remove();
 
     let xMin = xStart;
     if (!xStart) {
         xMin = d3.min(data, (d) => d[x_axis]);
     }
     let xMax = xEnd;
     if (!xEnd) {
         xMax = d3.max(data, (d) => d[x_axis]);
     }
 
-    const x = d3.scaleLinear().range([0, width]);
+    const x = d3.scaleLinear().range([0, innerWidth]);
 
-    const y = d3.scaleLinear().range([height, 0]);
+    const y = d3.scaleLinear().range([innerHeight, 0]);
 
     const xAxis = d3.axisBottom(x);
 
     const yAxis = d3.axisLeft(y);
 
     const bins = d3
         .bin()
         .thresholds(40)
         .value((d) => Math.round(d[x_axis] * 10) / 10)(data);
 
     const svg = d3
         .select(element)
         .append("svg")
-        .attr("width", width + margin.left + margin.right)
-        .attr("height", height + margin.top + margin.bottom)
+        .attr("width", width)
+        .attr("height", height)
         .append("g")
         .attr("transform", "translate(" + margin.left + "," + margin.top + ")");
 
     x.domain([xMin, xMax]);
     y.domain([0, d3.max(bins, (d) => d.length)]);
 
     svg
         .append("g")
-        .attr("transform", "translate(0," + height + ")")
+        .attr("transform", "translate(0," + innerHeight + ")")
         .call(xAxis)
         .append("text")
-        .attr("x", width)
+        .attr("x", innerWidth)
         .attr("y", -6)
         .style("text-anchor", "end");
 
     svg
         .append("g")
         .call(yAxis)
         .append("text")
```

### Comparing `d3vis_ipynb-0.1.1/js/lib/graphs/linearhistplot.js` & `d3vis_ipynb-0.1.2/js/lib/graphs/linearhistplot.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -2,43 +2,30 @@
 
 export function linearhistplot(
     linearData_x,
     linearData_y,
     histogramData,
     element,
     setValue,
-    that
+    width,
+    height,
+    margin
 ) {
-    var customHeight = 375;
-    var customWidth = 720;
-    if (element) {
-        element = document.getElementById(element)
-        customWidth = element.clientWidth;
-        customHeight = element.clientHeight;
-    } else {
-        element = that.el;
-    }
-    d3.select(element).selectAll("*").remove();
+    const innerWidth = width - margin.left - margin.right;
+    const innerHeight = height - margin.top - margin.bottom;
+    const heightHist = innerHeight / 4;
 
-    const margin = {
-        top: 20,
-        right: 20,
-        bottom: 30,
-        left: 40
-    };
-    const width = customWidth - margin.left - margin.right;
-    const height = customHeight - margin.top - margin.bottom;
-    const heightHist = customHeight / 5 - margin.top - margin.bottom;
+    d3.select(element).selectAll("*").remove();
 
     const xMin = Math.min(d3.min(linearData_x), d3.min(histogramData));
     const xMax = Math.max(d3.max(linearData_x), d3.max(histogramData));
 
-    const x = d3.scaleLinear().range([0, width]);
+    const x = d3.scaleLinear().range([0, innerWidth]);
 
-    const y = d3.scaleLinear().range([height, 0]);
+    const y = d3.scaleLinear().range([innerHeight, 0]);
     const yHist = d3.scaleLinear().range([heightHist, 0]);
 
     const xAxis = d3.axisBottom(x);
 
     const yAxis = d3.axisLeft(y);
 
     function mouseover(event, d) {
@@ -66,28 +53,28 @@
         const text =
             "x:" +
             Math.round(d["x"] * 10) / 10 +
             "  -  " +
             "y:" +
             Math.round(d["y"] * 10) / 10;
         if (setValue !== undefined) {
-            setValue(text, that);
+            setValue(text);
         }
     }
 
     const bins = d3
         .bin()
         .thresholds(20)
         .value((d) => Math.round(d * 10) / 10)(histogramData);
 
     const svg = d3
         .select(element)
         .append("svg")
-        .attr("width", width + margin.left + margin.right)
-        .attr("height", height + margin.top + margin.bottom)
+        .attr("width", width)
+        .attr("height", height)
         .append("g")
         .attr("transform", "translate(" + margin.left + "," + margin.top + ")");
 
     x.domain([xMin, xMax]);
     y.domain(d3.extent(linearData_y));
     yHist.domain([0, d3.max(bins, (d) => d.length)]);
 
@@ -97,27 +84,27 @@
         .style("fill", "none")
         .attr("width", 160)
         .attr("height", 40)
         .attr("stroke", "#69b3a2")
         .attr("stroke-width", 4)
         .style("opacity", 0);
 
-    var focusText = svg
+    const focusText = svg
         .append("g")
         .append("text")
         .style("opacity", 0)
         .attr("text-anchor", "left")
         .attr("alignment-baseline", "middle");
 
     svg
         .append("g")
-        .attr("transform", "translate(0," + height + ")")
+        .attr("transform", "translate(0," + innerHeight + ")")
         .call(xAxis)
         .append("text")
-        .attr("x", width)
+        .attr("x", innerWidth)
         .attr("y", -6)
         .style("text-anchor", "end");
 
     svg
         .append("g")
         .call(yAxis)
         .append("text")
@@ -133,19 +120,19 @@
         .attr("stroke", "steelblue")
         .attr("stroke-width", 1)
         .attr(
             "d",
             d3
             .line()
             .x((d) => x((d.x1 + d.x0) / 2))
-            .y((d) => yHist(d.length) + height - heightHist)
+            .y((d) => yHist(d.length) + innerHeight - heightHist)
             .curve(d3.curveCatmullRom)
         );
 
-    var coords = linearData_x
+    const coords = linearData_x
         .map((v, i) => [v, linearData_y[i]])
         .map(([x, y]) => ({
             x,
             y
         }));
 
     svg
```

### Comparing `d3vis_ipynb-0.1.1/js/lib/graphs/scatterplot.js` & `d3vis_ipynb-0.1.2/js/lib/graphs/scatterplot.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -7,52 +7,41 @@
     data,
     x_value,
     y_value,
     hue,
     element,
     setValue,
     setSelectedValues,
-    that
+    width,
+    height,
+    margin
 ) {
+    const innerWidth = width - margin.left - margin.right;
+    const innerHeight = height - margin.top - margin.bottom;
+
     for (let i = 0; i < data.length; i++) {
+        ("");
         data[i]["id"] = i;
     }
 
-    var randomString = Math.floor(Math.random() * Date.now() * 10000).toString(
+    const randomString = Math.floor(Math.random() * Date.now() * 10000).toString(
         36
     );
-    var customHeight = 375;
-    var customWidth = 720;
-    if (element) {
-        element = document.getElementById(element)
-        customWidth = element.clientWidth;
-        customHeight = element.clientHeight;
-    } else {
-        element = that.el;
-    }
-    d3.select(element).selectAll("*").remove();
 
-    const margin = {
-        top: 20,
-        right: 20,
-        bottom: 30,
-        left: 40
-    };
-    const width = customWidth - margin.left - margin.right;
-    const height = customHeight - margin.top - margin.bottom;
+    d3.select(element).selectAll("*").remove();
 
-    var x = d3.scaleLinear().range([0, width]);
+    const x = d3.scaleLinear().range([0, innerWidth]);
 
-    var y = d3.scaleLinear().range([height, 0]);
+    const y = d3.scaleLinear().range([innerHeight, 0]);
 
-    var color = d3.scaleOrdinal(d3.schemeCategory10);
+    const color = d3.scaleOrdinal(d3.schemeCategory10);
 
-    var xAxis = d3.axisBottom(x);
+    const xAxis = d3.axisBottom(x);
 
-    var yAxis = d3.axisLeft(y);
+    const yAxis = d3.axisLeft(y);
 
     function mouseover(event, d) {
         focus.style("opacity", 1);
         focusText.style("opacity", 1);
         focus.attr("x", event.offsetX - 30).attr("y", event.offsetY - 40);
         focusText
             .html(
@@ -75,23 +64,23 @@
         const text =
             "x:" +
             Math.round(d[x_value] * 10) / 10 +
             "    " +
             "y:" +
             Math.round(d[y_value] * 10) / 10;
         if (setValue !== undefined) {
-            setValue(text, that);
+            setValue(text);
         }
     }
 
-    var svg = d3
+    const svg = d3
         .select(element)
         .append("svg")
-        .attr("width", width + margin.left + margin.right)
-        .attr("height", height + margin.top + margin.bottom)
+        .attr("width", width)
+        .attr("height", height)
         .append("g")
         .attr("transform", "translate(" + margin.left + "," + margin.top + ")");
 
     x.domain(
         d3.extent(data, function(d) {
             return d[x_value];
         })
@@ -101,19 +90,19 @@
             return d[y_value];
         })
     ).nice();
 
     svg
         .append("g")
         .attr("class", "x axis")
-        .attr("transform", "translate(0," + height + ")")
+        .attr("transform", "translate(0," + innerHeight + ")")
         .call(xAxis)
         .append("text")
         .attr("class", "label")
-        .attr("x", width)
+        .attr("x", innerWidth)
         .attr("y", -6)
         .style("text-anchor", "end");
 
     svg
         .append("g")
         .attr("class", "y axis")
         .call(yAxis)
@@ -155,15 +144,15 @@
             .style("fill", function(d) {
                 return color(d[hue]);
             });
     }
 
     function setLassoValues(values) {
         if (setSelectedValues !== undefined) {
-            setSelectedValues(values, that);
+            setSelectedValues(values);
         }
     }
 
     lasso(
         element,
         x,
         y,
@@ -172,34 +161,34 @@
         margin.left,
         margin.top,
         resetColor,
         setLassoValues,
         randomString
     );
 
-    var legend = svg
+    const legend = svg
         .selectAll(".legend")
         .data(color.domain())
         .enter()
         .append("g")
         .attr("class", "legend")
         .attr("transform", function(d, i) {
             return "translate(0," + i * 20 + ")";
         });
 
     legend
         .append("rect")
-        .attr("x", width - 18)
+        .attr("x", innerWidth - 18)
         .attr("width", 18)
         .attr("height", 18)
         .style("fill", color);
 
     legend
         .append("text")
-        .attr("x", width - 24)
+        .attr("x", innerWidth - 24)
         .attr("y", 9)
         .attr("dy", ".35em")
         .style("text-anchor", "end")
         .text(function(d) {
             return d;
         });
 
@@ -209,14 +198,14 @@
         .style("fill", "none")
         .attr("width", 160)
         .attr("height", 40)
         .attr("stroke", "#69b3a2")
         .attr("stroke-width", 4)
         .style("opacity", 0);
 
-    var focusText = svg
+    const focusText = svg
         .append("g")
         .append("text")
         .style("opacity", 0)
         .attr("text-anchor", "left")
         .attr("alignment-baseline", "middle");
 }
```

### Comparing `d3vis_ipynb-0.1.1/js/lib/tools/lasso.js` & `d3vis_ipynb-0.1.2/js/lib/tools/lasso.js`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/js/lib/wrappers/embedding.wrapper.js` & `d3vis_ipynb-0.1.2/js/lib/wrappers/embedding.wrapper.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -13,51 +13,51 @@
 import "../../css/widget.css";
 const data = require("./data.json");
 
 function plot_linearhistplot(
     linearData_x,
     linearData_y,
     histogramData,
-    element,
+    elementId,
     setValue
 ) {
     setTimeout(() => {
         linearhistplot(
             linearData_x,
             linearData_y,
             histogramData,
-            element,
+            elementId,
             setValue
         );
     }, 50);
 }
 
 function plot_scatterplot(
     data,
     x,
     y,
     hue,
-    element,
+    elementId,
     setValue,
     setSelectedValues
 ) {
     setTimeout(() => {
-        scatterplot(data, x, y, hue, element, setValue, setSelectedValues);
+        scatterplot(data, x, y, hue, elementId, setValue, setSelectedValues);
     }, 50);
 }
 
-function plot_barplot(data, x, y, hue, element) {
+function plot_barplot(data, x, y, hue, elementId) {
     setTimeout(() => {
-        barplot(data, x, y, hue, element);
+        barplot(data, x, y, hue, elementId);
     }, 50);
 }
 
-function plot_histogramplot(data, x, start, end, element) {
+function plot_histogramplot(data, x, start, end, elementId) {
     setTimeout(() => {
-        histogramplot(data, x, start, end, element);
+        histogramplot(data, x, start, end, elementId);
     }, 50);
 }
 
 function main() {
     const node = document.createElement("div");
 
     const matrix = data.matrix;
@@ -127,83 +127,83 @@
     }
 
     let plot_linearhistplot_data = () =>
         plot_linearhistplot(
             linearhistplot_data.linearData_x,
             linearhistplot_data.linearData_y,
             linearhistplot_data.histogramData,
-            linearhistplot_data.element,
+            linearhistplot_data.elementId,
             linearhistplot_data.setValue
         );
     let plot_scatterplot_data = () =>
         plot_scatterplot(
             scatterplot_data.data,
             scatterplot_data.x,
             scatterplot_data.y,
             scatterplot_data.hue,
-            scatterplot_data.element,
+            scatterplot_data.elementId,
             scatterplot_data.setValue,
             scatterplot_data.setSelectedValues
         );
     let plot_barplot_data = () =>
         plot_barplot(
             barplot_data.data,
             barplot_data.x,
             barplot_data.y,
             barplot_data.hue,
-            barplot_data.element
+            barplot_data.elementId
         );
     let plot_histogramplot_data = () =>
         plot_histogramplot(
             histogramplot_data.data,
             histogramplot_data.x,
             histogramplot_data.start,
             histogramplot_data.end,
-            histogramplot_data.element
+            histogramplot_data.elementId
         );
 
     const widgets = data.widgets;
 
     if (widgets["linearhistplot"]) {
         const widget_data = widgets["linearhistplot"];
         linearhistplot_data.linearData_x = widget_data.linearData_x;
         linearhistplot_data.linearData_y = widget_data.linearData_y;
         linearhistplot_data.histogramData = widget_data.histogramData;
-        linearhistplot_data.element = widget_data.element;
+        linearhistplot_data.elementId = widget_data.elementId;
         linearhistplot_data.observing = widget_data.observing;
         linearhistplot_data.plot = plot_linearhistplot_data;
     }
     if (widgets["scatterplot"]) {
         const widget_data = widgets["scatterplot"];
         scatterplot_data.data = widget_data.data;
         scatterplot_data.x = widget_data.x;
         scatterplot_data.y = widget_data.y;
         scatterplot_data.hue = widget_data.hue;
-        scatterplot_data.element = widget_data.element;
+        scatterplot_data.elementId = widget_data.elementId;
         scatterplot_data.observing = widget_data.observing;
         scatterplot_data.plot = plot_scatterplot_data;
     }
     if (widgets["barplot"]) {
         const widget_data = widgets["barplot"];
         barplot_data.data = widget_data.data;
         barplot_data.x = widget_data.x;
         barplot_data.y = widget_data.y;
         barplot_data.hue = widget_data.hue;
-        barplot_data.element = widget_data.element;
+        barplot_data.elementId = widget_data.elementId;
         barplot_data.observing = widget_data.observing;
         barplot_data.plot = plot_barplot_data;
         check_for_observers(barplot_data);
     }
     if (widgets["histogramplot"]) {
         const widget_data = widgets["histogramplot"];
         histogramplot_data.data = widget_data.data;
         histogramplot_data.x = widget_data.x;
         histogramplot_data.y = widget_data.start;
         histogramplot_data.hue = widget_data.end;
-        histogramplot_data.element = widget_data.element;
+        histogramplot_data.elementId = widget_data.elementId;
         histogramplot_data.observing = widget_data.observing;
         histogramplot_data.plot = plot_histogramplot_data;
     }
     linearhistplot_data.plot();
     scatterplot_data.plot();
     barplot_data.plot();
     histogramplot_data.plot();
```

### Comparing `d3vis_ipynb-0.1.1/LICENSE.txt` & `d3vis_ipynb-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/README.md` & `d3vis_ipynb-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `d3vis_ipynb-0.1.1/pyproject.toml` & `d3vis_ipynb-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ipywidgets>=7.7.1",
     "simplejson >=3.19.0",
     "anywidget >= 0.9.6"
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -77,14 +77,15 @@
 "d3vis_ipynb/labextension" = "share/jupyter/labextensions/d3vis_ipynb"
 "./install.json" = "share/jupyter/labextensions/d3vis_ipynb/install.json"
 "./d3vis_ipynb.json" = "etc/jupyter/nbconfig/notebook.d/d3vis_ipynb.json"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     ".github",
+    "samples",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
     "d3vis_ipynb/nbextension/index.js",
     "d3vis_ipynb/labextension/package.json",
```

### Comparing `d3vis_ipynb-0.1.1/PKG-INFO` & `d3vis_ipynb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: d3vis_ipynb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Custom Jupyter Widget Library with visualizations created with D3.js.
 Project-URL: Homepage, https://github.com/H-IAAC/d3vis_ipynb
 Author-email: Daniel Adam Miranda <daniel.miranda@eldorado.org.br>
 License: Copyright (c) 2024 Daniel Adam Miranda
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

