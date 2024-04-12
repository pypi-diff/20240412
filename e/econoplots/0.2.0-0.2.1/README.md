# Comparing `tmp/econoplots-0.2.0.tar.gz` & `tmp/econoplots-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econoplots-0.2.0.tar", last modified: Wed Jul  5 16:11:26 2023, max compression
+gzip compressed data, was "/home/dylanrpenn/econoplots/dist/.tmp-k3jn9ig4/econoplots-0.2.1.tar", last modified: Fri Apr 12 17:17:28 2024, max compression
```

## Comparing `econoplots-0.2.0.tar` & `econoplots-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-05-19 14:19:37.000000 econoplots-0.2.0/LICENSE
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-07-05 16:11:26.770766 econoplots-0.2.0/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-05-19 14:40:50.000000 econoplots-0.2.0/README.md
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/econoplots/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2023-07-05 16:10:26.000000 econoplots-0.2.0/econoplots/__init__.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4963 2023-06-28 15:16:29.000000 econoplots-0.2.0/econoplots/_standalone_plotters.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3513 2023-06-28 17:44:48.000000 econoplots-0.2.0/econoplots/color_map.json
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3193 2023-06-28 17:44:29.000000 econoplots-0.2.0/econoplots/colors.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4731 2023-07-05 16:09:24.000000 econoplots-0.2.0/econoplots/converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1067 2023-06-20 19:01:06.000000 econoplots-0.2.0/econoplots/params.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    24011 2023-06-28 18:09:46.000000 econoplots-0.2.0/econoplots/utils.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/econoplots.egg-info/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2473 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/PKG-INFO
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      457 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/SOURCES.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/dependency_links.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2023-05-10 17:37:10.000000 econoplots-0.2.0/econoplots.egg-info/not-zip-safe
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/requires.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2023-07-05 16:11:26.000000 econoplots-0.2.0/econoplots.egg-info/top_level.txt
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-05-31 20:11:16.000000 econoplots-0.2.0/pyproject.toml
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2023-07-05 16:11:26.770766 econoplots-0.2.0/setup.cfg
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-05-10 17:07:57.000000 econoplots-0.2.0/setup.py
-drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2023-07-05 16:11:26.770766 econoplots-0.2.0/tests/
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2216 2023-06-28 17:21:08.000000 econoplots-0.2.0/tests/test_converter.py
--rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-05-18 20:49:32.000000 econoplots-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2024-04-12 17:17:28.420734 econoplots-0.2.1/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1053 2023-06-02 00:38:13.000000 econoplots-0.2.1/LICENSE
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2558 2024-04-12 17:17:28.420734 econoplots-0.2.1/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      799 2023-06-02 00:38:13.000000 econoplots-0.2.1/README.md
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2024-04-12 17:17:28.420734 econoplots-0.2.1/econoplots/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       22 2024-04-12 17:13:44.000000 econoplots-0.2.1/econoplots/__init__.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     4963 2023-07-31 18:56:42.000000 econoplots-0.2.1/econoplots/_standalone_plotters.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     3643 2023-07-31 18:56:42.000000 econoplots-0.2.1/econoplots/colors.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     5515 2024-04-10 17:34:28.000000 econoplots-0.2.1/econoplots/converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1258 2024-03-27 19:34:23.000000 econoplots-0.2.1/econoplots/params.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)    24483 2024-04-05 13:34:19.000000 econoplots-0.2.1/econoplots/utils.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2024-04-12 17:17:28.420734 econoplots-0.2.1/econoplots.egg-info/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2558 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/PKG-INFO
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      431 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/SOURCES.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/dependency_links.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)        1 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/not-zip-safe
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       40 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/requires.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       11 2024-04-12 17:17:28.000000 econoplots-0.2.1/econoplots.egg-info/top_level.txt
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     1336 2023-06-02 00:38:13.000000 econoplots-0.2.1/pyproject.toml
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       38 2024-04-12 17:17:28.420734 econoplots-0.2.1/setup.cfg
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)       60 2023-01-23 21:23:28.000000 econoplots-0.2.1/setup.py
+drwxr-xr-x   0 dylanrpenn  (1000) dylanrpenn  (1000)        0 2024-04-12 17:17:28.420734 econoplots-0.2.1/tests/
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)     2249 2024-03-18 13:40:00.000000 econoplots-0.2.1/tests/test_converter.py
+-rw-r--r--   0 dylanrpenn  (1000) dylanrpenn  (1000)      734 2023-06-02 00:38:13.000000 econoplots-0.2.1/tests/test_utils.py
```

### Comparing `econoplots-0.2.0/LICENSE` & `econoplots-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `econoplots-0.2.0/PKG-INFO` & `econoplots-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.2.0
+Version: 0.2.1
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -26,14 +26,17 @@
 Project-URL: Homepage, https://github.com/dylan906/econoplots
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.20
+Requires-Dist: matplotlib>=3.5
+Requires-Dist: black>=23.3
 
 # Description
 This project helps create Matplotlib plots in the style of *The Economist*. Only some plot styles are supported (line plots are the only style that works right now) and there are some stylistic differences from *The Economist* for the sake of convenience/laziness. 
 
 # Users Guide
 - Install fonts (see below) before using any functions.
 - The main function you will use is `converter.convert2Econo()`, which takes a Matplotlib `Axes` and returns and `Axes` that is formatted nicely.
```

### Comparing `econoplots-0.2.0/README.md` & `econoplots-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `econoplots-0.2.0/econoplots/_standalone_plotters.py` & `econoplots-0.2.1/econoplots/_standalone_plotters.py`

 * *Files identical despite different names*

### Comparing `econoplots-0.2.0/econoplots/colors.py` & `econoplots-0.2.1/econoplots/colors.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,34 +26,52 @@
     "red6": "#FFA39F",
     "blue1": "#00588D",
     "blue2": "#1270A8",
     "blue3": "#3D89C3",
     "blue4": "#5DA4DF",
     "blue5": "#7BBFFC",
     "blue6": "#98DAFF",
+    "cyan1": "#005F73",
+    "cyan2": "#00788D",
+    "cyan3": "#0092A7",
+    "cyan4": "#25ADC2",
+    "cyan5": "#4EC8DE",
+    "cyan6": "#6FE4FB",
     "green1": "#005F52",
     "green2": "#00786B",
     "green3": "#2E9284",
     "green4": "#4DAD9E",
     "green5": "#69C9B9",
     "green6": "#86E5D4",
+    "yellow1": "#714C00",
+    "yellow2": "#8D6300",
+    "yellow3": "#AA7C00",
+    "yellow4": "#C89608",
+    "yellow5": "#E7B030",
+    "yellow6": "#FFCB4D",
+    "olive1": "#4C5900",
+    "olive2": "#667100",
+    "olive3": "#818A00",
+    "olive4": "#9DA521",
+    "olive5": "#BAC03F",
+    "olive6": "#D7DB5A",
     "purple1": "#78405F",
     "purple2": "#925977",
     "purple3": "#AD7291",
     "purple4": "#C98CAC",
     "purple5": "#E6A6C7",
     "purple6": "#FFC2E3",
     "gold1": "#674E1F",
     "gold2": "#826636",
     "gold3": "#9D7F4E",
     "gold4": "#B99966",
     "gold5": "#D5B480",
     "gold6": "#F2CF9A",
-    "grey1": "#758D99",
-    "grey2": "#3F5661",
+    "grey1": "#3F5661",
+    "grey2": "#576E79",
     "grey3": "#6F8793",
     "grey4": "#89A2AE",
     "grey5": "#A4BDC9",
     "grey6": "#BFD8E5",
 }
 
 colors_print_dict = {
```

### Comparing `econoplots-0.2.0/econoplots/converter.py` & `econoplots-0.2.1/econoplots/converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module for converting input figure into Econoplots style."""
+
 # %% Imports
 
 # Standard Library Imports
 
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
@@ -73,23 +74,37 @@
     ax = converter_map[ax_type](ax, **kwargs)
 
     return ax
 
 
 def convertLine(
     ax: Axes,
+    econo_colors: bool = True,
     zero_dot: bool = False,
 ) -> Axes:
-    # Set general lie plot defaults
+    """
+    Converts Axes to a line plot with optional color and zero point settings.
+
+    Args:
+        ax (Axes): The matplotlib Axes object for conversion.
+        econo_colors (bool, optional): If True, sets line colors to default.
+            Defaults to True.
+        zero_dot (bool, optional): If True, plots a point at zero. Defaults
+            to False.
+
+    Returns:
+        Axes: The modified Axes object with line plot and optional settings.
+    """
+    # Set general line plot defaults
     ax = setLineDefaults(ax)
 
     # Change line colors
-    setDefaultLineColors(ax)
-
-    ax = updateLegendEntryColors(ax)
+    if econo_colors is True:
+        ax = setDefaultLineColors(ax)
+        ax = updateLegendEntryColors(ax)
 
     if zero_dot is True:
         ax = plotZeroPt(ax, marker_size=10)
 
     return ax
 
 
@@ -106,32 +121,33 @@
     # Move bottom spine before setting xAxis params to avoid Xticks being regenerated
     nudgeBottomSpine(ax)
     configIndependentXAxis(ax, pad_side="right", minor_ticks_on=True)
 
     # Add minor tick(s) if outer limits of data are NOT on major ticks. Unlike
     # minor ticks that are in-between major ticks, the outer minor ticks are not
     # optional.
-    addOuterMinorTicks(ax)
+    # TODO: Bring back option to promote an outer minor tick to a major tick
+    # addOuterMinorTicks(ax)
 
     # delete top, right, left spines
     makePatchSpinesInvisible(ax, ["top", "right", "left"])
 
     # Set legend background
     setLegendParams(ax)
 
     return ax
 
 
-def convertLineFill(ax: Axes) -> Axes:
+def convertLineFill(ax: Axes, econo_colors: bool = True) -> Axes:
     # Set general lie plot defaults
     ax = setLineDefaults(ax)
 
-    ax = setDefaultPatchColors(ax)
-
-    ax = updateLegendEntryColors(ax)
+    if econo_colors is True:
+        ax = setDefaultPatchColors(ax)
+        ax = updateLegendEntryColors(ax)
 
     return ax
 
 
 def convertBar(ax: Axes, orientation: str = "vertical") -> Axes:
     assert orientation in [
         "vertical",
@@ -156,23 +172,26 @@
         configIndependentXAxis(ax, pad_side="right", minor_ticks_on=False)
         configDependentYAxis(ax, side="right", label_location="right")
     else:
         configDepdendentXAxis(ax, side="top")
         configIndependentYAxis(ax)
 
     # Set bar zorder to be in front of grids
-    PutBarsInFront(ax)
+    # PutBarsInFront(ax) # done within setMajorGrids
 
     # Reset legend colors
     setLegendParams(ax)
 
     return ax
 
 
-def convertHBox(ax: Axes) -> Axes:
+def convertHBox(
+    ax: Axes,
+    econo_colors: bool = True,
+) -> Axes:
     assert (
         len(ax.patches) > 0
     ), "Input Axes does not have filled boxes. Remake plot by setting patch_artist=True."
 
     color_map = loadColorMap()
     # Set grid on and color
     setMajorGrids(ax, axis="x")
@@ -182,11 +201,12 @@
 
     # Set axis default params
     configDepdendentXAxis(ax, side="top")
     configIndependentYAxis(ax)
     replaceAxesMinusGlyphs(ax)
 
     # Set color of data series
-    setBoxColor(ax, color=color_map["web_all"]["blue"])
-    setLineColor(ax, color=color_map["web_all"]["blue"])
+    if econo_colors is True:
+        setBoxColor(ax, color=color_map["web_all"]["blue"])
+        setLineColor(ax, color=color_map["web_all"]["blue"])
 
     return ax
```

### Comparing `econoplots-0.2.0/econoplots/params.py` & `econoplots-0.2.1/econoplots/params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Set global parameters of matplotlib."""
+
 # %% Imports
 from __future__ import annotations
 
 # Third Party Imports
 import matplotlib as mpl
 from cycler import cycler
 
@@ -13,20 +14,25 @@
 # %% Set Params
 def setRCParams():
     color_map = loadColorMap()
 
     mpl.rcParams["font.sans-serif"] = [
         # "CMU Sans Serif Demi Condensed",
         # "CMU Sans Serif",
-        "CMU Bright",
+        "CMU Serif",
+        # "CMU Bright",
     ]
-    mpl.rcParams["font.family"] = "sans-serif"
+    # stix doesn't have the problem of unevenly-tall letters of CMU
+    mpl.rcParams["mathtext.fontset"] = "stix"
+    mpl.rcParams["font.family"] = "STIXGeneral"
+
+    # mpl.rcParams["font.family"] = "sans-serif"
     mpl.rcParams.update(
         {
-            "font.size": 14,
+            # "font.size": 14,
             # "font.weight": "bold",
             # "font.weight": "600",
         }
     )
     mpl.rcParams["lines.linestyle"] = "-"
     mpl.rcParams["lines.linewidth"] = 3
     mpl.rcParams["axes.prop_cycle"] = cycler(color=color_map["line_chart"])
```

### Comparing `econoplots-0.2.0/econoplots/utils.py` & `econoplots-0.2.1/econoplots/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities."""
+
 # Imports
 from __future__ import annotations
 
 # Standard Library Imports
 import importlib.resources
 import json
 from itertools import cycle
@@ -10,26 +11,26 @@
 
 # Third Party Imports
 from matplotlib import pyplot as plt  # noqa
 from matplotlib.axes import Axes
 from matplotlib.axis import Axis
 from matplotlib.collections import PolyCollection
 from matplotlib.container import BarContainer
-from matplotlib.patches import Patch, Rectangle
+from matplotlib.patches import Patch
 from matplotlib.text import Text
 from matplotlib.ticker import AutoMinorLocator, FixedLocator
 from numpy import (
     absolute,
     amax,
     amin,
     append,
     array,
     intersect1d,
+    linspace,
     logical_and,
-    max,
     min,
     nanmax,
     nanmin,
     ndarray,
     stack,
     where,
 )
@@ -75,25 +76,21 @@
     x_indx_inbound = inbound_indx[0]
     y_indx_inbound = inbound_indx[1]
 
     # Loop through in-range x and y tick labels. Use only in-range labels so that
     # when using ax.set_[x/y]ticks() we don't expand the axes limits beyond what
     # is already set.
     x_labels = []
-    tick_labels = ax.xaxis.get_ticklabels()[
-        x_indx_inbound[0] : x_indx_inbound[-1] + 1
-    ]
+    tick_labels = ax.xaxis.get_ticklabels()[x_indx_inbound[0] : x_indx_inbound[-1] + 1]
     for tl in tick_labels:
         x_labels.append(replaceMinusWithHyphen(tl))
     ax.set_xticks(x_locs_inbound, x_labels)
 
     y_labels = []
-    tick_labels = ax.yaxis.get_ticklabels()[
-        y_indx_inbound[0] : y_indx_inbound[-1] + 1
-    ]
+    tick_labels = ax.yaxis.get_ticklabels()[y_indx_inbound[0] : y_indx_inbound[-1] + 1]
     for tl in tick_labels:
         y_labels.append(replaceMinusWithHyphen(tl))
     ax.set_yticks(y_locs_inbound, y_labels)
 
     return
 
 
@@ -163,15 +160,15 @@
             major ticks. Defaults to None, which automatically determines number.
     """
     # Add empty space to x-axis to give space between y-tick labels and plotted
     # data. Do this BEFORE other operations, as resizing can mess up tick marks.
     padXAxis(ax, side=pad_side)
 
     # Set Major ticks. Make major ticks that are wider than span of the data invisible.
-    makeOutOfRangeXTicksInvisible(ax)
+    # makeOutOfRangeXTicksInvisible(ax)
 
     if minor_ticks_on is True:
         # Turn on minor ticks and set frequency between major ticks
         addInnerMinorTicks(ax, n_minortick_subdivisions)
 
     return
 
@@ -264,26 +261,32 @@
             "right": False,
             "left": True,
         }
 
     return tick_label_side
 
 
-def addInnerMinorTicks(ax: Axes, n_minortick_subdivisions: int | None):
+def addInnerMinorTicks(ax: Axes, n_minortick_subdivisions: int | None = 4):
     """Add minor ticks to x axis within data limits."""
-    ax.xaxis.set_minor_locator(AutoMinorLocator(n_minortick_subdivisions))
+    # Default is 4 minor ticks between each pair of major ticks
+    if n_minortick_subdivisions is None:
+        n_minortick_subdivisions = 4
+
+    major_ticks = ax.xaxis.get_majorticklocs()
+    # Calculate minor tick locations
+    # Skip over the major tick locations so that double-ticks aren't made
+    minor_ticks = []
+    for i in range(len(major_ticks) - 1):
+        minor_ticks += list(
+            linspace(major_ticks[i], major_ticks[i + 1], n_minortick_subdivisions + 2)[
+                1:-1
+            ]
+        )
+    ax.xaxis.set_minor_locator(FixedLocator(minor_ticks))
 
-    # Remove minor ticks that are beyond data range.
-    x_lims, _ = getDataLimits(ax)
-    # min_major_tick_loc = ax.xaxis.get_majorticklocs()[1]
-    # max_major_tick_loc = ax.xaxis.get_majorticklocs()[-2]
-    minor_tick_locs = ax.xaxis.get_minorticklocs()
-    minor_tick_locs = minor_tick_locs[minor_tick_locs > x_lims[0]]
-    minor_tick_locs = minor_tick_locs[minor_tick_locs < x_lims[1]]
-    ax.xaxis.set_minor_locator(FixedLocator(minor_tick_locs))
     return
 
 
 def makeOutOfRangeXTicksInvisible(ax: Axes):
     """Make major ticks that are < or > data range invisible."""
     major_tick_locs = ax.xaxis.get_majorticklocs()
     xticks = ax.xaxis.get_major_ticks()
@@ -412,63 +415,63 @@
     Returns:
         x_lims(list): x data limits [min, max]
         y_lims(list): y data limits [min, max]
     """
     x_lims = [0, 0]
     y_lims = [0, 0]
     lines = ax.get_lines()
-    if len(lines) == 0:
-        # If plot is a patch plot (no lines)
-        patch_likes = getFilledAreas(ax)
+    # Get limits of patches and lines (plots can have both)
+    patch_likes = getFilledAreas(ax)
+    if patch_likes:
+        # patch_likes is populated
         x_lims, y_lims = getPatchBounds(patch_likes, ax)
         x_lims = list(x_lims)
         y_lims = list(y_lims)
-    else:
-        for line in lines:
-            xdat = line.get_xdata()
-            ydat = line.get_ydata()
-
-            # extract data from MaskedArrays
-            if isinstance(xdat, MaskedArray):
-                xdat = getdata(xdat)
-            if isinstance(ydat, MaskedArray):
-                ydat = getdata(ydat)
-
-            # Use min/max with default values to account for 'empty' lines, which can
-            # occur in box plots.
-            min_x = nanmin(xdat, initial=x_lims[0])
-            max_x = nanmax(xdat, initial=x_lims[1])
-            min_y = nanmin(ydat, initial=y_lims[0])
-            max_y = nanmax(ydat, initial=y_lims[1])
-
-            if min_x < x_lims[0]:
-                x_lims[0] = min_x
-            if max_x > x_lims[1]:
-                x_lims[1] = max_x
-
-            if min_y < y_lims[0]:
-                y_lims[0] = min_y
-            if max_y > y_lims[1]:
-                y_lims[1] = max_y
+    for line in lines:
+        xdat = line.get_xdata()
+        ydat = line.get_ydata()
+
+        # extract data from MaskedArrays
+        if isinstance(xdat, MaskedArray):
+            xdat = getdata(xdat)
+        if isinstance(ydat, MaskedArray):
+            ydat = getdata(ydat)
+
+        # Use min/max with default values to account for 'empty' lines, which can
+        # occur in box plots.
+        min_x = nanmin(xdat, initial=x_lims[0])
+        max_x = nanmax(xdat, initial=x_lims[1])
+        min_y = nanmin(ydat, initial=y_lims[0])
+        max_y = nanmax(ydat, initial=y_lims[1])
+
+        if min_x < x_lims[0]:
+            x_lims[0] = min_x
+        if max_x > x_lims[1]:
+            x_lims[1] = max_x
+
+        if min_y < y_lims[0]:
+            y_lims[0] = min_y
+        if max_y > y_lims[1]:
+            y_lims[1] = max_y
 
     return x_lims, y_lims
 
 
-def getFilledAreas(ax: Axes) -> list[PolyCollection | BarContainer]:
+def getFilledAreas(ax: Axes) -> list[PolyCollection | BarContainer | list]:
     """Get filled areas, such as a PolyCollection or BarContainer."""
     children = ax.get_children()
     children_types = [type(child) for child in children]
     containers = ax.containers
     container_types = [type(container) for container in containers]
     if PolyCollection in children_types:
-        patches = [
-            child for child in children if isinstance(child, PolyCollection)
-        ]
+        patches = [child for child in children if isinstance(child, PolyCollection)]
     elif BarContainer in container_types:
         patches = [c for c in containers if isinstance(c, BarContainer)]
+    else:
+        patches = []
 
     return patches
 
 
 def getPatchBounds(
     patches: list[PolyCollection | BarContainer],
     ax: Axes,
@@ -518,40 +521,37 @@
         locs (list[ndarray]): A two-entry list with x and y in-bounds major tick
             locations.
         indices (list[ndarray]): A two-entry list with the indices of the in-bounds
             major ticks.
 
     """
     # get axis limits
+    # Ascending order not gauranteed, so use min and max to get limits.
     x_lim = ax.get_xlim()
     y_lim = ax.get_ylim()
 
     xtick_locs = ax.xaxis.get_majorticklocs()
     ytick_locs = ax.yaxis.get_majorticklocs()
 
     # Get the indices and corresponding locs that are within the axis limits.
     x_inbounds_indx = where(
         logical_and(
-            xtick_locs >= x_lim[0],
-            xtick_locs <= x_lim[1],
+            xtick_locs >= min(x_lim),
+            xtick_locs <= max(x_lim),
         )
     )[0]
     y_inbounds_indx = where(
         logical_and(
-            ytick_locs >= y_lim[0],
-            ytick_locs <= y_lim[1],
+            ytick_locs >= min(y_lim),
+            ytick_locs <= max(y_lim),
         )
     )[0]
 
-    xtick_locs_inbound = xtick_locs[
-        x_inbounds_indx[0] : x_inbounds_indx[-1] + 1
-    ]
-    ytick_locs_inbound = ytick_locs[
-        y_inbounds_indx[0] : y_inbounds_indx[-1] + 1
-    ]
+    xtick_locs_inbound = xtick_locs[x_inbounds_indx[0] : x_inbounds_indx[-1] + 1]
+    ytick_locs_inbound = ytick_locs[y_inbounds_indx[0] : y_inbounds_indx[-1] + 1]
 
     return (
         [xtick_locs_inbound, ytick_locs_inbound],
         [x_inbounds_indx, y_inbounds_indx],
     )
 
 
@@ -775,19 +775,31 @@
 
     color_map = loadColorMap()
 
     ax.grid(
         which="major",
         axis=axis,
         color=color_map["grid"]["grid_gray"],
-        zorder=1,
+        zorder=-100,  # set to low number to be in the back
         clip_on=True,
     )
     ax.grid(which="major", axis=opposite_axis, visible=False)
 
+    # Redraw lines and collections with different zorder to be in front
+    lines = ax.get_lines()
+    for line in lines:
+        line.set_zorder(2)
+    collections = ax.collections
+    for collection in collections:
+        collection.set_zorder(2)
+    ax = PutBarsInFront(ax)
+    # for container in ax.containers:
+    #     for element in container:
+    #         element.set_zorder(2)
+
     return ax
 
 
 def PutBarsInFront(ax: Axes) -> Axes:
     """Move bars in bar chart to zorder = 2."""
     bar_containers = [c for c in ax.containers if isinstance(c, BarContainer)]
     plt.setp(bar_containers, zorder=2)
```

### Comparing `econoplots-0.2.0/econoplots.egg-info/PKG-INFO` & `econoplots-0.2.1/econoplots.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econoplots
-Version: 0.2.0
+Version: 0.2.1
 Summary: Formats Matplotlib plots into the style of The Economist
 Author-email: Dylan Penn <dylan.penn@vt.edu>
 License: Copyright (c) 2022 Dylan Penn
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
@@ -26,14 +26,17 @@
 Project-URL: Homepage, https://github.com/dylan906/econoplots
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.20
+Requires-Dist: matplotlib>=3.5
+Requires-Dist: black>=23.3
 
 # Description
 This project helps create Matplotlib plots in the style of *The Economist*. Only some plot styles are supported (line plots are the only style that works right now) and there are some stylistic differences from *The Economist* for the sake of convenience/laziness. 
 
 # Users Guide
 - Install fonts (see below) before using any functions.
 - The main function you will use is `converter.convert2Econo()`, which takes a Matplotlib `Axes` and returns and `Axes` that is formatted nicely.
```

### Comparing `econoplots-0.2.0/pyproject.toml` & `econoplots-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `econoplots-0.2.0/tests/test_converter.py` & `econoplots-0.2.1/tests/test_converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 print(f"min(y) = {min(y)}")
 print(f"max(y) = {max(y)}")
 
 # %% Test line converter function
 fig, ax_line = plt.subplots()
 # ax_line.plot(x, y, color="red")
 ax_line.plot(x, y, color="red", label=["a", "b", "c"])
-ax_line.set_xlabel("X label")
+ax_line.set_xlabel(r"X label $\epsilon, \varepsilon \kappa$ ")
 ax_line.set_ylabel("Y label")
 ax_line.legend()
 
 ax_new = convert2Econo(deepcopy(ax_line))
 # %% Test line convert with 0,0 dot
 ax_new = convert2Econo(deepcopy(ax_line), zero_dot=True)
```

### Comparing `econoplots-0.2.0/tests/test_utils.py` & `econoplots-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

