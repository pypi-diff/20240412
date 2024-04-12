# Comparing `tmp/mastersign-datascience-0.2.8.tar.gz` & `tmp/mastersign-datascience-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastersign-datascience-0.2.8.tar", last modified: Sat Nov 26 16:39:31 2022, max compression
+gzip compressed data, was "mastersign-datascience-0.2.9.tar", last modified: Fri Apr 12 14:02:26 2024, max compression
```

## Comparing `mastersign-datascience-0.2.8.tar` & `mastersign-datascience-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.988526 mastersign-datascience-0.2.8/
--rw-rw-rw-   0        0        0     1555 2019-03-05 08:26:40.000000 mastersign-datascience-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     2289 2022-11-26 16:39:31.988526 mastersign-datascience-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1394 2019-03-06 08:08:54.000000 mastersign-datascience-0.2.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.915519 mastersign-datascience-0.2.8/mastersign/
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.915519 mastersign-datascience-0.2.8/mastersign/datascience/
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.931149 mastersign-datascience-0.2.8/mastersign/datascience/core/
--rw-rw-rw-   0        0        0      409 2022-11-26 16:23:15.000000 mastersign-datascience-0.2.8/mastersign/datascience/core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.931149 mastersign-datascience-0.2.8/mastersign/datascience/database/
--rw-rw-rw-   0        0        0     9611 2022-11-26 16:20:42.000000 mastersign-datascience-0.2.8/mastersign/datascience/database/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.931149 mastersign-datascience-0.2.8/mastersign/datascience/files/
--rw-rw-rw-   0        0        0     1868 2019-04-16 08:49:42.000000 mastersign-datascience-0.2.8/mastersign/datascience/files/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.931149 mastersign-datascience-0.2.8/mastersign/datascience/notebook/
--rw-rw-rw-   0        0        0       23 2019-02-28 14:57:49.000000 mastersign-datascience-0.2.8/mastersign/datascience/notebook/__init__.py
--rw-rw-rw-   0        0        0     2279 2019-03-20 08:06:51.000000 mastersign-datascience-0.2.8/mastersign/datascience/notebook/export_cell_code.py
--rw-rw-rw-   0        0        0     1111 2019-02-28 15:01:07.000000 mastersign-datascience-0.2.8/mastersign/datascience/notebook/remove_input_from_html.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.946776 mastersign-datascience-0.2.8/mastersign/datascience/plot/
--rw-rw-rw-   0        0        0    60083 2022-11-26 16:26:48.000000 mastersign-datascience-0.2.8/mastersign/datascience/plot/__init__.py
--rw-rw-rw-   0        0        0    10294 2019-03-04 14:42:01.000000 mastersign-datascience-0.2.8/mastersign/datascience/plot/basemap.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.946776 mastersign-datascience-0.2.8/mastersign/datascience/reversegeocoder/
--rw-rw-rw-   0        0        0     5346 2019-02-28 14:57:54.000000 mastersign-datascience-0.2.8/mastersign/datascience/reversegeocoder/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 16:39:31.978030 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/
--rw-rw-rw-   0        0        0     2289 2022-11-26 16:39:31.000000 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      665 2022-11-26 16:39:31.000000 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-26 16:39:31.000000 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2022-11-26 16:39:31.000000 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-26 16:39:31.000000 mastersign-datascience-0.2.8/mastersign_datascience.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-26 16:39:31.988526 mastersign-datascience-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1943 2019-03-27 12:39:31.000000 mastersign-datascience-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.817758 mastersign-datascience-0.2.9/
+-rw-rw-rw-   0        0        0     1555 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     2537 2024-04-12 14:02:26.816758 mastersign-datascience-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1394 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.786758 mastersign-datascience-0.2.9/mastersign/
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.789757 mastersign-datascience-0.2.9/mastersign/datascience/
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.792757 mastersign-datascience-0.2.9/mastersign/datascience/core/
+-rw-rw-rw-   0        0        0      409 2024-04-12 13:31:51.000000 mastersign-datascience-0.2.9/mastersign/datascience/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.792757 mastersign-datascience-0.2.9/mastersign/datascience/database/
+-rw-rw-rw-   0        0        0     9611 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.793757 mastersign-datascience-0.2.9/mastersign/datascience/files/
+-rw-rw-rw-   0        0        0     1868 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.795757 mastersign-datascience-0.2.9/mastersign/datascience/notebook/
+-rw-rw-rw-   0        0        0       23 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/notebook/__init__.py
+-rw-rw-rw-   0        0        0     2279 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/notebook/export_cell_code.py
+-rw-rw-rw-   0        0        0     1111 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/notebook/remove_input_from_html.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.796758 mastersign-datascience-0.2.9/mastersign/datascience/plot/
+-rw-rw-rw-   0        0        0    60223 2024-04-12 13:52:07.000000 mastersign-datascience-0.2.9/mastersign/datascience/plot/__init__.py
+-rw-rw-rw-   0        0        0    10637 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/plot/basemap.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.797757 mastersign-datascience-0.2.9/mastersign/datascience/reversegeocoder/
+-rw-rw-rw-   0        0        0     5518 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/mastersign/datascience/reversegeocoder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:02:26.815758 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/
+-rw-rw-rw-   0        0        0     2537 2024-04-12 14:02:26.000000 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-04-12 14:02:26.000000 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:02:26.000000 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2024-04-12 14:02:26.000000 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 14:02:26.000000 mastersign-datascience-0.2.9/mastersign_datascience.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:02:26.817758 mastersign-datascience-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1943 2024-04-05 09:03:36.000000 mastersign-datascience-0.2.9/setup.py
```

### Comparing `mastersign-datascience-0.2.8/LICENSE` & `mastersign-datascience-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/README.rst` & `mastersign-datascience-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/database/__init__.py` & `mastersign-datascience-0.2.9/mastersign/datascience/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/files/__init__.py` & `mastersign-datascience-0.2.9/mastersign/datascience/files/__init__.py`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/notebook/export_cell_code.py` & `mastersign-datascience-0.2.9/mastersign/datascience/notebook/export_cell_code.py`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/notebook/remove_input_from_html.py` & `mastersign-datascience-0.2.9/mastersign/datascience/notebook/remove_input_from_html.py`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/plot/__init__.py` & `mastersign-datascience-0.2.9/mastersign/datascience/plot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,24 +232,31 @@
     :return:        A tuple with Matplotlib figure and axes: ``(fig, ax)``.
     """
     if not _in_multiplot():
         raise Exception("No current figure. Did you use begin()?")
     return _plt(pos=pos, rowspan=rowspan, colspan=colspan)
 
 
+def _next_lines_color():
+    lines_ppva = plt.gca()._get_lines
+    try:
+        return lines_ppva.get_next_color()
+    except AttributeError:
+        return next(lines_ppva.prop_cycler)['color']
+
+
 def _build_key_colors(keys, color):
     if isinstance(color, str):
         return repeat(color, len(keys))
     elif isinstance(color, Mapping):
-        return [color.get(k, None) or next(plt.gca()._get_lines.prop_cycler)['color']
-                for k in keys]
+        return [color.get(k, None) or _next_lines_color() for k in keys]
     elif isinstance(color, Iterable):
         return cycle(color)
     else:
-        return [next(plt.gca()._get_lines.prop_cycler)['color'] for k in keys]
+        return [_next_lines_color() for _ in keys]
 
 
 def pie(data: Union[pd.DataFrame, pd.Series],
         column=None, label_column=None,
         color_column=None, color=None,
         startangle=180, counterclock=False,
         sort_by=None, title=None, pct=True,
@@ -310,16 +317,15 @@
 
     (fig, ax) = _plt(figsize=figsize, pos=pos,
                      rowspan=rowspan, colspan=colspan)
 
     if color_column:
         colors = data[color_column]
     elif isinstance(color, Mapping):
-        colors = [color.get(l) or next(plt.gca()._get_lines.prop_cycler)['color']
-                  for l in labels]
+        colors = [color.get(l) or _next_lines_color() for l in labels]
     elif color:
         colors = color
     else:
         colors = None
 
     if pct:
         ax.pie(x, labels=labels, colors=colors,
@@ -664,22 +670,23 @@
     (fig, ax) = _plt(figsize=figsize, pos=pos,
                      rowspan=rowspan, colspan=colspan)
 
     if labels:
         if isinstance(color, str):
             color = list(repeat(color, len(labels)))
         elif isinstance(color, Mapping):
-            color = [color.get(l) or next(plt.gca()._get_lines.prop_cycler)['color']
-                     for l in labels]
+            color = [color.get(l) or _next_lines_color() for l in labels]
         elif isinstance(color, Iterable):
             color = list(islice(cycle(color), len(labels)))
 
     if not labels and not isinstance(color, str) and isinstance(color, Iterable):
         colors = color
-        color = colors[0]
+        for c in colors:
+            color = c
+            break
     else:
         colors = None
 
     N, bins, patches = ax.hist(
         x, label=labels, bins=bins, cumulative=cumulative,
         stacked=stacked, color=color)
 
@@ -846,14 +853,16 @@
     s = (data[size_column] if size_column else 20) * size
     c = color
     if color_column:
         c = data[color_column]
         if not pd_types.is_numeric_dtype(c.dtype):
             cmap = None
             colorbar = False
+    else:
+        cmap = None
 
     (fig, ax) = _plt(figsize=figsize, pos=pos,
                      rowspan=rowspan, colspan=colspan)
     marker = ax.scatter(x, y, s=s, c=c, marker='o', cmap=cmap)
     ax.set_xlim(left=xmin, right=xmax)
     ax.set_ylim(bottom=ymin, top=ymax)
     if xticks is not None:
@@ -951,14 +960,16 @@
 
     c = color
     if color_column:
         c = data[color_column]
         if not pd_types.is_numeric_dtype(c.dtype):
             cmap = None
             colorbar = False
+    else:
+        cmap = None
 
     if autofit or region is None:
         region = [lat.min(), lon.min(), lat.max(), lon.max()]
         lat_margin = abs(region[2] - region[0]) * 0.15
         lon_margin = abs(region[3] - region[1]) * 0.15
         region[0] -= lat_margin
         region[1] -= lon_margin
```

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/plot/basemap.py` & `mastersign-datascience-0.2.9/mastersign/datascience/plot/basemap.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,343 +1,343 @@
-# -*- coding: utf-8 -*-
-
-"""
-This module contains functionality used to plot on a map.
-
-See e.g. `mastersign.datascience.plot.scatter_map()`.
-"""
-
-from typing import Any, Optional, Tuple, Sequence, Iterable, List, Mapping
-import numpy as np
-from mpl_toolkits.basemap import Basemap
-
-EPSG_WGS84_GIS = 3857  # Pseudo Mercator (Google Maps, OpenStreetView, Bing, ...)
-EPSG_WGS84_GPS = 4326  # GPS
-EPSG_ETRS89 = 5243     # LCC Germany
-
-
-def lat_lon_region(lower_left_corner_latitude,
-           lower_left_corner_longitude,
-           upper_right_corner_latitude,
-           upper_right_corner_longitude):
-    """
-    Converts a geographical region with lower left corner
-    and upper right corner into a Basemap compatible structure.
-
-    :param lower_left_corner_latitude:
-        The latitude of the lower left corner.
-    :param lower_left_corner_longitude:
-        The longitude of the lower left corner.
-    :param upper_right_corner_latitude:
-        The latitude of the lower left corner.
-    :param upper_right_corner_longitude:
-        The longitude of the lower left corner.
-
-    :return: A dict with the keys ``llcrnrlat``, ``llcrnrlon``,
-             ``urcrnrlat``, and ``urcrnrlon``.
-    """
-    return {
-        'llcrnrlat': lower_left_corner_latitude,
-        'llcrnrlon': lower_left_corner_longitude,
-        'urcrnrlat': upper_right_corner_latitude,
-        'urcrnrlon': upper_right_corner_longitude
-    }
-
-
-map_styles = {
-    'default': {
-        'ocean': '#D0E8FF',
-        'continent': '#E0FFC0',
-        'coast': '#60A0FF',
-        'lake': '#D0E8FF',
-        'river': '#60A0FF',
-        'border': '#C08080',
-        'region': '#E0A0A0',
-        'district': '#F0C0C0',
-        'grid': '#00000020',
-        'coast_width': 0.5,
-        'river_width': 0.3,
-        'border_width': 0.8,
-        'region_width': 0.4,
-        'district_width': 0.2,
-        'grid_width': 1.0,
-        'grid_dashes': [4, 2],
-        'draw_coast': True,
-        'draw_river': True,
-        'draw_border': True,
-        'draw_region': True,
-        'draw_district': True,
-        'draw_grid': True,
-        'local_border': False,
-    },
-    'gray': {
-        'ocean': '#E0E0E0',
-        'continent': '#FFFFFF',
-        'coast': '#C0C0C0',
-        'lake': '#D0D0D0',
-        'river': '#D0D0D0',
-        'border': '#A0A0A0',
-        'region': '#C0C0C0',
-        'district': '#E0E0E0',
-        'grid': '#00000020',
-        'coast_width': 0.8,
-        'river_width': 0.6,
-        'border_width': 1.1,
-        'region_width': 0.8,
-        'district_width': 0.2,
-        'grid_width': 1.0,
-        'grid_dashes': [4, 2],
-        'draw_coast': True,
-        'draw_river': True,
-        'draw_border': True,
-        'draw_region': True,
-        'draw_district': True,
-        'draw_grid': True,
-        'local_border': False,
-    },
-}
-
-
-def _draw_grid(m, dlat=30.0, dlon=60.0, color='#BBBBBB', linewidth=1, dashes=[4,2]):
-    m.drawparallels(np.arange(-180.0 + dlat, +180 - dlat, dlat),
-                    color=color, linewidth=linewidth, dashes=dashes)
-    m.drawmeridians(np.arange(0.0, 360.0, dlon),
-                    color=color, linewidth=linewidth, dashes=dashes)
-
-
-def base_map(region: Mapping[str, float],
-             projection: str = 'cyl',
-             epsg: Optional[int] = None,
-             grid: Tuple[float, float] = (30, 60),
-             resolution: str = 'i',
-             style_name: Optional[str] = None,
-             style_attributes: Optional[Mapping[str, Any]] = None,
-             ax = None) -> Basemap:
-    """
-    Creates a Basemap instance containing continents, coastlines,
-    rivers and country borders.
-
-    :param region:
-        A Basemap compatible structure defining a rectangular
-        geographical region. (See `lat_lon_region()`.)
-    :type region: Mapping[str, float]
-
-    :param projection:
-        A named projection from Basemap.
-        E.g. `cyl`, `robin`, `mill`, `ortho`, `merc`, and a lot more.
-
-        See https://matplotlib.org/basemap/users/mapsetup.html
-        for more details.
-
-    :param epsg:
-        An EPSG projection code as an alternative to the named
-        projection types.
-        E.g. `EPSG_WGS84_GIS`, `EPSG_WGS84_GPS`, or `EPSG_ETRS89`.
-
-        See http://spatialreference.org/ref/epsg/ for EPSG codes.
-
-    :type epsg: Optional[int]
-
-    :param lat_0:
-        The latitude facing the viewer for orthographic projections.
-    :type lat_0: float
-
-    :param lon_0:
-        The longitude facing the viewer for orthographic projections.
-    :type lon_0: float
-
-    :param grid:
-        A tuple with latitude and longitude intervals for drawing a grid.
-    :type grid: Tuple[float, float]
-
-    :param resolution:
-        The Basemap resolution level: ``c`` (crude), ``l`` (low),
-        ``i`` (intermediate), ``h`` (high), or ``f`` (full).
-    :type resolution: str
-
-    :param style_name:
-        The name of a style in `map_styles`.
-    :type style_name: str
-
-    :param style_attributes:
-        A dict like structure with overridings for the style.
-    :type style_attributes: Optional[Mapping[str, Any]]
-
-    :param ax:
-        A mapplotlib Axes object.
-
-    :return:
-        The initialized Basemap instance.
-    :rtype: mpl_toolkits.basemap.Basemap
-    """
-
-    style = map_styles[style_name or 'default']
-    if style_attributes:
-        style = {**style, **style_attributes}
-
-    m = Basemap(projection=projection, epsg=epsg, resolution=resolution,
-                ax=ax, lat_0=0, lon_0=0, **region)
-    m.drawmapboundary(fill_color=style['ocean'])
-    m.fillcontinents(color=style['continent'], lake_color=style['lake'])
-    if style['draw_river']:
-        m.drawrivers(color=style['river'], linewidth=style['river_width'])
-    if style['draw_coast']:
-        m.drawcoastlines(color=style['coast'], linewidth=style['coast_width'])
-    if style['draw_border']:
-        m.drawcountries(color=style['border'], linewidth=style['border_width'])
-    if style['draw_grid']:
-        _draw_grid(m, *grid, color=style['grid'], linewidth=style['grid_width'])
-    return m
-
-
-def g2m(m: Basemap, coord: Tuple[float, float]) \
-        -> Tuple[float, float]:
-    """
-    Convert geographical coordinate into x-y-coordinates in the plotting space.
-
-    :param m:
-        The Basemap instance to use for conversion.
-    :type m: mpl_toolkits.basemap.Basemap
-
-    :param coord:
-        A tuple with the latitude and longitude.
-    :type coord: Tuple[float, float]
-
-    :return:
-        A tuple with the x and y coordinates in the plotting space.
-    :rtype: Tuple[float, float]
-    """
-    return m(coord[1], coord[0])
-
-
-def g2ms(m: Basemap, coords: Iterable[Tuple[float, float]]) \
-         -> List[Tuple[float, float]]:
-    """
-    Convert an iterable with geographical coordinates into
-    a list of x-y-coordinates in the plotting space.
-
-    :param m:
-        The Basemap instance to use for conversion.
-    :type m: mpl_toolkits.basemap.Basemap
-
-    :param coords:
-        An iterable with geographical coordinates (lat, lon).
-    :type coords: Iterable[Tuple[float, float]]
-
-    :return:
-        A list with x-y-coordinates in the plotting space.
-    :rtype:
-        List[Tuple[float, float]]
-    """
-    return [m(c[1], c[0]) for c in coords]
-
-
-def g2xys(m: Basemap, coords: Iterable[Tuple[float, float]]) \
-          -> Tuple[Sequence[float], Sequence[float]]:
-    """
-    Convert an iterable with geographical coordinates into
-    two sequences with x- and y-coordinates in the plotting space.
-
-    Can be used to convert an iterable with geographic coordinates
-    into the input for a line or scatter plot.
-
-    :param m:
-        The Basemap instance to use for conversion.
-    :type m: mpl_toolkits.basemap.Basemap
-
-    :param coords:
-        An iterable with geographical coordinates (lat, lon).
-    :type coords: Iterable[Tuple[float, float]]
-
-    :return:
-        Two lists with x- and y-coordinates in the plotting space.
-    :rtype:
-        Tuple[Sequence[float], Sequence[float]]
-    """
-    x, y = zip(*g2ms(m, coords))
-    return x, y
-
-
-def _shoot(lon: float, lat: float, azimuth: float, maxdist: float):
-    """
-    Shooter Function
-    Original javascript on http://williams.best.vwh.net/gccalc.htm
-    Translated to python by Thomas Lecocq
-    """
-    glat1 = lat * np.pi / 180.
-    glon1 = lon * np.pi / 180.
-    s = maxdist / 1.852
-    faz = azimuth * np.pi / 180.
-
-    EPS= 0.00000000005
-    if ((np.abs(np.cos(glat1))<EPS) and not (np.abs(np.sin(faz))<EPS)):
-        raise Exception("Only N-S courses are meaningful, starting at a pole!")
-
-    a=6378.13/1.852
-    f=1/298.257223563
-    r = 1 - f
-    tu = r * np.tan(glat1)
-    sf = np.sin(faz)
-    cf = np.cos(faz)
-    if (cf==0):
-        b=0.
-    else:
-        b=2. * np.arctan2 (tu, cf)
-
-    cu = 1. / np.sqrt(1 + tu * tu)
-    su = tu * cu
-    sa = cu * sf
-    c2a = 1 - sa * sa
-    x = 1. + np.sqrt(1. + c2a * (1. / (r * r) - 1.))
-    x = (x - 2.) / x
-    c = 1. - x
-    c = (x * x / 4. + 1.) / c
-    d = (0.375 * x * x - 1.) * x
-    tu = s / (r * a * c)
-    y = tu
-    c = y + 1
-    while (np.abs (y - c) > EPS):
-
-        sy = np.sin(y)
-        cy = np.cos(y)
-        cz = np.cos(b + y)
-        e = 2. * cz * cz - 1.
-        c = y
-        x = e * cy
-        y = e + e - 1.
-        y = (((sy * sy * 4. - 3.) * y * cz * d / 6. + x) *
-              d / 4. - cz) * sy * d + tu
-
-    b = cu * cy * cf - su * sy
-    c = r * np.sqrt(sa * sa + b * b)
-    d = su * cy + cu * sy * cf
-    glat2 = (np.arctan2(d, c) + np.pi) % (2*np.pi) - np.pi
-    c = cu * cy - su * sy * cf
-    x = np.arctan2(sy * sf, c)
-    c = ((-3. * c2a + 4.) * f + 4.) * c2a * f / 16.
-    d = ((e * cy * c + cz) * sy * c + y) * sa
-    glon2 = ((glon1 + x - (1. - c) * d * f + np.pi) % (2*np.pi)) - np.pi
-
-    baz = (np.arctan2(sa, b) + np.pi) % (2 * np.pi)
-
-    glon2 *= 180./np.pi
-    glat2 *= 180./np.pi
-    baz *= 180./np.pi
-
-    return (glon2, glat2, baz)
-
-
-def _equi(m: Basemap, centerlon: float, centerlat: float, radius: float) \
-          -> Tuple[float, float]:
-    glon1 = centerlon
-    glat1 = centerlat
-    X = []
-    Y = []
-    for azimuth in range(0, 360):
-        glon2, glat2, baz = _shoot(glon1, glat1, azimuth, radius)
-        X.append(glon2)
-        Y.append(glat2)
-    X.append(X[0])
-    Y.append(Y[0])
-
-    #~ m.plot(X,Y,**kwargs) #Should work, but doesn't...
-    return m(X, Y)
+# -*- coding: utf-8 -*-
+
+"""
+This module contains functionality used to plot on a map.
+
+See e.g. `mastersign.datascience.plot.scatter_map()`.
+"""
+
+from typing import Any, Optional, Tuple, Sequence, Iterable, List, Mapping
+import numpy as np
+from mpl_toolkits.basemap import Basemap
+
+EPSG_WGS84_GIS = 3857  # Pseudo Mercator (Google Maps, OpenStreetView, Bing, ...)
+EPSG_WGS84_GPS = 4326  # GPS
+EPSG_ETRS89 = 5243     # LCC Germany
+
+
+def lat_lon_region(lower_left_corner_latitude,
+           lower_left_corner_longitude,
+           upper_right_corner_latitude,
+           upper_right_corner_longitude):
+    """
+    Converts a geographical region with lower left corner
+    and upper right corner into a Basemap compatible structure.
+
+    :param lower_left_corner_latitude:
+        The latitude of the lower left corner.
+    :param lower_left_corner_longitude:
+        The longitude of the lower left corner.
+    :param upper_right_corner_latitude:
+        The latitude of the lower left corner.
+    :param upper_right_corner_longitude:
+        The longitude of the lower left corner.
+
+    :return: A dict with the keys ``llcrnrlat``, ``llcrnrlon``,
+             ``urcrnrlat``, and ``urcrnrlon``.
+    """
+    return {
+        'llcrnrlat': lower_left_corner_latitude,
+        'llcrnrlon': lower_left_corner_longitude,
+        'urcrnrlat': upper_right_corner_latitude,
+        'urcrnrlon': upper_right_corner_longitude
+    }
+
+
+map_styles = {
+    'default': {
+        'ocean': '#D0E8FF',
+        'continent': '#E0FFC0',
+        'coast': '#60A0FF',
+        'lake': '#D0E8FF',
+        'river': '#60A0FF',
+        'border': '#C08080',
+        'region': '#E0A0A0',
+        'district': '#F0C0C0',
+        'grid': '#00000020',
+        'coast_width': 0.5,
+        'river_width': 0.3,
+        'border_width': 0.8,
+        'region_width': 0.4,
+        'district_width': 0.2,
+        'grid_width': 1.0,
+        'grid_dashes': [4, 2],
+        'draw_coast': True,
+        'draw_river': True,
+        'draw_border': True,
+        'draw_region': True,
+        'draw_district': True,
+        'draw_grid': True,
+        'local_border': False,
+    },
+    'gray': {
+        'ocean': '#E0E0E0',
+        'continent': '#FFFFFF',
+        'coast': '#C0C0C0',
+        'lake': '#D0D0D0',
+        'river': '#D0D0D0',
+        'border': '#A0A0A0',
+        'region': '#C0C0C0',
+        'district': '#E0E0E0',
+        'grid': '#00000020',
+        'coast_width': 0.8,
+        'river_width': 0.6,
+        'border_width': 1.1,
+        'region_width': 0.8,
+        'district_width': 0.2,
+        'grid_width': 1.0,
+        'grid_dashes': [4, 2],
+        'draw_coast': True,
+        'draw_river': True,
+        'draw_border': True,
+        'draw_region': True,
+        'draw_district': True,
+        'draw_grid': True,
+        'local_border': False,
+    },
+}
+
+
+def _draw_grid(m, dlat=30.0, dlon=60.0, color='#BBBBBB', linewidth=1, dashes=[4,2]):
+    m.drawparallels(np.arange(-180.0 + dlat, +180 - dlat, dlat),
+                    color=color, linewidth=linewidth, dashes=dashes)
+    m.drawmeridians(np.arange(0.0, 360.0, dlon),
+                    color=color, linewidth=linewidth, dashes=dashes)
+
+
+def base_map(region: Mapping[str, float],
+             projection: str = 'cyl',
+             epsg: Optional[int] = None,
+             grid: Tuple[float, float] = (30, 60),
+             resolution: str = 'i',
+             style_name: Optional[str] = None,
+             style_attributes: Optional[Mapping[str, Any]] = None,
+             ax = None) -> Basemap:
+    """
+    Creates a Basemap instance containing continents, coastlines,
+    rivers and country borders.
+
+    :param region:
+        A Basemap compatible structure defining a rectangular
+        geographical region. (See `lat_lon_region()`.)
+    :type region: Mapping[str, float]
+
+    :param projection:
+        A named projection from Basemap.
+        E.g. `cyl`, `robin`, `mill`, `ortho`, `merc`, and a lot more.
+
+        See https://matplotlib.org/basemap/users/mapsetup.html
+        for more details.
+
+    :param epsg:
+        An EPSG projection code as an alternative to the named
+        projection types.
+        E.g. `EPSG_WGS84_GIS`, `EPSG_WGS84_GPS`, or `EPSG_ETRS89`.
+
+        See http://spatialreference.org/ref/epsg/ for EPSG codes.
+
+    :type epsg: Optional[int]
+
+    :param lat_0:
+        The latitude facing the viewer for orthographic projections.
+    :type lat_0: float
+
+    :param lon_0:
+        The longitude facing the viewer for orthographic projections.
+    :type lon_0: float
+
+    :param grid:
+        A tuple with latitude and longitude intervals for drawing a grid.
+    :type grid: Tuple[float, float]
+
+    :param resolution:
+        The Basemap resolution level: ``c`` (crude), ``l`` (low),
+        ``i`` (intermediate), ``h`` (high), or ``f`` (full).
+    :type resolution: str
+
+    :param style_name:
+        The name of a style in `map_styles`.
+    :type style_name: str
+
+    :param style_attributes:
+        A dict like structure with overridings for the style.
+    :type style_attributes: Optional[Mapping[str, Any]]
+
+    :param ax:
+        A mapplotlib Axes object.
+
+    :return:
+        The initialized Basemap instance.
+    :rtype: mpl_toolkits.basemap.Basemap
+    """
+
+    style = map_styles[style_name or 'default']
+    if style_attributes:
+        style = {**style, **style_attributes}
+
+    m = Basemap(projection=projection, epsg=epsg, resolution=resolution,
+                ax=ax, lat_0=0, lon_0=0, **region)
+    m.drawmapboundary(fill_color=style['ocean'])
+    m.fillcontinents(color=style['continent'], lake_color=style['lake'])
+    if style['draw_river']:
+        m.drawrivers(color=style['river'], linewidth=style['river_width'])
+    if style['draw_coast']:
+        m.drawcoastlines(color=style['coast'], linewidth=style['coast_width'])
+    if style['draw_border']:
+        m.drawcountries(color=style['border'], linewidth=style['border_width'])
+    if style['draw_grid']:
+        _draw_grid(m, *grid, color=style['grid'], linewidth=style['grid_width'])
+    return m
+
+
+def g2m(m: Basemap, coord: Tuple[float, float]) \
+        -> Tuple[float, float]:
+    """
+    Convert geographical coordinate into x-y-coordinates in the plotting space.
+
+    :param m:
+        The Basemap instance to use for conversion.
+    :type m: mpl_toolkits.basemap.Basemap
+
+    :param coord:
+        A tuple with the latitude and longitude.
+    :type coord: Tuple[float, float]
+
+    :return:
+        A tuple with the x and y coordinates in the plotting space.
+    :rtype: Tuple[float, float]
+    """
+    return m(coord[1], coord[0])
+
+
+def g2ms(m: Basemap, coords: Iterable[Tuple[float, float]]) \
+         -> List[Tuple[float, float]]:
+    """
+    Convert an iterable with geographical coordinates into
+    a list of x-y-coordinates in the plotting space.
+
+    :param m:
+        The Basemap instance to use for conversion.
+    :type m: mpl_toolkits.basemap.Basemap
+
+    :param coords:
+        An iterable with geographical coordinates (lat, lon).
+    :type coords: Iterable[Tuple[float, float]]
+
+    :return:
+        A list with x-y-coordinates in the plotting space.
+    :rtype:
+        List[Tuple[float, float]]
+    """
+    return [m(c[1], c[0]) for c in coords]
+
+
+def g2xys(m: Basemap, coords: Iterable[Tuple[float, float]]) \
+          -> Tuple[Sequence[float], Sequence[float]]:
+    """
+    Convert an iterable with geographical coordinates into
+    two sequences with x- and y-coordinates in the plotting space.
+
+    Can be used to convert an iterable with geographic coordinates
+    into the input for a line or scatter plot.
+
+    :param m:
+        The Basemap instance to use for conversion.
+    :type m: mpl_toolkits.basemap.Basemap
+
+    :param coords:
+        An iterable with geographical coordinates (lat, lon).
+    :type coords: Iterable[Tuple[float, float]]
+
+    :return:
+        Two lists with x- and y-coordinates in the plotting space.
+    :rtype:
+        Tuple[Sequence[float], Sequence[float]]
+    """
+    x, y = zip(*g2ms(m, coords))
+    return x, y
+
+
+def _shoot(lon: float, lat: float, azimuth: float, maxdist: float):
+    """
+    Shooter Function
+    Original javascript on http://williams.best.vwh.net/gccalc.htm
+    Translated to python by Thomas Lecocq
+    """
+    glat1 = lat * np.pi / 180.
+    glon1 = lon * np.pi / 180.
+    s = maxdist / 1.852
+    faz = azimuth * np.pi / 180.
+
+    EPS= 0.00000000005
+    if ((np.abs(np.cos(glat1))<EPS) and not (np.abs(np.sin(faz))<EPS)):
+        raise Exception("Only N-S courses are meaningful, starting at a pole!")
+
+    a=6378.13/1.852
+    f=1/298.257223563
+    r = 1 - f
+    tu = r * np.tan(glat1)
+    sf = np.sin(faz)
+    cf = np.cos(faz)
+    if (cf==0):
+        b=0.
+    else:
+        b=2. * np.arctan2 (tu, cf)
+
+    cu = 1. / np.sqrt(1 + tu * tu)
+    su = tu * cu
+    sa = cu * sf
+    c2a = 1 - sa * sa
+    x = 1. + np.sqrt(1. + c2a * (1. / (r * r) - 1.))
+    x = (x - 2.) / x
+    c = 1. - x
+    c = (x * x / 4. + 1.) / c
+    d = (0.375 * x * x - 1.) * x
+    tu = s / (r * a * c)
+    y = tu
+    c = y + 1
+    while (np.abs (y - c) > EPS):
+
+        sy = np.sin(y)
+        cy = np.cos(y)
+        cz = np.cos(b + y)
+        e = 2. * cz * cz - 1.
+        c = y
+        x = e * cy
+        y = e + e - 1.
+        y = (((sy * sy * 4. - 3.) * y * cz * d / 6. + x) *
+              d / 4. - cz) * sy * d + tu
+
+    b = cu * cy * cf - su * sy
+    c = r * np.sqrt(sa * sa + b * b)
+    d = su * cy + cu * sy * cf
+    glat2 = (np.arctan2(d, c) + np.pi) % (2*np.pi) - np.pi
+    c = cu * cy - su * sy * cf
+    x = np.arctan2(sy * sf, c)
+    c = ((-3. * c2a + 4.) * f + 4.) * c2a * f / 16.
+    d = ((e * cy * c + cz) * sy * c + y) * sa
+    glon2 = ((glon1 + x - (1. - c) * d * f + np.pi) % (2*np.pi)) - np.pi
+
+    baz = (np.arctan2(sa, b) + np.pi) % (2 * np.pi)
+
+    glon2 *= 180./np.pi
+    glat2 *= 180./np.pi
+    baz *= 180./np.pi
+
+    return (glon2, glat2, baz)
+
+
+def _equi(m: Basemap, centerlon: float, centerlat: float, radius: float) \
+          -> Tuple[float, float]:
+    glon1 = centerlon
+    glat1 = centerlat
+    X = []
+    Y = []
+    for azimuth in range(0, 360):
+        glon2, glat2, baz = _shoot(glon1, glat1, azimuth, radius)
+        X.append(glon2)
+        Y.append(glat2)
+    X.append(X[0])
+    Y.append(Y[0])
+
+    #~ m.plot(X,Y,**kwargs) #Should work, but doesn't...
+    return m(X, Y)
```

### Comparing `mastersign-datascience-0.2.8/mastersign/datascience/reversegeocoder/__init__.py` & `mastersign-datascience-0.2.9/mastersign/datascience/reversegeocoder/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,172 @@
-# -*- coding: utf-8 -*-
-
-import re
-import urllib
-import requests
-
-
-class HttpClient(object):
-    def __init__(self):
-        self.session = requests.Session()
-
-    @staticmethod
-    def _write_debug_file(filename, text, *args):
-        pass
-
-    def get(self, url):
-        try:
-            response = self.session.get(url, timeout=10.0)
-        except requests.RequestException as exc:
-            print("RequestException: {}".format(type(exc).__name__))
-            print(url)
-            return None
-        if response.status_code != 200:
-            print("HTTP Status Code {} {}".format(response.status_code, response.reason))
-            print(url)
-            return None
-        return response
-
-    def get_text(self, url, encoding=None):
-        response = self.get(url)
-        if response is None:
-            return None
-        if encoding:
-            response.encoding = encoding
-        return response.text
-
-    def get_json(self, url, debug_file=None):
-        response = self.get(url)
-        if response is None:
-            return None
-        return response.json()
-
-
-# street_pattern = re.compile(r"^(.*?)(\d+\s*[a-z]?(?:-\d+\s*[a-z]?)?)\s*$")
-district_pattern = re.compile(r"^(.*?)\s*/?\s*OT.*$")
-
-def strip_district(city):
-    m = district_pattern.match(city)
-    if m is not None:
-        return m.group(1)
-    return None
-
-
-class ReverseGeoCoder(object):
-
-    def __init__(self):
-        self.http = HttpClient()
-        self.base_url = 'http://nominatim.openstreetmap.org/search'
-
-    def _build_url(self, query):
-        return self.base_url + '?' + '&'.join([k + '=' + urllib.parse.quote_plus(str(v)) for k, v in query.items()])
-
-    @staticmethod
-    def _format_query(query):
-        if 'q' in query:
-            return query['q']
-        parts = []
-        if 'country' in query:
-            parts.append(query['country'])
-        if 'city' in query and 'postalcode' in query:
-            parts.append(query['postalcode'] + ' ' + query['city'])
-        elif 'city' in query:
-            parts.append(query['city'])
-        elif 'postalcode' in query:
-            parts.append(query['postalcode'])
-        if 'street' in query:
-            parts.append(query['street'])
-        return ', '.join(parts)
-
-    @staticmethod
-    def _build_query(country, city, postalcode, street, house_number, **kwargs):
-        query = {}
-        if country:
-            query['country'] = country
-        if city:
-            query['city'] = city
-        if postalcode:
-            query['postalcode'] = postalcode
-        if street and house_number:
-            query['street'] = '{} {}'.format(house_number, street)
-        elif street:
-            query['street'] = street
-        return query
-
-    @staticmethod
-    def _build_soft_query(**kwargs):
-        return {'q': __class__._format_query(__class__._build_query(**kwargs))}
-
-    def _lookup(self, query):
-        query['limit'] = 1
-        query['format'] = 'json'
-        if 'country' in query and query['country'] == 'Schweiz':
-            query['countrycodes'] = 'ch'
-        elif 'country' in query and query['country'] == 'Österreich':
-            query['countrycodes'] = 'at'
-        else:
-            query['countrycodes'] = 'de'
-        url = self._build_url(query)
-        data = self.http.get_json(url)
-        if data is None or len(data) == 0:
-            print("DID NOT RESOLVE LOCATION FOR {}".format(
-                  self._format_query(query)))
-            return None
-        else:
-            lat = data[0]['lat']
-            lon = data[0]['lon']
-            return {
-                'latitude': float(lat),
-                'longitude': float(lon)
-            }
-
-    def lookup(self, **kwargs):
-        template = {
-            'country': '',
-            'city': '',
-            'postalcode': '',
-            'street': '',
-            'house_number': '',
-        }
-        template.update(kwargs)
-        kwargs = template
-
-        # try structured query method
-        kwargs2 = kwargs.copy()
-        org_query = query = self._build_query(**kwargs2)
-        result = self._lookup(query)
-
-        # strip potentially existing district
-        stripped_city = strip_district(kwargs['city'])
-        if result is None and stripped_city:
-            kwargs2['city'] = stripped_city
-            query = self._build_query(**kwargs2)
-            result = self._lookup(query)
-
-        # omit street
-        if result is None and kwargs2['street']:
-            kwargs2['street'] = None
-            query = self._build_query(**kwargs2)
-            result = self._lookup(query)
-
-        # try unstructured query method
-        if result is None:
-            kwargs2 = dict(kwargs)
-            query = self._build_soft_query(**kwargs2)
-            result = self._lookup(query)
-
-        # strip potentially existing district
-        if result is None and stripped_city:
-            kwargs2['city'] = stripped_city
-            query = self._build_soft_query(**kwargs2)
-            result = self._lookup(query)
-
-        # omit street
-        if result is None and kwargs2['street']:
-            kwargs2['street'] = None
-            query = self._build_soft_query(**kwargs2)
-            result = self._lookup(query)
-
-        if result is None:
-            print("FAILED TO GEOCODE {}".format(
-                  self._format_query(org_query)))
-        return result
+# -*- coding: utf-8 -*-
+
+import re
+import urllib
+import requests
+
+
+class HttpClient(object):
+    def __init__(self):
+        self.session = requests.Session()
+
+    @staticmethod
+    def _write_debug_file(filename, text, *args):
+        pass
+
+    def get(self, url):
+        try:
+            response = self.session.get(url, timeout=10.0)
+        except requests.RequestException as exc:
+            print("RequestException: {}".format(type(exc).__name__))
+            print(url)
+            return None
+        if response.status_code != 200:
+            print("HTTP Status Code {} {}".format(response.status_code, response.reason))
+            print(url)
+            return None
+        return response
+
+    def get_text(self, url, encoding=None):
+        response = self.get(url)
+        if response is None:
+            return None
+        if encoding:
+            response.encoding = encoding
+        return response.text
+
+    def get_json(self, url, debug_file=None):
+        response = self.get(url)
+        if response is None:
+            return None
+        return response.json()
+
+
+# street_pattern = re.compile(r"^(.*?)(\d+\s*[a-z]?(?:-\d+\s*[a-z]?)?)\s*$")
+district_pattern = re.compile(r"^(.*?)\s*/?\s*OT.*$")
+
+def strip_district(city):
+    m = district_pattern.match(city)
+    if m is not None:
+        return m.group(1)
+    return None
+
+
+class ReverseGeoCoder(object):
+
+    def __init__(self):
+        self.http = HttpClient()
+        self.base_url = 'http://nominatim.openstreetmap.org/search'
+
+    def _build_url(self, query):
+        return self.base_url + '?' + '&'.join([k + '=' + urllib.parse.quote_plus(str(v)) for k, v in query.items()])
+
+    @staticmethod
+    def _format_query(query):
+        if 'q' in query:
+            return query['q']
+        parts = []
+        if 'country' in query:
+            parts.append(query['country'])
+        if 'city' in query and 'postalcode' in query:
+            parts.append(query['postalcode'] + ' ' + query['city'])
+        elif 'city' in query:
+            parts.append(query['city'])
+        elif 'postalcode' in query:
+            parts.append(query['postalcode'])
+        if 'street' in query:
+            parts.append(query['street'])
+        return ', '.join(parts)
+
+    @staticmethod
+    def _build_query(country, city, postalcode, street, house_number, **kwargs):
+        query = {}
+        if country:
+            query['country'] = country
+        if city:
+            query['city'] = city
+        if postalcode:
+            query['postalcode'] = postalcode
+        if street and house_number:
+            query['street'] = '{} {}'.format(house_number, street)
+        elif street:
+            query['street'] = street
+        return query
+
+    @staticmethod
+    def _build_soft_query(**kwargs):
+        return {'q': __class__._format_query(__class__._build_query(**kwargs))}
+
+    def _lookup(self, query):
+        query['limit'] = 1
+        query['format'] = 'json'
+        if 'country' in query and query['country'] == 'Schweiz':
+            query['countrycodes'] = 'ch'
+        elif 'country' in query and query['country'] == 'Österreich':
+            query['countrycodes'] = 'at'
+        else:
+            query['countrycodes'] = 'de'
+        url = self._build_url(query)
+        data = self.http.get_json(url)
+        if data is None or len(data) == 0:
+            print("DID NOT RESOLVE LOCATION FOR {}".format(
+                  self._format_query(query)))
+            return None
+        else:
+            lat = data[0]['lat']
+            lon = data[0]['lon']
+            return {
+                'latitude': float(lat),
+                'longitude': float(lon)
+            }
+
+    def lookup(self, **kwargs):
+        template = {
+            'country': '',
+            'city': '',
+            'postalcode': '',
+            'street': '',
+            'house_number': '',
+        }
+        template.update(kwargs)
+        kwargs = template
+
+        # try structured query method
+        kwargs2 = kwargs.copy()
+        org_query = query = self._build_query(**kwargs2)
+        result = self._lookup(query)
+
+        # strip potentially existing district
+        stripped_city = strip_district(kwargs['city'])
+        if result is None and stripped_city:
+            kwargs2['city'] = stripped_city
+            query = self._build_query(**kwargs2)
+            result = self._lookup(query)
+
+        # omit street
+        if result is None and kwargs2['street']:
+            kwargs2['street'] = None
+            query = self._build_query(**kwargs2)
+            result = self._lookup(query)
+
+        # try unstructured query method
+        if result is None:
+            kwargs2 = dict(kwargs)
+            query = self._build_soft_query(**kwargs2)
+            result = self._lookup(query)
+
+        # strip potentially existing district
+        if result is None and stripped_city:
+            kwargs2['city'] = stripped_city
+            query = self._build_soft_query(**kwargs2)
+            result = self._lookup(query)
+
+        # omit street
+        if result is None and kwargs2['street']:
+            kwargs2['street'] = None
+            query = self._build_soft_query(**kwargs2)
+            result = self._lookup(query)
+
+        if result is None:
+            print("FAILED TO GEOCODE {}".format(
+                  self._format_query(org_query)))
+        return result
```

### Comparing `mastersign-datascience-0.2.8/mastersign_datascience.egg-info/SOURCES.txt` & `mastersign-datascience-0.2.9/mastersign_datascience.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mastersign-datascience-0.2.8/setup.py` & `mastersign-datascience-0.2.9/setup.py`

 * *Files identical despite different names*

