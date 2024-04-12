# Comparing `tmp/nnsom-1.5.6.tar.gz` & `tmp/nnsom-1.5.7.tar.gz`

## Comparing `nnsom-1.5.6.tar` & `nnsom-1.5.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    80117 2020-02-02 00:00:00.000000 nnsom-1.5.6/src/NNSOM/plots.py
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.6/src/NNSOM/som.py
--rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.6/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.6/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.6/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.6/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.6/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0    80383 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/som.py
+-rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.7/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.7/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.7/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.7/PKG-INFO
```

### Comparing `nnsom-1.5.6/src/NNSOM/plots.py` & `nnsom-1.5.7/src/NNSOM/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1159,32 +1159,14 @@
             kwargs['num1'] = x
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
-    def multiplot(self, plot_type, *args):
-        # Dictionary mapping plot types to corresponding plotting methods
-        plot_functions = {
-            'wgts' : self.plt_wgts,
-            'pie': self.plt_pie,
-            'stem': self.plt_stem,
-            'hist': self.plt_histogram,
-            'box': self.plt_boxplot,
-            'violin': self.plt_violin_plot,
-            'scatter': self.plt_scatter
-        }
-
-        selected_plot = plot_functions.get(plot_type)
-        if selected_plot:
-            return selected_plot(*args)
-        else:
-            raise ValueError("Invalid function type")
-
     def plt_scatter(self, x, y, reg_line=True, mouse_click=False, connect_pick_event=True, **kwargs):
         """ Generate Scatter Plot for Each Neuron.
 
         Args:
             x: input data
             indices: array-like indices e.g. (0, 1) or [0, 1]
             clust: list of indices of input data for each cluster
@@ -1195,24 +1177,42 @@
         """
         pos = self.pos
         numNeurons = self.numNeurons
 
         # Setup figure, main axes, and sub-axes
         fig, ax, h_axes, hexagons, hexagon_to_neuron = self.setup_axes()
 
+        # Determine the global minimum and maximum of x and y for the axes limits
+        x_min, x_max = get_global_min_max(x)
+        y_min, y_max = get_global_min_max(y)
+
         # Loop over each neuron for hexagons and scatter plots
         for neuron in range(numNeurons):
             # Make Scatter Plot for each neuron
             if len(x[neuron]) > 0 and len(y[neuron]) > 0:
                 h_axes[neuron].scatter(x[neuron], y[neuron], s=1, c='k')
 
                 if reg_line:
                     m, p = np.polyfit(x[neuron], y[neuron], 1)
                     h_axes[neuron].plot(x[neuron], m * x[neuron] + p, c='r', linewidth=1)
 
+                # Set the same x and y limits for each sub-plot based on global min and max
+                h_axes[neuron].set_xlim(x_min, x_max)
+                h_axes[neuron].set_ylim(y_min, y_max)
+
+                # Show only the left and bottom spines
+                h_axes[neuron].spines['top'].set_visible(False)
+                h_axes[neuron].spines['right'].set_visible(False)
+                h_axes[neuron].spines['left'].set_visible(True)
+                h_axes[neuron].spines['bottom'].set_visible(True)
+
+                # Enable the axes and show tick marks
+                h_axes[neuron].set_frame_on(True)
+                h_axes[neuron].tick_params(axis='both', which='both', length=5)
+
             else:
                 h_axes[neuron] = None
 
         if mouse_click and connect_pick_event:
             kwargs['num1'] = x
             kwargs['num2'] = y
             fig.canvas.mpl_connect(
```

### Comparing `nnsom-1.5.6/src/NNSOM/som.py` & `nnsom-1.5.7/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.6/src/NNSOM/utils.py` & `nnsom-1.5.7/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.6/.gitignore` & `nnsom-1.5.7/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.6/pyproject.toml` & `nnsom-1.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.6"
+version = "1.5.7"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.6/PKG-INFO` & `nnsom-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.6
+Version: 1.5.7
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

