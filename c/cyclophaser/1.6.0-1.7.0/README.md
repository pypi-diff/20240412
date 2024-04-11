# Comparing `tmp/cyclophaser-1.6.0.tar.gz` & `tmp/cyclophaser-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclophaser-1.6.0.tar", last modified: Mon Dec 18 20:54:15 2023, max compression
+gzip compressed data, was "cyclophaser-1.7.0.tar", last modified: Thu Apr 11 23:09:34 2024, max compression
```

## Comparing `cyclophaser-1.6.0.tar` & `cyclophaser-1.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/cyclophaser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16352 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser/determine_periods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12199 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser/find_stages.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser/lanczos_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12762 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser/plots.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/cyclophaser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/cyclophaser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-12-18 20:54:15.822295 cyclophaser-1.6.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1897 2023-12-18 20:54:15.000000 cyclophaser-1.6.0/tests/test_determine_periods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/cyclophaser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17593 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/determine_periods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12997 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/find_stages.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/lanczos_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12837 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/plots.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/cyclophaser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/tests/test_determine_periods.py
```

### Comparing `cyclophaser-1.6.0/PKG-INFO` & `cyclophaser-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.6.0
+Version: 1.7.0
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.6.0/README.md` & `cyclophaser-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.6.0/cyclophaser/determine_periods.py` & `cyclophaser-1.7.0/cyclophaser/determine_periods.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    determine_periods.py                               :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: daniloceano <danilo.oceano@gmail.com>      +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/05/19 19:06:47 by danilocs          #+#    #+#              #
-#    Updated: 2023/12/18 11:22:58 by daniloceano      ###   ########.fr        #
+#    Updated: 2024/04/11 19:59:55 by daniloceano      ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import os
 import csv
 
 import xarray as xr
 import pandas as pd
 import numpy as np
 
 from scipy.signal import argrelextrema
 from scipy.signal import savgol_filter 
 
-from cyclophaser import lanczos_filter as lanfil
+import cyclophaser.lanczos_filter as lanfil
 from cyclophaser.plots import plot_all_periods, plot_didactic
-from cyclophaser.find_stages import find_incipient_period, find_intensification_period, find_decay_period, find_mature_stage, find_residual_period
+from cyclophaser.find_stages import find_incipient_period 
+from cyclophaser.find_stages import find_intensification_period
+from cyclophaser.find_stages import find_decay_period 
+from cyclophaser.find_stages import find_mature_stage
+from cyclophaser.find_stages import find_residual_period
 
 def check_create_folder(DirName, verbosity=False):
     if not os.path.exists(DirName):
                 os.makedirs(DirName)
                 print(DirName+' created')
     else:
         if verbosity:
@@ -264,15 +268,28 @@
     da = da.assign(variables={'dz_dt_filt': dz_dt_filt,
                               'dz_dt2_filt': dz_dt2_filt,
                               'dz_dt_smoothed2': dz_dt_smoothed2,
                               'dz_dt2_smoothed2': dz_dt2_smoothed2})
 
     return da 
 
-def get_periods(vorticity,  plot=False, plot_steps=False, export_dict=False):
+def get_periods(vorticity,  plot=False, plot_steps=False, export_dict=False, periods_args=None):
+    default_args = {
+        'threshold_intensification_length': 0.125,
+        'threshold_intensification_gap': 0.075,
+        'threshold_mature_distance': 0.125,
+        'threshold_mature_length': 0.03,
+        'threshold_decay_length': 0.075,
+        'threshold_decay_gap': 0.075,
+        'threshold_incipient_length': 0.4
+    }
+
+    # Update the default arguments with any user-provided arguments
+    if periods_args is not None:
+        default_args.update(periods_args)
 
     z = vorticity.vorticity_smoothed2
     dz = vorticity.dz_dt_smoothed2
     dz2 = vorticity.dz_dt2_smoothed2
 
     df = z.to_dataframe().rename(columns={'vorticity_smoothed2':'z'})
     df['z_unfil'] = vorticity.zeta.to_dataframe()
@@ -282,51 +299,49 @@
     df['z_peaks_valleys'] = find_peaks_valleys(df['z'])
     df['dz_peaks_valleys'] = find_peaks_valleys(df['dz'])
     df['dz2_peaks_valleys'] = find_peaks_valleys(df['dz2'])
 
     df['periods'] = np.nan
     df['periods'] = df['periods'].astype('object')
 
-    df = find_intensification_period(df)
-
-    df = find_decay_period(df)
-
-    df = find_mature_stage(df)
-
+    df = find_intensification_period(df, **default_args)
+    df = find_decay_period(df, **default_args)
+    df = find_mature_stage(df, **default_args)
     df = find_residual_period(df)
 
     # 1) Fill consecutive intensification or decay periods that have NaNs between them
     # 2) Remove periods that are too short and fill with the previous period
     # (or the next one if there is no previous period)
     df = post_process_periods(df)
 
-    df = find_incipient_period(df)
+    df = find_incipient_period(df, **default_args)
 
     # Pass the periods to a dictionary with each period's name as key
     #  and their corresponding start and end times as values.
     # Also, add extra 6 hours to the start and end of the periods as "confidence intervals"
     periods_dict = periods_to_dict(df)
 
     # Create plots, if requested
     if plot:
         plot_all_periods(periods_dict, df, ax=None, vorticity=vorticity, periods_outfile_path=plot)
     if plot_steps:
-        plot_didactic(df, vorticity, plot_steps)
+        plot_didactic(df, vorticity, plot_steps, **default_args)
     # Export csv, if requested
     if export_dict:
         export_periods_to_csv(periods_dict, export_dict)
 
     return df
 
 def determine_periods(series,
                       x=None,
                       plot=False,
                       plot_steps=False,
                       export_dict=False,
-                      process_vorticity_args=None):
+                      process_vorticity_args=None,
+                      periods_args=None):
     """
     Determine meteorological periods from a series of vorticity data.
 
     Args:
         series (list): List of vorticity values.
         x (list, optional): Temporal range or other labels for the series. Default is None.
         vorticity_column (str, optional): Column name for the 'zeta' data in the DataFrame. Default is 'zeta'.
@@ -355,33 +370,45 @@
 
     # Rest of the function remains the same as before
     if process_vorticity_args is None:
         process_vorticity_args = {}
     vorticity = process_vorticity(zeta_df.copy(), **process_vorticity_args)
 
     args = [plot, plot_steps, export_dict]
-    return get_periods(vorticity.copy(), *args)
+    if periods_args is None:
+        periods_args = {}
+    return get_periods(vorticity.copy(), *args, periods_args)
 
 
 if __name__ == '__main__':
     # Read the data from the CSV file
     track_file = '../tests/test.csv'
     track = pd.read_csv(track_file, parse_dates=[0], delimiter=';', index_col=[0])
 
     # Extract the vorticity data as a list and the index as a temporal range
-    series = track['min_zeta_850'].tolist()
+    series = track['min_max_zeta_850'].tolist()
     x = track.index.tolist()  # Using the DataFrame index as the temporal range
 
     # Testing options
-    options = {
-        "x": x,
-        "plot": 'test',
-        "plot_steps": 'test_steps',
-        "export_dict": False,
-        "process_vorticity_args": {
+    process_vorticity_args = {
             "use_filter": False,
-            "use_smoothing_twice": "auto"
+            "use_smoothing_twice": False
+        }
+
+    periods_args= {
+        'threshold_intensification_length': 0.10,  # Decreased threshold
+        'threshold_intensification_gap': 0.05,
+        'threshold_mature_distance': 0.10,
+        'threshold_mature_length': 0.02,
+        'threshold_decay_length': 0.06,
+        'threshold_decay_gap': 0.06,
+        'threshold_incipient_length': 0.35
         }
-    }
 
     # Test the determine_periods function
-    result = determine_periods(series, **options)
+    result = determine_periods(series,
+            x=x,
+            plot="test",
+            plot_steps="test_steps",
+            export_dict=False,
+            process_vorticity_args=process_vorticity_args,
+            periods_args=periods_args)
```

### Comparing `cyclophaser-1.6.0/cyclophaser/find_stages.py` & `cyclophaser-1.7.0/cyclophaser/find_stages.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 import numpy as np
 import pandas as pd
 
-def find_mature_stage(df):
-    dz_peaks = df[df['dz_peaks_valleys'] == 'peak'].index
-    dz_valleys = df[df['dz_peaks_valleys'] == 'valley'].index
+def find_mature_stage(df, **args_periods):
+
+    threshold_mature_distance = args_periods['threshold_mature_distance']
+    threshold_mature_length = args_periods['threshold_mature_length']
+
     z_valleys = df[df['z_peaks_valleys'] == 'valley'].index
     z_peaks = df[df['z_peaks_valleys'] == 'peak'].index
 
     series_length = df.index[-1] - df.index[0]
     dt = df.index[1] - df.index[0]
 
     # Iterate over z valleys
     for z_valley in z_valleys:
+
         # Find the previous and next dz valleys relative to the current z valley
         next_z_peak = z_peaks[z_peaks > z_valley]
         previous_z_peak =  z_peaks[z_peaks < z_valley]
 
         # Check if there is a previous or next z_peak
         if len(previous_z_peak) == 0 or len(next_z_peak) == 0:
             continue
 
         previous_z_peak = previous_z_peak[-1]
         next_z_peak = next_z_peak[0]
 
+
         # Calculate the distances between z valley and the previous/next dz valleys
         distance_to_previous_z_peak = z_valley - previous_z_peak
         distance_to_next_z_peak = next_z_peak - z_valley
 
-        mature_distance_previous = 0.125 * distance_to_previous_z_peak
-        mature_distance_next = 0.125 * distance_to_next_z_peak
+        # Calculate the mature stage start and end 
+        mature_distance_previous = distance_to_previous_z_peak * threshold_mature_distance
+        mature_distance_next = distance_to_next_z_peak * threshold_mature_distance
 
         mature_start = z_valley - mature_distance_previous
         mature_end = z_valley + mature_distance_next
 
         # Mature stage needs to be at least 3% of total length
         mature_indexes = df.loc[mature_start:mature_end].index
-        if mature_indexes[-1] - mature_indexes[0] > 0.03 * series_length:
+
+        if len(mature_indexes) == 0:
+            continue
+
+        if mature_indexes[-1] - mature_indexes[0] > threshold_mature_length * series_length:
             # Fill the period between mature_start and mature_end with 'mature'
             df.loc[mature_start:mature_end, 'periods'] = 'mature'
 
     # Check if all mature stages are preceded by an intensification and followed by decay
     mature_periods = df[df['periods'] == 'mature'].index
     if len(mature_periods) > 0:
         blocks = np.split(mature_periods, np.where(np.diff(mature_periods) != dt)[0] + 1)
@@ -47,50 +56,57 @@
             block_start, block_end = block[0], block[-1]
             if df.loc[block_start - dt, 'periods'] != 'intensification' or \
                df.loc[block_end + dt, 'periods'] != 'decay':
                 df.loc[block_start:block_end, 'periods'] = np.nan
 
     return df
 
+def find_intensification_period(df, **args_periods):
+
+    threshold_intensification_length = args_periods['threshold_intensification_length']
+    threshold_intensification_gap = args_periods['threshold_decay_length']
 
-def find_intensification_period(df):
     # Find z peaks and valleys
     z_peaks = df[df['z_peaks_valleys'] == 'peak'].index
     z_valleys = df[df['z_peaks_valleys'] == 'valley'].index
 
     length = df.index[-1] - df.index[0]
     dt = df.index[1] - df.index[0]
 
     # Find intensification periods between z peaks and valleys
     for z_peak in z_peaks:
         next_z_valley = z_valleys[z_valleys > z_peak].min()
         if next_z_valley is not pd.NaT:
             intensification_start = z_peak
             intensification_end = next_z_valley
 
-            # Intensification needs to be at least 7.5% of the total series length
-            if intensification_end-intensification_start > length*0.12:
+            # Intensification needs to be at least 12.5% of the total series length
+            if intensification_end-intensification_start > length * threshold_intensification_length:
                 df.loc[intensification_start:intensification_end, 'periods'] = 'intensification'
     
     # Check if there are multiple blocks of consecutive intensification periods
     intensefication_periods = df[df['periods'] == 'intensification'].index
     blocks = np.split(intensefication_periods, np.where(np.diff(intensefication_periods) != dt)[0] + 1)
 
     for i in range(len(blocks) - 1):
         block_end = blocks[i][-1]
         next_block_start = blocks[i+1][0]
         gap = next_block_start - block_end
 
         # If the gap between blocks is smaller than 7.5%, fill with intensification
-        if gap < length*0.075:
+        if gap < length * threshold_intensification_gap:
             df.loc[block_end:next_block_start, 'periods'] = 'intensification'
 
     return df
 
-def find_decay_period(df):
+def find_decay_period(df, **args_periods):
+
+    threshold_decay_length = args_periods['threshold_decay_length']
+    threshold_decay_gap = args_periods['threshold_decay_gap']
+
     # Find z peaks and valleys
     z_peaks = df[df['z_peaks_valleys'] == 'peak'].index
     z_valleys = df[df['z_peaks_valleys'] == 'valley'].index
 
     length = df.index[-1] - df.index[0]
     dt = df.index[1] - df.index[0]
 
@@ -100,29 +116,29 @@
         if next_z_peak is not pd.NaT:
             decay_start = z_valley
             decay_end = next_z_peak
         else:
             decay_start = z_valley
             decay_end = df.index[-1]  # Last index of the DataFrame
 
-        # Decay needs to be at least 12% of the total series length
-        if decay_end - decay_start > length*0.075:
+        # Decay needs to be at least 7.5% of the total series length
+        if decay_end - decay_start > length * threshold_decay_length:
             df.loc[decay_start:decay_end, 'periods'] = 'decay'
 
     # Check if there are multiple blocks of consecutive decay periods
     decay_periods = df[df['periods'] == 'decay'].index
     blocks = np.split(decay_periods, np.where(np.diff(decay_periods) != dt)[0] + 1)
 
     for i in range(len(blocks) - 1):
         block_end = blocks[i][-1]
         next_block_start = blocks[i+1][0]
         gap = next_block_start - block_end
 
         # If the gap between blocks is smaller than 7.5%, fill with decay
-        if gap < length*0.075:
+        if gap < length * threshold_decay_gap:
             df.loc[block_end:next_block_start, 'periods'] = 'decay'
 
     return df
 
 def find_residual_period(df):
     unique_phases = [item for item in df['periods'].unique() if pd.notnull(item)]
     num_unique_phases = len(unique_phases)
@@ -181,15 +197,17 @@
         elif 'mature' in unique_phases:
             last_decay_index = df[df['periods'] == 'mature'].index[-1]
         dt = df.index[1] - df.index[0]
         df.loc[last_decay_index + dt:, 'periods'].fillna('residual', inplace=True)
 
     return df
 
-def find_incipient_period(df):
+def find_incipient_period(df, **args_periods):
+
+    threshold_incipient_length = args_periods['threshold_incipient_length']
 
     periods = df['periods']
     
     df['periods'].fillna('incipient', inplace=True)
 
     phases_order = []
     current_phase = None
@@ -198,43 +216,43 @@
         if pd.notnull(phase) and phase != 'residual':
             if phase != current_phase:
                 phases_order.append(phase)
                 current_phase = phase
 
     # If there's more than 2 unique phases other than residual, and the life cycle
     # begins with intensification or decay, incipient phase will be from the beginning
-    # of it until 2/5 to the next dz_valley/dz_peak
+    # of it until 40% to the next dz_valley/dz_peak
     # If there is a cycle of intensification and decay before the next mature stage it
     #  will cganged to incipient
     if len(phases_order) > 2:
         if phases_order[:3] == ['intensification', 'decay', 'intensification']:
             start_time = df[df['periods'] == "intensification"].index.min()
             decay_blocks = np.split(df[df['periods'] == "decay"].index,
                                 np.where(np.diff(df['periods'] == "decay") != 0)[0] + 1)
             end_time = decay_blocks[0].max()
             if end_time is not pd.NaT:
-                time_range = start_time + 2 * (end_time - start_time) / 5
+                time_range = start_time + ((end_time - start_time) * threshold_incipient_length)
                 df.loc[start_time:time_range, 'periods'] = 'incipient'
 
         elif phases_order[0] == 'intensification':
             start_time = df[df['periods'] == 'intensification'].index.min()
             # Check if there's a dz valley before the next mature stage
             next_dz_valley = df[1:][df[1:]['dz_peaks_valleys'] == 'valley'].index.min()
             next_mature = df[periods == 'mature'].index.min()
             if next_dz_valley < next_mature:
-                time_range = start_time + 2 * (next_dz_valley - start_time) / 5
+                time_range = start_time + ((next_dz_valley - start_time) * threshold_incipient_length)
                 df.loc[start_time:time_range, 'periods'] = 'incipient'
 
         elif phases_order[0] == 'decay':
             start_time = df[df['periods'] == 'decay'].index.min()
             # Check if there's a dz peak before the next mature stage
             next_dz_peak = df[1:][df[1:]['dz_peaks_valleys'] == 'peak'].index.min()
             next_mature = df[periods == 'mature'].index.min()
             if next_dz_peak < next_mature:
-                time_range = start_time + 2 * (next_dz_peak - start_time) / 5
+                time_range = start_time + ((next_dz_peak - start_time) * threshold_incipient_length)
                 df.loc[start_time:time_range, 'periods'] = 'incipient'
         
             
 
     return df
 
 if __name__ == '__main__':
```

### Comparing `cyclophaser-1.6.0/cyclophaser/lanczos_filter.py` & `cyclophaser-1.7.0/cyclophaser/lanczos_filter.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.6.0/cyclophaser/plots.py` & `cyclophaser-1.7.0/cyclophaser/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 
 import cmocean.cm as cmo
 
-from .find_stages import find_intensification_period, find_decay_period, find_mature_stage
+from cyclophaser.find_stages import find_intensification_period, find_decay_period, find_mature_stage
 
 def plot_phase(df, phase, ax=None, show_title=True):
     # Create a copy of the DataFrame
     df_copy = df.copy()
 
     zeta = df_copy['z_unfil']
     vorticity_smoothed = df_copy['z']
@@ -247,15 +247,15 @@
 
     if periods_outfile_path is not None:
         fname = f"{periods_outfile_path}.png"
         plt.savefig(fname, dpi=500)
         print(f"{fname} created.")
 
 
-def plot_didactic(df, vorticity, output_directory):
+def plot_didactic(df, vorticity, output_directory, **periods_args):
     
     # First step: filter vorticity data
     fig = plt.figure(figsize=(10, 8.5))
     ax1 = fig.add_subplot(331)
     plot_vorticity(ax1, vorticity)
 
     # Second step: identify peaks and valleys of vorticity
@@ -268,27 +268,27 @@
         df['z'], ax3,
         df['z_peaks_valleys'],
         df['dz_peaks_valleys'],
         df['dz2_peaks_valleys'], 
         )
     
     # Intensification phase
-    df_int = find_intensification_period(df.copy())
+    df_int = find_intensification_period(df.copy(), **periods_args)
     ax4 = fig.add_subplot(334)
     plot_phase(df_int, "intensification", ax4)
     plot_specific_peaks_valleys(df_int, ax4, "z_peaks", "z_valleys")
 
     # Decay phase
-    df_decay = find_decay_period(df.copy())
+    df_decay = find_decay_period(df.copy(), **periods_args)
     ax5 = fig.add_subplot(335)
     plot_phase(df_decay, "decay", ax5)
     plot_specific_peaks_valleys(df_decay, ax5, "z_peaks", "z_valleys")
 
     # Mature phase
-    df_mature = find_mature_stage(df.copy())
+    df_mature = find_mature_stage(df.copy(), **periods_args)
     ax6 = fig.add_subplot(336)
     plot_phase(df_mature, "mature", ax6)
     plot_specific_peaks_valleys(df_mature, ax6, "z_peaks", "z_valleys", "dz_valleys", "dz_peaks")
 
     # Residual stage
     ax7 = fig.add_subplot(337)
     plot_phase(df, "residual", ax7)
```

### Comparing `cyclophaser-1.6.0/cyclophaser.egg-info/PKG-INFO` & `cyclophaser-1.7.0/cyclophaser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.6.0
+Version: 1.7.0
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.6.0/setup.py` & `cyclophaser-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '1.6.0'
+VERSION = '1.7.0'
 DESCRIPTION = 'Determine phases from extratropical cyclone life cycle'
 # LONG_DESCRIPTION = 'This script processes vorticity data, identifies different phases of the cyclone \
     # and plots the identified periods on periods.png and periods_didatic.png'
 
 setup(
     name="cyclophaser",
     version=VERSION,
```

### Comparing `cyclophaser-1.6.0/tests/test_determine_periods.py` & `cyclophaser-1.7.0/tests/test_determine_periods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from cyclophaser.determine_periods import determine_periods
 import pandas as pd
 
 def test_determine_periods_with_options():
     # Read the data from the CSV file
     track_file = 'tests/test.csv'
     track = pd.read_csv(track_file, parse_dates=[0], delimiter=';', index_col=[0])
-    series = track['min_zeta_850'].tolist()
+    series = track['min_max_zeta_850'].tolist()
     x = track.index.tolist()
 
     # Specify options for the determine_periods function
     options_era5 = {
         "plot": 'test_ERA5',
         "plot_steps": 'test_steps_ERA5',
         "export_dict": 'test_ERA5',
```

