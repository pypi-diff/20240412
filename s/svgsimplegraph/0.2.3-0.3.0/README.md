# Comparing `tmp/svgsimplegraph-0.2.3.tar.gz` & `tmp/svgsimplegraph-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgsimplegraph-0.2.3.tar", last modified: Mon Apr  8 19:58:32 2024, max compression
+gzip compressed data, was "svgsimplegraph-0.3.0.tar", last modified: Fri Apr 12 18:59:47 2024, max compression
```

## Comparing `svgsimplegraph-0.2.3.tar` & `svgsimplegraph-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.886684 svgsimplegraph-0.2.3/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.3/LICENSE
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-08 19:58:32.886436 svgsimplegraph-0.2.3/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.2.3/README.md
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-08 19:58:32.886757 svgsimplegraph-0.2.3/setup.cfg
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      936 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/setup.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.881829 svgsimplegraph-0.2.3/svgsimplegraph/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/svgsimplegraph/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/base.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    42429 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/svgsimplegraph/categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.2.3/svgsimplegraph/ribbon.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10543 2024-04-08 19:58:23.000000 svgsimplegraph-0.2.3/svgsimplegraph/utils.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.882947 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      487 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/SOURCES.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/dependency_links.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-08 19:58:32.000000 svgsimplegraph-0.2.3/svgsimplegraph.egg-info/top_level.txt
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-08 19:58:32.885826 svgsimplegraph-0.2.3/tests/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.2.3/tests/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7535 2024-04-05 23:32:24.000000 svgsimplegraph-0.2.3/tests/test_categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_gist.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.2.3/tests/test_readme_examples.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.2.3/tests/test_ribbon.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.793273 svgsimplegraph-0.3.0/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.3.0/LICENSE
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-12 18:59:47.792978 svgsimplegraph-0.3.0/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.3.0/README.md
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-12 18:59:47.793361 svgsimplegraph-0.3.0/setup.cfg
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      936 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/setup.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.788014 svgsimplegraph-0.3.0/svgsimplegraph/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/svgsimplegraph/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/base.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    45924 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/svgsimplegraph/categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/ribbon.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10543 2024-04-08 19:58:23.000000 svgsimplegraph-0.3.0/svgsimplegraph/utils.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.789463 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      487 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/top_level.txt
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.792235 svgsimplegraph-0.3.0/tests/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.3.0/tests/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     8165 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/tests/test_categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_gist.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.3.0/tests/test_readme_examples.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_ribbon.py
```

### Comparing `svgsimplegraph-0.2.3/LICENSE` & `svgsimplegraph-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/PKG-INFO` & `svgsimplegraph-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.3
+Version: 0.3.0
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.3/README.md` & `svgsimplegraph-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/setup.py` & `svgsimplegraph-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read in the README.md for the long description on PyPI
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = "0.2.3"
+VERSION = "0.3.0"
 DESCRIPTION = "Simple SVG graphing package"
 
 setup(
     name="svgsimplegraph",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
```

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph/base.py` & `svgsimplegraph-0.3.0/svgsimplegraph/base.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph/bubble_and_arrow.py` & `svgsimplegraph-0.3.0/svgsimplegraph/bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph/categorical.py` & `svgsimplegraph-0.3.0/svgsimplegraph/categorical.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,14 +133,15 @@
         secondary_scale_max=None,
         secondary_scale_min=None,
         primary_tick_prefix="",
         primary_tick_suffix="",
         secondary_tick_prefix="",
         secondary_tick_suffix="",
         legend_position="right",
+        line_curvature=0,
     ):
         super().__init__(
             width=width,
             height=height,
             padding=padding,
             x_padding=x_padding,
             y_padding=y_padding,
@@ -170,32 +171,39 @@
         self.secondary_scale_max = secondary_scale_max
         self.secondary_scale_min = secondary_scale_min
         self.primary_tick_prefix = primary_tick_prefix
         self.primary_tick_suffix = primary_tick_suffix
         self.secondary_tick_prefix = secondary_tick_prefix
         self.secondary_tick_suffix = secondary_tick_suffix
         self.legend_position = legend_position
+        assert (
+            line_curvature >= 0 and line_curvature <= 0.5
+        ), f"Invalid line_curvature value: {line_curvature}. Must be between 0 and 0.5."
+        self.line_curvature = line_curvature
         self.x_labels = []
         self.series_types = []
         self.secondary = []
         self.horizontal_lines = []
         self.vertical_lines = []
+        self.stroke_width = []
 
     def add_series(
         self,
         series,
         legend_label=None,
         series_type="bar",
         print_values=False,
         secondary=False,
+        stroke_width=1,
     ):
         self.data.append(series)
         self.legend_labels.append(legend_label or None)
         self.series_types.append((series_type, print_values))
         self.secondary.append(secondary)
+        self.stroke_width.append(stroke_width)
 
     def add_horizontal_line(
         self,
         y,
         color=None,
         label=None,
         label_x_position="right",
@@ -289,16 +297,86 @@
             self.most_extreme_dimensions["top"], y1, y2
         )
         self.most_extreme_dimensions["bottom"] = max(
             self.most_extreme_dimensions["bottom"], y1, y2
         )
         return f'<line x1="{x1}" y1="{y1}" x2="{x2}" y2="{y2}" stroke="{stroke}" stroke-width="{stroke_width}" />'
 
+    def _draw_path(self, points, stroke="black", stroke_width=1, curvature=0):
+        path_data = ""
+        current_path = []
+
+        def append_current_path():
+            nonlocal path_data, current_path
+            if not current_path:
+                return
+
+            path_data += f" M {current_path[0][0]} {current_path[0][1]}"
+            if len(current_path) == 1:
+                return  # Only one point, nothing more to draw
+
+            if curvature == 0:
+                # Draw straight lines between points
+                for i in range(1, len(current_path)):
+                    p1 = current_path[i]
+                    path_data += f" L {p1[0]} {p1[1]}"
+            else:
+                for i in range(1, len(current_path)):
+                    p0 = current_path[i - 1]
+                    p1 = current_path[i]
+
+                    if i < len(current_path) - 1:
+                        p2 = current_path[i + 1]
+                        is_valley = p0[1] <= p1[1] >= p2[1]
+                        is_peak = p0[1] >= p1[1] <= p2[1]
+
+                        if is_valley or is_peak:
+                            # Handle peaks and valleys with a flatter approach
+                            ctrl1_x = p0[0] + (p1[0] - p0[0]) * curvature
+                            ctrl1_y = p1[1]  # Keep Y same to prevent overshoot
+                            ctrl2_x = p1[0] - (p2[0] - p1[0]) * curvature
+                            ctrl2_y = p1[1]  # Keep Y same to prevent overshoot
+                        else:
+                            # Adapt curvature based on the slope and overall direction
+                            delta_x1 = p1[0] - p0[0]
+                            delta_y1 = p1[1] - p0[1]
+                            delta_x2 = p2[0] - p1[0]
+                            delta_y2 = p2[1] - p1[1]
+                            ctrl1_x = p0[0] + delta_x1 * curvature
+                            ctrl1_y = p0[1] + delta_y1 * curvature
+                            ctrl2_x = p1[0] - delta_x2 * curvature
+                            ctrl2_y = p1[1] - delta_y2 * curvature
+                    else:
+                        # Last point, use the slope from the previous points
+                        delta_x = p1[0] - p0[0]
+                        delta_y = p1[1] - p0[1]
+                        ctrl1_x = p0[0] + delta_x * curvature
+                        ctrl1_y = p0[1] + delta_y * curvature
+                        ctrl2_x = p1[0] + delta_x * curvature
+                        ctrl2_y = p1[1] + delta_y * curvature
+
+                    if i == 1:
+                        path_data += f" C {ctrl1_x} {ctrl1_y} {ctrl2_x} {ctrl2_y} {p1[0]} {p1[1]}"
+                    else:
+                        path_data += f" S {ctrl2_x} {ctrl2_y} {p1[0]} {p1[1]}"
+
+            current_path = []
+
+        for point in points:
+            if point is None:
+                append_current_path()
+            else:
+                current_path.append(point)
+
+        append_current_path()
+        return f'<path d="{path_data}" stroke="{stroke}" stroke-width="{stroke_width}" fill="none"/>'
+
     def render(self):
         self._reset_graph()
+        self.paths = {}
         graph_width = self.width
         has_secondary = any(self.secondary)
         max_value_secondary = None
         min_value_secondary = None
         if self.stacked:
             bar_series_indices = [
                 i for i, series in enumerate(self.series_types) if series[0] == "bar"
@@ -399,21 +477,26 @@
         negative_bar_heights = [0] * num_categories
 
         for sub_index in range(num_categories):
             bar_count = 0
             for index in range(num_series):
                 value = self.data[index][sub_index]
 
-                if value is None:
-                    continue
-
                 secondary_value = self.secondary[index]
 
                 series_type, print_values = self.series_types[index]
 
+                if value is None:
+                    if series_type == "line":
+                        if index not in self.paths:
+                            self.paths[index] = []
+                        self.paths[index].append(None)
+
+                    continue
+
                 if series_type == "dot" or series_type == "line" or self.stacked:
                     x = (0.5 + sub_index) * bar_spacing + (bar_spacing - bar_width) / 2
                 else:
                     # Calculate the starting x-position of the bars in each category
                     start_x = (0.5 + sub_index) * bar_spacing + (
                         bar_spacing - total_bars_width
                     ) / 2
@@ -461,30 +544,18 @@
                         self._draw_dot(
                             center_x,
                             y,
                             radius=5,
                             fill=self.colors[index],
                         )
                     )
-                elif series_type == "line" and sub_index > 0:
-                    last_data_point = self.data[index][sub_index - 1]
-                    if last_data_point is not None:
-                        prev_y = self.height - (last_data_point - min_value) * scale
-                        prev_x = (sub_index - 0.5) * bar_spacing + (
-                            bar_spacing - bar_width
-                        ) / 2
-                        self.svg_elements.append(
-                            self._draw_line(
-                                prev_x,
-                                prev_y,
-                                x,
-                                y,
-                                stroke=self.colors[index],
-                            )
-                        )
+                elif series_type == "line":
+                    if index not in self.paths:
+                        self.paths[index] = []
+                    self.paths[index].append((x, y))
 
                 if print_values:
                     if series_type == "dot":
                         value_x = center_x
                     elif series_type == "line":
                         value_x = x
                     else:
@@ -493,14 +564,25 @@
                     value_y = y - 5 if series_type == "bar" else y - 10
                     self.svg_elements.append(
                         self._generate_text(
                             value, value_x, value_y, fill=self.text_color
                         )
                     )
 
+        # Draw paths
+        for index, points in self.paths.items():
+            self.svg_elements.append(
+                self._draw_path(
+                    points,
+                    stroke=self.colors[index],
+                    curvature=self.line_curvature,
+                    stroke_width=self.stroke_width[index],
+                )
+            )
+
         # Draw horizontal lines
         for (
             y,
             color,
             stroke_width,
             label,
             label_x_position,
@@ -786,14 +868,15 @@
                             self.svg_elements.append(
                                 self._draw_line(
                                     legend_x,
                                     legend_y + legend_rect_size / 2,
                                     legend_x + legend_rect_size,
                                     legend_y + legend_rect_size / 2,
                                     stroke=self.colors[index],
+                                    stroke_width=self.stroke_width[index],
                                 )
                             )
                         else:  # series_type == "bar"
                             self.svg_elements.append(
                                 f'<rect x="{legend_x}" y="{legend_y}" width="{legend_rect_size}" '
                                 + f'height="{legend_rect_size}" fill="{self.colors[index]}" />'
                             )
@@ -1008,15 +1091,15 @@
                                 legend_x + legend_rect_size + self.element_spacing / 2,
                                 legend_y + (2 / 3) * legend_rect_size,
                                 fill=self.text_color,
                                 anchor="start",
                             )
                         )
                         legend_x += (
-                            (2 * self.element_spacing) / 3
+                            self.element_spacing
                             + legend_rect_size
                             + estimate_text_dimensions(
                                 label, 10, self.font_width_estimate_multiplier
                             )[0]
                         )
 
                         next_index_with_label = index + 1
```

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph/ribbon.py` & `svgsimplegraph-0.3.0/svgsimplegraph/ribbon.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph/utils.py` & `svgsimplegraph-0.3.0/svgsimplegraph/utils.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/svgsimplegraph.egg-info/PKG-INFO` & `svgsimplegraph-0.3.0/svgsimplegraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svgsimplegraph
-Version: 0.2.3
+Version: 0.3.0
 Summary: Simple SVG graphing package
 Author: Garrett M. Petersen
 Author-email: garrett.m.petersen@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
 Keywords: graph,svg,base64,svg simple graph
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `svgsimplegraph-0.2.3/tests/test_bubble_and_arrow.py` & `svgsimplegraph-0.3.0/tests/test_bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/tests/test_categorical.py` & `svgsimplegraph-0.3.0/tests/test_categorical.py`

 * *Files 8% similar despite different names*

```diff
@@ -201,42 +201,61 @@
     # New graph with a very long series
     graph = CategoricalGraph(
         width=600,
         height=400,
         bar_width=30,
         title="Categorical Graph",
         primary_tick_prefix="$",
+        line_curvature=0.5,
     )
 
     number_of_bars = 100
 
     graph.x_labels = [f"Label {i}" for i in range(number_of_bars)]
     graph.x_axis_label = "X Axis"
     graph.primary_y_axis_label = "Primary Y Axis"
     graph.secondary_y_axis_label = "Secondary Y Axis"
 
     graph.add_series([abs(i - number_of_bars // 2) for i in range(number_of_bars)])
+    graph.add_series(
+        [(i**2) % number_of_bars for i in range(number_of_bars)], series_type="line"
+    )
 
     large_base64 = graph.to_base64_src()
     print(f"\n<img src='{large_base64}' />")
 
     # New graph with stacked primary and line secondary
     graph = CategoricalGraph(
         width=600,
         height=400,
         bar_width=30,
         title="Categorical Graph",
         secondary_tick_suffix="%",
         stacked=True,
+        line_curvature=0.5,
+        legend_position="top",
     )
 
     graph.x_labels = [f"Label {i}" for i in range(5)]
     graph.x_axis_label = "X Axis"
     graph.primary_y_axis_label = "Primary Y Axis"
     graph.secondary_y_axis_label = "Secondary Y Axis"
 
-    graph.add_series([1, 2, 3, 4, 5])
-    graph.add_series([50, 40, 30, 20, 10], series_type="line", secondary=True)
-    graph.add_series([3, 4, 3, 2, 1])
+    graph.add_series([1, 2, 3, 4, 5, 1, 1, 1, 5, 6, 7, 8], legend_label="Primary Bar")
+    graph.add_series(
+        [50, 10, 35, 25, 10, 5, 30, 5, 10, 15, 20, 25],
+        series_type="line",
+        secondary=True,
+        stroke_width=2,
+        legend_label="Secondary Line",
+    )
+    graph.add_series(
+        [50, None, 35, 25, 10, 5, None, None, 10, 15, None, 25],
+        series_type="line",
+        secondary=True,
+        stroke_width=2,
+        legend_label="Secondary Line 2",
+    )
+    graph.add_series([3, 4, 3, 2, 1, 1, 3, 4, 1, 2, 1, 3], legend_label="Primary Bar 2")
 
     stacked_base64 = graph.to_base64_src()
     print(f"\n<img src='{stacked_base64}' />")
```

### Comparing `svgsimplegraph-0.2.3/tests/test_gist.py` & `svgsimplegraph-0.3.0/tests/test_gist.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/tests/test_readme_examples.py` & `svgsimplegraph-0.3.0/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.2.3/tests/test_ribbon.py` & `svgsimplegraph-0.3.0/tests/test_ribbon.py`

 * *Files identical despite different names*

