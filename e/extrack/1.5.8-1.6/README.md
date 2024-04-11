# Comparing `tmp/extrack-1.5.8.tar.gz` & `tmp/extrack-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrack-1.5.8.tar", last modified: Wed Jul 12 18:46:59 2023, max compression
+gzip compressed data, was "extrack-1.6.tar", last modified: Thu Apr 11 23:25:46 2024, max compression
```

## Comparing `extrack-1.5.8.tar` & `extrack-1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 18:46:59.034444 extrack-1.5.8/
--rw-rw-rw-   0        0        0     1074 2023-07-12 18:27:38.000000 extrack-1.5.8/LICENSE
--rw-rw-rw-   0        0        0     6889 2023-07-12 18:46:59.034444 extrack-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     6083 2023-07-12 18:27:38.000000 extrack-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 18:46:58.981034 extrack-1.5.8/Tutorials/
--rw-rw-rw-   0        0        0        1 2023-07-12 18:27:38.000000 extrack-1.5.8/Tutorials/__init__.py
--rw-rw-rw-   0        0        0     3979 2023-07-12 18:27:38.000000 extrack-1.5.8/Tutorials/automated_fitting.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:46:58.996658 extrack-1.5.8/extrack/
--rw-rw-rw-   0        0        0      367 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/__init__.py
--rw-rw-rw-   0        0        0     6484 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/auto_fitting.py
--rw-rw-rw-   0        0        0    23781 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/exporters.py
--rw-rw-rw-   0        0        0    24031 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/histograms.py
--rw-rw-rw-   0        0        0    40699 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/old_tracking.py
--rw-rw-rw-   0        0        0    10492 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/readers.py
--rw-rw-rw-   0        0        0    22606 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/refined_loc_old.py
--rw-rw-rw-   0        0        0    25414 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/refined_localization.py
--rw-rw-rw-   0        0        0    10688 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/simulate_tracks.py
--rw-rw-rw-   0        0        0    73925 2023-07-12 18:44:27.000000 extrack-1.5.8/extrack/tracking.py
--rw-rw-rw-   0        0        0    58805 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/tracking_0.py
--rw-rw-rw-   0        0        0       23 2023-07-12 18:28:46.000000 extrack-1.5.8/extrack/version.py
--rw-rw-rw-   0        0        0     5227 2023-07-12 18:27:38.000000 extrack-1.5.8/extrack/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-12 18:46:59.034444 extrack-1.5.8/extrack.egg-info/
--rw-rw-rw-   0        0        0     6889 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      935 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-12 18:46:58.000000 extrack-1.5.8/extrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      104 2023-07-12 18:27:38.000000 extrack-1.5.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-12 18:46:59.034444 extrack-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-07-12 18:27:38.000000 extrack-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:25:46.920197 extrack-1.6/
+-rw-rw-rw-   0        0        0     1074 2024-04-11 23:22:23.000000 extrack-1.6/LICENSE
+-rw-rw-rw-   0        0        0     6985 2024-04-11 23:25:46.919199 extrack-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6083 2024-04-11 23:22:23.000000 extrack-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 23:25:46.838196 extrack-1.6/Tutorials/
+-rw-rw-rw-   0        0        0        1 2024-04-11 23:22:38.000000 extrack-1.6/Tutorials/__init__.py
+-rw-rw-rw-   0        0        0     3979 2024-04-11 23:22:38.000000 extrack-1.6/Tutorials/automated_fitting.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:25:46.868196 extrack-1.6/extrack/
+-rw-rw-rw-   0        0        0      367 2024-04-11 23:22:39.000000 extrack-1.6/extrack/__init__.py
+-rw-rw-rw-   0        0        0     6484 2024-04-11 23:22:39.000000 extrack-1.6/extrack/auto_fitting.py
+-rw-rw-rw-   0        0        0    23781 2024-04-11 23:22:39.000000 extrack-1.6/extrack/exporters.py
+-rw-rw-rw-   0        0        0    24031 2024-04-11 23:22:39.000000 extrack-1.6/extrack/histograms.py
+-rw-rw-rw-   0        0        0    40699 2024-04-11 23:22:39.000000 extrack-1.6/extrack/old_tracking.py
+-rw-rw-rw-   0        0        0    10311 2024-04-11 23:22:39.000000 extrack-1.6/extrack/readers.py
+-rw-rw-rw-   0        0        0    22606 2024-04-11 23:22:39.000000 extrack-1.6/extrack/refined_loc_old.py
+-rw-rw-rw-   0        0        0    25414 2024-04-11 23:22:39.000000 extrack-1.6/extrack/refined_localization.py
+-rw-rw-rw-   0        0        0    10688 2024-04-11 23:22:39.000000 extrack-1.6/extrack/simulate_tracks.py
+-rw-rw-rw-   0        0        0    73924 2024-04-11 23:22:39.000000 extrack-1.6/extrack/tracking.py
+-rw-rw-rw-   0        0        0    58805 2024-04-11 23:22:39.000000 extrack-1.6/extrack/tracking_0.py
+-rw-rw-rw-   0        0        0       20 2024-04-11 23:23:24.000000 extrack-1.6/extrack/version.py
+-rw-rw-rw-   0        0        0     5227 2024-04-11 23:22:39.000000 extrack-1.6/extrack/visualization.py
+drwxrwxrwx   0        0        0        0 2024-04-11 23:25:46.917198 extrack-1.6/extrack.egg-info/
+-rw-rw-rw-   0        0        0     6985 2024-04-11 23:25:46.000000 extrack-1.6/extrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      935 2024-04-11 23:25:46.000000 extrack-1.6/extrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 23:25:46.000000 extrack-1.6/extrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-11 23:25:46.000000 extrack-1.6/extrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-11 23:25:46.000000 extrack-1.6/extrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      104 2024-04-11 23:22:23.000000 extrack-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 23:25:46.921196 extrack-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2024-04-11 23:22:23.000000 extrack-1.6/setup.py
```

### Comparing `extrack-1.5.8/LICENSE` & `extrack-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/PKG-INFO` & `extrack-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: extrack
-Version: 1.5.8
+Version: 1.6
 Summary: SPT kinetic modelling and states annotation of tracks
 Home-page: https://github.com/FrancoisSimon/ExTrack-python3
 Author: Francois Simon
 Author-email: simon.francois@protonmail.com
 Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lmfit
+Requires-Dist: xmltodict
+Requires-Dist: pandas
+Requires-Dist: matplotlib
 
 ExTrack
 -------
 
 This repository contains the necessary scripts to run the method ExTrack. ExTrack is a method to detemine kinetics of particles able to transition between different motion states. It can assess diffusion coefficients, transition rates, localization error as well as annotating the probability for any track to be in each state for every time points. It can produce histograms of durations in each state to highlight no markovian transition kinetics. Eventually it can be used to refine the localization precision of tracks by considering the most likely positions which is especially efficient when the particle do not move.
 
 More details on the methods are available on BioarXiv https://www.biorxiv.org/content/10.1101/2022.07.13.499913v1.
```

### Comparing `extrack-1.5.8/README.md` & `extrack-1.6/README.md`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/Tutorials/automated_fitting.py` & `extrack-1.6/Tutorials/automated_fitting.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/auto_fitting.py` & `extrack-1.6/extrack/auto_fitting.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/exporters.py` & `extrack-1.6/extrack/exporters.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/histograms.py` & `extrack-1.6/extrack/histograms.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/old_tracking.py` & `extrack-1.6/extrack/old_tracking.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/readers.py` & `extrack-1.6/extrack/readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,28 +147,21 @@
             None_ID = (data[colnames[3]] == 'None' ) + pd.isna(data[colnames[3]])
             max_ID = np.max(data[colnames[3]][(data[colnames[3]] != 'None' ) * (pd.isna(data[colnames[3]]) == False)].astype(int))
             data.loc[None_ID, colnames[3]] = np.arange(max_ID+1, max_ID+1 + np.sum(None_ID))
         except:
             None_ID = (data[colnames[3]] == 'None' ) + pd.isna(data[colnames[3]])
             data = data.drop(data[None_ID].index)
         
-        IDs = data[colnames[3]].astype(str)
-
         data = data[colnames + opt_colnames]
         
-        track_list = []
-        for ID in np.unique(IDs):
-            track_list.append(data[IDs == ID])
-        
         zero_disp_tracks = 0
             
         try:
-            for ID in np.unique(IDs):
+            for ID, track in data.groupby(colnames[3]):
                 
-                track = data[IDs == ID]
                 track = track.sort_values(colnames[2], axis = 0)
                 track_mat = track.values[:,:3].astype('float64')
                 dists = np.sum((track_mat[1:, :2] - track_mat[:-1, :2])**2, axis = 1)**0.5
                 if track_mat[0, 2] >= frames_boundaries[0] and track_mat[0, 2] <= frames_boundaries[1] : #and np.all(dists<dist_th):
                     if not np.any(dists>dist_th):
                         
                         if np.any([len(track_mat)]*len(lengths) == np.array(lengths)):
```

### Comparing `extrack-1.5.8/extrack/refined_loc_old.py` & `extrack-1.6/extrack/refined_loc_old.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/refined_localization.py` & `extrack-1.6/extrack/refined_localization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/simulate_tracks.py` & `extrack-1.6/extrack/simulate_tracks.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/tracking.py` & `extrack-1.6/extrack/tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -600,15 +600,15 @@
         m_arr = cp.repeat(m_arr, nb_states**nb_substeps , axis = 1)
         s2_arr = cp.repeat(s2_arr, nb_states**nb_substeps, axis = 1)
         LP = cp.repeat(LP, nb_states**nb_substeps, axis = 1)
         
         end_p_stay = p_stay[cur_states[:,None:,:-1]][:,:,0]
         LL = cp.log(pBL + (1-end_p_stay) - pBL * (1-end_p_stay)) + LT
         cur_Bs_cat = cur_Bs_cat[:,:,1:]
-    
+
     new_s2_arr = cp.array((s2_arr + LocErr2[:,:, min(LocErr_index, nb_locs-current_step)]))
     log_integrated_term = cp.sum(-0.5*cp.log(2*np.pi*new_s2_arr) - (Cs[:,:,0] - m_arr)**2/(2*new_s2_arr),axis=2)
     #LF = cp.log(Fs[cur_Bs[:,:,0].astype(int)]) # Log proba of starting in a given state (fractions)
     #LF = cp.log(0.5)
     # cp.mean(cp.log(Fs[cur_Bs[:,:,:].astype(int)]), 2) # Log proba of starting in a given state (fractions)
     LP += log_integrated_term + LL
     
@@ -823,15 +823,15 @@
     Csss = []
     sigss = []
     isBLs = []
     for k in range(len(all_tracks)):
         Css = all_tracks[k]
         if input_LocErr != None:
             sigs = LocErr[k]
-        nb_max = 1
+        nb_max = 1000
         for n in range(int(np.ceil(len(Css)/nb_max))):
             Csss.append(Css[n*nb_max:(n+1)*nb_max])
             if input_LocErr != None:
                 sigss.append(sigs[n*nb_max:(n+1)*nb_max])
             if Css.shape[1] == max_len:
                 isBLs.append(0) # last position correspond to tracks which didn't disapear within maximum track length
             else:
```

### Comparing `extrack-1.5.8/extrack/tracking_0.py` & `extrack-1.6/extrack/tracking_0.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack/visualization.py` & `extrack-1.6/extrack/visualization.py`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/extrack.egg-info/PKG-INFO` & `extrack-1.6/extrack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: extrack
-Version: 1.5.8
+Version: 1.6
 Summary: SPT kinetic modelling and states annotation of tracks
 Home-page: https://github.com/FrancoisSimon/ExTrack-python3
 Author: Francois Simon
 Author-email: simon.francois@protonmail.com
 Project-URL: Bug Tracker, https://github.com/FrancoisSimon/ExTrack-python3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: lmfit
+Requires-Dist: xmltodict
+Requires-Dist: pandas
+Requires-Dist: matplotlib
 
 ExTrack
 -------
 
 This repository contains the necessary scripts to run the method ExTrack. ExTrack is a method to detemine kinetics of particles able to transition between different motion states. It can assess diffusion coefficients, transition rates, localization error as well as annotating the probability for any track to be in each state for every time points. It can produce histograms of durations in each state to highlight no markovian transition kinetics. Eventually it can be used to refine the localization precision of tracks by considering the most likely positions which is especially efficient when the particle do not move.
 
 More details on the methods are available on BioarXiv https://www.biorxiv.org/content/10.1101/2022.07.13.499913v1.
```

### Comparing `extrack-1.5.8/extrack.egg-info/SOURCES.txt` & `extrack-1.6/extrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extrack-1.5.8/setup.py` & `extrack-1.6/setup.py`

 * *Files identical despite different names*

