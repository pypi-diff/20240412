# Comparing `tmp/esy-osm-shape-0.2.tar.gz` & `tmp/esy-osm-shape-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esy-osm-shape-0.2.tar", last modified: Mon Feb 27 13:24:51 2023, max compression
+gzip compressed data, was "esy-osm-shape-0.3.tar", last modified: Fri Apr 12 13:58:49 2024, max compression
```

## Comparing `esy-osm-shape-0.2.tar` & `esy-osm-shape-0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.186854 esy-osm-shape-0.2/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)    35130 2023-02-27 13:18:14.000000 esy-osm-shape-0.2/LICENSE
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     2068 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/PKG-INFO
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1254 2022-11-08 13:39:31.000000 esy-osm-shape-0.2/README.md
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       38 2023-02-27 13:24:51.186854 esy-osm-shape-0.2/setup.cfg
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1442 2023-02-16 11:06:18.000000 esy-osm-shape-0.2/setup.py
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/src/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/src/esy/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/src/esy/osm/
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/src/esy/osm/shape/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       55 2023-02-27 13:21:42.000000 esy-osm-shape-0.2/src/esy/osm/shape/__init__.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     6202 2023-01-13 09:48:29.000000 esy-osm-shape-0.2/src/esy/osm/shape/index.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     3252 2022-11-10 09:16:58.000000 esy-osm-shape-0.2/src/esy/osm/shape/mpl.py
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)    12562 2022-11-08 13:59:12.000000 esy-osm-shape-0.2/src/esy/osm/shape/shape.py
-drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2023-02-27 13:24:51.182854 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     2068 2023-02-27 13:24:51.000000 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/PKG-INFO
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)      339 2023-02-27 13:24:51.000000 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/SOURCES.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        1 2023-02-27 13:24:51.000000 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/dependency_links.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       32 2023-02-27 13:24:51.000000 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/requires.txt
--rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        4 2023-02-27 13:24:51.000000 esy-osm-shape-0.2/src/esy_osm_shape.egg-info/top_level.txt
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.318209 esy-osm-shape-0.3/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1088 2024-04-12 10:34:37.000000 esy-osm-shape-0.3/LICENSE
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     9466 2024-04-12 13:58:49.318209 esy-osm-shape-0.3/PKG-INFO
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     7061 2024-04-12 13:31:24.000000 esy-osm-shape-0.3/README.md
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     1231 2024-04-12 12:15:55.000000 esy-osm-shape-0.3/pyproject.toml
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       38 2024-04-12 13:58:49.318209 esy-osm-shape-0.3/setup.cfg
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.314209 esy-osm-shape-0.3/src/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.314209 esy-osm-shape-0.3/src/esy/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.314209 esy-osm-shape-0.3/src/esy/osm/
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.318209 esy-osm-shape-0.3/src/esy/osm/shape/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     7095 2024-04-12 13:23:50.000000 esy-osm-shape-0.3/src/esy/osm/shape/__init__.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     5025 2024-04-11 10:16:29.000000 esy-osm-shape-0.3/src/esy/osm/shape/index.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     5506 2024-04-12 12:10:36.000000 esy-osm-shape-0.3/src/esy/osm/shape/mpl.py
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)    13711 2024-04-11 10:16:29.000000 esy-osm-shape-0.3/src/esy/osm/shape/shape.py
+-rwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)     2101 2024-04-12 13:49:45.000000 esy-osm-shape-0.3/src/esy/osm/shape/test.py
+drwxr-xr-x   0 luen_on  (118004) dlr_luen_on_p (420591)        0 2024-04-12 13:58:49.318209 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)     9466 2024-04-12 13:58:49.000000 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/PKG-INFO
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)      371 2024-04-12 13:58:49.000000 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/SOURCES.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        1 2024-04-12 13:58:49.000000 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/dependency_links.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)       63 2024-04-12 13:58:49.000000 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/requires.txt
+-rw-r--r--   0 luen_on  (118004) dlr_luen_on_p (420591)        4 2024-04-12 13:58:49.000000 esy-osm-shape-0.3/src/esy_osm_shape.egg-info/top_level.txt
```

### Comparing `esy-osm-shape-0.2/src/esy/osm/shape/index.py` & `esy-osm-shape-0.3/src/esy/osm/shape/index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys, zlib, itertools, pickle
 from bisect import bisect
 
 import shapely.geometry
 
-import esy.osm.pbf
+import esy.osm.pbf.index
 from esy.osm.pbf.file import (
     decode_strmap, iter_nodes, iter_ways, iter_relations, Node, Way, Relation
 )
 from esy.osm.shape.shape import multipolygon_shape
 
 
 _blob = esy.osm.pbf.fileformat_pb2.Blob()
@@ -20,29 +20,17 @@
     osmheader = esy.osm.pbf.osmformat_pb2.HeaderBlock()
     osmheader.ParseFromString(esy.osm.pbf.file.read_blob(
         file, block.ofs, block.header.datasize
     ))
     return osmheader
 
 
-def read_blob2(data):
-    '''Read and decompress a openstreetmap blob from `file`.'''
-    _blob.ParseFromString(data)
-    if _blob.raw:
-        return _blob.raw
-    elif _blob.zlib_data:
-        return zlib.decompress(_blob.zlib_data)
-    else:
-        raise ValueError('lzma blob not supported')
-
-
 def unsupported(osm, entry):
     description = '{} (id={})'.format(type(entry).__name__, entry.id)
     return (None, entry.id, {'@error': description})
-    #raise NotImplementedError(description)
     yield
 
 
 def point(osm, node):
     shape = shapely.Point(node.lonlat)
     return (shape, node.id, node.tags)
     yield
@@ -56,48 +44,34 @@
 
 
 def polygon(osm, way):
     outer = shapely.LinearRing(
         [n.lonlat for n in (yield esy.osm.pbf.Node, way.refs)]
     )
 
-    # TODO This seems to happen because all ways with the same start and end
-    # node are treated as polygons. Falling back to a linestring like this is
-    # inefficient.
-    if not outer.is_valid:
-        print('Invalid polygon {}'.format(way.tags))
-        return (shapely.LineString(outer.coords), way.id, way.tags)
-        
     # Switch winding order if necessary.
     if not outer.is_ccw:
         outer = shapely.geometry.polygon.LinearRing(outer.coords[::-1])
 
     shape = shapely.geometry.Polygon(outer)
-    if not shape.is_valid:
-        print(list(shape.exterior.coords))
-        print('Invalid polygon {}'.format(way.tags))
-        return (None, way.id, way.tags)
-        #raise ValueError('Invalid polygon {}'.format(way.tags))
-    return (shape, way.id, way.tags)
+    return (shape if shape.is_valid else None, way.id, way.tags)
 
 
 def multipolygon(osm, relation):
     way_ids = set(
         id for id, type, role in relation.members if type == 'WAY'
     )
 
     ways = {way.id: way for way in (yield esy.osm.pbf.Way, way_ids)}
 
     node_ids = set.union(*(set(w.refs) for w in ways.values()))
     nodes = {entry.id: entry for entry in (yield esy.osm.pbf.Node, node_ids)}
 
     shape = multipolygon_shape(relation, ways, nodes)
-    if not shape.is_valid:
-        raise ValueError('Invalid multipolygon relation {}'.format(relation))
-    return (shape, relation.id, relation.tags)
+    return (shape if shape.is_valid else None, relation.id, relation.tags)
 
 
 def shape_function(entry):
     entry_type = type(entry)
     if entry_type is esy.osm.pbf.Node:
         return point
     elif entry_type is esy.osm.pbf.Way:
@@ -107,32 +81,25 @@
             return linestring
     elif entry_type is esy.osm.pbf.Relation:
         if entry.tags.get('type') == 'multipolygon':
             return multipolygon
     return unsupported
 
 
-#entry_typeids = {
-#    esy.osm.pbf.Node: 0, esy.osm.pbf.Way: 1, esy.osm.pbf.Relation: 2
-#}
-
 osmtypeidxmap = {
     type: idx for idx, type in enumerate(
         (esy.osm.pbf.Node, esy.osm.pbf.Way, esy.osm.pbf.Relation)
     )
 }
 
 
 class Shape(object):
-    # TODO Maybe generalize task batching and expose as general scheme to access
-    # OSM data? Extracting non-shape relations might be handy.
-
     def __init__(self, osm):
         if type(osm) is str:
-            osm = esy.osm.pbf.Index(osm)
+            osm = esy.osm.pbf.index.Index(osm)
         self.osm = osm
 
         header = parse_header_block(self.osm.pbf.file, next(self.osm.pbf.blocks))
         self.box = shapely.geometry.box(
             header.bbox.left / 1000000000, header.bbox.bottom / 1000000000,
             header.bbox.right / 1000000000, header.bbox.top / 1000000000
         )
```

### Comparing `esy-osm-shape-0.2/src/esy/osm/shape/shape.py` & `esy-osm-shape-0.3/src/esy/osm/shape/shape.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,48 @@
 
 
 def is_linestring(entry):
     if type(entry) is not esy.osm.pbf.Way: return False
     return entry.tags.get('area', 'no') == 'no'
 
 
+area_keys = set((
+    'building', 'landuse', 'amenity', 'shop', 'building:part', 'boundary',
+    'historic', 'place', 'area:highway',
+))
+area_highway_values = set(('highway', 'rest_area', 'services', 'platform'))
+area_natural_values = set((
+    'natural', 'water', 'wood', 'scrub', 'wetland', 'grassland', 'heath',
+    'rock', 'bare_rock', 'sand', 'beach', 'scree', 'bay', 'glacier', 'shingle',
+    'fell', 'reef', 'stone', 'mud', 'landslide', 'sinkhole', 'crevasse',
+    'desert',
+))
+area_leisure_values = set(('picnic_table', 'slipway', 'firepit'))
+
+
 def is_polygon(entry):
-    if type(entry) is not esy.osm.pbf.Way: return False
-    if entry.tags.get('area') == 'no': return False
-    return entry.refs[0] == entry.refs[-1]
+    if (
+        type(entry) is not esy.osm.pbf.Way or
+        entry.refs[0] != entry.refs[-1] or
+        entry.tags.get('area') == 'no'
+    ):
+        return False
+
+    # Area filter based on JOSM code:
+    # https://josm.openstreetmap.de/browser/josm/trunk/src/org/openstreetmap/
+    # josm/data/osm/OsmPrimitive.java?rev=18516#L1063
+    return (
+        any(key in entry.tags for key in area_keys) or
+        entry.tags.get('waterway') == 'riverbank' or
+        entry.tags.get('highway') in area_highway_values or
+        entry.tags.get('railway') == 'platform' or
+        entry.tags.get('leisure') not in area_leisure_values or
+        entry.tags.get('natural') in area_natural_values or
+        entry.tags.get('aeroway') == 'aerodrome'
+    )
 
 
 def is_multipolygon(entry):
     if type(entry) is not esy.osm.pbf.Relation: return False
     return entry.tags.get('type') == 'multipolygon'
```

