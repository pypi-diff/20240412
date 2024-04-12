# Comparing `tmp/geoserver-rest-2.5.3.tar.gz` & `tmp/geoserver-rest-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoserver-rest-2.5.3.tar", last modified: Thu Nov  9 16:54:45 2023, max compression
+gzip compressed data, was "geoserver-rest-2.6.0.tar", last modified: Fri Jan 26 22:25:40 2024, max compression
```

## Comparing `geoserver-rest-2.5.3.tar` & `geoserver-rest-2.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:54:45.448179 geoserver-rest-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2023-11-09 16:54:45.448179 geoserver-rest-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:54:45.444179 geoserver-rest-2.5.3/geo/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/Calculation_gdal.py
--rw-r--r--   0 runner    (1001) docker     (127)    79371 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/Geoserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    13227 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/Style.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/geo/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:54:45.444179 geoserver-rest-2.5.3/geoserver_rest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2023-11-09 16:54:45.000000 geoserver-rest-2.5.3/geoserver_rest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-11-09 16:54:45.000000 geoserver-rest-2.5.3/geoserver_rest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 16:54:45.000000 geoserver-rest-2.5.3/geoserver_rest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-09 16:54:45.000000 geoserver-rest-2.5.3/geoserver_rest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-09 16:54:45.000000 geoserver-rest-2.5.3/geoserver_rest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-09 16:54:45.448179 geoserver-rest-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 16:54:45.444179 geoserver-rest-2.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/tests/test_geoserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2023-11-09 16:54:30.000000 geoserver-rest-2.5.3/tests/test_layergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:25:40.576900 geoserver-rest-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-01-26 22:25:40.576900 geoserver-rest-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:25:40.572900 geoserver-rest-2.6.0/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/Calculation_gdal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80566 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/Geoserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/Style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/geo/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:25:40.572900 geoserver-rest-2.6.0/geoserver_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-01-26 22:25:40.000000 geoserver-rest-2.6.0/geoserver_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-01-26 22:25:40.000000 geoserver-rest-2.6.0/geoserver_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 22:25:40.000000 geoserver-rest-2.6.0/geoserver_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-26 22:25:40.000000 geoserver-rest-2.6.0/geoserver_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-26 22:25:40.000000 geoserver-rest-2.6.0/geoserver_rest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-26 22:25:40.576900 geoserver-rest-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 22:25:40.572900 geoserver-rest-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5520 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/tests/test_geoserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-01-26 22:25:30.000000 geoserver-rest-2.6.0/tests/test_layergroup.py
```

### Comparing `geoserver-rest-2.5.3/LICENSE` & `geoserver-rest-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/PKG-INFO` & `geoserver-rest-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoserver-rest
-Version: 2.5.3
+Version: 2.6.0
 Summary: Package for GeoServer rest API
 Home-page: https://github.com/iamtekson/geoserver-rest-python
 Author: Tek Kshetri
 Author-email: iamtekson@gmail.com
 License: MIT License
 Keywords: geoserver-rest-python,geoserver rest,python geoserver,geoserver api,api,rest geoserver,python,geoserver python,geoserver rest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geoserver-rest-2.5.3/README.md` & `geoserver-rest-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/geo/Calculation_gdal.py` & `geoserver-rest-2.6.0/geo/Calculation_gdal.py`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/geo/Geoserver.py` & `geoserver-rest-2.6.0/geo/Geoserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,18 +607,18 @@
             assert isinstance(workspace, str), "Workspace must be of type String:''"
             # check if the workspace is valid in Geoserver
             if self.get_workspace(workspace) is None:
                 raise Exception("Workspace is not valid in Geoserver Instance")
 
         supported_modes: Set = {
             "single",
-            "opaque container",
-            "named tree",
-            "container tree",
-            "earth observation tree",
+            "opaque",
+            "named",
+            "container",
+            "eo",
         }
         supported_formats: Set = {"html", "json", "xml"}
 
         if mode.lower() != "single" and mode.lower() not in supported_modes:
             raise Exception(
                 f"Mode not supported. Acceptable modes are : {supported_modes}"
             )
@@ -638,27 +638,31 @@
             raise Exception(f"Layergroup: {name} already exist in Geoserver instance")
 
         if len(layers) == 0:
             raise Exception("No layer provided!")
         else:
             for layer in layers:
                 # check if it is valid in geoserver
-
-                if (
+                try:
+                    # Layer check
                     self.get_layer(
                         layer_name=layer,
                         workspace=workspace if workspace is not None else None,
                     )
-                    is not None
-                ):
-                    ...
-                else:
-                    raise Exception(
-                        f"Layer: {layer} is not a valid layer in the Geoserver instance"
-                    )
+                except GeoserverException:
+                    try:
+                        # Layer group check
+                        self.get_layergroup(
+                            layer_name=layer,
+                            workspace=workspace if workspace is not None else None,
+                        )
+                    except GeoserverException:
+                        raise Exception(
+                            f"Layer: {layer} is not a valid layer in the Geoserver instance"
+                        )
 
         skeleton = ""
 
         if workspace:
             skeleton += f"<workspace><name>{workspace}</name></workspace>"
         # metadata structure = [{about:"",content_url:""},{...}]
         metadata_xml_list = []
@@ -679,16 +683,26 @@
                 )
 
             metadata_xml = f"<metadataLinks>{''.join(['{}'] * len(metadata_xml_list)).format(*metadata_xml_list)}</metadataLinks>"
             skeleton += metadata_xml
         layers_xml_list: List[str] = []
 
         for layer in layers:
+            published_type = "layer"
+            try:
+                # Layer check
+                self.get_layer(
+                    layer_name=layer,
+                    workspace=workspace if workspace is not None else None,
+                )
+            except GeoserverException: # It's a layer group
+                published_type = "layerGroup"
+
             layers_xml_list.append(
-                f"""<published type="layer">
+                f"""<published type="{published_type}">
                             <name>{layer}</name>
                             <link>{self.service_url}/layers/{layer}.xml</link>
                         </published>
                     """
             )
 
         layers_xml: str = f"<publishables>{''.join(['{}'] * len(layers)).format(*layers_xml_list)}</publishables>"
@@ -1163,25 +1177,27 @@
         self,
         raster_path: str,
         style_name: Optional[str] = None,
         workspace: str = None,
         color_ramp: str = "RdYlGn_r",
         cmap_type: str = "ramp",
         number_of_classes: int = 5,
+        opacity: float = 1,
     ):
         """Dynamically create style for raster.
 
         Parameters
         ----------
         raster_path : str
         style_name : str, optional
         workspace : str
         color_ramp : str
         cmap_type : str TODO: This should be a set of the available options : {"ramp", "linear", ... }
         number_of_classes : int
+        opacity : float
         overwrite : bool
 
         Notes
         -----
         The name of the style file will be, rasterName:workspace
         This function will dynamically create the style file for raster.
         Inputs: name of file, workspace, cmap_type (two options: values, range), ncolors: determines the number of class, min for minimum value of the raster, max for the max value of raster
@@ -1195,14 +1211,15 @@
         coverage_style_xml(
             color_ramp,
             style_name,
             cmap_type,
             min_value,
             max_value,
             number_of_classes,
+            opacity,
         )
         style_xml = "<style><name>{}</name><filename>{}</filename></style>".format(
             style_name, style_name + ".sld"
         )
 
         if style_name is None:
             style_name = os.path.basename(raster_path)
@@ -1307,14 +1324,15 @@
         else:
             raise GeoserverException(r.status_code, r.content)
 
     def create_outline_featurestyle(
         self,
         style_name: str,
         color: str = "#3579b1",
+        width: str = "2",
         geom_type: str = "polygon",
         workspace: Optional[str] = None,
     ):
         """Dynamically creates the outline style for postgis geometry
 
         Parameters
         ----------
@@ -1328,15 +1346,15 @@
         -------
 
         Notes
         -----
         The geometry type must be point, line or polygon
         Inputs: style_name (name of the style file in geoserver), workspace, color (style color)
         """
-        outline_only_xml(color, geom_type)
+        outline_only_xml(color, width, geom_type)
 
         style_xml = "<style><name>{}</name><filename>{}</filename></style>".format(
             style_name, style_name + ".sld"
         )
 
         headers = {"content-type": "text/xml"}
         url = "{}/rest/workspaces/{}/styles".format(self.service_url, workspace)
@@ -1796,27 +1814,29 @@
         store_name: str,
         pg_table: str,
         workspace: Optional[str] = None,
         title: Optional[str] = None,
         advertised: Optional[bool] = True,
         abstract: Optional[str] = None,
         keywords: Optional[List[str]] = None,
+        cqlfilter: Optional[str] = None
     ):
         """
         Publish a featurestore to geoserver.
 
         Parameters
         ----------
         store_name : str
         pg_table : str
         workspace : str, optional
         title : str, optional
         advertised : bool, optional
         abstract : str, optional
         keywords : list, optional
+        cqlfilter : str, optional
 
         Returns
         -------
 
         Notes
         -----
         Only user for postgis vector data
@@ -1835,20 +1855,22 @@
         keywords_xml = ""
         if keywords:
             keywords_xml = "<keywords>"
             for keyword in keywords:
                 keywords_xml += f"<string>{keyword}</string>"
             keywords_xml += "</keywords>"
 
+        cqlfilter_xml = f"<cqlFilter>{cqlfilter}</cqlFilter>" if cqlfilter else ""
         layer_xml = f"""<featureType>
                     <name>{pg_table}</name>
                     <title>{title}</title>
                     <advertised>{advertised}</advertised>
                     {abstract_xml}
                     {keywords_xml}
+                    {cqlfilter_xml}
                 </featureType>"""
         headers = {"content-type": "text/xml"}
 
         r = requests.post(
             url,
             data=layer_xml,
             auth=(self.username, self.password),
@@ -1864,19 +1886,21 @@
         store_name: str,
         workspace: Optional[str],
         pg_table: str,
         name: str,
         title: str,
         abstract: Optional[str] = None,
         keywords: Optional[List[str]] = None,
+        recalculate : Optional[str] = None
     ):
         """
 
         Parameters
         ----------
+        recalculate : str, optional. Recalculate param. Can be: empty string, nativebbox and nativebbox,latlonbbox
         store_name : str
         workspace : str, optional
         pg_table : str
         name : str
         title : str
         abstract : str, optional
         keywords : list, optional
@@ -1886,27 +1910,30 @@
 
         Notes
         -----
         """
         if workspace is None:
             workspace = "default"
 
-        url = "{}/rest/workspaces/{}/datastores/{}/featuretypes/{}.xml".format(
-            self.service_url, workspace, store_name, pg_table
+        recalculate_param = f"?recalculate={recalculate}" if recalculate else ""
+
+        url = "{}/rest/workspaces/{}/datastores/{}/featuretypes/{}.xml{}".format(
+            self.service_url, workspace, store_name, pg_table, recalculate_param
         )
 
         # Create XML for abstract and keywords
         abstract_xml = f"<abstract>{abstract}</abstract>" if abstract else ""
         keywords_xml = ""
         if keywords:
             keywords_xml = "<keywords>"
             for keyword in keywords:
                 keywords_xml += f"<string>{keyword}</string>"
             keywords_xml += "</keywords>"
 
+
         layer_xml = f"""<featureType>
                     <name>{name}</name>
                     <title>{title}</title>
                     {abstract_xml}{keywords_xml}
                     </featureType>"""
         headers = {"content-type": "text/xml"}
```

### Comparing `geoserver-rest-2.5.3/geo/Style.py` & `geoserver-rest-2.6.0/geo/Style.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 )
             )
 
     return style_append
 
 
 def coverage_style_xml(
-    color_ramp, style_name, cmap_type, min_value, max_value, number_of_classes
+    color_ramp, style_name, cmap_type, min_value, max_value, number_of_classes, opacity
 ):
     min_max_difference = max_value - min_value
     style_append = ""
     interval = min_max_difference / (number_of_classes - 1)  # noqa
 
     # The main style of the coverage style
     if isinstance(color_ramp, str):
@@ -104,14 +104,15 @@
         <sld:FeatureTypeConstraint/>
         </sld:LayerFeatureConstraints>
         <sld:UserStyle>
         <sld:Name>{2}</sld:Name>
         <sld:FeatureTypeStyle>
             <sld:Rule>
             <sld:RasterSymbolizer>
+                <sld:Opacity>{3}</sld:Opacity>
                 <sld:ChannelSelection>
                 <sld:GrayChannel>
                     <sld:SourceChannelName>1</sld:SourceChannelName>
                 </sld:GrayChannel>
                 </sld:ChannelSelection>
                 <sld:ColorMap type="{0}">
                     {1}
@@ -119,22 +120,22 @@
             </sld:RasterSymbolizer>
             </sld:Rule>
         </sld:FeatureTypeStyle>
         </sld:UserStyle>
     </UserLayer>
     </StyledLayerDescriptor>
     """.format(
-        cmap_type, style_append, style_name
+        cmap_type, style_append, style_name, opacity
     )
 
     with open("style.sld", "w") as f:
         f.write(style)
 
 
-def outline_only_xml(color, geom_type="polygon"):
+def outline_only_xml(color, width, geom_type="polygon"):
     if geom_type == "point":
         symbolizer = """
             <PointSymbolizer>
                 <Graphic>
                 <Mark>
                     <WellKnownName>circle</WellKnownName>
                     <Fill>
@@ -149,34 +150,31 @@
         )
 
     elif geom_type == "line":
         symbolizer = """
                 <LineSymbolizer>
                     <Stroke>
                     <CssParameter name="stroke">{}</CssParameter>
-                    <CssParameter name="stroke-width">3</CssParameter>
+                    <CssParameter name="stroke-width"{}</CssParameter>
                     </Stroke>
                 </LineSymbolizer>
             """.format(
-            color
+            color, width
         )
 
     elif geom_type == "polygon":
         symbolizer = """
                 <PolygonSymbolizer>
-                    <Fill>
-                        <CssParameter name="fill">#FFFFFF</CssParameter>
-                    </Fill>
                     <Stroke>
                     <CssParameter name="stroke">{}</CssParameter>
-                    <CssParameter name="stroke-width">0.26</CssParameter>
+                    <CssParameter name="stroke-width">{}</CssParameter>
                     </Stroke>
                 </PolygonSymbolizer>
             """.format(
-            color
+            color, width
         )
 
     else:
         print("Error: Invalid geometry type")
         return
 
     style = """
```

### Comparing `geoserver-rest-2.5.3/geo/supports.py` & `geoserver-rest-2.6.0/geo/supports.py`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/geoserver_rest.egg-info/PKG-INFO` & `geoserver-rest-2.6.0/geoserver_rest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoserver-rest
-Version: 2.5.3
+Version: 2.6.0
 Summary: Package for GeoServer rest API
 Home-page: https://github.com/iamtekson/geoserver-rest-python
 Author: Tek Kshetri
 Author-email: iamtekson@gmail.com
 License: MIT License
 Keywords: geoserver-rest-python,geoserver rest,python geoserver,geoserver api,api,rest geoserver,python,geoserver python,geoserver rest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `geoserver-rest-2.5.3/setup.py` & `geoserver-rest-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/tests/test_geoserver.py` & `geoserver-rest-2.6.0/tests/test_geoserver.py`

 * *Files identical despite different names*

### Comparing `geoserver-rest-2.5.3/tests/test_layergroup.py` & `geoserver-rest-2.6.0/tests/test_layergroup.py`

 * *Files identical despite different names*

