# Comparing `tmp/nnsom-1.5.7.tar.gz` & `tmp/nnsom-1.5.8.tar.gz`

## Comparing `nnsom-1.5.7.tar` & `nnsom-1.5.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    80383 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/plots.py
--rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/som.py
--rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.7/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.7/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.7/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.7/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0    77247 2020-02-02 00:00:00.000000 nnsom-1.5.8/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    18019 2020-02-02 00:00:00.000000 nnsom-1.5.8/src/NNSOM/som.py
+-rw-r--r--   0        0        0    19295 2020-02-02 00:00:00.000000 nnsom-1.5.8/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.5.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.5.8/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.5.8/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.5.8/PKG-INFO
```

### Comparing `nnsom-1.5.7/src/NNSOM/plots.py` & `nnsom-1.5.8/src/NNSOM/plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from matplotlib.widgets import Button
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.colors as mcolors
+
 class SOMPlots(SOM):
     """
     SOMPlots extends the SOM class by adding visualization capabilities to
     the Self-Organizing Map (SOM). It allows for the graphical representation
     of the SOM's structure, the distribution of input data across its neurons,
     and various other analytical visualizations that aid in the interpretation
     of the SOM's behavior and characteristics.
@@ -238,14 +239,15 @@
                 temp = plt.text(pos[0, i], pos[1, i], '9', horizontalalignment='center', verticalalignment='center', color='w')
                 temp._fontproperties._weight = 'bold'
                 temp._fontproperties._size = 12.0
                 text.append(temp)
 
         # Compute the SOM outputs for the data set
         if self.sim_flag:
+            x = self.normalize(x, self.norm_func)
             outputs = self.sim_som(x)
             outputs = outputs
             self.sim_flag = False
         else:
             outputs = self.outputs
 
         # Find out how many inputs fall into each cluster
@@ -278,24 +280,24 @@
 
     def gray_hist(self, x, perc, mouse_click=False, **kwargs):
         # Make another hit histogram figure, and change the colors of the hexagons
         # to indicate the perc of pdb (or gb) ligands in each cluster. Lighter color
         # means more PDB ligands, darker color means more well-docked bad binders.
 
         numNeurons = self.numNeurons
+        dmax = np.amax(np.abs(perc))    # Find the maximum value of perc across all clusters
 
         fig, ax, patches, text = self.hit_hist(x, False, mouse_click, **kwargs)
 
         # Scale the gray scale to the perc value
         for neuron in range(numNeurons):
-            scale = perc[neuron] / 100.0
-            color = [scale for i in range(3)]
-            color.append(1.0)
-            color = tuple(color)
-            patches[neuron][0]._facecolor = color
+            scale = perc[neuron] / dmax
+            color = [scale for i in range(3)]  # Create a gray color based on the scaled value
+            color.append(1.0)  # Add alpha value
+            patches[neuron][0]._facecolor = tuple(color)  # Apply the color to the patch
 
         # Get rid of extra white space on sides
         plt.tight_layout()
 
         return fig, ax, patches, text
 
     def color_hist(self, x, avg, mouse_click=False, **kwargs):
@@ -441,15 +443,15 @@
 
         # Check if the input data is a sequence of vectors
         if x.ndim != 2:
             raise ValueError("x must be a 2D array")
 
         # Check if the input data can be cdist with self.w
         # the input data must be transposed
-        if x.shape[0] != self.w.shape[1]:
+        if x.shape[1] != self.w.shape[1]:
             raise ValueError("The input data must have the same number of features as the SOM")
 
         # Check if the face color, line width and edge color are 1D arrays
         if face_labels.ndim != 1 or edge_width.ndim != 1 or edge_labels.ndim != 1:
             raise ValueError("fcolor, lwidth and ecolor must be 1D arrays")
 
         # Check if the length of fcolor, lwidth and ecolor are equal to the number of neurons
@@ -1217,33 +1219,36 @@
             kwargs['num2'] = y
             fig.canvas.mpl_connect(
                 'pick_event', lambda event: self.onpick(event, hexagons, hexagon_to_neuron, **kwargs)
             )
 
         return fig, ax, h_axes
 
-    def component_positions(self, X_scaled):
+    def component_positions(self, x):
         """
         Plots the SOM weight vectors, the Iris dataset input vectors, and connects neighboring neurons.
 
         Parameters:
         - som: A trained SOM instance with attributes 'w' for weight vectors and 'dimensions' for grid dimensions.
         - X_scaled: The normalized Iris dataset input vectors.
         """
+
+        x = np.transpose(x)
+
         # Extract the trained weight vectors and the SOM grid dimensions
         weight_vectors = self.w
         grid_x, grid_y = self.dimensions
 
         # Plot the SOM weight vectors as gray dots
         plt.scatter(weight_vectors[:, 0], weight_vectors[:, 1], color='gray', s=50, label='Weight Vectors')
         # for i, vec in enumerate(weight_vectors):
         #     plt.annotate(str(i), (vec[0], vec[1]), textcoords="offset points", xytext=(0,5), ha='center')
 
         # Plot the Iris data points as blue dots
-        plt.scatter(X_scaled[:, 0], X_scaled[:, 1], color='green', s=20, label='Input Vectors', alpha=0.5)
+        plt.scatter(x[:, 0], x[:, 1], color='green', s=20, label='Input Vectors', alpha=0.5)
 
         # Draw red lines to connect neighboring neurons
         for i in range(grid_x):
             for j in range(grid_y):
                 index = i * grid_y + j  # Calculate the linear index of the neuron in the SOM
                 neuron = weight_vectors[index]
 
@@ -1368,16 +1373,16 @@
         # Display the plot
         plt.show()
 
         # Return the figure components
         return fig, ax, patches
 
     # Generic Plot Function
-    def plot(self, plot_type, data_dict=None, ind=None, target_class=None, use_add_1darray=False,
-             use_add_2darray=False, **kwargs):
+    def plot(self, plot_type, data_dict=None, ind=None, target_class=None, use_add_array=False,
+             **kwargs):
         """ Generic Plot Function.
         It generates a plot based on the plot type and data provides.
 
         Parameters
         ----------
         plot_type : str
             The type of plot to be generated:
@@ -1386,29 +1391,25 @@
             "simple_grid", "stem", "pie", "wgts", "pie", "hist",
             "box", "violin", "scatter", "component_positions",
             "component_planes"]
 
         data_dict: dict (optional)
             A dictionary containing the data to be plotted.
             The key is prefixed with the data type and the value is the data itself.
-            {"original_data", "input_data", "target", "clust","cat_1darray", "cat_2darray",
-            "num_1darray"}
+            {"data", "target", "clust", "add_1d_array", "add_2d_array"}
 
         ind : int, str or array-like (optional)
             The indices of the data to be plotted.
 
         target_class: int (optional)
             The target class to be plotted.
 
-        use_add_1darray: bool (optional)
+        use_add_array: bool (optional)
             If true, the additional array to be used.
 
-        use_add_2darray: bool (optional)
-            If true, the additional 2D array to be used.
-
         **kwargs : dict
             Additional arguments to be passed to the interactive plot function.
         """
         # Plot Types allowed
         plot_types = ["top", "top_num",
                       "hit_hist", "gray_hist", "color_hist", "complex_hist",
                       "neuron_connection", "neuron_dist",
@@ -1459,318 +1460,263 @@
 
         # ======== Topology, Neuron Connection, Neuron Distance, and Weight Plot ==========
         if plot_type in ["top", "top_num", "neuron_connection", "neuron_dist", "wgts"]:
             # Call the plot function
             return selected_plot(**kwargs)
 
         # ======== Components Plane Family ==========
-        # Need to be modified
         elif plot_type in ['component_positions', 'component_planes']:
             # Error Handling if the data_dict have the scaled input data X
-            validate_data_dict(["input_data"])
+            validate_data_dict(["data"])
             # Data Preparation
-            x_scaled = data_dict['input_data']
+            x = data_dict['data']
+            x = self.normalize(x, self.norm_func)
             # Invoke Function
-            return selected_plot(x_scaled)
+            return selected_plot(x)
 
         # =====================  Hit Histogram Family =====================
         elif plot_type in ['hit_hist', 'gray_hist', 'color_hist', 'complex_hist']:
             # Validate the data_dict have the scaled input data
-            validate_data_dict(["input_data"])
+            validate_data_dict(["data"])
 
             # Extract input data
-            x = data_dict['input_data']
+            x = data_dict['data']
 
             if plot_type in ['hit_hist']:
                 # Invoke the function
                 return selected_plot(x, True, **kwargs)
 
             elif plot_type in ['gray_hist']:
-                if use_add_1darray:  # Check if user want to use additional 1D array
-
-                    # Validate the data_dict have the additional 1D array and original data
-                    validate_data_dict(["cat_1darray", "original_data"])
+                # Gray Hist with add_1d_array
+                if use_add_array:
+                    # Validate the data_dict have the additional 1D array
+                    validate_data_dict(["add_1d_array"])
 
-                    # Validate the length of additional 1D array is equal to number of neuron or length of original data.
-                    if len(data_dict['cat_1darray']) != self.numNeurons and len(data_dict['cat_1darray']) != len(
-                            data_dict['original_data']):
+                    if len(data_dict['add_1d_array']) != self.numNeurons:
                         raise ValueError(
                             "The additional 1D array must have the same length as the clust data or original data.")
 
-                    # If the length of additional 1D array is equal to the length of clust data just extract data
-                    elif len(data_dict['cat_1darray']) == self.numNeurons:
-                        perc = data_dict['cat_1darray']
-
-                    # If the length of additional 1D array is equal to the length of original data then preprocess the data
-                    elif len(data_dict['cat_1darray']) == len(data_dict['original_data']):
-
-                        # Validate the data_dict have the clust data
-                        validate_data_dict(["clust"])
-
-                        if target_class is None:
-                            raise ValueError("The target class is required. Eg. target_class = 1")
-
-                        # Preprocess and extract the data
-                        perc = get_perc_cluster(data_dict['cat_1darray'], target_class, data_dict['clust'])
+                    perc = data_dict['add_1d_array']
 
+                # Gray hist with data
                 else:
                     # Error Handling if the target data not provided
-                    validate_data_dict(["target", "clust"])
+                    validate_data_dict(["clust"])
+
+                    if target_class is None and ind is None:
+                        raise ValueError("This plot requires either the target class or ind.")
+
+                    elif target_class is not None and ind is not None:
+                        raise ValueError("This plot requires only either the target class or ind.")
 
-                    # Validate the data_dict have the clust data
-                    if target_class is None:
-                        raise ValueError("The target class is required. Eg. target_class = 1")
+                    elif target_class is not None:
+                        validate_data_dict(['target'])
+                        perc = get_perc_cluster(data_dict['target'], target_class, data_dict['clust'])
 
-                    perc = get_perc_cluster(data_dict['target'], target_class, data_dict['clust'])
+                    elif ind is not None:
+                        feature = x[:, ind]
+                        perc = get_cluster_avg(feature, data_dict['clust'])
 
                 # Invoke the gray hist function
                 return selected_plot(x, perc, **kwargs)
 
             elif plot_type in ['color_hist']:
-                # Check if user want to use additional 1D array
-                if use_add_1darray:
-                    # Check if the additional 1D array and original data are provided
-                    validate_data_dict(["num_1darray", "original_data"])
-
-                    num_feature = data_dict['num_1darray']
-                    original_data_size = len(data_dict['original_data'])
-
-                    if len(num_feature) != original_data_size and len(num_feature) != self.numNeurons:
-                        raise ValueError(
-                            "The additional 1D array must have the same length as the clust data or original data.")
+                # Color Hist with additional data
+                if use_add_array:
+                    validate_data_dict(['add_1d_array'])
 
-                    elif len(num_feature) == original_data_size:
-                        # Check if the clust data is provided
-                        validate_data_dict(["clust"])
-
-                        clust = data_dict['clust']
-                        avg = get_cluster_avg(num_feature, clust)
-
-                    elif len(num_feature) == self.numNeurons:
-
-                        avg = num_feature
+                    if len(data_dict['add_1d_array']) != self.numNeurons:
+                        raise ValueError("The additional 1D array must have the same length as the clust data or original data.")
 
+                    avg = data_dict['add_1d_array']
+                # Color Hist with input data
                 else:
-                    # Error Handling if the original data and clust are provided
-                    validate_data_dict(["original_data", "clust"])
+                    validate_data_dict(["clust"])
 
-                    if ind is None:
-                        raise ValueError(
-                            "The indices is required for this plot type. Which numerical feature in the original data you want to plot? Eg. ind = 0")
+                    if target_class is None and ind is None:
+                        raise ValueError("This plot requires either the target class or ind.")
 
-                    feature = data_dict['original_data'][:, ind]
+                    elif target_class is not None and ind is not None:
+                        raise ValueError("This plot requires only either the target class or ind.")
 
-                    avg = get_cluster_avg(feature, data_dict['clust'])
+                    elif target_class is not None:
+                        validate_data_dict(['target'])
+                        avg = get_perc_cluster(data_dict['target'], target_class, data_dict['clust'])
+
+                    elif ind is not None:
+                        feature = x[:, ind]
+                        avg = get_cluster_avg(feature, data_dict['clust'])
 
                 return selected_plot(x, avg, **kwargs)
 
             elif plot_type in ['complex_hist']:
-                if use_add_2darray:
+                if use_add_array:
                     # Validate the data_dict have the additional 2D array
-                    validate_data_dict(["cat_2darray"])
+                    validate_data_dict(["add_2d_array"])
 
-                    cat_2darray = data_dict['cat_2darray']
+                    add_2d_array = np.array(data_dict['add_2d_array'])
 
-                    if cat_2darray.shape[0] != self.numNeurons:
+                    if add_2d_array.shape[0] != self.numNeurons:
                         raise ValueError(
                             "The additional 2D array must have the same length as the number of neurons.")
 
-                    # Validate the additional 2D array have 3 features
-                    if cat_2darray.shape[1] != 3:
-                        raise ValueError(
-                            "The additional 2D array must have 3 features. E.g. [numNeurons, [face_labels, edge_labels, edge_widths]]")
+                    # Assuming add_2d_array is a list of lists
+                    if add_2d_array.shape[1] != 3:
+                        raise ValueError("Each inner list in the additional 2D array must have exactly 3 items. \
+                        E.g. [numNeurons, [face_labels, edge_labels, edge_widths[0-20]]")
 
                     # Extract Data
-                    face_labels = cat_2darray[:, 0]
-                    edge_labels = cat_2darray[:, 1]
-                    edge_widths = cat_2darray[:, 2]
+                    face_labels = add_2d_array[:, 0]
+                    edge_labels = add_2d_array[:, 1]
+                    edge_widths = add_2d_array[:, 2]
 
                 else:
-                    # Error Handling if the target and clust data not provided
-                    validate_data_dict(["target", "clust"])
-                    # Error Handling if the target class not provided
-                    if target_class is None:
-                        raise ValueError("The target class is required")
-
-                    # Generate Data
-                    target = data_dict['target']
-                    clust = data_dict['clust']
-
-                    face_labels = majority_class_cluster(target, clust)
-                    edge_labels = closest_class_cluster(target, clust)
-                    target_ind = np.where(target == target_class)[0]
-                    edge_widths = get_edge_widths(target_ind, clust)
+                    raise ValueError("This plot requires an additional 2-D array in data_dict. "
+                                     "The additional 2D array must have 3 features. "
+                                     "E.g. [numNeurons, [face_labels, edge_labels, edge_widths[0-20]]")
 
                 return selected_plot(x, face_labels, edge_labels, edge_widths, **kwargs)
 
         # ===================== Simple Grid =====================
         elif plot_type in ['simple_grid']:
             # Validate the data_dict have the original data
-            validate_data_dict(["original_data"])
+            validate_data_dict(["data"])
+            data = data_dict['data']
+            # Simple grid with addtional variable
+            if use_add_array:
+                # Error Handlig if the additional 2D arrays not privided
+                validate_data_dict(["add_2d_array"])
+                add_2d_array = np.asarray(data_dict["add_2d_array"], np.float32)
+                # Validate Length
+                if add_2d_array.shape[0] != self.numNeurons:
+                    raise ValueError("The additional 2D array must have the same length as the number of cluster")
+                # Validate number of items in each cluster
+                if add_2d_array.shpae[1] != 2:
+                    raise ValueError("Each cluster must have only 2 items in the additional 2D array")
 
-            original_data = data_dict['original_data']
-
-            # Check if there're additional variables
-            if use_add_1darray:
-                # Error Handling if the additional 1D arrays and clust not provided
-                validate_data_dict(["cat_1darray", "num_1darray", "clust"])
-
-                cat_feature = data_dict['cat_1darray']
-                num_feature = data_dict['num_1darray']
-                clust = data_dict['clust']
-
-                # ================================
-                # Extract avg from num_1darray
-                # potential input of num_1darray
-                # 1. the specific column of the original data
-                # 2. the pre-processes 1-d array with average value for each cluster
-                # ================================
-                # Validate the length of additional 1D array is equal to the number of neuron or length of original data.
-                if len(num_feature) != self.numNeurons and len(num_feature) != len(original_data):
-                    raise ValueError(
-                        "The additional 1D array must have the same length as the clust data or original data.")
-                elif len(num_feature) == self.numNeurons:
-                    avg = num_feature
-                elif len(num_feature) == len(original_data):
-                    avg = get_cluster_avg(num_feature, clust)
-
-                # ===============================
-                # Extract sizes from cat_1darray
-                # potential input of cat_1darray
-                # 1. The specific feature of the original data (e.g. the specific column) <- it'requres target class
-                # 2. The specific feature of the pre-processes 1-d array with magnitude for each cluster (e.g. percentage)
-                # ===============================
-                if len(cat_feature) != self.numNeurons and len(cat_feature) != len(original_data):
-                    raise ValueError(
-                        "The additional 1D array must have the same length as the clust data or original data.")
-
-                elif len(cat_feature) == self.numNeurons:
-                    sizes = cat_feature
-
-                elif len(cat_feature) == len(original_data):
-                    if target_class is None:
-                        raise ValueError("The target class is required")
-                    sizes = get_perc_cluster(cat_feature, target_class, clust)
+                avg = add_2d_array[:, 0]
+                sizes = add_2d_array[:, 1]
 
             else:
                 # Error Handling if the target and clust data not provided
                 validate_data_dict(["clust", "target"])
 
                 if ind is None:
                     raise ValueError("The indices is required for this plot type.")
 
                 if target_class is None:
                     raise ValueError("The target class is required")
 
                 clust = data_dict['clust']
 
                 # Extract avg from the original data
-                num_feature = original_data[:, ind]
+                num_feature = data[:, ind]
                 avg = get_cluster_avg(num_feature, clust)
 
                 # Extract size from the target
                 target = data_dict['target']
                 sizes = get_perc_cluster(target, target_class, clust)
 
             return selected_plot(avg, sizes, **kwargs)
 
         # ===================== Basic Plot Family =====================
         elif plot_type in ['stem', 'pie']:
-            # Error Handling if the clust data not provided
-            validate_data_dict(["target", "clust"])
-
-            # Extract Information
-            clust = data_dict['clust']
 
-            # If the user wanna plot input data
-            if use_add_2darray:
+            # If the user want to plot addtional data
+            if use_add_array:
                 # Error Handling if the additional 2D array not provided
-                validate_data_dict(["cat_2darray"])
+                validate_data_dict(["add_2d_array"])
 
                 # Error Handling if additional vategorical variable has correct length
-                if len(data_dict["cat_2darray"]) != len(clust):
+                if len(data_dict["add_2d_array"]) != self.numNeurons:
                     raise ValueError("The additional categorical data must have the same length as the clust data.")
 
                 #  Get Additional Data
-                sizes = data_dict['cat_2darray']
+                sizes = data_dict['add_2d_array']
 
             else:
+                # Error Handling if the clust data not provided
+                validate_data_dict(["target", "clust"])
+
+                # Extract Information
+                clust = data_dict['clust']
                 target = data_dict['target']
+
                 sizes = count_classes_in_cluster(target, clust)
 
             if plot_type == 'pie':
 
                 # =============================================
                 # It needs to handle scale (need to implement)
                 # =============================================
 
                 # Call the pie plot
                 return selected_plot(sizes, **kwargs)
 
             elif plot_type == 'stem':
                 # Extract Align
-                if use_add_2darray:
+                if use_add_array:
                     align = [i for i in range(sizes.shape[1])]
                 else:
                     align = [i for i in range(len(np.unique(target)))]
                 # Call the stem plot
                 return selected_plot(align, sizes, **kwargs)
 
         elif plot_type in ['hist']:
             # Error Handling if the index not provided
             if ind is None:
                 raise ValueError("The indices is required for this plot type.")
 
             # Error Handling if the original data not provided
-            validate_data_dict(["original_data", "clust"])
+            validate_data_dict(["data", "clust"])
 
             # Extract the feature from the original data
             clust = data_dict['clust']
-            feature = data_dict['original_data'][:, ind]
+            feature = data_dict['data'][:, ind]
 
             x = get_cluster_array(feature, clust)
 
             return selected_plot(x, **kwargs)
 
         elif plot_type in ['scatter']:
             # Error Handling if the index not provided
             if ind is None:
                 raise ValueError("The indices is required for this plot type.")
 
             if len(ind) != 2:
                 raise ValueError("The indices must contain exactly two elements. Eg. [0, 1]")
 
             # Error Handling if the original data and clust not provided
-            validate_data_dict(["original_data", "clust"])
+            validate_data_dict(["data", "clust"])
 
             # Extract the feature from the original data
-            x = data_dict['original_data'][:, ind[0]]
-            y = data_dict['original_data'][:, ind[1]]
+            x = data_dict['data'][:, ind[0]]
+            y = data_dict['data'][:, ind[1]]
             clust = data_dict['clust']
             x = get_cluster_array(x, clust)
             y = get_cluster_array(y, clust)
 
             # Call the scatter plot function
             return selected_plot(x, y, **kwargs)
 
         elif plot_type in ['box', 'violin']:
             # Error Handling if the original data not provided
-            validate_data_dict(["original_data", "clust"])
+            validate_data_dict(["data", "clust"])
 
             # Extract the feature from the original data
             clust = data_dict['clust']
 
             if ind is None:  # Extract All data
-                data = data_dict['original_data']
+                data = data_dict['data']
                 x = get_cluster_data(data, clust)
             elif isinstance(ind, int):  # index just have 1 index
-                data = data_dict['original_data'][:, ind]
+                data = data_dict['data'][:, ind]
                 x = get_cluster_array(data, clust)
             elif isinstance(ind, (list, np.ndarray)):  # index have multiple indices
-                data = data_dict['original_data'][:, ind]
+                data = data_dict['data'][:, ind]
                 x = get_cluster_data(data, clust)
 
             # Call the box plot and violin function
             return selected_plot(x, **kwargs)
 
     # Interactive Functionality
     def onpick(self, event, hexagons, hexagon_to_neuron, **kwargs):
```

### Comparing `nnsom-1.5.7/src/NNSOM/som.py` & `nnsom-1.5.8/src/NNSOM/som.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.7/src/NNSOM/utils.py` & `nnsom-1.5.8/src/NNSOM/utils.py`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.7/.gitignore` & `nnsom-1.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nnsom-1.5.7/pyproject.toml` & `nnsom-1.5.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.5.7"
+version = "1.5.8"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.5.7/PKG-INFO` & `nnsom-1.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.5.7
+Version: 1.5.8
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

