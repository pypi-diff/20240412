# Comparing `tmp/GeoHD-0.2.4.tar.gz` & `tmp/GeoHD-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.2.4.tar", last modified: Wed Apr 10 15:09:23 2024, max compression
+gzip compressed data, was "GeoHD-0.2.5.tar", last modified: Fri Apr 12 10:00:57 2024, max compression
```

## Comparing `GeoHD-0.2.4.tar` & `GeoHD-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:09:23.003081 GeoHD-0.2.4/
-drwxrwxrwx   0        0        0        0 2024-04-10 15:09:22.992452 GeoHD-0.2.4/GeoHD/
--rw-rw-rw-   0        0        0    14398 2024-04-10 13:56:54.000000 GeoHD-0.2.4/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.2.4/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.2.4/GeoHD/analyze.py
--rw-rw-rw-   0        0        0    13354 2024-04-10 15:04:36.000000 GeoHD-0.2.4/GeoHD/clustering.py
--rw-rw-rw-   0        0        0     5860 2024-04-10 14:39:39.000000 GeoHD-0.2.4/GeoHD/process.py
--rw-rw-rw-   0        0        0    39484 2024-04-10 14:26:39.000000 GeoHD-0.2.4/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.2.4/GeoHD/visualize.py
--rw-rw-rw-   0        0        0     9597 2024-04-09 17:31:08.000000 GeoHD-0.2.4/GeoHD/zone.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:09:22.999326 GeoHD-0.2.4/GeoHD.egg-info/
--rw-rw-rw-   0        0        0     5268 2024-04-10 15:09:22.000000 GeoHD-0.2.4/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-10 15:09:22.000000 GeoHD-0.2.4/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 15:09:22.000000 GeoHD-0.2.4/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-10 15:09:22.000000 GeoHD-0.2.4/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-10 15:09:22.000000 GeoHD-0.2.4/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     5268 2024-04-10 15:09:22.999326 GeoHD-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4772 2024-04-10 15:05:14.000000 GeoHD-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 15:09:23.003081 GeoHD-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      718 2024-04-10 15:05:17.000000 GeoHD-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:09:22.999326 GeoHD-0.2.4/test_local/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.2.4/test_local/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:00:57.925868 GeoHD-0.2.5/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:00:57.916743 GeoHD-0.2.5/GeoHD/
+-rw-rw-rw-   0        0        0    14398 2024-04-11 18:22:13.000000 GeoHD-0.2.5/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      161 2024-04-05 18:06:35.000000 GeoHD-0.2.5/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     5330 2024-04-12 08:52:23.000000 GeoHD-0.2.5/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     5860 2024-04-10 14:39:39.000000 GeoHD-0.2.5/GeoHD/process.py
+-rw-rw-rw-   0        0        0    39256 2024-04-12 08:52:35.000000 GeoHD-0.2.5/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-05 18:31:26.000000 GeoHD-0.2.5/GeoHD/visualize.py
+-rw-rw-rw-   0        0        0    10016 2024-04-12 08:52:35.000000 GeoHD-0.2.5/GeoHD/zone.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:00:57.924671 GeoHD-0.2.5/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0     5591 2024-04-12 10:00:57.000000 GeoHD-0.2.5/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-12 10:00:57.000000 GeoHD-0.2.5/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:00:57.000000 GeoHD-0.2.5/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-12 10:00:57.000000 GeoHD-0.2.5/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-12 10:00:57.000000 GeoHD-0.2.5/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     5591 2024-04-12 10:00:57.924860 GeoHD-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5095 2024-04-12 09:59:09.000000 GeoHD-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 10:00:57.925868 GeoHD-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      718 2024-04-12 09:19:06.000000 GeoHD-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:00:57.922203 GeoHD-0.2.5/test/
+-rw-rw-rw-   0        0        0     2273 2024-04-12 09:42:46.000000 GeoHD-0.2.5/test/test_automation.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:00:57.923201 GeoHD-0.2.5/test_local/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.2.5/test_local/__init__.py
```

### Comparing `GeoHD-0.2.4/GeoHD/AKDE.py` & `GeoHD-0.2.5/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.4/GeoHD/analyze.py` & `GeoHD-0.2.5/GeoHD/analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,13 +140,24 @@
 
     plt.xlabel('Distance')
     plt.ylabel('L Function')
     plt.title('L Function Plot')
     plt.show()
 
 # Example usage:
-# Replace './data/crash.shp' with the path to your shapefile
-# plot_g_function('./data/crash.shp')
-# plot_f_function('./data/crash.shp')
-# plot_j_function('./data/crash.shp')
-# plot_k_function('./data/crash.shp')
-# plot_l_function('./data/crash.shp')
+if __name__ == "__main__":
+    import os
+    # Define the name of the folder to be created
+    folder_name = 'output'
+    # Check if the folder exists, if not, create it
+    if not os.path.exists(folder_name):
+        os.makedirs(folder_name)
+        print(f"Folder '{folder_name}' has been created.")
+    else:
+        print(f"Folder '{folder_name}' already exists.")
+    # Example usage:
+    # Replace './data/crash.shp' with the path to your shapefile
+    plot_g_function('./data/crash.shp')
+    plot_f_function('./data/crash.shp')
+    plot_j_function('./data/crash.shp')
+    plot_k_function('./data/crash.shp')
+    plot_l_function('./data/crash.shp')
```

### Comparing `GeoHD-0.2.4/GeoHD/process.py` & `GeoHD-0.2.5/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.4/GeoHD/utils.py` & `GeoHD-0.2.5/GeoHD/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,17 +987,7 @@
                 print(f"  {col}: {row[col]}")
         
         return True  # The file is a valid GeoDataFrame
     except Exception as e:
         print("Error:", e)
         return False  # The file is not a valid GeoDataFrame
 
-
-
-
-
-
-# Example usage:
-if __name__ == "__main__":
-    density_data_path = './output/AKDE_density_grid.npy'
-    hotspots = extract_hotspots(density_data_path)
-    visualize_hotspots(np.load(density_data_path), hotspots)
```

### Comparing `GeoHD-0.2.4/GeoHD/visualize.py` & `GeoHD-0.2.5/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.4/GeoHD/zone.py` & `GeoHD-0.2.5/GeoHD/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,20 +226,30 @@
     intersections.plot(column='point_count', cmap='Blues', edgecolor='black', linewidth=0.5, ax=ax, legend=True)
     area.plot(ax=ax, color='none', edgecolor='black')
     plt.title('Heatmap of Hexagonal Grids based on Crash Point Count')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.show()
 
+# Example usage:
+if __name__ == "__main__":
+    import os
+    # Define the name of the folder to be created
+    folder_name = 'output'
+    # Check if the folder exists, if not, create it
+    if not os.path.exists(folder_name):
+        os.makedirs(folder_name)
+        print(f"Folder '{folder_name}' has been created.")
+    else:
+        print(f"Folder '{folder_name}' already exists.")
+
+    # Example usage
+    create_cell_zones('./data/area.shp', './data/crash.shp')
 
+    # Example usage
+    create_hex_grid_zones('./data/area.shp', './data/crash.shp')
 
-# Example usage
-# create_cell_zones('./data/area.shp', './data/crash.shp')
+    # Example usage
+    create_cell_heatmap('./data/area.shp', './data/crash.shp')
 
-# Example usage
-# create_hex_grid_zones('./data/area.shp', './data/crash.shp')
-
-# Example usage
-# create_cell_heatmap('./data/area.shp', './data/crash.shp')
-
-# Example usage
-# create_hexagonal_heatmap('./data/area.shp', './data/crash.shp')
+    # Example usage
+    create_hexagonal_heatmap('./data/area.shp', './data/crash.shp')
```

### Comparing `GeoHD-0.2.4/GeoHD.egg-info/PKG-INFO` & `GeoHD-0.2.5/GeoHD.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.4-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.4-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.5-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.5-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -36,62 +36,75 @@
 * Culture ([Zhang, Haiping, et al.  (2021)](https://doi.org/10.1111/tgis.12682))
 * Ecology ([Qian, Chunhua, et al.  (2021)](https://doi.org/10.1177/15501477211039137))
 
 The main functions of GeoHD are fast visualization and hotspot detection based on geospatial point data, and it realizes fixed-bandwidth hotspot detection with adjustable parameters and adaptive-bandwidth hotspot detection. In addition, GeoHD provides spatial point pattern distribution analysis such as Ripley G-function calculation and fast comparison image drawing.
 
 ## Getting Started
 
+### Documentation
+
+We recommend starting your GeoHD journey with the [documentation](https://geohd.readthedocs.io/en/latest/).
+
 ### Install with pip
 
 The package is available in PyPi and requires [Python 3.11](https://www.python.org/downloads/) or higher. It can be installed using:
 
 ```bash
 $ pip install GeoHD
 ```
 
 ### Usage
 
+A case-testing approach:
+
+```bash
+$ cd test
+$ python -m test_automation
+```
+
+You can also run `test.ipynb` in jupyter notebook
+
 Visualization of hotspots on real maps:
 
 ```python
 visualize_shapefile('data.shp', output_image_path='custom_image.png')
 ```
 
 <p align="center">
-  <img src="./doc/1.png" width="400" height="300"/>
+  <img src="./picture/1.png" width="400" height="300"/>
 </p>
 
 
 Analytic Plane Point Patterns: Ripley G, Ripley F, Ripley J, Ripley K, Ripley L, etc. through the plotting function.
 
 ```python
 plot_g_function('data.shp')
 ```
 
 <p align="center">
-  <img src="./doc/2.png" width="400" height="300"/>
+  <img src="./picture/2.png" width="400" height="300"/>
 </p>
 
 The study area was divided into a quadrilateral (hexagonal) grid and fast visualization was achieved based on the density of point data within the divided area.
 
 ```python
 create_cell_zones(area_file, crash_file)
 create_hex_grid_zones(area_file, crash_file)
 create_cell_heatmap(area_file, crash_file)
 create_hexagonal_heatmap(area_file, crash_file)
 ```
 
 <p align="center">
-  <img src="./doc/3.png" width="400" height="300"/>
-  <img src="./doc/4.png" width="400" height="300"/>
+  <img src="./picture/3.png" width="400" height="300"/>
+  <img src="./picture/4.png" width="400" height="300"/>
 </p>
 
 <p align="center">
-  <img src="./doc/5.png" width="400" height="300"/>
-  <img src="./doc/6.png" width="400" height="300"/>
+  <img src="./picture/5.png" width="400" height="300"/>
+  <img src="./picture/6.png" width="400" height="300"/>
 </p>
 
 Realization of kernel density analysis with fixed bandwidth:
 
 ```python
 density_raster = process_shapefile(input_file_path)
 plot_density_raster(density_raster,output_data_path, *gpd.read_file(input_file_path).total_bounds)
@@ -100,27 +113,27 @@
 Kernel density analysis for realizing adaptive bandwidth:
 
 ```python
 adaptiveKDE(shp_file,output_data_path)
 ```
 
 <p align="center">
-  <img src="./doc/8.png" width="400" height="300"/>
+  <img src="./picture/8.png" width="400" height="300"/>
 </p>
 
 
 Hotspot Identification:
 
 ```python
 hotspots = extract_hotspots(density_data_path)
 visualize_hotspots(np.load(density_data_path), hotspots)
 ```
 
 <p align="center">
-  <img src="./doc/9.png" width="400" height="300"/>
+  <img src="./picture/9.png" width="400" height="300"/>
 </p>
 
 
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with GeoHD, please create a post using our package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
@@ -133,12 +146,12 @@
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
-
-
 ## Authors
 
 * Yuchen Yan
+* Yuxin Wang
+* Wei Quan
```

### Comparing `GeoHD-0.2.4/LICENSE` & `GeoHD-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.2.4/PKG-INFO` & `GeoHD-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoHD
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data
 Home-page: https://github.com/yan-yuchen/GeoHD
 Author: Yuchen Yan
 Author-email: ycyan001@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -14,16 +14,16 @@
 Requires-Dist: geopandas
 Requires-Dist: pointpats
 Requires-Dist: h3
 
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.4-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.4-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.5-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.5-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -36,62 +36,75 @@
 * Culture ([Zhang, Haiping, et al.  (2021)](https://doi.org/10.1111/tgis.12682))
 * Ecology ([Qian, Chunhua, et al.  (2021)](https://doi.org/10.1177/15501477211039137))
 
 The main functions of GeoHD are fast visualization and hotspot detection based on geospatial point data, and it realizes fixed-bandwidth hotspot detection with adjustable parameters and adaptive-bandwidth hotspot detection. In addition, GeoHD provides spatial point pattern distribution analysis such as Ripley G-function calculation and fast comparison image drawing.
 
 ## Getting Started
 
+### Documentation
+
+We recommend starting your GeoHD journey with the [documentation](https://geohd.readthedocs.io/en/latest/).
+
 ### Install with pip
 
 The package is available in PyPi and requires [Python 3.11](https://www.python.org/downloads/) or higher. It can be installed using:
 
 ```bash
 $ pip install GeoHD
 ```
 
 ### Usage
 
+A case-testing approach:
+
+```bash
+$ cd test
+$ python -m test_automation
+```
+
+You can also run `test.ipynb` in jupyter notebook
+
 Visualization of hotspots on real maps:
 
 ```python
 visualize_shapefile('data.shp', output_image_path='custom_image.png')
 ```
 
 <p align="center">
-  <img src="./doc/1.png" width="400" height="300"/>
+  <img src="./picture/1.png" width="400" height="300"/>
 </p>
 
 
 Analytic Plane Point Patterns: Ripley G, Ripley F, Ripley J, Ripley K, Ripley L, etc. through the plotting function.
 
 ```python
 plot_g_function('data.shp')
 ```
 
 <p align="center">
-  <img src="./doc/2.png" width="400" height="300"/>
+  <img src="./picture/2.png" width="400" height="300"/>
 </p>
 
 The study area was divided into a quadrilateral (hexagonal) grid and fast visualization was achieved based on the density of point data within the divided area.
 
 ```python
 create_cell_zones(area_file, crash_file)
 create_hex_grid_zones(area_file, crash_file)
 create_cell_heatmap(area_file, crash_file)
 create_hexagonal_heatmap(area_file, crash_file)
 ```
 
 <p align="center">
-  <img src="./doc/3.png" width="400" height="300"/>
-  <img src="./doc/4.png" width="400" height="300"/>
+  <img src="./picture/3.png" width="400" height="300"/>
+  <img src="./picture/4.png" width="400" height="300"/>
 </p>
 
 <p align="center">
-  <img src="./doc/5.png" width="400" height="300"/>
-  <img src="./doc/6.png" width="400" height="300"/>
+  <img src="./picture/5.png" width="400" height="300"/>
+  <img src="./picture/6.png" width="400" height="300"/>
 </p>
 
 Realization of kernel density analysis with fixed bandwidth:
 
 ```python
 density_raster = process_shapefile(input_file_path)
 plot_density_raster(density_raster,output_data_path, *gpd.read_file(input_file_path).total_bounds)
@@ -100,27 +113,27 @@
 Kernel density analysis for realizing adaptive bandwidth:
 
 ```python
 adaptiveKDE(shp_file,output_data_path)
 ```
 
 <p align="center">
-  <img src="./doc/8.png" width="400" height="300"/>
+  <img src="./picture/8.png" width="400" height="300"/>
 </p>
 
 
 Hotspot Identification:
 
 ```python
 hotspots = extract_hotspots(density_data_path)
 visualize_hotspots(np.load(density_data_path), hotspots)
 ```
 
 <p align="center">
-  <img src="./doc/9.png" width="400" height="300"/>
+  <img src="./picture/9.png" width="400" height="300"/>
 </p>
 
 
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with GeoHD, please create a post using our package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
@@ -133,12 +146,12 @@
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
-
-
 ## Authors
 
 * Yuchen Yan
+* Yuxin Wang
+* Wei Quan
```

### Comparing `GeoHD-0.2.4/README.md` & `GeoHD-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # GeoHD
 
 ![python](https://img.shields.io/badge/python-3.11-black)
-![GitHub release](https://img.shields.io/badge/release-v0.2.4-blue)
-![pypi](https://img.shields.io/badge/pypi-v0.2.4-orange)
+![GitHub release](https://img.shields.io/badge/release-v0.2.5-blue)
+![pypi](https://img.shields.io/badge/pypi-v0.2.5-orange)
 ![license](https://img.shields.io/badge/license-GNU%20AGPLv3-green)
 
 [**Getting Started**](#getting-started)
 | [**Issues**](#issues)
 | [**Contribute**](#contribute)
 | [**Citation**](#citation)
 | [**Authors**](#authors)
@@ -19,62 +19,75 @@
 * Culture ([Zhang, Haiping, et al.  (2021)](https://doi.org/10.1111/tgis.12682))
 * Ecology ([Qian, Chunhua, et al.  (2021)](https://doi.org/10.1177/15501477211039137))
 
 The main functions of GeoHD are fast visualization and hotspot detection based on geospatial point data, and it realizes fixed-bandwidth hotspot detection with adjustable parameters and adaptive-bandwidth hotspot detection. In addition, GeoHD provides spatial point pattern distribution analysis such as Ripley G-function calculation and fast comparison image drawing.
 
 ## Getting Started
 
+### Documentation
+
+We recommend starting your GeoHD journey with the [documentation](https://geohd.readthedocs.io/en/latest/).
+
 ### Install with pip
 
 The package is available in PyPi and requires [Python 3.11](https://www.python.org/downloads/) or higher. It can be installed using:
 
 ```bash
 $ pip install GeoHD
 ```
 
 ### Usage
 
+A case-testing approach:
+
+```bash
+$ cd test
+$ python -m test_automation
+```
+
+You can also run `test.ipynb` in jupyter notebook
+
 Visualization of hotspots on real maps:
 
 ```python
 visualize_shapefile('data.shp', output_image_path='custom_image.png')
 ```
 
 <p align="center">
-  <img src="./doc/1.png" width="400" height="300"/>
+  <img src="./picture/1.png" width="400" height="300"/>
 </p>
 
 
 Analytic Plane Point Patterns: Ripley G, Ripley F, Ripley J, Ripley K, Ripley L, etc. through the plotting function.
 
 ```python
 plot_g_function('data.shp')
 ```
 
 <p align="center">
-  <img src="./doc/2.png" width="400" height="300"/>
+  <img src="./picture/2.png" width="400" height="300"/>
 </p>
 
 The study area was divided into a quadrilateral (hexagonal) grid and fast visualization was achieved based on the density of point data within the divided area.
 
 ```python
 create_cell_zones(area_file, crash_file)
 create_hex_grid_zones(area_file, crash_file)
 create_cell_heatmap(area_file, crash_file)
 create_hexagonal_heatmap(area_file, crash_file)
 ```
 
 <p align="center">
-  <img src="./doc/3.png" width="400" height="300"/>
-  <img src="./doc/4.png" width="400" height="300"/>
+  <img src="./picture/3.png" width="400" height="300"/>
+  <img src="./picture/4.png" width="400" height="300"/>
 </p>
 
 <p align="center">
-  <img src="./doc/5.png" width="400" height="300"/>
-  <img src="./doc/6.png" width="400" height="300"/>
+  <img src="./picture/5.png" width="400" height="300"/>
+  <img src="./picture/6.png" width="400" height="300"/>
 </p>
 
 Realization of kernel density analysis with fixed bandwidth:
 
 ```python
 density_raster = process_shapefile(input_file_path)
 plot_density_raster(density_raster,output_data_path, *gpd.read_file(input_file_path).total_bounds)
@@ -83,27 +96,27 @@
 Kernel density analysis for realizing adaptive bandwidth:
 
 ```python
 adaptiveKDE(shp_file,output_data_path)
 ```
 
 <p align="center">
-  <img src="./doc/8.png" width="400" height="300"/>
+  <img src="./picture/8.png" width="400" height="300"/>
 </p>
 
 
 Hotspot Identification:
 
 ```python
 hotspots = extract_hotspots(density_data_path)
 visualize_hotspots(np.load(density_data_path), hotspots)
 ```
 
 <p align="center">
-  <img src="./doc/9.png" width="400" height="300"/>
+  <img src="./picture/9.png" width="400" height="300"/>
 </p>
 
 
 
 ## Issues
 
 If you encounter any **bugs** or **problems** with GeoHD, please create a post using our package [issue tracker](https://github.com/yan-yuchen/GeoHD/issues). Please provide a clear and concise description of the problem, with images or code-snippets where appropriate. We will do our best to address these problems as fast and efficiently as possible.
@@ -116,12 +129,12 @@
 * Ensure your modifications or additions adhere to the existing standard of the GeoHD package, specifically detailed documentation for new methods (see existing methods for example documentation)
 * Test your modifications to ensure that the core functionality of the package has not been altered by running the unit tests 
 * Once the issue has been discussed with a package author, you may open a pull request containing your modifications
 
 ## Citation
 
 
-
-
 ## Authors
 
 * Yuchen Yan
+* Yuxin Wang
+* Wei Quan
```

### Comparing `GeoHD-0.2.4/setup.py` & `GeoHD-0.2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='GeoHD',
-    version='0.2.4',
+    version='0.2.5',
     description='A Python toolkit for geospatial hotspot detection, Avisualization, and analysis using urban data',
     author='Yuchen Yan',
     author_email='ycyan001@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yan-yuchen/GeoHD",    
     packages=find_packages(),
```

