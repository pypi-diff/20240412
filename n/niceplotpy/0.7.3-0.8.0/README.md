# Comparing `tmp/niceplotpy-0.7.3.tar.gz` & `tmp/niceplotpy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niceplotpy-0.7.3.tar", last modified: Mon Mar 25 15:52:40 2024, max compression
+gzip compressed data, was "niceplotpy-0.8.0.tar", last modified: Fri Apr 12 09:48:41 2024, max compression
```

## Comparing `niceplotpy-0.7.3.tar` & `niceplotpy-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:52:40.994234 niceplotpy-0.7.3/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3439 2024-03-25 15:52:40.994234 niceplotpy-0.7.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2839 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:52:40.991235 niceplotpy-0.7.3/niceplot/
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2791 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:52:40.992235 niceplotpy-0.7.3/niceplot/data/
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     7579 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     9356 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     3486 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv
--rw-rw-rw-   0 root         (0) root         (0)     4423 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv
--rw-rw-rw-   0 root         (0) root         (0)     3706 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/draw1d.py
--rw-rw-rw-   0 root         (0) root         (0)     5699 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/draw2d.py
--rw-rw-rw-   0 root         (0) root         (0)     6716 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/process_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)     5095 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     8187 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/niceplot/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 15:52:40.994234 niceplotpy-0.7.3/niceplotpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3439 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      736 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       84 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-25 15:52:40.000000 niceplotpy-0.7.3/niceplotpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 15:52:40.994234 niceplotpy-0.7.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-03-25 15:52:26.000000 niceplotpy-0.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2397 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.714411 niceplotpy-0.8.0/niceplot/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3789 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.715411 niceplotpy-0.8.0/niceplot/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     7579 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3486 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv
+-rw-rw-rw-   0 root         (0) root         (0)     4423 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv
+-rw-rw-rw-   0 root         (0) root         (0)     5079 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw1dratio.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw2dhist.py
+-rw-rw-rw-   0 root         (0) root         (0)     3736 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/draw2dscatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/process_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)     5095 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8445 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/niceplot/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/niceplotpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      771 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 09:48:41.000000 niceplotpy-0.8.0/niceplotpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 09:48:41.716411 niceplotpy-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-04-12 09:48:32.000000 niceplotpy-0.8.0/setup.py
```

### Comparing `niceplotpy-0.7.3/PKG-INFO` & `niceplotpy-0.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplotpy
-Version: 0.7.3
+Version: 0.8.0
 Summary: A package collecting things to make nice plots from root files
 Home-page: https://gitlab.cern.ch/jwuerzin/nice-plot
 Author: Jonas Wuerzinger
 Author-email: jonas.wuerzinger@tum.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -33,15 +33,15 @@
 After installation, the the module can be used with:
 
 ```python
 niceplot CONFIG_FILE
 ```
 Where the `CONFIG_FILE` includes all information on which plots to make, variables to plot, etc. 
 
-Currently supported plot types are: `1dratio` and `2dhist`. For a detailled example config file, see: [example_configs/GMSB.yaml](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/GMSB.yaml). Here a shortened example config file:
+Currently supported plot types are: `1dratio`, `2dhist` and `2dscatter`. For detailled example config files, see: [example_configs](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/). Here a shortened example config file:
 
 ```yaml
 input_file: 'data/susy.root'
 output_dir: 'plots/GMSB_Factory'
 treename: 'susy'
 configurations:
   - name: 'GMSBpresel'
@@ -69,17 +69,16 @@
       - 'BF_chi_10_to_e_L'
       - 'BF_chi_10_to_e_R'
     # 1D histograms:
     - {<<: *ploting_common, x: !evaluate "${BF}" }
     # 2D histograms:
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True }
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
+  
+  - { type: 2dscatter, x: 'BF_chi_10_to_gravitino_Z', y: 'BF_chi_10_to_gravitino_gam', z: 'EWSummary_ObsCLs_Overall', range: [ [0, 1.], [0, 1.]], subdir: '2dscatter'}
 ```
 
 ## ToDo:
 
+- Move 2Dscatterplot grid to background.
 - Add more options for plots:
-  - 2dplot with custom z-axis
   - data/MC plots
```

### Comparing `niceplotpy-0.7.3/README.md` & `niceplotpy-0.8.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 After installation, the the module can be used with:
 
 ```python
 niceplot CONFIG_FILE
 ```
 Where the `CONFIG_FILE` includes all information on which plots to make, variables to plot, etc. 
 
-Currently supported plot types are: `1dratio` and `2dhist`. For a detailled example config file, see: [example_configs/GMSB.yaml](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/GMSB.yaml). Here a shortened example config file:
+Currently supported plot types are: `1dratio`, `2dhist` and `2dscatter`. For detailled example config files, see: [example_configs](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/). Here a shortened example config file:
 
 ```yaml
 input_file: 'data/susy.root'
 output_dir: 'plots/GMSB_Factory'
 treename: 'susy'
 configurations:
   - name: 'GMSBpresel'
@@ -53,17 +53,16 @@
       - 'BF_chi_10_to_e_L'
       - 'BF_chi_10_to_e_R'
     # 1D histograms:
     - {<<: *ploting_common, x: !evaluate "${BF}" }
     # 2D histograms:
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True }
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
+  
+  - { type: 2dscatter, x: 'BF_chi_10_to_gravitino_Z', y: 'BF_chi_10_to_gravitino_gam', z: 'EWSummary_ObsCLs_Overall', range: [ [0, 1.], [0, 1.]], subdir: '2dscatter'}
 ```
 
 ## ToDo:
 
+- Move 2Dscatterplot grid to background.
 - Add more options for plots:
-  - 2dplot with custom z-axis
   - data/MC plots
```

### Comparing `niceplotpy-0.7.3/niceplot/__main__.py` & `niceplotpy-0.8.0/niceplot/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,90 @@
 import click
 from tqdm import tqdm
 
 # Own imports:
-from niceplot.draw2d import draw2dplot
-from niceplot.draw1d import draw1dratio
+from niceplot.draw1dratio import draw1dratio
+from niceplot.draw2dhist import draw2dhist
+from niceplot.draw2dscatter import draw2dscatter
 import niceplot.utils as utils
 from niceplot.reader import Reader
 
 @click.command()
 @click.argument('config_file')
 def niceplot(config_file: str) -> None:
     """Module to make nice looking root plots in the ATLAS Style.
     See https://gitlab.cern.ch/jwuerzin/nice-plot or https://pypi.org/project/niceplotpy/ for documentation.
     """
     # Print welcome message and version number:
     utils.printwelcome()
     
     # Read in config file and prep corresponding dictionary with pandas.DataFrames:
     reader = Reader(config_file)   
-    utils.paddefaults(reader, mode='reader')
     
     dfdict = reader.prepdfdict()
 
     savestr = "\n"
 
     # Loop over all configurations and plotting configs; Make one plot for all configs & plot configs:
     # for plot in reader.plots:
     for plot in tqdm(reader.plots, desc="Generating Plots", unit="plots"):
-        utils.paddefaults(plot, mode='plot')
         
-        if plot.type == '2dhist':
+        if plot.type == '1dratio':
+            # Make one 1dratio plot with specific configuration:
+            savestr += draw1dratio(
+                dfdict=dfdict,
+                x=plot.x,
+                denominator=plot.denominator,
+                numerator=plot.numerator,
+                denomlab=utils.getaddinfo(reader.configurations, plot.denominator),
+                numlab=utils.getaddinfo(reader.configurations, plot.numerator),
+                nbins=plot.nbins,
+                range=plot.range,
+                ylab=plot.ylab,
+                suffix=f"{plot.denominator}_over_{plot.numerator}",
+                logy=plot.logy,
+                output_dir=reader.output_dir,
+                subdir=plot.subdir
+            ) 
+        elif plot.type == '2dhist':
             # Make one 2D (exclusion) Histogram for every dataframe configuration:
             for config in reader.configurations:
-                savestr += draw2dplot(
+                # plot only for specified configs:
+                if plot.configurations is not None and config.name not in plot.configurations: continue
+                savestr += draw2dhist(
                     x=dfdict[config.name].get(plot.x),
                     y=dfdict[config.name].get(plot.y),
-                    binrange=plot.range,
                     nbins=plot.nbins,
+                    binrange=plot.range,
                     xlab=plot.xlab,
                     ylab=plot.ylab,
                     z=dfdict[config.name].get(plot.z),
                     zopt=plot.zopt,
                     suffix=config.name,
                     addinfo=config.addinfo,
-                    output_dir=f"{reader.output_dir}/{plot.subdir}",
+                    output_dir=reader.output_dir,
+                    subdir=plot.subdir,
                     addnumbers=plot.addnumbers,
                     doballs=plot.doballs
                 )
-        elif plot.type == '1dratio':
-            # Make one 1dratio plot with specific configuration:
-            savestr += draw1dratio(
-                dfdict=dfdict,
-                denominator=plot.denominator,
-                numerator=plot.numerator,
-                x=plot.x,
-                range=plot.range,
-                ylab=plot.ylab,
-                denomlab=utils.getaddinfo(reader.configurations, plot.denominator),
-                numlab=utils.getaddinfo(reader.configurations, plot.numerator),
-                nbins=plot.nbins,
-                suffix=f"{plot.denominator}_over_{plot.numerator}",
-                logy=plot.logy,
-                output_dir=f"{reader.output_dir}/{plot.subdir}"
-            )
+        elif plot.type == '2dscatter':
+            # Make one 2D scatter plot for every dataframe configuration:
+            for config in reader.configurations:
+                # plot only for specified configs:
+                if plot.configurations is not None and config.name not in plot.configurations: continue
+                savestr += draw2dscatter(
+                    x=dfdict[config.name].get(plot.x),
+                    y=dfdict[config.name].get(plot.y),
+                    z=dfdict[config.name].get(plot.z),
+                    range=plot.range,
+                    xlab=plot.xlab,
+                    ylab=plot.ylab,
+                    suffix=config.name,
+                    addinfo=config.addinfo,
+                    output_dir=reader.output_dir,
+                    subdir=plot.subdir
+                )
         else:
-            raise(ValueError(f"Plot type {plot.type} not recognised! Supported types are: 2dhist and 1dratio"))
+            raise(ValueError(f"Plot type {plot.type} not recognised! Supported types are: 1dratio, 2dhist and 2dscatter"))
         
     print(savestr)
     print("Plots generated successfully. Have a great day!!")
```

### Comparing `niceplotpy-0.7.3/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv` & `niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv` & `niceplotpy-0.8.0/niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv` & `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv` & `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv` & `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Exp.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv` & `niceplotpy-0.8.0/niceplot/data/Stitched_m_chi_10_min_m_mu_Obs.csv`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/draw1d.py` & `niceplotpy-0.8.0/niceplot/draw1dratio.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,46 +9,70 @@
 monkeypatch_axis_labels()
 
 # Import own utility functions
 import niceplot.utils as utils
 
 def draw1dratio(
     dfdict: dict[pd.DataFrame],
+    x: str,
     denominator: str,
     numerator: str,
-    x: str,
-    range: list,
-    nbins: int,
-    xlab: str = None,
-    ylab: str = "events",
-    denomlab: str = None,
-    numlab: str = None,
-    suffix: str = "",
-    addinfo: str = "",
-    logy: bool = False,
-    output_dir: str = None
+    denomlab: str,
+    numlab: str,
+    **kwargs
   ) -> str:
-  """Function to draw two 1d histograms and their ratio, both including statistical uncertainties. Returns location of saved plot."""
+  """
+  Function to draw two 1d histograms and their ratio, both including statistical uncertainties.
+  
+  Args:
+    dfdict (dict[pd.DataFrame]): DataFrame dictionary containing DataFrames to plot.
+    x (str): Name of the DataFrame column to use as x-axis.
+    denominator (str): Denominator configuration for ratio.
+    numerator (str): Numerator configuration for ratio.
+    denomlab (str): Legend label for denominator.
+    numlab (str): Legend label for Numerator.
+  
+  Keyword Args:
+    nbins (int) = 50: Number of bins to plot.
+    range (list) = None: Range to use for plotting. Should have format: [xmin, xmax].
+      If None, will automatically generate range to include all data.
+    xlab (str) = utils.getnicestr(x): X-axis Label.
+    ylab (str) = "events": Y-axis Label.
+    suffix (str) = "": Suffix for pdf name.
+    addinfo (str) = "": Additional information to add to plot.
+    logy (bool) = False: Boolean for making log plot.
+    output_dir (str) = "plots": Output directory to save plots in.
+    subdir (str) = "": Output subdirectory to save plots in.
+  
+  Returns:
+    Location of saved plot.
+  """
+  
+  # Read kwargs if provided:
+  nbins = utils.popnonan(kwargs,'nbins', 50)
+  range = utils.popnonan(kwargs,'range', None)
+  xlab = utils.popnonan(kwargs,'xlab', utils.getnicestr(x))
+  ylab = utils.popnonan(kwargs,'ylab', "events")
+  suffix = utils.popnonan(kwargs,'suffix', "")
+  addinfo = utils.popnonan(kwargs,'addinfo', "")
+  logy = utils.popnonan(kwargs,'logy', False)
+  output_dir = utils.popnonan(kwargs,'output_dir', "plots")
+  subdir = utils.popnonan(kwargs,'subdir', "")
   
-  # Replace x-axis label by nice string if custom xlab is not provided:
-  xlab = utils.getnicestr(x) if xlab == None else xlab
   fig, (ax_top, ax_bottom) = plt.subplots(nrows=2, ncols=1, height_ratios=[1.5,1])
   
   # Get denominator and numerator:
   x_den = dfdict[denominator][x]
   x_num = dfdict[numerator][x]
   
   # If range is not provided, take min/max of the two histograms:
-  if range == None:
-    minval = min(min(x_den.values), min(x_num.values))
-    maxval = max(max(x_den.values), max(x_num.values))
+  if range is None:
+    minval = min(min(dfdict[denominator][x].values), min(dfdict[numerator][x].values))
+    maxval = max(max(dfdict[denominator][x].values), max(dfdict[numerator][x].values))
     range = [minval, maxval]
-
-  # Get automatic nbins if value is not provided:
-  nbins = nbins if nbins != None else 50
   
   # Make histograms and bar plots for errors:
   hist_num, bins, _ = ax_top.hist(x_num, bins=nbins, range=range, label=numlab, histtype='step')
   bincenters = bins[:-1]+np.diff(bins)[0]/2.
   band_num = ax_top.bar(bincenters, height=2*np.sqrt(hist_num), bottom=(hist_num-np.sqrt(hist_num)), width=np.diff(bins), alpha=0.5, facecolor='tab:blue')
   hist_den, _, _ = ax_top.hist(x_den, bins=nbins, range=range, label=denomlab, histtype='step')
   band_denom = ax_top.bar(bincenters, height=2*np.sqrt(hist_den), bottom=(hist_den-np.sqrt(hist_den)), width=np.diff(bins), alpha=0.5, facecolor='tab:orange')
@@ -56,15 +80,20 @@
   # Fixing legend to include uncertainty by creating new legend handles but use the colors from the existing ones
   handles, labels = ax_top.get_legend_handles_labels()
   new_handles = [Line2D([], [], c=h.get_edgecolor()) for h in handles]
   ax_top.legend(handles=[(new_handles[0], band_num), (new_handles[1], band_denom)] , labels=labels, loc='upper right')
 
   # Make ratio and error:  
   ratio, ratioerr = utils.saferatio(hist_num, hist_den)
-  ax_bottom.errorbar(bincenters, ratio, yerr=ratioerr, fmt='ko', label='ratio', markersize=4)
+  ax_bottom.errorbar(bincenters, ratio, yerr=ratioerr, fmt='ko', label='ratio', markersize=4, zorder=2)
+  
+  # Add dashed line at 1.0
+  xlinearr = np.linspace(ax_bottom.get_xlim()[0], ax_bottom.get_xlim()[1], 1000)
+  ylinearr = np.ones(1000)
+  ax_bottom.plot(xlinearr, ylinearr, linestyle='dashed', color='grey', zorder=1)
   
   if logy:
     ax_top.set_yscale('log')
     ax_top.set_ylim(1., 2*max( [max(hist_den), max(hist_num)]) )
   else:
     ax_top.set_ylim(1., max( [max(hist_den), max(hist_num)]) )
   
@@ -85,8 +114,8 @@
   if addinfo == "":
     atlasify("Internal", outside=True, axes=ax_top) 
   else:
     atlasify("Internal", addinfo, outside=True, axes=ax_top) 
   atlasify(False, axes=ax_bottom)
   
   # Save:
-  return utils.savefile(fig, output_dir, f'1dratio_{x}_{suffix}.pdf')
+  return utils.savefile(fig, output_dir, subdir, f'1dratio_{x}_{suffix}.pdf')
```

### Comparing `niceplotpy-0.7.3/niceplot/draw2d.py` & `niceplotpy-0.8.0/niceplot/draw2dhist.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,51 +18,74 @@
 cmaplist = [plt.cm.plasma(i) for i in range(N)]
 cmaplist[0] = mpl.colors.to_rgba('black')
 cmaplist[-1] = cmaplist_magma[-1]
 
 mycmap = mpl.colors.LinearSegmentedColormap.from_list('Custom cmap', cmaplist, N)
 mycmap.set_bad('gainsboro')
 
-def draw2dplot(
+def draw2dhist(
     x: pd.core.series.Series,
     y: pd.core.series.Series,
-    binrange: list,
-    nbins: int,
-    xlab: str = None,
-    ylab: str = None,
-    z: pd.core.series.Series = None,
-    zopt: str = "counts",
-    suffix: str = "",
-    addinfo: str = "",
-    output_dir: str = None,
-    addnumbers: bool = False,
-    doballs: bool = False
+    **kwargs
   ) -> str:
-  """Function to draw a 2D histogram of x vs y. Returns location of saved plot."""
-  # Replace x- and y-axis labels by nice strings if custom xlab and ylab are not provided:
-  xlab = utils.getnicestr(x.name) if xlab == None else xlab
-  ylab = utils.getnicestr(y.name) if ylab == None else ylab
+  """
+  Function to draw a 2D histogram of x vs y. 
+  
+  Args:
+    x (pd.core.series.Series): Pandas series for x-axis.
+    y (pd.core.series.Series): Pandas series for y-axis.
+  
+  Keyword Args:
+    nbins (int) = 50: Number of bins to plot.
+    binrange (list) = [[min(x.values), max(x.values)], [min(y.values), max(y.values)]]: Range to use for plotting.
+      Should have format: [[xmin, xmax], [ymin, ymax]].
+    xlab (str) = utils.getnicestr(x.name): X-axis Label.
+    ylab (str) = utils.getnicestr(y.name): Y-axis Label.
+    z (pd.core.series.Series) = None: Pandas series for z-axis.
+    zopt (str) = "counts": Option for z-axis. Supported are: "counts", "excl_frac" and "excl_max".
+    suffix (str) = "": Suffix for pdf name.
+    addinfo (str) = "": Additional information to add to plot.
+    output_dir (str) = "plots": Output directory to save plots in.
+    subdir (str) = "": Output subdirectory to save plots in.
+    addnumbers (bool) = False: Add grey numbers in overlay.
+    doballs (bool) = False: Plot balls with number of entries in bin for size.
+  
+  Returns:
+    Location of saved plot.
+  """
+  
+  # Read kwargs if provided:
+  nbins = utils.popnonan(kwargs,'nbins', 50)
+  binrange = utils.popnonan(kwargs,'binrange', [[min(x.values), max(x.values)], [min(y.values), max(y.values)]])
+  xlab = utils.popnonan(kwargs,'xlab', utils.getnicestr(x.name))
+  ylab = utils.popnonan(kwargs,'ylab', utils.getnicestr(y.name))
+  z = utils.popnonan(kwargs,'z', None)
+  zopt = utils.popnonan(kwargs,'zopt', "counts")
+  suffix = utils.popnonan(kwargs,'suffix', "")
+  addinfo = utils.popnonan(kwargs,'addinfo', "")
+  output_dir = utils.popnonan(kwargs,'output_dir', "plots")
+  subdir = utils.popnonan(kwargs,'subdir', "")
+  addnumbers = utils.popnonan(kwargs,'addnumbers', False)
+  doballs = utils.popnonan(kwargs,'doballs', False)
+  
   fig, ax = plt.subplots(nrows=1, ncols=1)
   
-  # Get automatic range and nbins if values are not provided:
-  binrange = binrange if binrange != None else [ [min(x.values), max(x.values)], [min(y.values), max(y.values)]]
-  nbins = nbins if nbins != None else 50
-  #TODO: fix log-log plot using this binning sheme:
+  # TODO: fix log-log plot using this binning sheme:
   # nbins = [np.logspace(-4, 0, nbins), np.logspace(-4, 0, nbins)]
   
-  # Make 2d hist (defending on zopt):
+  # Make 2d hist (depending on zopt):
   if zopt == "counts":
     z_matrix, x_edges, y_edges, h = ax.hist2d(x, y, bins=nbins, range=binrange, cmin=1)
     clab = 'no. of models'
     figname = f'2dhist_{x.name}_vs_{y.name}_{suffix}.pdf'
     anncol = 'white'
     numdig = 0
 
   else:
-    # Plot fraction of excluded models on z-axis. First, cast data into dataframe:
+    # Plot either exclusion fraction/max on z-axis. First, cast data into dataframe:
     df = pd.DataFrame( {
       'x': x,
       'y': y,
       'z': z
     } )
     
     # Next, we make a simple histogram to get the bin edges:
@@ -114,15 +137,14 @@
     ax.plot(xylinearr, xylinearr, linestyle='dashed', color='grey')
 
   # Overlay simplified model limits if they exist:
   simplified_limit = utils.get_simplified_limit(x.name, y.name, z)
   if simplified_limit is not None:
     ax.plot(simplified_limit[x.name], simplified_limit[y.name], linestyle='-', color='white', linewidth = 2.0)
     ax.plot(simplified_limit[x.name], simplified_limit[y.name], linestyle='--', color='black')
-    
 
   if addnumbers:
     # Annotate numbers:  
     x_width = x_edges[1] - x_edges[0]
     y_width = y_edges[1] - y_edges[0]
     for i in range(len(x_edges) -1):
       for j in range(len(y_edges) -1):
@@ -140,14 +162,11 @@
   
   # Correct offset for potential exponential on x and y axes; fix layout:
   ax.xaxis._update_offset_text_position = types.MethodType(utils.bottom_offset, ax.xaxis)
   ax.yaxis._update_offset_text_position = types.MethodType(utils.top_offset, ax.yaxis)
   fig.tight_layout(rect=(0, 0, 1, 0.94)) # default: left=0, bottom=0, right=1, top=1
   
   # Add ATLAS label + info:
-  if addinfo == "":
-    atlasify("Internal", outside=True) 
-  else:
-    atlasify("Internal", addinfo, outside=True) 
+  atlasify("Internal", addinfo, outside=True) 
   
   # Save:
-  return utils.savefile(fig, output_dir, figname)
+  return utils.savefile(fig, output_dir, subdir, figname)
```

### Comparing `niceplotpy-0.7.3/niceplot/process_yaml.py` & `niceplotpy-0.8.0/niceplot/process_yaml.py`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/reader.py` & `niceplotpy-0.8.0/niceplot/reader.py`

 * *Files identical despite different names*

### Comparing `niceplotpy-0.7.3/niceplot/utils.py` & `niceplotpy-0.8.0/niceplot/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,44 +24,48 @@
                    |_|                            """+"\n")
 
     print(f"Welcome to Niceplot v{__version__}!")
     print(f"Author: {__author__} ({__credits__})\n")
     
     return None
 
+def popnonan(dic: dict, key: str, default) -> any:
+    """Apply pop to dic for key and return default if None is returned."""
+    retval = dic.pop(key, default)
+    return default if retval is None else retval
+
 def getaddinfo(conflist: list[dict], name: str) -> str:
     """Get and return addinfo entry from conflist for entry with name."""
     addinfo = None
     for conf in conflist:
         addinfo = conf.addinfo if conf.name == name else addinfo
     
     return addinfo
 
-def softpad(value, default):
-        """Replace value by default if None."""
-        return default if value is None else value
+# def softpad(value, default):
+#         """Replace value by default if None."""
+#         return default if value is None else value
 
-def paddefaults(obj: DotAccessibleDict, mode: str) -> None:
-    """Function for padding configuration dicts. Contains default plotting/config values!"""
+# def paddefaults(obj: DotAccessibleDict, mode: str) -> None:
+#     """Function for padding configuration dicts. Contains default plotting/config values!"""
         
-    if mode == 'plot':
-        obj.logy = softpad(obj.logy, default=False)
-        obj.range = softpad(obj.range, default=None)
-        obj.nbins = softpad(obj.nbins, default=None)
-        obj.ylab = softpad(obj.ylab, default='events')
-        obj.ratio = softpad(obj.ratio, default=True)
-        obj.zopt = softpad(obj.zopt, default='counts')
-        obj.addnumbers = softpad(obj.addnumbers, default=False)
-        obj.subdir = softpad(obj.subdir, default='')
-    elif mode == 'reader':
-        obj.output_dir = softpad(obj.output_dir, default='plots')    
-    else:
-        raise ValueError(f"Padding mode {mode} not supported!")
+#     if mode == 'plot':
+#         obj.logy = softpad(obj.logy, default=False)
+#         # obj.range = softpad(obj.range, default=None)
+#         # obj.nbins = softpad(obj.nbins, default=None)
+#         obj.ratio = softpad(obj.ratio, default=True)
+#         obj.zopt = softpad(obj.zopt, default='counts')
+#         obj.addnumbers = softpad(obj.addnumbers, default=False)
+#         obj.subdir = softpad(obj.subdir, default='')
+#     elif mode == 'reader':
+#         obj.output_dir = softpad(obj.output_dir, default='plots')    
+#     else:
+#         raise ValueError(f"Padding mode {mode} not supported!")
     
-    return
+#     return
 
 def getnicestr(string: str) -> str:
     """Function to get nice TeX version of string."""
     
     # Try to auto-generate nicestr:  
     leftlist = [""]
     rightlist = [""]
@@ -95,18 +99,19 @@
         '20' : ["_2^0", ""],
         '30' : ["_3^0", ""],
         '40' : ["_4^0", ""],
         '1p' : ["_1^\\pm", ""],
         '2p' : ["_2^\\pm", ""],
         '3p' : ["_3^\\pm", ""],
         '4p' : ["_4^\\pm", ""],
-        'Bino' : ["\\mathrm{Bino }", ""],
-        'Wino' : ["\\mathrm{Wino }", ""],
-        'Higgsino' : ["\\mathrm{Higgsino }", ""],
-        'fraction' : ["\\mathrm{fraction} ", ""],
+        'Bino' : ["~\\mathrm{Bino}", ""],
+        'Wino' : ["~\\mathrm{Wino}", ""],
+        'Higgsino' : ["~\\mathrm{Higgsino}", ""],
+        'fraction' : ["~\\mathrm{fraction}", ""],
+        'frac' : ["~\\mathrm{fraction}", ""],
         # General tex:
         'to' : ["\\rightarrow", ""],
         'other' : ["\\rightarrow \\mathrm{Other}", ""],
         # Precision measurements:
         'gmuon' : ["\\Delta a_{\\mu}",""],
         # Prefixes:
         'SPfh' : ["", "\\mathrm{ (SPfh)}"],
@@ -170,23 +175,22 @@
     """Function for calculate safe ratio numlist/denomlist and the corresponding Poission uncertianty, replacing infinities in the ratio by -1. Returns (ratio, ratioerr)."""
     ratio = [denomlist[i]/numlist[i] if denomlist[i] != 0 else -1. for i in range(len(numlist))]
     # Assume Poissionian errors on both numlist and denomlist; set unc. to 0 for invalid ratio values:
     ratioerr = [ratio[i]*np.sqrt( 1./numlist[i] + 1./denomlist[i] ) if denomlist[i] != 0 else 0 for i in range(len(numlist))]
     
     return ratio, ratioerr
         
-def savefile(fig: matplotlib.figure.Figure, dirn: str, filen: str) -> None:
-    """Make dirn if it does not exist already and save fig into filen in dirn."""
-    # Set dirn to default if None:
-    dirn = 'plots' if dirn == None else dirn
-    # Make dir and parents if they don't exist already:
-    Path(dirn).mkdir(parents=True, exist_ok=True)
+def savefile(fig: matplotlib.figure.Figure, dirn: str, subdir: str, filen: str) -> None:
+    """Make plot directory dirn/subdir if it does not exist already and save fig into filen in dirn."""
+    # Combine dirn and subdir; Make dir and parents if they don't exist already:
+    outdir = f"{dirn}/{subdir}"
+    Path(outdir).mkdir(parents=True, exist_ok=True)
     
     # Save file and close plot:
-    filepath = f'{dirn}/{filen}'
+    filepath = f'{outdir}/{filen}'
     # print(f"Saving plot: {filepath}")
     savestr = f"Saving plot: {filepath}\n"
     fig.savefig(filepath)
     plt.close(fig)
     
     return savestr
```

### Comparing `niceplotpy-0.7.3/niceplotpy.egg-info/PKG-INFO` & `niceplotpy-0.8.0/niceplotpy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceplotpy
-Version: 0.7.3
+Version: 0.8.0
 Summary: A package collecting things to make nice plots from root files
 Home-page: https://gitlab.cern.ch/jwuerzin/nice-plot
 Author: Jonas Wuerzinger
 Author-email: jonas.wuerzinger@tum.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -33,15 +33,15 @@
 After installation, the the module can be used with:
 
 ```python
 niceplot CONFIG_FILE
 ```
 Where the `CONFIG_FILE` includes all information on which plots to make, variables to plot, etc. 
 
-Currently supported plot types are: `1dratio` and `2dhist`. For a detailled example config file, see: [example_configs/GMSB.yaml](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/GMSB.yaml). Here a shortened example config file:
+Currently supported plot types are: `1dratio`, `2dhist` and `2dscatter`. For detailled example config files, see: [example_configs](https://gitlab.cern.ch/jwuerzin/nice-plot/-/blob/master/example_configs/). Here a shortened example config file:
 
 ```yaml
 input_file: 'data/susy.root'
 output_dir: 'plots/GMSB_Factory'
 treename: 'susy'
 configurations:
   - name: 'GMSBpresel'
@@ -69,17 +69,16 @@
       - 'BF_chi_10_to_e_L'
       - 'BF_chi_10_to_e_R'
     # 1D histograms:
     - {<<: *ploting_common, x: !evaluate "${BF}" }
     # 2D histograms:
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True }
     - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_frac', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ExpCLs_Overall' }
-    - { type: 2dhist, x: 'min_m_chi', y: !evaluate "${BF}", z: 'EWSummary_ExpCLs_Overall', zopt: 'excl_max', range: [ [0, 2000], [0, 1.]], nbins: 20, addnumbers: True, subdir: 'EWSummary_ObsCLs_Overall' }
+  
+  - { type: 2dscatter, x: 'BF_chi_10_to_gravitino_Z', y: 'BF_chi_10_to_gravitino_gam', z: 'EWSummary_ObsCLs_Overall', range: [ [0, 1.], [0, 1.]], subdir: '2dscatter'}
 ```
 
 ## ToDo:
 
+- Move 2Dscatterplot grid to background.
 - Add more options for plots:
-  - 2dplot with custom z-axis
   - data/MC plots
```

### Comparing `niceplotpy-0.7.3/niceplotpy.egg-info/SOURCES.txt` & `niceplotpy-0.8.0/niceplotpy.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 niceplot/__init__.py
 niceplot/__main__.py
-niceplot/draw1d.py
-niceplot/draw2d.py
+niceplot/draw1dratio.py
+niceplot/draw2dhist.py
+niceplot/draw2dscatter.py
 niceplot/process_yaml.py
 niceplot/reader.py
 niceplot/utils.py
 niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Exp.csv
 niceplot/data/ATLAS-CONF-2023-046_min_m_chi_BF_chi_10_to_gravitino_h_Obs.csv
 niceplot/data/Stitched_m_chi_10_m_chi_1p_Exp.csv
 niceplot/data/Stitched_m_chi_10_m_chi_1p_Obs.csv
```

### Comparing `niceplotpy-0.7.3/setup.py` & `niceplotpy-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='niceplotpy',
-    version='0.7.3',
+    version='0.8.0',
     description='A package collecting things to make nice plots from root files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.cern.ch/jwuerzin/nice-plot',
     author='Jonas Wuerzinger',
     author_email='jonas.wuerzinger@tum.de',
     packages=find_packages(),
```

