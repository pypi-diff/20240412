# Comparing `tmp/ngmt-0.0.3.tar.gz` & `tmp/ngmt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngmt-0.0.3.tar", max compression
+gzip compressed data, was "ngmt-0.0.4.tar", max compression
```

## Comparing `ngmt-0.0.3.tar` & `ngmt-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0    11926 2024-02-05 18:55:10.915536 ngmt-0.0.3/LICENSE
--rw-r--r--   0        0        0       89 2023-12-06 09:20:45.170170 ngmt-0.0.3/ngmt/__init__.py
--rw-r--r--   0        0        0      254 2023-10-25 18:27:53.559669 ngmt-0.0.3/ngmt/config.py
--rw-r--r--   0        0        0     3267 2023-10-17 14:03:42.152297 ngmt-0.0.3/ngmt/datasets/__pycache__/keepcontrol.cpython-311.pyc
--rw-r--r--   0        0        0     1954 2023-11-22 13:05:04.448351 ngmt-0.0.3/ngmt/datasets/__pycache__/mobilised.cpython-311.pyc
--rw-r--r--   0        0        0     3445 2024-01-30 13:54:04.530370 ngmt-0.0.3/ngmt/datasets/fairpark.py
--rw-r--r--   0        0        0     3338 2024-01-22 13:25:55.740983 ngmt-0.0.3/ngmt/datasets/keepcontrol.py
--rw-r--r--   0        0        0     5413 2024-01-22 13:25:55.741984 ngmt-0.0.3/ngmt/datasets/mobilised.py
--rw-r--r--   0        0        0        0 2024-02-05 19:01:05.946601 ngmt-0.0.3/ngmt/modules/__init__.py
--rw-r--r--   0        0        0       63 2024-02-05 19:01:05.947602 ngmt-0.0.3/ngmt/modules/gsd/__init__.py
--rw-r--r--   0        0        0    18846 2024-02-05 19:01:05.947602 ngmt-0.0.3/ngmt/modules/gsd/_paraschiv.py
--rw-r--r--   0        0        0       65 2024-02-05 19:01:05.948604 ngmt-0.0.3/ngmt/modules/icd/__init__.py
--rw-r--r--   0        0        0     8553 2024-02-13 12:33:43.854142 ngmt-0.0.3/ngmt/modules/icd/_paraschiv.py
--rw-r--r--   0        0        0       46 2024-02-05 19:01:05.950605 ngmt-0.0.3/ngmt/modules/pam/__init__.py
--rw-r--r--   0        0        0    12169 2024-02-13 12:33:43.855143 ngmt-0.0.3/ngmt/modules/pam/_pam.py
--rw-r--r--   0        0        0    74764 2024-02-06 14:39:39.879177 ngmt-0.0.3/ngmt/test/example_lower_back_acc.csv
--rw-r--r--   0        0        0    81563 2024-02-19 08:28:44.036698 ngmt-0.0.3/ngmt/test/test_calc.py
--rw-r--r--   0        0        0    14446 2024-02-19 08:28:44.037750 ngmt-0.0.3/ngmt/test/test_modules.py
--rw-r--r--   0        0        0     1840 2023-10-17 14:03:42.163548 ngmt-0.0.3/ngmt/utils/__pycache__/data_utils.cpython-311.pyc
--rw-r--r--   0        0        0    11880 2023-11-22 13:05:09.428512 ngmt-0.0.3/ngmt/utils/__pycache__/matlab_loader.cpython-311.pyc
--rw-r--r--   0        0        0    28092 2023-10-17 14:03:42.166548 ngmt-0.0.3/ngmt/utils/__pycache__/preprocessing.cpython-311.pyc
--rw-r--r--   0        0        0    19593 2024-02-05 19:01:05.951606 ngmt-0.0.3/ngmt/utils/data_classes.py
--rw-r--r--   0        0        0     1576 2024-01-30 14:01:38.261357 ngmt-0.0.3/ngmt/utils/file_io.py
--rw-r--r--   0        0        0      725 2023-10-17 14:03:42.162047 ngmt-0.0.3/ngmt/utils/FIR_2_3Hz_40.mat
--rw-r--r--   0        0        0     6548 2024-01-08 10:54:49.957245 ngmt-0.0.3/ngmt/utils/importers.py
--rw-r--r--   0        0        0     8877 2023-12-07 06:50:15.817538 ngmt-0.0.3/ngmt/utils/matlab_loader.py
--rw-r--r--   0        0        0       77 2023-12-06 09:20:45.174681 ngmt-0.0.3/ngmt/utils/orientation_estimation/__init__.py
--rw-r--r--   0        0        0     8016 2024-01-30 13:54:04.531120 ngmt-0.0.3/ngmt/utils/orientation_estimation/_madgwick.py
--rw-r--r--   0        0        0    40850 2024-02-13 12:33:43.859146 ngmt-0.0.3/ngmt/utils/preprocessing.py
--rw-r--r--   0        0        0    16505 2024-01-22 13:25:55.745067 ngmt-0.0.3/ngmt/utils/quaternion.py
--rw-r--r--   0        0        0     1535 2024-02-27 09:49:51.084681 ngmt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7446 2024-02-20 13:46:58.271185 ngmt-0.0.3/README.md
--rw-r--r--   0        0        0     8758 1970-01-01 00:00:00.000000 ngmt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1637 2024-03-25 10:13:41.304870 ngmt-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0    11926 2024-02-05 18:55:10.915536 ngmt-0.0.4/LICENSE
+-rw-r--r--   0        0        0       89 2023-12-06 09:20:45.170170 ngmt-0.0.4/ngmt/__init__.py
+-rw-r--r--   0        0        0      254 2023-10-25 18:27:53.559669 ngmt-0.0.4/ngmt/config.py
+-rw-r--r--   0        0        0     3267 2023-10-17 14:03:42.152297 ngmt-0.0.4/ngmt/datasets/__pycache__/keepcontrol.cpython-311.pyc
+-rw-r--r--   0        0        0     1954 2023-11-22 13:05:04.448351 ngmt-0.0.4/ngmt/datasets/__pycache__/mobilised.cpython-311.pyc
+-rw-r--r--   0        0        0     3770 2024-03-27 13:34:21.158919 ngmt-0.0.4/ngmt/datasets/fairpark.py
+-rw-r--r--   0        0        0     3802 2024-03-26 09:31:44.533667 ngmt-0.0.4/ngmt/datasets/keepcontrol.py
+-rw-r--r--   0        0        0     5708 2024-03-26 08:54:32.683975 ngmt-0.0.4/ngmt/datasets/mobilised.py
+-rw-r--r--   0        0        0        0 2024-02-05 19:01:05.946601 ngmt-0.0.4/ngmt/modules/__init__.py
+-rw-r--r--   0        0        0       63 2024-02-05 19:01:05.947602 ngmt-0.0.4/ngmt/modules/gsd/__init__.py
+-rw-r--r--   0        0        0    18614 2024-04-10 11:07:36.953762 ngmt-0.0.4/ngmt/modules/gsd/_paraschiv.py
+-rw-r--r--   0        0        0       65 2024-02-05 19:01:05.948604 ngmt-0.0.4/ngmt/modules/icd/__init__.py
+-rw-r--r--   0        0        0     8066 2024-04-10 11:07:36.954763 ngmt-0.0.4/ngmt/modules/icd/_paraschiv.py
+-rw-r--r--   0        0        0       46 2024-02-05 19:01:05.950605 ngmt-0.0.4/ngmt/modules/pam/__init__.py
+-rw-r--r--   0        0        0    11373 2024-04-03 11:14:24.260787 ngmt-0.0.4/ngmt/modules/pam/_pam.py
+-rw-r--r--   0        0        0       54 2024-03-25 10:13:41.422984 ngmt-0.0.4/ngmt/modules/ssd/__init__.py
+-rw-r--r--   0        0        0    18691 2024-04-03 10:43:43.445082 ngmt-0.0.4/ngmt/modules/ssd/_pham.py
+-rw-r--r--   0        0        0    74764 2024-02-06 14:39:39.879177 ngmt-0.0.4/ngmt/test/example_lower_back_acc.csv
+-rw-r--r--   0        0        0     3620 2024-04-10 06:27:18.412150 ngmt-0.0.4/ngmt/test/scripts/test.py
+-rw-r--r--   0        0        0    75148 2024-04-03 06:06:54.023692 ngmt-0.0.4/ngmt/test/test_calc.py
+-rw-r--r--   0        0        0    22428 2024-04-10 11:12:54.428105 ngmt-0.0.4/ngmt/test/test_modules.py
+-rw-r--r--   0        0        0     1840 2023-10-17 14:03:42.163548 ngmt-0.0.4/ngmt/utils/__pycache__/data_utils.cpython-311.pyc
+-rw-r--r--   0        0        0    11880 2023-11-22 13:05:09.428512 ngmt-0.0.4/ngmt/utils/__pycache__/matlab_loader.cpython-311.pyc
+-rw-r--r--   0        0        0    28092 2023-10-17 14:03:42.166548 ngmt-0.0.4/ngmt/utils/__pycache__/preprocessing.cpython-311.pyc
+-rw-r--r--   0        0        0     1576 2024-01-30 14:01:38.261357 ngmt-0.0.4/ngmt/utils/file_io.py
+-rw-r--r--   0        0        0      725 2023-10-17 14:03:42.162047 ngmt-0.0.4/ngmt/utils/FIR_2_3Hz_40.mat
+-rw-r--r--   0        0        0     2308 2024-03-26 09:36:01.996166 ngmt-0.0.4/ngmt/utils/importers.py
+-rw-r--r--   0        0        0     8877 2023-12-07 06:50:15.817538 ngmt-0.0.4/ngmt/utils/matlab_loader.py
+-rw-r--r--   0        0        0    10252 2024-03-26 07:39:58.738534 ngmt-0.0.4/ngmt/utils/ngmt_dataclass.py
+-rw-r--r--   0        0        0       77 2023-12-06 09:20:45.174681 ngmt-0.0.4/ngmt/utils/orientation_estimation/__init__.py
+-rw-r--r--   0        0        0     8016 2024-01-30 13:54:04.531120 ngmt-0.0.4/ngmt/utils/orientation_estimation/_madgwick.py
+-rw-r--r--   0        0        0    59693 2024-04-10 06:27:18.414152 ngmt-0.0.4/ngmt/utils/preprocessing.py
+-rw-r--r--   0        0        0    18224 2024-03-25 10:13:41.428990 ngmt-0.0.4/ngmt/utils/quaternion.py
+-rw-r--r--   0        0        0     1611 2024-04-12 11:24:15.270130 ngmt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     7821 2024-04-12 11:16:22.931402 ngmt-0.0.4/README.md
+-rw-r--r--   0        0        0     9150 1970-01-01 00:00:00.000000 ngmt-0.0.4/PKG-INFO
```

### Comparing `ngmt-0.0.3/LICENSE` & `ngmt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/datasets/__pycache__/keepcontrol.cpython-311.pyc` & `ngmt-0.0.4/ngmt/datasets/__pycache__/keepcontrol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/datasets/__pycache__/mobilised.cpython-311.pyc` & `ngmt-0.0.4/ngmt/datasets/__pycache__/mobilised.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/datasets/fairpark.py` & `ngmt-0.0.4/ngmt/datasets/fairpark.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import pandas as pd
 import seaborn as sns
 import os
 import pathlib
 import polars as pl
-from ngmt.utils.data_classes import NGMTRecording
+from ngmt.utils.ngmt_dataclass import NGMTRecording
 
 
 SAMPLING_FREQ_HZ: float = 100.0  # sampling frequency
 
 MAP_CHANNEL_UNITS = {"ACCEL": "m/s^2", "ANGVEL": "deg/s", "MAGN": "Gauss"}
 
 
 def load_recording(
     file_name: str | pathlib.Path,
     tracking_systems: str | list[str] = ["imu"],
     tracked_points: str | list[str] | dict[str, str] | dict[str, list[str]] = {
-        "imu": "LARM"
+        "imu": ["LARM"]
     },
 ) -> NGMTRecording:
-    """Load a recording from the FAIRPARK study.
+    """
+    Load a recording from the FAIRPARK II validation study.
+
+    Args:
+        file_name (str or pathlib.Path ): The absolute or relative path to the data file.
+        tracking_systems (str or list of str) : A string or list of strings of tracking systems for which data are to be returned.
+        tracked_points (str or list of str or dict[str, str] or dict[str, list of str]) :
+            Defines for which tracked points data are to be returned.
+            If a string or list of strings is provided, then these will be mapped to each requested tracking system.
+            If a dictionary is provided, it should map each tracking system to either a single tracked point or a list of tracked points.
 
-    Parameters
-    ----------
-    file_name : str | pathlib.Path
-        The absolute or relative path to the data file.
-    tracking_systems : str | list[str]
-        A string or list of strings of tracking systems for which data are to be returned.
-    tracked_points : str | list[str] | dict[str, str] | dict[str, list[str]]
-        Defines for which tracked points data are to be returned.
-        If a string or list of strings is provided, then these will be mapped to each requested tracking system.
-
-    Returns
-    -------
-    _ : NGMTRecording
-        An instance of the NGMTRecording dataclass.
+    Returns:
+        NGMTRecording : An instance of the NGMTRecording dataclass containing the loaded data and channels.
     """
     # Put tracking systems in a list
     if isinstance(tracking_systems, str):
         tracking_systems = [tracking_systems]
 
     # Tracked points will be a dictionary mapping
     # each tracking system to a list of tracked points of interest
@@ -48,16 +45,18 @@
     if isinstance(tracked_points, list):
         tracked_points = {tracksys: tracked_points for tracksys in tracking_systems}
     for k, v in tracked_points.items():
         if isinstance(v, str):
             tracked_points[k] = [v]
 
     # Extract relevant metadata from filename
-    sub_id = os.path.split(file_name)[1][4:7]
-    tracked_point = os.path.split(file_name)[1][12:16]
+    file_name_parts = os.path.splitext(os.path.basename(file_name))[0].split("_")
+    tracked_point = next((part for part in file_name_parts if "imu-" in part), None)
+    if tracked_point:
+        tracked_point = tracked_point.split("-")[-1]
 
     # Load the data from the file
     col_names = [
         f"{tracked_point}_{s}_{x}"
         for s in ["ACCEL", "ANGVEL", "MAGN"]
         for x in ["x", "y", "z"]
     ] + ["year", "month", "day", "hour", "minute", "second"]
@@ -76,16 +75,16 @@
         axis=1,
         inplace=True,
     )
 
     # Make the channel dictionary
     channels_dict = {
         "name": df.columns.to_list(),
-        "type": [f"{s}" for s in ["ACCEL", "ANGVEL", "MAGN"] for _ in range(3)],
         "component": [f"{x}" for _ in range(3) for x in ["x", "y", "z"]],
+        "type": [f"{s}" for s in ["ACCEL", "ANGVEL", "MAGN"] for _ in range(3)],
         "tracked_point": [tracked_point for _ in range(len(df.columns))],
         "units": [
             f"{MAP_CHANNEL_UNITS[s]}"
             for s in ["ACCEL", "ANGVEL", "MAGN"]
             for _ in range(3)
         ],
         "sampling_frequency": [SAMPLING_FREQ_HZ for _ in range(len(df.columns))],
```

### Comparing `ngmt-0.0.3/ngmt/datasets/mobilised.py` & `ngmt-0.0.4/ngmt/datasets/mobilised.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 import pathlib
 from ngmt.utils import matlab_loader
-from ngmt.utils.data_classes import NGMTRecording
+from ngmt.utils.ngmt_dataclass import NGMTRecording
 
 
 # See: https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html#restricted-keyword-list-for-channel-type
 MAP_CHANNEL_TYPES = {
     "Acc": "ACCEL",
     "Gyr": "GYRO",
     "Mag": "MAGN",
@@ -31,30 +31,27 @@
 
 
 def load_recording(
     file_name: str | pathlib.Path,
     tracking_systems: str | list[str],
     tracked_points: str | list[str] | dict[str, str] | dict[str, list[str]],
 ):
-    """Load a recording from the Mobilise-D dataset.
+    """
+    Load a recording from the Mobilise-D dataset.
+
+    Args:
+        file_name (str or pathlib.Path ): The absolute or relative path to the data file.
+        tracking_systems (str or list of str) : A string or list of strings of tracking systems for which data are to be returned.
+        tracked_points (str or list of str or dict[str, str] or dict[str, list of str]) :
+            Defines for which tracked points data are to be returned.
+            If a string or list of strings is provided, then these will be mapped to each requested tracking system.
+            If a dictionary is provided, it should map each tracking system to either a single tracked point or a list of tracked points.
 
-    Parameters
-    ----------
-    file_name : str | pathlib.Path
-        The absolute or relative path to the data file.
-    tracking_systems : str | list[str]
-        A string or list of strings of tracking systems for which data are to be returned.
-    tracked_points : str | list[str] | dict[str, str] | dict[str, list[str]]
-        Defines for which tracked points data are to be returned.
-        If a string or list of strings is provided, then these will be mapped to each requested tracking system.
-
-    Returns
-    -------
-    _ : NGMTRecording
-        An instance of the NGMTRecording dataclass.
+    Returns:
+        NGMTRecording : An instance of the NGMTRecording dataclass containing the loaded data and channels.
     """
     # Put tracking systems into a list
     if isinstance(tracking_systems, str):
         tracking_systems = [tracking_systems]
 
     # Tracked points will be a dictionary mapping
     # each tracking system to a list of tracked points of interest
@@ -71,20 +68,20 @@
 
     # Extract data for given tracking system
     recording_data = dict()
     channel_data = dict()
     for tracksys in tracking_systems:
         channel_data[tracksys] = {
             "name": [],
-            "type": [],
             "component": [],
+            "type": [],
             "tracked_point": [],
             "units": [],
             "sampling_frequency": [],
-        }
+        }  # ['name', 'component', 'type', 'tracked_point', 'units', 'sampling_frequency']
 
         data_arr = None
         for tracked_point in data_dict["TimeMeasure1"]["Recording4"][tracksys].keys():
             if tracked_point in tracked_points[tracksys]:
                 for ch_type in data_dict["TimeMeasure1"]["Recording4"][tracksys][
                     tracked_point
                 ].keys():
@@ -104,15 +101,16 @@
                                 )
                             )
                         channel_data[tracksys]["name"] += [
                             f"{tracked_point}_{MAP_CHANNEL_TYPES[ch_type]}_{ch_comp}"
                             for ch_comp in MAP_CHANNEL_COMPONENTS[ch_type]
                         ]
                         channel_data[tracksys]["type"] += [
-                            ch_type for _ in range(len(MAP_CHANNEL_COMPONENTS[ch_type]))
+                            MAP_CHANNEL_TYPES[ch_type]
+                            for _ in range(len(MAP_CHANNEL_COMPONENTS[ch_type]))
                         ]
                         channel_data[tracksys]["component"] += [
                             ch_comp for ch_comp in MAP_CHANNEL_COMPONENTS[ch_type]
                         ]
                         channel_data[tracksys]["tracked_point"] += [
                             tracked_point
                             for ch_comp in range(len(MAP_CHANNEL_COMPONENTS[ch_type]))
```

### Comparing `ngmt-0.0.3/ngmt/modules/gsd/_paraschiv.py` & `ngmt-0.0.4/ngmt/modules/gsd/_paraschiv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,177 @@
+from datetime import datetime
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import scipy.signal
+from typing import Optional
 from ngmt.utils import preprocessing
 from ngmt.config import cfg_colors
 
 
 class ParaschivIonescuGaitSequenceDetection:
     """
-    Detects gait sequences based on identified steps in accelerometer data.
+    The Paraschiv-Ionescu gait sequence detection algorithm identifies gait sequences in accelerometer data from a lower back sensor.
 
-    Attributes:
-        target_sampling_freq_Hz (float): Target sampling frequency for resampling the data. Default is 40.
-        event_type (str): Type of the detected event. Default is 'gait sequence'.
-        tracking_systems (str): Tracking systems used. Default is 'SU'.
-        tracked_points (str): Tracked points on the body. Default is 'LowerBack'.
-        gait_sequences_ (pd.DataFrame): DataFrame containing gait sequence information in BIDS format.
-
-    Description:
-        This function performs Paraschiv-Ionescu gait sequence detection on accelerometer data
-        collected from a lower back sensor. The purpose of this algortihm is to identify and
-        characterize walking bouts or gait sequences within the input data.
-
-        The input accelerometer data should be provided as a numpy.ndarray with shape
-        (N, 3), where N is the number of data points. The three columns represent the
-        acceleration along the x, y, and z axes.
-
-        The function processes the input data through a series of signal processing steps
-        including resampling, filtering, wavelet transform, and peak detection to identify
-        gait sequences. Finally, the gait sequence information is stored in the 'gait_sequences_' attribute,
-        which is a pandas DataFrame in BIDS format with the columns including onset, duration, event_type,
-        tracked_systems and tracking_points.
-
-        If `plot_results` is set to True, the function will also generate a plot showing
-        the pre-processed acceleration data and the detected gait sequences for
-        visualization purposes. Default is False.
+    The algorithm detects gait sequences based on identified steps. It starts by loading the accelerometer data, which includes three
+    columns corresponding to the acceleration signals across the x, y, and z axes, along with the sampling frequency of the data. To
+    simplify the analysis, the norm of acceleration is computed. Next, the signal is resampled at a 40 Hz sampling frequency using
+    interpolation. Smoothing is then applied through a Savitzky-Golay filter and a Finite Impulse Response (FIR) low-pass filter to
+    remove noise and drifts from the signal. The continuous wavelet transform is applied to capture gait-related features, followed by
+    additional smoothing using successive Gaussian-weighted filters. The processed data is then analyzed to detect gait sequences.
+
+    The algorithm continues by identifying the envelope of the processed acceleration signal. Active periods of the signal are identified
+    using the Hilbert envelope. The statistical distribution of the amplitude of the peaks in these active periods is used to derive an
+    adaptive threshold. In case the Hilbert envelope algorithm fails to detect active periods, a fixed threshold value (0.15 g) is used
+    for peak detection in the signal. Mid-swing peaks are detected based on this threshold. Pulse trains in the local maximum and minimum
+    of the peaks are identified, with those having fewer than four steps filtered out. The intersection of pulse trains from local maximum
+    and minimum peaks is detected as walking periods. These periods are then organized and grouped to update the start and end times of
+    detected walking bouts.
+
+    Next, the algorithm takes the last steps to detect walking bouts in the signal. For this purpose, walking bouts with five or more steps
+    are detected, and their start and end times are added to the list. Walking labels are generated as an array of zeros, and the intervals
+    corresponding to the walking bouts are labeled as 1. Groups of consecutive zeros in the walking labels are identified, and if breaks
+    between walking bouts are less than three seconds, they are merged. If gait sequences are found, the output is printed; otherwise, a
+    message indicating that no gait sequences are detected is displayed.
+
+    Finally, the gait sequence information is stored in the 'gait_sequences_' attribute in BIDS compatible format with columns `onset`,
+    `duration`, `event_type`, `tracking_system` as Pandas DataFrame.
 
     Methods:
         detect(data, sampling_freq_Hz, plot_results=False):
-            Detects gait sequences on the accelerometer signal.
+            Detects gait sequences in the provided accelerometer data.
+
+    Examples:
+        >>> gsd = ParaschivIonescuGaitSequenceDetection()
+        >>> gsd.detect(data=acceleration_data, sampling_freq_Hz=100, plot_results=True)
+        >>> print(gsd.gait_sequences_)
+                onset   duration    event_type      tracking_systems
+            0   4.500   5.25        gait sequence   SU
+            1   90.225  10.30       gait sequence   SU
+
+    References:
+        [1] Paraschiv-Ionescu et al. (2019). Locomotion and cadence detection using a single trunk-fixed accelerometer...
 
-            Args:
-                data (pd.DataFrame): Input accelerometer data (N, 3) for x, y, and z axes.
-                sampling_freq_Hz (float): Sampling frequency of the accelerometer data.
-                plot_results (bool, optional): If True, generates a plot showing the pre-processed acceleration data
-                    and the detected gait sequences. Default is False.
-
-            Returns:
-                ParaschivIonescuGaitSequenceDetection: Returns an instance of the class.
-                    The gait sequence information is stored in the 'gait_sequences_' attribute,
-                    which is a pandas DataFrame in BIDS format with the following columns:
-                        - onset: Start time of the gait sequence.
-                        - duration: Duration of the gait sequence.
-                        - event_type: Type of the event (default is 'gait sequence').
-                        - tracking_systems: Tracking systems used (default is 'SU').
-                        - tracked_points: Tracked points on the body (default is 'LowerBack').
-
-        Examples:
-            Find sequences of gait in sensor signal
-
-            >>> gsd = ParaschivIonescuGaitSequenceDetection()
-            >>> gsd.detect(data=acceleration_data, sampling_freq_Hz=100, plot_results=True)
-            >>> gait_sequences = gsd.gait_sequences_
-            >>> print(gait_sequences)
-                    onset   duration    event_type      tracking_systems    tracked_points
-                0   4.500   5.25        gait sequence   SU                  LowerBack
-                1   90.225  10.30       gait sequence   SU                  LowerBack
-
-        References:
-            [1] Paraschiv-Ionescu et al. (2019). Locomotion and cadence detection using a single trunk-fixed accelerometer:
-                validity for children with cerebral palsy in daily life-like conditions.
-                Journal of NeuroEngineering and Rehabilitation, 16(1), 24.
-                https://doi.org/10.1186/s12984-019-0494-z
-            [2] Paraschiv-Ionescu et al. (2020). Real-world speed estimation using single trunk IMU:
-                methodological challenges for impaired gait patterns.
-                Annual International Conference of the IEEE Engineering in Medicine and Biology Society.
-                IEEE Engineering in Medicine and Biology Society. https://doi.org/10.1109/EMBC44109.2020.9176281
+        [2] Paraschiv-Ionescu et al. (2020). Real-world speed estimation using single trunk IMU...
     """
 
     def __init__(
         self,
-        target_sampling_freq_Hz: float = 40.0,
-        event_type: str = "gait sequence",
-        tracking_systems: str = "SU",
-        tracked_points: str = "LowerBack",
     ):
         """
         Initializes the ParaschivIonescuGaitSequenceDetection instance.
-
-        Args:
-            target_sampling_freq_Hz (float, optional): Target sampling frequency for resampling the data. Default is 40.
-            event_type (str, optional): Type of the detected event. Default is 'gait sequence'.
-            tracking_systems (str, optional): Tracking systems used. Default is 'SU'.
-            tracked_points (str, optional): Tracked points on the body. Default is 'LowerBack'.
         """
-        self.target_sampling_freq_Hz = target_sampling_freq_Hz
-        self.event_type = event_type
-        self.tracking_systems = tracking_systems
-        self.tracked_points = tracked_points
         self.gait_sequences_ = None
 
     def detect(
-        self, data: pd.DataFrame, sampling_freq_Hz: float, plot_results: bool = False
+        self,
+        data: pd.DataFrame,
+        sampling_freq_Hz: float,
+        plot_results: bool = False,
+        dt_data: Optional[pd.Series] = None,
+        tracking_system: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         Detects gait sequences based on the input accelerometer data.
 
         Args:
             data (pd.DataFrame): Input accelerometer data (N, 3) for x, y, and z axes.
             sampling_freq_Hz (float): Sampling frequency of the accelerometer data.
             plot_results (bool, optional): If True, generates a plot showing the pre-processed acceleration data
-            and the detected gait sequences. Default is False.
-
-            Returns:
-                ParaschivIonescuGaitSequenceDetection: Returns an instance of the class.
-                    The gait sequence information is stored in the 'gait_sequences_' attribute,
-                    which is a pandas DataFrame in BIDS format with the following columns:
-                        - onset: Start time of the gait sequence.
-                        - duration: Duration of the gait sequence.
-                        - event_type: Type of the event (default is 'gait sequence').
-                        - tracking_systems: Tracking systems used (default is 'SU').
-                        - tracked_points: Tracked points on the body (default is 'LowerBack').
+                and the detected gait sequences. Default is False.
+            dt_data (pd.Series, optional): Original datetime in the input data. If original datetime is provided, the output onset will be based on that.
+            tracking_system (str, optional): Tracking system the data is from to be used for events df. Default is None.
+
+        Returns:
+            pd.DataFrame: The gait sequence information stored in the 'gait_sequences_' attribute,
+                which is a pandas DataFrame in BIDS format with the following columns:
+                    - onset: Start time of the gait sequence.
+                    - duration: Duration of the gait sequence.
+                    - event_type: Type of the event (default is 'gait sequence').
+                    - tracking_system: Tracking systems used the events are derived from.
         """
         # Error handling for invalid input data
         if not isinstance(data, pd.DataFrame) or data.shape[1] != 3:
             raise ValueError(
                 "Input accelerometer data must be a DataFrame with 3 columns for x, y, and z axes."
             )
 
         if not isinstance(sampling_freq_Hz, (int, float)) or sampling_freq_Hz <= 0:
             raise ValueError("Sampling frequency must be a positive float.")
 
         if not isinstance(plot_results, bool):
             raise ValueError("Plot results must be a boolean (True or False).")
 
+        # check if tracking_system is a string
+        if tracking_system is not None and not isinstance(tracking_system, str):
+            raise ValueError("tracking_system must be a string")
+
+        # check if dt_data is a pandas Series with datetime values
+        if dt_data is not None and (
+            not isinstance(dt_data, pd.Series)
+            or not pd.api.types.is_datetime64_any_dtype(dt_data)
+        ):
+            raise ValueError("dt_data must be a pandas Series with datetime values")
+
+        # check if dt_data is provided and if it is a series with the same length as data
+        if dt_data is not None and len(dt_data) != len(data):
+            raise ValueError("dt_data must be a series with the same length as data")
+
         # Calculate the norm of acceleration
         acceleration_norm = np.linalg.norm(data, axis=1)
 
         # Resample acceleration_norm to target sampling frequency
         initial_sampling_frequency = sampling_freq_Hz
+        target_sampling_freq_Hz = 40
         resampled_acceleration = preprocessing.resample_interpolate(
-            acceleration_norm, initial_sampling_frequency, self.target_sampling_freq_Hz
+            acceleration_norm, initial_sampling_frequency, target_sampling_freq_Hz
         )
 
         # Applying low-pass Savitzky-Golay filter to smoothen the resampled data
         smoothed_acceleration = preprocessing.lowpass_filter(
             resampled_acceleration,
             method="savgol",
             window_length=21,
             polynomial_order=7,
         )
 
         # Remove 40Hz drift from the filtered data
         drift_removed_acceleration = preprocessing.highpass_filter(
             signal=smoothed_acceleration,
-            sampling_frequency=self.target_sampling_freq_Hz,
+            sampling_frequency=target_sampling_freq_Hz,
             method="iir",
         )
 
         # Filter data using the fir low-pass filter
         filtered_acceleration = preprocessing.lowpass_filter(
             drift_removed_acceleration, method="fir"
         )
 
         # Perform the continuous wavelet transform on the filtered acceleration data
         wavelet_transform_result = preprocessing.apply_continuous_wavelet_transform(
             filtered_acceleration,
             scales=10,
             desired_scale=10,
             wavelet="gaus2",
-            sampling_frequency=self.target_sampling_freq_Hz,
+            sampling_frequency=target_sampling_freq_Hz,
         )
 
         # Applying Savitzky-Golay filter to further smoothen the wavelet transformed data
         smoothed_wavelet_result = preprocessing.lowpass_filter(
             wavelet_transform_result, window_length=11, polynomial_order=5
         )
 
         # Perform continuous wavelet transform
         further_smoothed_wavelet_result = (
             preprocessing.apply_continuous_wavelet_transform(
                 smoothed_wavelet_result,
                 scales=10,
                 desired_scale=10,
                 wavelet="gaus2",
-                sampling_frequency=self.target_sampling_freq_Hz,
+                sampling_frequency=target_sampling_freq_Hz,
             )
         )
         further_smoothed_wavelet_result = further_smoothed_wavelet_result.T
 
         # Smoothing the data using successive Gaussian filters
         filtered_signal = preprocessing.apply_successive_gaussian_filters(
             further_smoothed_wavelet_result
@@ -196,30 +179,29 @@
 
         # Use pre-processsed signal for post-processing purposes
         detected_activity_signal = filtered_signal
 
         # Compute the envelope of the processed acceleration data
         envelope, _ = preprocessing.calculate_envelope_activity(
             detected_activity_signal,
-            int(round(self.target_sampling_freq_Hz)),
+            int(round(target_sampling_freq_Hz)),
             1,
-            int(round(self.target_sampling_freq_Hz)),
-            0,
+            int(round(target_sampling_freq_Hz)),
         )
 
         # Initialize a list for walking bouts
         walking_bouts = [0]
 
         # Process alarm data to identify walking bouts
         if envelope.size > 0:
             index_ranges = preprocessing.find_consecutive_groups(envelope > 0)
             for j in range(len(index_ranges)):
                 if (
                     index_ranges[j, 1] - index_ranges[j, 0]
-                    <= 3 * self.target_sampling_freq_Hz
+                    <= 3 * target_sampling_freq_Hz
                 ):
                     envelope[index_ranges[j, 0] : index_ranges[j, 1] + 1] = 0
                 else:
                     walking_bouts.extend(
                         detected_activity_signal[
                             index_ranges[j, 0] : index_ranges[j, 1] + 1
                         ]
@@ -277,45 +259,51 @@
             preprocessing.convert_pulse_train_to_array(pulse_trains_max),
             preprocessing.convert_pulse_train_to_array(pulse_trains_min),
         )
 
         # Check if walking_periods is empty
         if walking_periods is None:
             walking_bouts = []
-            MidSwing = []
+
         else:
             # Call the organize_and_pack_results function with walking_periods and MaxPeaks
-            walking_bouts, MidSwing = preprocessing.organize_and_pack_results(
+            walking_bouts, _ = preprocessing.organize_and_pack_results(
                 walking_periods, max_peaks
             )
             if walking_bouts:
                 # Update the start value of the first element
                 walking_bouts[0]["start"] = max([1, walking_bouts[0]["start"]])
 
                 # Update the end value of the last element
                 walking_bouts[-1]["end"] = min(
                     [walking_bouts[-1]["end"], len(detected_activity_signal)]
                 )
 
         # Calculate the length of walking bouts
         walking_bouts_length = len(walking_bouts)
 
-        # Initialize an empty list
+        # Initialize an empty list for filtered walking bouts
         filtered_walking_bouts = []
 
-        # Initialize a counter variable "counter"
+        # Initialize a counter variable to count walking bouts
         counter = 0
 
+        # Iterate through walking bouts to filter those with steps less than 5
         for j in range(walking_bouts_length):
             if walking_bouts[j]["steps"] >= 5:
                 counter += 1
                 filtered_walking_bouts.append(
                     {"start": walking_bouts[j]["start"], "end": walking_bouts[j]["end"]}
                 )
 
+        # If no walking bouts are detected, print a message
+        if counter == 0:
+            print("No gait sequences detected due to insufficient steps in the data.")
+            return self
+
         # Initialize an array of zeros with the length of detected_activity_signal
         walking_labels = np.zeros(len(detected_activity_signal))
 
         # Calculate the length of the filtered_walking_bouts
         filtered_walking_bouts_length = len(filtered_walking_bouts)
 
         for j in range(filtered_walking_bouts_length):
@@ -327,85 +315,90 @@
         # Call the find_consecutive_groups function with the walking_labels variable
         ind_noWk = []
         ind_noWk = preprocessing.find_consecutive_groups(walking_labels == 0)
 
         # Merge walking bouts if break less than 3 seconds
         if ind_noWk.size > 0:
             for j in range(len(ind_noWk)):
-                if ind_noWk[j, 1] - ind_noWk[j, 0] <= self.target_sampling_freq_Hz * 3:
+                if ind_noWk[j, 1] - ind_noWk[j, 0] <= target_sampling_freq_Hz * 3:
                     walking_labels[ind_noWk[j, 0] : ind_noWk[j, 1] + 1] = 1
 
         # Merge walking bouts if break less than 3 seconds
         ind_Wk = []
         walkLabel_1_indices = np.where(walking_labels == 1)[0]
+        GSD_Output = []
 
         if walkLabel_1_indices.size > 0:
             ind_Wk = preprocessing.find_consecutive_groups(walking_labels == 1)
             # Create an empty list to store 'walk' dictionaries
             walk = []
             if ind_Wk.size > 0:
                 for j in range(len(ind_Wk)):
                     walk.append({"start": (ind_Wk[j, 0]), "end": ind_Wk[j, 1]})
 
             n = len(walk)
-            GSD_Output = []
 
             for j in range(n):
                 GSD_Output.append(
                     {
-                        "Start": walk[j]["start"] / self.target_sampling_freq_Hz,
-                        "End": walk[j]["end"] / self.target_sampling_freq_Hz,
+                        "Start": walk[j]["start"] / target_sampling_freq_Hz,
+                        "End": walk[j]["end"] / target_sampling_freq_Hz,
                         "fs": sampling_freq_Hz,
                     }
                 )
             print(f"{n} gait sequence(s) detected.")
         else:
             print("No gait sequence(s) detected.")
 
         # Create a DataFrame from the gait sequence data
         gait_sequences_ = pd.DataFrame(GSD_Output)
         gait_sequences_["onset"] = gait_sequences_["Start"]
         gait_sequences_["duration"] = gait_sequences_["End"] - gait_sequences_["Start"]
-        gait_sequences_["event_type"] = self.event_type
-        gait_sequences_["tracking_systems"] = self.tracking_systems
-        gait_sequences_["tracked_points"] = self.tracked_points
+        gait_sequences_["event_type"] = "gait sequence"
+        gait_sequences_["tracking_system"] = tracking_system
+
+        # Check if the indices in ind_Wk are within the range of dt_data's index
+        if ind_Wk.size > 0 and dt_data is not None:
+            valid_indices = [index for index in ind_Wk[:, 0] if index < len(dt_data)]
+            invalid_indices = len(ind_Wk[:, 0]) - len(valid_indices)
+
+            if invalid_indices > 0:
+                print(f"Warning: {invalid_indices} invalid index/indices found.")
+
+            # Only use valid indices to access dt_data
+            valid_dt_data = dt_data.iloc[valid_indices]
+
+            # Create a DataFrame from the gait sequence data
+            gait_sequences_ = pd.DataFrame(GSD_Output)
+            gait_sequences_["onset"] = gait_sequences_["Start"]
+            gait_sequences_["duration"] = (
+                gait_sequences_["End"] - gait_sequences_["Start"]
+            )
+            gait_sequences_["event_type"] = "gait sequence"
+            gait_sequences_["tracking_system"] = tracking_system
+
+            # If original datetime is available, update the 'onset' column
+            gait_sequences_["onset"] = valid_dt_data.reset_index(drop=True)
 
-        # Select and reorder columns
+        # Create a DataFrame from the gait sequence data
         gait_sequences_ = gait_sequences_[
-            ["onset", "duration", "event_type", "tracking_systems", "tracked_points"]
+            ["onset", "duration", "event_type", "tracking_system"]
         ]
 
         # Return gait_sequences_ as an output
         self.gait_sequences_ = gait_sequences_
 
+        # If Plot_results set to true
+        # currently no plotting for datetime values
+        if dt_data is not None and plot_results:
+            print("No plotting for datetime values.")
+            plot_results = False
+            return self
+
         # Plot results if set to true
         if plot_results:
-            plt.figure(figsize=(22, 14))
-            plt.plot(
-                np.arange(len(detected_activity_signal))
-                / (60 * self.target_sampling_freq_Hz),
-                detected_activity_signal,
-                label="Pre-processed acceleration signal",
-            )
-            plt.title("Detected gait sequences", fontsize=20)
-            plt.xlabel("Time (minutes)", fontsize=20)
-            plt.ylabel("Acceleration (g)", fontsize=20)
-
-            # Fill the area between start and end times
-            for index, sequence in gait_sequences_.iterrows():
-                onset = sequence["onset"] / 60  # Convert to minutes
-                end_time = (
-                    sequence["onset"] + sequence["duration"]
-                ) / 60  # Convert to minutes
-                plt.axvline(onset, color="g")
-                plt.axvspan(onset, end_time, facecolor="grey", alpha=0.8)
-            plt.legend(
-                ["Pre-processed acceleration signal", "Gait onset", "Gait duration"],
-                fontsize=20,
-                loc="best",
+
+            preprocessing.gsd_plot_results(
+                target_sampling_freq_Hz, detected_activity_signal, gait_sequences_
             )
-            plt.grid(visible=None, which="both", axis="both")
-            plt.xticks(fontsize=20)
-            plt.yticks(fontsize=20)
-            plt.show()
 
         return self
```

### Comparing `ngmt-0.0.3/ngmt/modules/icd/_paraschiv.py` & `ngmt-0.0.4/ngmt/modules/icd/_paraschiv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,144 +1,129 @@
 # Import libraries
+from typing import Optional
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import scipy.io
 import scipy.signal
 from ngmt.utils import preprocessing
 from ngmt.config import cfg_colors
 
 
 class ParaschivIonescuInitialContactDetection:
     """
-    Performs Initial Contact Detection on lower back IMU accelerometer data for detecting initial contacts.
+    This Paraschiv-Ionescu initial contact detection algorithm identifies initial contact in accelerometer data
+    collected from a low back IMU sensor. The purpose of algorithm is to identify and characterize initial contacts
+    within walking bouts.
+
+    The algorithm takes accelerometer data as input, and the vertical acceleration component, and processes each
+    specified gait sequence independently. The signal is first detrended and then low-pass filtered. The resulting
+    signal is numerically integrated and differentiated using a Gaussian continuous wavelet transformation. The
+    initial contact (IC) events are identified as the positive maximal peaks between successive zero-crossings.
 
-    Attributes:
-        target_sampling_freq_Hz (float): Target sampling frequency for resampling the data. Default is 40.
-        event_type (str): Type of the detected event. Default is 'initial contact'.
-        tracking_systems (str): Tracking systems used. Default is 'SU'.
-        tracked_points (str): Tracked points on the body. Default is 'LowerBack'.
-        initial_contacts_ (pd.DataFrame): DataFrame containing initial contacts information in BIDS format.
-
-    Description:
-        This class implements the Initial Contact Detection Algorithm on accelerometer data
-        collected from a low back sensor. The purpose of ICD is to identify and characterize initial contacts
-        within walking bouts.
-
-        The algorithm takes accelerometer data as input, specifically the vertical acceleration component,
-        and processes each specified gait sequence independently. The sampling frequency of the accelerometer
-        data is also required. Initial contacts information are provided as a DataFrame with columns 'onset',
-        'event_type', 'tracking_systems', and 'tracked_points'.
-
-        The algorithm is applied to a pre-processed vertical acceleration signal recorded on the lower back.
-        This signal is first detrended and then low-pass filtered. The resulting signal is numerically integrated
-        and differentiated using a Gaussian continuous wavelet transformation. The initial contact (IC) events
-        are identified as the positive maximal peaks between successive zero-crossings.
+    Finally, initial contacts information is provided as a DataFrame with columns `onset`, `event_type`, and
+    `tracking_systems`.
 
     Methods:
         detect(data, gait_sequences, sampling_freq_Hz):
             Detects initial contacts on the accelerometer signal.
 
-            Args:
-                data (pd.DataFrame): Input accelerometer data (N, 3) for x, y, and z axes.
-                gait_sequences (pd.DataFrame): Gait sequences detected using ParaschivIonescuGaitSequenceDetectionDataframe algorithm.
-                sampling_freq_Hz (float): Sampling frequency of the accelerometer data.
-
-            Returns:
-                self (pd.DataFrame): DataFrame containing initial contact information in BIDS format.
-
     Examples:
         Find initial contacts based on the detected gait sequence
 
         >>> icd = ParaschivIonescuInitialContactDetection()
         >>> icd = icd.detect(data=acceleration_data, sampling_freq_Hz=100)
-        >>> initial_contacts = icd.initial_contacts_
-        >>> print(initial_contacts_)
-                onset   event_type       tracking_systems   tracked_points
-            0   5       initial contact  SU                 LowerBack
-            1   5.6     initial contact  SU                 LowerBack
+        >>> print(icd.initial_contacts_)
+                onset   event_type       duration   tracking_systems
+            0   5       initial contact  0          SU
+            1   5.6     initial contact  0          SU
 
     References:
-        [1] Paraschiv-Ionescu et al. (2019). Locomotion and cadence detection using a single trunk-fixed accelerometer:
-            validity for children with cerebral palsy in daily life-like conditions.
-            Journal of NeuroEngineering and Rehabilitation, 16(1), 24.
-            https://doi.org/10.1186/s12984-019-0494-z
-        [2] Paraschiv-Ionescu et al. (2020). Real-world speed estimation using single trunk IMU:
-            methodological challenges for impaired gait patterns.
-            Annual International Conference of the IEEE Engineering in Medicine and Biology Society.
-            IEEE Engineering in Medicine and Biology Society. https://doi.org/10.1109/EMBC44109.2020.9176281
+        [1] Paraschiv-Ionescu et al. (2019). Locomotion and cadence detection using a single trunk-fixed accelerometer...
+
+        [2] Paraschiv-Ionescu et al. (2020). Real-world speed estimation using single trunk IMU: methodological challenges...
     """
 
     def __init__(
         self,
-        target_sampling_freq_Hz: float = 40.0,
-        event_type: str = "initial contact",
-        tracking_systems: str = "SU",
-        tracked_points: str = "LowerBack",
     ):
         """
         Initializes the ParaschivIonescuInitialContactDetection instance.
-
-        Args:
-            target_sampling_freq_Hz (float, optional): Target sampling frequency for resampling the data. Default is 40.
-            event_type (str, optional): Type of the detected event. Default is 'gait sequence'.
-            tracking_systems (str, optional): Tracking systems used. Default is 'SU'.
-            tracked_points (str, optional): Tracked points on the body. Default is 'LowerBack'.
         """
-        self.target_sampling_freq_Hz = target_sampling_freq_Hz
-        self.event_type = event_type
-        self.tracking_systems = tracking_systems
-        self.tracked_points = tracked_points
         self.initial_contacts_ = None
 
     def detect(
         self,
         data: pd.DataFrame,
-        gait_sequences: pd.DataFrame,
-        sampling_freq_Hz: float = 100,
+        sampling_freq_Hz: float,
+        v_acc_col_name: str,
+        gait_sequences: Optional[pd.DataFrame] = None,
+        dt_data: Optional[pd.Series] = None,
+        tracking_system: Optional[str] = None,
     ) -> pd.DataFrame:
         """
         Detects initial contacts based on the input accelerometer data.
 
         Args:
             data (pd.DataFrame): Input accelerometer data (N, 3) for x, y, and z axes.
-            gait_sequences (pd.DataFrame): Gait sequence calculated using ParaschivIonescuGaitSequenceDetectionDataframe algorithm.
             sampling_freq_Hz (float): Sampling frequency of the accelerometer data.
-
-            Returns:
-                ParaschivIonescuInitialContactDetection: Returns an instance of the class.
-                    The initial contacts information is stored in the 'initial_contacts_' attribute,
-                    which is a pandas DataFrame in BIDS format with the following columns:
-                        - onset: Initial contacts.
-                        - event_type: Type of the event (default is 'gait sequence').
-                        - tracking_systems: Tracking systems used (default is 'SU').
-                        - tracked_points: Tracked points on the body (default is 'LowerBack').
+            v_acc_col_name (str): The column name that corresponds to the vertical acceleration.
+            gait_sequences (pd.DataFrame, optional): A dataframe of detected gait sequences. If not provided, the entire acceleration time series will be used for detecting initial contacts.
+            dt_data (pd.Series, optional): Original datetime in the input data. If original datetime is provided, the output onset will be based on that.
+            tracking_system (str, optional): Tracking system the data is from to be used for events df. Default is None.
+
+        Returns:
+            ParaschivIonescuInitialContactDetection: Returns an instance of the class.
+                The initial contacts information is stored in the 'initial_contacts_' attribute,
+                which is a pandas DataFrame in BIDS format with the following columns:
+                    - onset: Initial contacts.
+                    - event_type: Type of the event (default is 'Inital contact').
+                    - tracking_system: Tracking systems used the events are derived from.
         """
         # Check if data is empty
         if data.empty:
             self.initial_contacts_ = pd.DataFrame()
-            return  # Return without performing further processing
+            return self  # Return without performing further processing
 
-        # Extract vertical accelerometer data
-        acc_vertical = data["LowerBack_ACCEL_x"]
+        # check if dt_data is a pandas Series with datetime values
+        if dt_data is not None and (
+            not isinstance(dt_data, pd.Series)
+            or not pd.api.types.is_datetime64_any_dtype(dt_data)
+        ):
+            raise ValueError("dt_data must be a pandas Series with datetime values")
+
+        # check if tracking_system is a string
+        if tracking_system is not None and not isinstance(tracking_system, str):
+            raise ValueError("tracking_system must be a string")
+
+        # check if dt_data is provided and if it is a series with the same length as data
+        if dt_data is not None and len(dt_data) != len(data):
+            raise ValueError("dt_data must be a series with the same length as data")
+
+        # Extract vertical accelerometer data using the specified index
+        acc_vertical = data[v_acc_col_name]
 
         # Initialize an empty list to store the processed output
         processed_output = []
 
         # Initialize an empty list to store all onsets
         all_onsets = []
 
         # Process each gait sequence
+        if gait_sequences is None:
+            gait_sequences = pd.DataFrame(
+                {"onset": [0], "duration": [len(data) / sampling_freq_Hz]}
+            )
         for _, gait_seq in gait_sequences.iterrows():
             # Calculate start and stop indices for the current gait sequence
-            start_index = int(sampling_freq_Hz * gait_seq["onset"] - 1)
+            start_index = int(sampling_freq_Hz * gait_seq["onset"])
             stop_index = int(
-                sampling_freq_Hz * (gait_seq["onset"] + gait_seq["duration"]) - 1
+                sampling_freq_Hz * (gait_seq["onset"] + gait_seq["duration"])
             )
-            accv_gait_seq = acc_vertical[start_index : stop_index + 2].to_numpy()
+            accv_gait_seq = acc_vertical[start_index:stop_index].to_numpy()
 
             try:
                 # Perform Signal Decomposition Algorithm for Initial Contacts (ICs)
                 initial_contacts_rel, _ = preprocessing.signal_decomposition_algorithm(
                     accv_gait_seq, sampling_freq_Hz
                 )
                 initial_contacts = gait_seq["onset"] + initial_contacts_rel
@@ -167,14 +152,32 @@
         # Create a DataFrame from the processed_output list
         initial_contacts_ = pd.DataFrame(processed_output)
 
         # Create a BIDS-compatible DataFrame with all onsets
         self.initial_contacts_ = pd.DataFrame(
             {
                 "onset": all_onsets,
-                "event_type": self.event_type,
-                "tracking_systems": self.tracking_systems,
-                "tracked_points": self.tracked_points,
+                "event_type": "initial contact",
+                "duration": 0,
+                "tracking_systems": tracking_system,
             }
         )
 
+        # If original datetime is available, update the 'onset' column
+        if dt_data is not None:
+            valid_indices = [
+                index
+                for index in self.initial_contacts_["onset"]
+                if index < len(dt_data)
+            ]
+            invalid_indices = len(self.initial_contacts_["onset"]) - len(valid_indices)
+
+            if invalid_indices > 0:
+                print(f"Warning: {invalid_indices} invalid index/indices found.")
+
+            # Only use valid indices to access dt_data
+            valid_dt_data = dt_data.iloc[valid_indices]
+
+            # Update the 'onset' column
+            self.initial_contacts_["onset"] = valid_dt_data.reset_index(drop=True)
+
         return self
```

### Comparing `ngmt-0.0.3/ngmt/modules/pam/_pam.py` & `ngmt-0.0.4/ngmt/modules/pam/_pam.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,135 +3,142 @@
 import matplotlib.pyplot as plt
 from ngmt.config import cfg_colors
 from ngmt.utils import preprocessing
 
 
 class PhysicalActivityMonitoring:
     """
-    Monitors physical activity levels based on accelerometer data.
+    The algortihm monitors physical activity levels based on accelerometer data. It determines the
+    intensity level of physical activities based on accelerometer signals using the following steps:
 
-    Description:
-        The algorithm determines the intensity level of physical activities based on accelerometer
-        signals using the following steps:
-
-        - Load Data: Includes a time index and accelerometer data (N, 3) for x, y, and z axes. The
-          sampling frequency (sampling_freq_Hz) is in Hz, with a default value of 100. Thresholds
-          (thresholds_mg) are provided as a dictionary containing threshold values for physical
-          activity detection in mg unit. The epoch duration (epoch_duration_sec) is defined in
-          seconds, with a default of 5 seconds. The last input is plot_results, which, if set to
-          True, generates a plot showing the average Euclidean Norm Minus One (ENMO) per hour for
-          each date. The default is True.
-
-        - Preprocess Signal: Calculate the sample-level Euclidean norm (EN) of the acceleration
-          signal. Apply a fourth-order Butterworth low-pass filter with a cut-off frequency of 20Hz
-          to remove noise. Calculate the Euclidean Norm Minus One (ENMO) index and truncate negative
-          values to zero. Convert the indices by multiplying them by 1000 to convert units from g to
-          mg.
-
-        - Classify Intensity: Classify the intensity of physical activities based on the calculated
-          ENMO values using 5-second epochs. Thresholds for categorization are as follows: sedentary
-          activity < 45 mg, light activity 45–100 mg, moderate activity 100–400 mg, vigorous activity
-          > 400 mg.
-
-        - Classify Activities: Classify different levels of activities and calculate the time spent
-          on each activity level for each day. If `plot_results` is True, the function generates a
-          plot showing the averaged ENMO values for each day.
+    - Load Data: Includes a time index and accelerometer data (N, 3) for x, y, and z axes. The
+        sampling frequency (sampling_freq_Hz) is in Hz, with a default value of 100. Thresholds
+        (thresholds_mg) are provided as a dictionary containing threshold values for physical
+        activity detection in mg unit. The epoch duration (epoch_duration_sec) is defined in
+        seconds, with a default of 5 seconds. The last input is plot, which, if set to
+        True, generates a plot showing the average Euclidean Norm Minus One (ENMO) per hour for
+        each date. The default is True.
+
+    - Preprocess Signal: Calculate the sample-level Euclidean norm (EN) of the acceleration
+        signal. Apply a fourth-order Butterworth low-pass filter with a cut-off frequency of 20Hz
+        to remove noise. Calculate the Euclidean Norm Minus One (ENMO) index and truncate negative
+        values to zero. Convert the indices by multiplying them by 1000 to convert units from g to
+        mg.
+
+    - Classify Intensity: Classify the intensity of physical activities based on the calculated
+        ENMO values using 5-second epochs. Thresholds for categorization are as follows: sedentary
+        activity < 45 mg, light activity 45–100 mg, moderate activity 100–400 mg, vigorous activity
+        > 400 mg.
+
+    - Classify Activities: Classify different levels of activities and calculate the time spent
+        on each activity level for each day. If `plot` is True, the function generates a
+        plot showing the averaged ENMO values for each day.
 
     Attributes:
         physical_activities_ (pd.DataFrame): DataFrame containing physical activity information for each day.
 
     Methods:
-        detect(data, sampling_freq_Hz, thresholds_mg, epoch_duration_sec, plot_results):
+        detect(data, sampling_freq_Hz, thresholds_mg, epoch_duration_sec, plot):
             Detects gait sequences on the accelerometer signal.
 
-        __init__():
-            Initializes the physical activity instance.
+    Examples:
+        >>> pam = PhysicalActivityMonitoring()
+        >>> pam.detect(
+                data=acceleration_data,
+                acceleration_unit:"m/s^2",
+                sampling_freq_Hz=100,
+                thresholds_mg={
+                    "sedentary_threshold": 45,
+                    "light_threshold": 100,
+                    "moderate_threshold": 400,
+                },
+                epoch_duration_sec=5,
+                plot=True)
+        >>> print(pam.physical_activities_)
+                        sedentary_mean_mg  sedentary_time_min  light_mean_mg  light_time_min  moderate_mean_mg  moderate_time_min  vigorous_mean_mg  vigorous_time_min
+        3/19/2018       23.48              733.08              60.78          72              146.2             21.58              730.34            0.58
+        3/20/2018       27.16              753.83              57.06          102.25          137.26            7.92               737.9             0.42
 
-        Examples:
-            Determines physical activity levels in the sensor signal.
+    References:
+        [1] Doherty, Aiden, et al. (2017). Large scale population assessment of physical activity using wrist-worn accelerometers...
 
-            >>> pam = PhysicalActivityMonitoring()
-            >>> pam.detect(
-                    data=acceleration_data,
-                    sampling_freq_Hz=100,
-                    thresholds_mg={
-                        "sedentary_threshold": 45,
-                        "light_threshold": 100,
-                        "moderate_threshold": 400,
-                    },
-                    epoch_duration_sec=5,
-                    plot_results=True)
-            >>> physical_activities = pam.physical_activities_
-            >>> print(physical_activities)
-                           sedentary_mean_mg  sedentary_time_min  light_mean_mg  light_time_min  moderate_mean_mg  moderate_time_min  vigorous_mean_mg  vigorous_time_min
-            3/19/2018               23.48               733.08          60.78              72             146.2              21.58             730.34                0.58
-            3/20/2018               27.16               753.83          57.06           102.25            137.26               7.92             737.9                 0.42
-
-        References:
-            [1] Doherty, Aiden, et al. (2017). Large scale population assessment of physical
-                activity using wrist-worn accelerometers: the UK biobank study. PloS one 12.2.
-                https://doi.org/10.1371/journal.pone.0169649
-
-            [2] Van Hees, Vincent T., et al. (2013). Separating movement and gravity components
-                in an acceleration signal and implications for the assessment of human daily physical
-                activity. PloS one 8.4. https://doi.org/10.1371/journal.pone.0061691
+        [2] Van Hees, Vincent T., et al. (2013). Separating movement and gravity components in an acceleration signal and implications...
     """
 
     def __init__(self):
         """
         Initializes the physical activity instance.
         """
         self.physical_activities_ = None
 
     def detect(
         self,
         data: pd.DataFrame,
+        acceleration_unit: str,
         sampling_freq_Hz: float,
-        thresholds_mg: dict = {
+        thresholds_mg: dict[str, float] = {
             "sedentary_threshold": 45,
             "light_threshold": 100,
             "moderate_threshold": 400,
         },
-        epoch_duration_sec: int = 5,
-        plot_results: bool = True,
+        epoch_duration_sec: float = 5,
+        plot: bool = True,
     ) -> pd.DataFrame:
         """
         Detects and classifies physical activity levels.
 
         Args:
             data (pd.DataFrame): Input data with time index and accelerometer data (N, 3) for x, y, and z axes.
+            acceleration_unit (str): Unit of input acceleration data.
             sampling_freq_Hz (float): Sampling frequency of the accelerometer data (in Hertz).
             thresholds_mg (dict): Dictionary containing threshold values for physical activity detection.
             epoch_duration_sec (int): Duration of each epoch in seconds.
-            plot_results (bool): If True, generates a plot showing the average Euclidean Norm Minus One (ENMO). Default is True.
+            plot (bool): If True, generates a plot showing the average Euclidean Norm Minus One (ENMO). Default is True.
 
         Returns:
             pd.DataFrame: Contains date, sedentary_mean_mg, sedentary_time_min, light_mean_mg, light_time_min,
                           moderate_mean_mg, moderate_time_min, vigorous_mean_mg, vigorous_time_min
         """
         # Error handling for invalid input data
+
+        # Check if data is a DataFrame
+        if not isinstance(data, pd.DataFrame):
+            raise ValueError("Input data must be a DataFrame.")
+
+        # check if index column is datetime
+        if not isinstance(data.index, pd.DatetimeIndex):
+            raise ValueError("Index column must be a datetime index.")
+
+        # check if index column in named timestamp
+        if data.index.name != "timestamp":
+            raise ValueError("Index column must be named timestamp.")
+
+        # Check if data has at least 3 columns
+        if data.shape[1] < 3:
+            raise ValueError("Input data must have at least 3 columns.")
+
         if not isinstance(sampling_freq_Hz, (int, float)) or sampling_freq_Hz <= 0:
             raise ValueError("Sampling frequency must be a positive float.")
 
         if not isinstance(thresholds_mg, dict):
             raise ValueError("Thresholds must be a dictionary.")
 
         if not isinstance(epoch_duration_sec, int) or epoch_duration_sec <= 0:
             raise ValueError("Epoch duration must be a positive integer.")
 
-        if not isinstance(plot_results, bool):
+        if not isinstance(plot, bool):
             raise ValueError("Plot results must be a boolean (True or False).")
 
-        # Select accelerometer data columns and convert units from m/s^2 to g
-        data[["LARM_ACCEL_x", "LARM_ACCEL_y", "LARM_ACCEL_z"]] /= 9.81
+        # Check unit of acceleration data if it is in g or m/s^2
+        if acceleration_unit == "m/s^2":
+            # Convert acceleration data from m/s^2 to g (if not already is in g)
+            data /= 9.81
 
         # Calculate Euclidean Norm (EN)
-        data["en"] = np.linalg.norm(
-            data[["LARM_ACCEL_x", "LARM_ACCEL_y", "LARM_ACCEL_z"]], axis=1
-        )
+        data["en"] = np.linalg.norm(data, axis=1)
 
         # Apply 4th order low-pass Butterworth filter with the cutoff frequency of 20Hz
         data["en"] = preprocessing.lowpass_filter(
             data["en"].values,
             method="butter",
             order=4,
             cutoff_freq_hz=20,
@@ -151,23 +158,23 @@
         processed_data = pd.DataFrame(
             data=data["enmo"], index=data.index, columns=["enmo"]
         )
 
         # Classify activities based on thresholds using activity_classification
         classified_processed_data = preprocessing.classify_physical_activity(
             processed_data,
-            sedentary_threshold=thresholds_mg.get("sedentary_threshold", 45),
-            light_threshold=thresholds_mg.get("light_threshold", 100),
-            moderate_threshold=thresholds_mg.get("moderate_threshold", 400),
+            sedentary_threshold=thresholds_mg.get("sedentary_threshold"),
+            light_threshold=thresholds_mg.get("light_threshold"),
+            moderate_threshold=thresholds_mg.get("moderate_threshold"),
             epoch_duration=epoch_duration_sec,
         )
 
         # Extract date from the datetime index
         classified_processed_data["date"] = classified_processed_data[
-            "timestamp"
+            data.index.name
         ].dt.date
 
         # Calculate time spent in each activity level for each epoch
         classified_processed_data["sedentary_time_min"] = (
             classified_processed_data["sedentary"] * epoch_duration_sec
         ) / 60
         classified_processed_data["light_time_min"] = (
@@ -182,88 +189,70 @@
 
         # Group by date and calculate mean and total time spent in each activity level
         physical_activities_ = (
             classified_processed_data.groupby("date")
             .agg(
                 sedentary_mean_enmo=(
                     "enmo",
-                    lambda x: np.mean(x[classified_processed_data["sedentary"] == 1]),
+                    lambda x: np.mean(
+                        np.where(
+                            classified_processed_data.loc[x.index, "sedentary"] == 1,
+                            x,
+                            np.nan,
+                        )
+                    ),
                 ),
                 sedentary_time_min=("sedentary_time_min", "sum"),
                 light_mean_enmo=(
                     "enmo",
-                    lambda x: np.mean(x[classified_processed_data["light"] == 1]),
+                    lambda x: np.mean(
+                        np.where(
+                            classified_processed_data.loc[x.index, "light"] == 1,
+                            x,
+                            np.nan,
+                        )
+                    ),
                 ),
                 light_time_min=("light_time_min", "sum"),
                 moderate_mean_enmo=(
                     "enmo",
-                    lambda x: np.mean(x[classified_processed_data["moderate"] == 1]),
+                    lambda x: np.mean(
+                        np.where(
+                            classified_processed_data.loc[x.index, "moderate"] == 1,
+                            x,
+                            np.nan,
+                        )
+                    ),
                 ),
                 moderate_time_min=("moderate_time_min", "sum"),
                 vigorous_mean_enmo=(
                     "enmo",
-                    lambda x: np.mean(x[classified_processed_data["vigorous"] == 1]),
+                    lambda x: np.mean(
+                        np.where(
+                            classified_processed_data.loc[x.index, "vigorous"] == 1,
+                            x,
+                            np.nan,
+                        )
+                    ),
                 ),
                 vigorous_time_min=("vigorous_time_min", "sum"),
             )
             .reset_index()
         )
 
-        # Return gait_sequences_ as an output
+        # Return physical activities as an output
         self.physical_activities_ = physical_activities_
 
-        # Plot results if set to true
-        if plot_results:
-            # Group by date and hour to calculate the average ENMO for each hour
-            hourly_average_data = processed_data.groupby(
-                [processed_data.index.date, processed_data.index.hour]
-            )["enmo"].mean()
-
-            # Reshape the data to have dates as rows, hours as columns, and average ENMO as values
-            hourly_average_data = hourly_average_data.unstack()
-
-            # Plotting
-            fig, ax = plt.subplots(figsize=(14, 8))
-
-            # Choose the 'turbo' colormap for coloring each day
-            colormap = plt.cm.turbo
-
-            # Plot thresholds
-            ax.axhline(
-                y=thresholds_mg.get("sedentary_threshold", 45),
-                color="y",
-                linestyle="--",
-                label="Sedentary threshold",
-            )
-            ax.axhline(
-                y=thresholds_mg.get("light_threshold", 100),
-                color="g",
-                linestyle="--",
-                label="Light physical activity threshold",
-            )
-            ax.axhline(
-                y=thresholds_mg.get("moderate_threshold", 400),
-                color="r",
-                linestyle="--",
-                label="Moderate physical activity threshold",
-            )
+        # Group by date and hour to calculate the average ENMO for each hour
+        hourly_average_data = processed_data.groupby(
+            [processed_data.index.date, processed_data.index.hour]
+        )["enmo"].mean()
 
-            # Plot each day data with a different color
-            for i, date in enumerate(hourly_average_data.index):
-                color = colormap(i)
-                ax.plot(hourly_average_data.loc[date], label=str(date), color=color)
-
-            # Customize plot appearance
-            plt.xticks(range(24), [str(i).zfill(2) for i in range(24)])
-            plt.xlabel("Time (h)", fontsize=16)
-            plt.ylabel("ENMO (mg)", fontsize=16)
-            plt.title(
-                "Hourly averaged ENMO for each day along with activity level thresholds"
-            )
-            plt.legend(loc="upper left", fontsize=16)
-            plt.grid(visible=None, which="both", axis="both")
-            plt.xticks(fontsize=16)
-            plt.yticks(fontsize=16)
-            plt.tight_layout()
-            plt.show()
+        # Reshape the data to have dates as rows, hours as columns, and average ENMO as values
+        hourly_average_data = hourly_average_data.unstack()
+
+        # Plot if set to true
+        if plot:
+
+            preprocessing.pam_plot_results(hourly_average_data, thresholds_mg)
 
         return self
```

### Comparing `ngmt-0.0.3/ngmt/test/example_lower_back_acc.csv` & `ngmt-0.0.4/ngmt/test/example_lower_back_acc.csv`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/test/test_calc.py` & `ngmt-0.0.4/ngmt/test/test_calc.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,27 +16,20 @@
 1. Make sure you have pytest installed. If not, install it using 'pip install -U pytest'.
 2. Run this script, and pytest will execute all the test functions.
 3. Any failures in tests will be reported as failed with red color, and also the number of passed tests will be represented with green color.
 
 By running these tests, the reliability and correctness of the signal processing functions in the 'ngmt.utils.preprocessing' module will be ensured.
 """
 
-
 # Import necessary libraries and functions to be tested.
 import pandas as pd
 import numpy as np
 import warnings
 import numpy.testing as npt
 import pytest
-import scipy
-import matplotlib.pyplot as plt
-from ngmt.modules.gsd import ParaschivIonescuGaitSequenceDetection
-from ngmt.modules.icd import ParaschivIonescuInitialContactDetection
-from ngmt.modules.pam import PhysicalActivityMonitoring
-from matplotlib.testing.compare import compare_images
 from ngmt.utils.preprocessing import (
     resample_interpolate,
     lowpass_filter,
     highpass_filter,
     _iir_highpass_filter,
     apply_continuous_wavelet_transform,
     apply_successive_gaussian_filters,
@@ -46,46 +39,43 @@
     identify_pulse_trains,
     convert_pulse_train_to_array,
     find_interval_intersection,
     organize_and_pack_results,
     max_peaks_between_zc,
     signal_decomposition_algorithm,
     classify_physical_activity,
+    tilt_angle_estimation,
+    wavelet_decomposition,
+    moving_var,
+    gsd_plot_results,
+    pam_plot_results,
+    pham_plot_results,
+    process_postural_transitions_stationary_periods,
+)
+from ngmt.utils.quaternion import (
+    quatinv,
+    quatnormalize,
+    quatnorm,
+    quatconj,
+    quatmultiply,
+    rotm2quat,
+    quat2rotm,
+    quat2axang,
+    axang2rotm,
 )
-from ngmt.modules.gsd import ParaschivIonescuGaitSequenceDetection
-from ngmt.modules.icd import ParaschivIonescuInitialContactDetection
+
 
 # Generate a random sinusoidal signal with varying amplitudes to use as an input in testing functions
 time = np.linspace(0, 100, 1000)  # Time vector from 0 to 100 with 1000 samples
 amplitudes = np.random.uniform(-3, 3, 1000)  # Random amplitudes between 3 and -3
 sampling_frequency = 100  # Sampling frequency
 random_input_signal = np.sin(2 * np.pi * sampling_frequency * time) * amplitudes
 
 
 # Each test function checks a specific function.
-# Test function for the 'resample_interpolate' function: Case 1
-def test_resample_interpolate():
-    """
-    Test for resample_interpolate function in the 'ngmt.utils.preprocessing' module.
-    """
-    # Test with inputs
-    input_signal = random_input_signal
-    initial_sampling_frequency = sampling_frequency
-    target_sampling_frequency = 40
-
-    # Call the resample_interpolate function with the specified inputs
-    with warnings.catch_warnings():
-        # Ignore the specific warning (invalid value encountered in divide)
-        warnings.simplefilter("ignore", category=RuntimeWarning)
-
-        resampled_signal = resample_interpolate(
-            input_signal, initial_sampling_frequency, target_sampling_frequency
-        )
-
-
 # Test function for the 'resample_interpolate' function: Case 2
 def test_resample_interpolate_non_numpy_input():
     # Test with non-NumPy array input
     input_signal = [1, 2, 3, 4, 5]
     initial_sampling_frequency = 1
     target_sampling_frequency = 0.5
 
@@ -556,28 +546,14 @@
         wavelet,
         sampling_frequency,
     )
     assert (
         wavelet_transform_result_negative is None
     ), "Function should handle negative scales or desired_scale and return None."
 
-    # Test case for non-integer scales or desired_scale
-    non_integer_scales = 5.5
-    non_integer_desired_scale = 2.3
-    wavelet_transform_result_non_integer = apply_continuous_wavelet_transform(
-        test_signal,
-        non_integer_scales,
-        non_integer_desired_scale,
-        wavelet,
-        sampling_frequency,
-    )
-    assert (
-        wavelet_transform_result_non_integer is None
-    ), "Function should handle non-integer scales or desired_scale and return None."
-
 
 # Test function for the 'apply_continuous_wavelet_transform' function: case 2
 def test_apply_continuous_wavelet_transform_valid_input():
     # Test with valid input
     input_signal = np.array([1, 2, 3, 4, 5])
     scales = 10
     desired_scale = 5
@@ -802,80 +778,20 @@
     Test for calculate_envelope_activity function in the 'ngmt.utils.preprocessing' module.
     """
     # Test with inputs
     test_signal = random_input_signal
     smooth_window = 20
     threshold_style = 1
     duration = 20
-    plot_results = 0
 
     # Call the calculate_envelope_activity function with the specified inputs
     alarm, env = calculate_envelope_activity(
-        test_signal, smooth_window, threshold_style, duration, plot_results=0
+        test_signal, smooth_window, threshold_style, duration
     )
 
-    # Assertions to be checked:
-    # Check that the input signal is a NumPy array
-    assert isinstance(test_signal, np.ndarray), "Input signal should be a NumPy array."
-
-    # Check that the window length is a positive integer
-    assert (
-        isinstance(smooth_window, int) and smooth_window > 0
-    ), "The window length must be a positive integer."
-
-    # Check that the threshold style is a positive integer
-    assert (
-        isinstance(threshold_style, int) and threshold_style > 0
-    ), "The threshold style must be a positive integer."
-
-    # Check that the duration of activity is a positive integer
-    assert (
-        isinstance(duration, int) and duration > 0
-    ), "The duration of activity must be a positive integer."
-
-    # Check that the plotting results is 0 or 1
-    assert plot_results in [0, 1], "The plotting results must be 0 or 1."
-
-    # Check that the outputs of the function are NumPy arrays
-    assert isinstance(
-        alarm, np.ndarray
-    ), "Vector indicating active parts of the signal (alarm) should be a NumPy array."
-    assert isinstance(
-        env, np.ndarray
-    ), "Smoothed envelope of the signal (env) should be a NumPy array."
-
-    # Check that the outputs do not contain any NaN or Inf values
-    assert not np.isnan(
-        alarm
-    ).any(), "Vector indicating active parts of the signal (alarm) contains NaN values."
-    assert not np.isinf(
-        alarm
-    ).any(), "Vector indicating active parts of the signal (alarm) contains Inf values."
-    assert not np.isnan(
-        env
-    ).any(), "Smoothed envelope of the signal (env) contains NaN values."
-    assert not np.isinf(
-        env
-    ).any(), "Smoothed envelope of the signal (env) contains Inf values."
-
-    # Additional assertions for specific scenarios
-    assert len(alarm) > len(
-        test_signal
-    ), "Length of alarm vector should be greater than the length of the input signal."
-
-    # Check that the length of the smoothed envelope vector is greater than or equal to the length of the input signal
-    assert len(env) >= len(
-        test_signal
-    ), "Length of smoothed envelope vector should be greater than or equal to the length of the input signal."
-
-    # Use pytest.approx for floating-point comparisons
-    assert alarm[0] == pytest.approx(
-        0.0
-    ), "First element of alarm vector should be approximately 0.0."
-
 
 # Test function for the 'calculate_envelope_activity' function: case 2
 def test_calculate_envelope_activity_invalid_input():
     # Test with invalid input data type
     input_signal = [1, 2, 3, 4, 5]
 
     with pytest.raises(ValueError, match="Input signal should be a NumPy array."):
@@ -909,23 +825,14 @@
     # Test with invalid duration value
     input_signal = np.array([1, 2, 3, 4, 5])
 
     with pytest.raises(ValueError, match="The duration must be a positive integer."):
         calculate_envelope_activity(input_signal, duration=0)
 
 
-# Test function for the 'calculate_envelope_activity' function: case 6
-def test_calculate_envelope_activity_invalid_plot_results():
-    # Test with invalid plot_results value
-    input_signal = np.array([1, 2, 3, 4, 5])
-
-    with pytest.raises(ValueError, match="The plotting results must be 0 or 1."):
-        calculate_envelope_activity(input_signal, plot_results=2)
-
-
 # Test function for the 'find_consecutive_groups' function: case 1
 def test_find_consecutive_groups():
     """
     Test for find_consecutive_groups function in the 'ngmt.utils.preprocessing' module.
     """
     # Test with inputs
     test_signal = np.array([0, 1, 1, 0, 2, 2, 2, 0, 0, 3, 3])
@@ -1431,34 +1338,14 @@
     expected_result_empty = np.array([])
 
     # Assertions to be checked:
     # Check if set_a_empty and set_b_empty are NumPy arrays
     assert isinstance(set_a_empty, np.ndarray), "set_a_empty should be a NumPy array."
     assert isinstance(set_b_empty, np.ndarray), "set_b_empty should be a NumPy array."
 
-    try:
-        # Call the find_interval_intersection function with the specified inputs
-        result_empty = find_interval_intersection(set_a_empty, set_b_empty)
-
-        # Check the data type of the output
-        assert isinstance(result_empty, np.ndarray), "Output should be a NumPy array."
-
-        # Check if the output matches the expected result
-        npt.assert_array_equal(
-            result_empty,
-            expected_result_empty,
-            "Output does not match the expected result.",
-        )
-
-    except IndexError:
-        # Handle the case where an IndexError occurs (empty array)
-        assert (
-            len(set_a_empty) == 0 and len(set_b_empty) == 0
-        ), "Empty arrays should result in empty output."
-
     # Additional Test Case 2: Identical sets
     set_a_identical = np.array([[1, 5], [7, 10]])
     set_b_identical = np.array([[1, 5], [7, 10]])
     expected_result_identical = np.array([[1, 5], [7, 10]])
 
     # Assertions to be checked:
     # Check if set_a_identical and set_b_identical are NumPy arrays
@@ -1533,100 +1420,14 @@
 
     # Expecting the interval [3, 5] from set B to be appended
     expected_result = np.array([[3, 5]])
     assert np.array_equal(result, expected_result)
 
 
 # Test function for the 'organize_and_pack_results' function
-def test_organize_and_pack_results():
-    # Test case 1: Basic case with non-overlapping walking periods
-    walking_periods = [(0, 10), (20, 30), (40, 50)]
-    peak_steps = [5, 25, 45]
-    expected_results = [
-        {
-            "start": 0,
-            "end": 10,
-            "steps": 1,
-            "mid_swing": [5],
-        },
-        {
-            "start": 20,
-            "end": 30,
-            "steps": 1,
-            "mid_swing": [25],
-        },
-        {
-            "start": 40,
-            "end": 50,
-            "steps": 1,
-            "mid_swing": [45],
-        },
-    ]
-    expected_peak_steps = [5, 25, 45]
-
-    # Assertions to be checked:
-    # Check if walking_periods is a list
-    assert isinstance(walking_periods, list), "walking_periods should be a list."
-
-    # Check that each element in walking_periods is a tuple with two elements
-    for period in walking_periods:
-        assert isinstance(
-            period, tuple
-        ), "Each element in walking_periods should be a tuple."
-        assert (
-            len(period) == 2
-        ), "Each tuple in walking_periods should contain start and end indices."
-
-    # Check if peak_steps is a list
-    assert isinstance(peak_steps, list), "peak_steps should be a list."
-
-    # Call the organize_and_pack_results function with the specified inputs
-    results, peak_steps_result = organize_and_pack_results(walking_periods, peak_steps)
-
-    # Check if results is a list of dictionaries
-    assert isinstance(results, list), "Output results should be a list."
-
-    for result in results:
-        assert isinstance(
-            result, dict
-        ), "Each element in results should be a dictionary."
-        assert "start" in result, "Dictionary should contain 'start' key."
-        assert "end" in result, "Dictionary should contain 'end' key."
-        assert "steps" in result, "Dictionary should contain 'steps' key."
-        assert "mid_swing" in result, "Dictionary should contain 'mid_swing' key."
-
-    # Check the values in the output results
-    assert (
-        results == expected_results
-    ), "Output results do not match the expected results."
-
-    # Check that the 'steps' value for each result is a positive integer
-    for result in results:
-        assert (
-            result["steps"] > 0
-        ), "'steps' value in results should be a positive integer."
-
-    # Check that the 'mid_swing' values are within the 'start' and 'end' range for each result
-    for result in results:
-        assert all(
-            result["start"] <= step <= result["end"] for step in result["mid_swing"]
-        ), "Mid-swing values are out of range for some results."
-
-    # Check if peak_steps_result is a list
-    assert isinstance(
-        peak_steps_result, list
-    ), "Output peak_steps_result should be a list."
-
-    # Check the values in the output peak_steps_result
-    assert (
-        peak_steps_result == expected_peak_steps
-    ), "Output peak_steps_result do not match the expected peak_steps."
-
-
-# Test function for the 'organize_and_pack_results' function
 def test_step_time_calculation_no_peak_steps():
     # Mock input data
     walking_periods = [(0, 10)]
     peak_steps = []
 
     # Call the function
     organized_results, _ = organize_and_pack_results(walking_periods, peak_steps)
@@ -1763,459 +1564,530 @@
     )
 
     # Call the classify_physical_activity function with negative epoch_duration
     with pytest.raises(ValueError, match="Epoch_duration must be a positive integer."):
         classify_physical_activity(invalid_data, epoch_duration=-5)
 
 
-@pytest.fixture
-def sample_accelerometer_data():
-    # Create sample accelerometer data
-    np.random.seed(0)
-    timestamps = pd.date_range(start="2024-01-01", periods=1000, freq="1s")
-    accelerometer_data = pd.DataFrame(
-        {
-            "LowerBack_ACCEL_x": np.random.randn(1000),
-            "LowerBack_ACCEL_y": np.random.randn(1000),
-            "LowerBack_ACCEL_z": np.random.randn(1000),
-        },
-        index=timestamps,
-    )
-    return accelerometer_data
+# Test function for wavelet_decomposition function
+def test_wavelet_decomposition():
+    """
+    Test for wavelet_decomposition function in the 'ngmt.utils.preprocessing' module.
+    """
+    # Generate a random input signal
+    input_signal = np.random.randn(1000)
 
+    # Test with valid inputs
+    denoised_signal = wavelet_decomposition(input_signal, level=3, wavetype="haar")
 
-@pytest.fixture
-def sample_gait_sequences():
-    # Create sample gait sequences DataFrame
-    gait_sequences = pd.DataFrame(
-        {"onset": [1.5, 3.5, 5.5], "duration": [0.5, 0.7, 0.6]}
-    )
-    return gait_sequences
+    # Assertions
+    assert isinstance(
+        denoised_signal, np.ndarray
+    ), "Denoised signal should be a NumPy array."
+    assert len(denoised_signal) == len(
+        input_signal
+    ), "Denoised signal length should match input signal length."
+    assert not np.isnan(denoised_signal).any(), "Denoised signal contains NaN values."
+    assert not np.isinf(
+        denoised_signal
+    ).any(), "Denoised signal contains infinite values."
 
 
-def test_detect_method(sample_accelerometer_data, sample_gait_sequences):
-    # Initialize ParaschivIonescuInitialContactDetection instance
-    icd_instance = ParaschivIonescuInitialContactDetection()
+# Test function for moving_var function
+def test_moving_var():
+    """
+    Test for moving_var function in the 'ngmt.utils.preprocessing' module.
+    """
+    # Generate a random input signal
+    input_signal = np.random.randn(1000)
 
-    # Call detect method
-    icd_instance.detect(
-        data=sample_accelerometer_data,
-        gait_sequences=sample_gait_sequences,
-        sampling_freq_Hz=100,
-    )
+    # Test with valid inputs
+    moving_variance = moving_var(input_signal, window=10)
+
+    # Assertions
+    assert isinstance(
+        moving_variance, np.ndarray
+    ), "Moving variance should be a NumPy array."
+    assert len(moving_variance) == len(
+        input_signal
+    ), "Moving variance length should match input signal length."
+    assert not np.isnan(moving_variance).any(), "Moving variance contains NaN values."
+    assert not np.isinf(
+        moving_variance
+    ).any(), "Moving variance contains infinite values."
 
-    # Check if initial_contacts_ attribute is a DataFrame
-    assert isinstance(icd_instance.initial_contacts_, pd.DataFrame)
 
-    # Check the columns in the initial_contacts_ DataFrame
-    expected_columns = ["onset", "event_type", "tracking_systems", "tracked_points"]
-    assert all(
-        col in icd_instance.initial_contacts_.columns for col in expected_columns
+# Test function for test_tilt_angle_estimation function
+def test_tilt_angle_estimation():
+    """
+    Test for tilt_angle_estimation function.
+    """
+    # Generate some sample gyro data
+    gyro_data = np.array(
+        [[0.1, 0.2, 0.3], [0.2, 0.3, 0.4], [0.3, 0.4, 0.5], [0.4, 0.5, 0.6]]
     )
 
-    # Check the data type of the 'onset' column
-    assert pd.api.types.is_float_dtype(icd_instance.initial_contacts_["onset"])
+    sampling_frequency_hz = 10  # Sampling frequency of 10 Hz
 
-    # Check if onset values are within the expected range
-    assert all(0 <= onset <= 6 for onset in icd_instance.initial_contacts_["onset"])
+    # Calculate expected tilt angle
+    expected_tilt_angle = np.array([-0.02, -0.05, -0.1, -0.18])  # Manually calculated
 
+    # Test tilt_angle_estimation function
+    tilt_angle = tilt_angle_estimation(gyro_data, sampling_frequency_hz)
 
-## Module test
-# Test data
-num_samples = 50000  # Number of samples
-acceleration_data = {
-    "LowerBack_ACCEL_x": np.random.uniform(-2, 2, num_samples),
-    "LowerBack_ACCEL_y": np.random.uniform(-2, 2, num_samples),
-    "LowerBack_ACCEL_z": np.random.uniform(-2, 2, num_samples),
-}
-acceleration_data = pd.DataFrame(acceleration_data)
-sampling_frequency = 100  # Sampling frequency
+    # Assertions
+    assert isinstance(tilt_angle, np.ndarray), "Tilt angle should be a NumPy array."
+    assert len(tilt_angle) == len(
+        gyro_data
+    ), "Tilt angle length should match input data length."
+
+    # Test with DataFrame input
+    gyro_df = pd.DataFrame(gyro_data)
+    tilt_angle_df = tilt_angle_estimation(gyro_df, sampling_frequency_hz)
+
+    # Assertions for DataFrame input
+    assert isinstance(
+        tilt_angle_df, np.ndarray
+    ), "Tilt angle from DataFrame should be a NumPy array."
+    assert len(tilt_angle_df) == len(
+        gyro_data
+    ), "Tilt angle length from DataFrame should match input data length."
 
+    # Test for invalid input type
+    with pytest.raises(
+        TypeError, match="Input data must be a numpy array or pandas DataFrame"
+    ):
+        tilt_angle_estimation(
+            list(gyro_data), sampling_frequency_hz
+        )  # Passing a list instead of numpy array
 
-def test_gsd_detect():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
-
-    # Call the detect method
-    gsd.detect(data=acceleration_data, sampling_freq_Hz=sampling_frequency)
-    gait_sequences_ = gsd.gait_sequences_
 
-    # Assertions
-    assert isinstance(
-        gait_sequences_, pd.DataFrame
-    ), "Gait sequences should be a DataFrame."
-    assert (
-        "onset" in gait_sequences_.columns
-    ), "Gait sequences should have 'onset' column."
-    assert (
-        "duration" in gait_sequences_.columns
-    ), "Gait sequences should have 'duration' column."
-    assert (
-        "event_type" in gait_sequences_.columns
-    ), "Gait sequences should have 'event_type' column."
-    assert (
-        "tracking_systems" in gait_sequences_.columns
-    ), "Gait sequences should have 'tracking_systems' column."
-    assert (
-        "tracked_points" in gait_sequences_.columns
-    ), "Gait sequences should have 'tracked_points' column."
+# Test gsd_plot_results without plotting
+# Sample data for testing
+target_sampling_freq_Hz = 100
+detected_activity_signal = np.random.rand(1000)
+gait_sequences_ = pd.DataFrame(
+    {"onset": np.array([100, 300, 500]), "duration": np.array([50, 60, 70])}
+)
+hourly_average_data = pd.DataFrame(
+    np.random.rand(24, 7),
+    columns=pd.date_range(start="2024-01-01", periods=7),
+    index=np.arange(24),
+)
+thresholds_mg = {
+    "sedentary_threshold": 45,
+    "light_threshold": 100,
+    "moderate_threshold": 400,
+}
 
 
-def test_invalid_input_data():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
+# Test function for gsd_plot_results without plotting
+def test_gsd_plot_results_without_plot(monkeypatch):
+    # Define a mock function for plt.show() that does nothing
+    def mock_show():
+        pass
 
-    # Test with invalid input data
-    invalid_data = pd.DataFrame({"x": [1, 2, 3], "y": [4, 5, 6]})
-    with pytest.raises(ValueError):
-        gsd.detect(data=invalid_data, sampling_freq_Hz=sampling_frequency)
+    # Monkeypatch plt.show() with the mock function
+    monkeypatch.setattr("matplotlib.pyplot.show", mock_show)
 
+    # Call the function
+    gsd_plot_results(target_sampling_freq_Hz, detected_activity_signal, gait_sequences_)
 
-def test_invalid_sampling_freq():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
 
-    # Test with invalid sampling frequency
-    invalid_sampling_freq = "invalid"
-    with pytest.raises(ValueError):
-        gsd.detect(data=acceleration_data, sampling_freq_Hz=invalid_sampling_freq)
+# Test function for pam_plot_results without plotting
+def test_pam_plot_results_without_plot(monkeypatch):
+    # Define a mock function for plt.show() that does nothing
+    def mock_show():
+        pass
 
+    # Monkeypatch plt.show() with the mock function
+    monkeypatch.setattr("matplotlib.pyplot.show", mock_show)
 
-def test_gait_sequence_detection():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
+    # Call the function
+    pam_plot_results(hourly_average_data, thresholds_mg)
 
-    # Call the detect method
-    gsd.detect(data=acceleration_data, sampling_freq_Hz=sampling_frequency)
 
-    # Check if gait_sequences_ attribute is a DataFrame
-    assert isinstance(
-        gsd.gait_sequences_, pd.DataFrame
-    ), "Gait sequences should be a DataFrame."
+# Test function for test_pham_plot_results
+def test_pham_plot_results(monkeypatch):
+    # Generate sample data
+    np.random.seed(0)
+    accel = np.random.randn(100, 3)
+    gyro = np.random.randn(100, 3)
 
-    # Check if gait_sequences_ DataFrame has the expected columns
-    expected_columns = [
-        "onset",
-        "duration",
-        "event_type",
-        "tracking_systems",
-        "tracked_points",
-    ]
-    assert all(
-        col in gsd.gait_sequences_.columns for col in expected_columns
-    ), "Gait sequences DataFrame should have the expected columns."
-
-    # Check if all onset values are within the correct range
-    assert all(
-        onset >= 0 and onset <= acceleration_data.shape[0] / sampling_frequency
-        for onset in gsd.gait_sequences_["onset"]
-    ), "Onset values should be within the valid range."
-
-    # Check if all duration values are non-negative
-    assert all(
-        duration >= 0 for duration in gsd.gait_sequences_["duration"]
-    ), "Duration values should be non-negative."
-
-
-def test_invalid_input_data_type():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
+    # Ensure 'onset' and 'duration' arrays have the same length
+    onset = np.arange(10, 90, 20)
+    duration = [5] * len(onset)
 
-    # Test with invalid input data type
-    invalid_data = np.array([[1, 2, 3], [4, 5, 6]])
-    with pytest.raises(ValueError):
-        gsd.detect(data=invalid_data, sampling_freq_Hz=sampling_frequency)
+    postural_transitions_ = pd.DataFrame({"onset": onset, "duration": duration})
 
+    sampling_freq_Hz = 100
 
-def test_invalid_sampling_freq_type():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
+    # Define a mock function for plt.show() that does nothing
+    def mock_show():
+        pass
 
-    # Test with invalid sampling frequency type
-    invalid_sampling_freq = "invalid"
-    with pytest.raises(ValueError):
-        gsd.detect(data=acceleration_data, sampling_freq_Hz=invalid_sampling_freq)
+    # Monkeypatch plt.show() with the mock function
+    monkeypatch.setattr("matplotlib.pyplot.show", mock_show)
 
+    # Call the function
+    pham_plot_results(accel, gyro, postural_transitions_, sampling_freq_Hz)
 
-def test_plot_results_type():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
 
-    # Test with invalid plot_results type
-    invalid_plot_results = "invalid"
-    with pytest.raises(ValueError):
-        gsd.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=sampling_frequency,
-            plot_results=invalid_plot_results,
-        )
+# Test function for test_organize_and_pack_results
+@pytest.mark.parametrize(
+    "walking_periods, peak_steps, expected_results",
+    [
+        # Test case 1
+        (
+            [(0, 20)],  # Walking periods
+            [2, 6, 10, 12, 15, 20],  # Peak steps
+            [
+                {
+                    "start": -2,
+                    "end": 22,
+                    "steps": 6,
+                    "mid_swing": [2, 6, 10, 12, 15, 20],
+                }
+            ],  # Expected results
+        ),
+        # Test case 2
+        (
+            [(0, 15), (16, 30)],  # Walking periods
+            [0, 2, 6, 10, 12, 15, 20, 25, 26, 28, 30],  # Peak steps
+            [
+                {
+                    "start": -1,
+                    "end": 31,
+                    "steps": 11,
+                    "mid_swing": [0, 2, 6, 10, 12, 15, 20, 25, 26, 28, 30],
+                }
+            ],  # Expected results
+        ),
+    ],
+)
+# Test function for test_organize_and_pack_results
+def test_organize_and_pack_results(walking_periods, peak_steps, expected_results):
+    # Call the function and get the actual results
+    actual_results, actual_peak_steps = organize_and_pack_results(
+        walking_periods, peak_steps
+    )
 
+    # Sort the peak steps in the actual results
+    actual_peak_steps.sort()
+
+    # Flatten the nested lists
+    actual_results_flat = [
+        item for sublist in actual_results for item in sublist.items()
+    ]
 
-# Tests for ParaschivIonescuInitialContactDetection
-def test_detect_empty_data():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
-    icd = ParaschivIonescuInitialContactDetection()
-
-    # Call detect with an empty DataFrame instead of None
-    icd.detect(data=pd.DataFrame(), gait_sequences=pd.DataFrame(), sampling_freq_Hz=100)
-
-
-# Define test_detect_no_gait_sequences function
-def test_detect_no_gait_sequences():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
-    icd = ParaschivIonescuInitialContactDetection()
-
-    # Create a DataFrame with only one column for each axis
-    acceleration_data_single_axis = {
-        "LowerBack_ACCEL_x": np.random.uniform(-2, 2, num_samples),
-        "LowerBack_ACCEL_y": np.random.uniform(-2, 2, num_samples),
-        "LowerBack_ACCEL_z": np.random.uniform(-2, 2, num_samples),
-    }
-    acceleration_data_single_axis = pd.DataFrame(acceleration_data_single_axis)
-
-    # Call detect without gait sequences
-    icd.detect(
-        data=acceleration_data_single_axis,
-        gait_sequences=pd.DataFrame(),
-        sampling_freq_Hz=100,
-    )
 
+# Define some test data
+quaternions = np.array(
+    [
+        [0.5, 0.5, 0.5, 0.5],  # Quaternion 1
+        [1.0, 0.0, 0.0, 0.0],  # Quaternion 2
+        [0.707, 0.0, 0.707, 0.0],  # Quaternion 3
+    ]
+)
+rotation_matrices = np.array(
+    [
+        [[1, 0, 0], [0, 1, 0], [0, 0, 1]],  # Rotation Matrix 1
+        [[1, 0, 0], [0, -1, 0], [0, 0, -1]],  # Rotation Matrix 2
+        [[1, 0, 0], [0, 0, -1], [0, 1, 0]],  # Rotation Matrix 3
+    ]
+)
+axis_angle_rep = np.array(
+    [
+        [1, 0, 0, np.pi / 2],  # Axis-Angle Representation 1
+        [1, 0, 0, 0],  # Axis-Angle Representation 2
+        [0, 1, 0, np.pi / 2],  # Axis-Angle Representation 3
+    ]
+)
 
-def test_detect_no_plot():
-    # Initialize the class
-    gsd = ParaschivIonescuGaitSequenceDetection()
-    icd = ParaschivIonescuInitialContactDetection()
-
-    # Create a DataFrame with only one column for each axis
-    acceleration_data_single_axis = {
-        "LowerBack_ACCEL_x": np.random.uniform(-2, 2, num_samples),
-        "LowerBack_ACCEL_y": np.random.uniform(-2, 2, num_samples),
-        "LowerBack_ACCEL_z": np.random.uniform(-2, 2, num_samples),
-    }
-    acceleration_data_single_axis = pd.DataFrame(acceleration_data_single_axis)
-
-    # Call detect without gait sequences
-    icd.detect(
-        data=acceleration_data_single_axis,
-        gait_sequences=pd.DataFrame(),
-        sampling_freq_Hz=100,
-    )
 
-    # Check if initial_contacts_ is None
-    assert (
-        icd.initial_contacts_ is None
-    ), "Initial contacts should be None if no gait sequences are provided"
+# Test function for quatinv function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[0], np.array([0.5, -0.5, -0.5, -0.5])),  # Test case 1
+        (quaternions[1], np.array([1.0, 0.0, 0.0, 0.0])),  # Test case 2
+        (quaternions[2], np.array([0.707, 0.0, -0.707, 0.0])),  # Test case 3
+    ],
+)
+def test_quatinv(q, expected):
+    result = quatinv(q)
 
 
-# Test data
-num_samples = 50000  # Number of samples
-acceleration_data = {
-    "LARM_ACCEL_x": np.random.uniform(-2, 2, num_samples),
-    "LARM_ACCEL_y": np.random.uniform(-2, 2, num_samples),
-    "LARM_ACCEL_z": np.random.uniform(-2, 2, num_samples),
-}
-acceleration_data = pd.DataFrame(acceleration_data)
-sampling_frequency = 100  # Sampling frequency
-time_index = pd.date_range(
-    start="2024-02-07", periods=num_samples, freq=f"{1/sampling_frequency}S"
+# Test function for quatnormalize function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[0], np.array([0.5, 0.5, 0.5, 0.5])),  # Test case 1
+        (quaternions[1], np.array([1.0, 0.0, 0.0, 0.0])),  # Test case 2
+        (quaternions[2], np.array([0.707, 0.0, 0.707, 0.0])),  # Test case 3
+    ],
 )
-acceleration_data["timestamp"] = time_index
-acceleration_data.set_index("timestamp", inplace=True)
+def test_quatnormalize(q, expected):
+    result = quatnormalize(q)
 
 
-# Tests for PhysicalActivityMonitoring
-def test_pam_detect():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
-
-    # Call the detect method
-    pam.detect(
-        data=acceleration_data,
-        sampling_freq_Hz=sampling_frequency,
-        thresholds_mg={
-            "sedentary_threshold": 45,
-            "light_threshold": 100,
-            "moderate_threshold": 400,
-        },
-        epoch_duration_sec=5,
-        plot_results=False,  # Set to False to avoid plotting for this test
-    )
-    physical_activities_ = pam.physical_activities_
+# Test function for quatnorm function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[0], np.array([1.0] * 3)),  # Test case 1
+        (quaternions[1], np.array([1.0] * 3)),  # Test case 2
+        (quaternions[2], np.array([1.0] * 3)),  # Test case 3
+    ],
+)
+def test_quatnorm(q, expected):
+    result = quatnorm(q)
 
-    # Assertions
-    assert isinstance(
-        physical_activities_, pd.DataFrame
-    ), "Physical activity information should be stored in a DataFrame."
 
+# Test function for quatconj function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[0], np.array([0.5, -0.5, -0.5, -0.5])),  # Test case 1
+        (quaternions[1], np.array([1.0, 0.0, 0.0, 0.0])),  # Test case 2
+        (quaternions[2], np.array([0.707, 0.0, -0.707, 0.0])),  # Test case 3
+    ],
+)
+def test_quatconj(q, expected):
+    result = quatconj(q)
 
-def test_invalid_sampling_freq_pam():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
 
-    # Test with invalid sampling frequency
-    invalid_sampling_freq = "invalid"
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=invalid_sampling_freq,
-            thresholds_mg={
-                "sedentary_threshold": 45,
-                "light_threshold": 100,
-                "moderate_threshold": 400,
-            },
-            epoch_duration_sec=5,
-        )
+# Test function for quatmultiply function
+@pytest.mark.parametrize(
+    "q1, q2, expected",
+    [
+        (quaternions[0], quaternions[1], np.array([0.0, 1.0, 0.0, 0.0])),  # Test case 1
+        (
+            quaternions[1],
+            quaternions[2],
+            np.array([0.707, 0.0, 0.0, -0.707]),
+        ),  # Test case 2
+        (
+            quaternions[2],
+            quaternions[0],
+            np.array([0.0, 0.0, -0.707, 0.707]),
+        ),  # Test case 3
+    ],
+)
+def test_quatmultiply(q1, q2, expected):
+    result = quatmultiply(q1, q2)
 
 
-def test_invalid_thresholds_type():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
+# Test function for rotm2quat function
+@pytest.mark.parametrize(
+    "R, expected",
+    [
+        (rotation_matrices[0], quaternions[1]),  # Test case 1
+        (rotation_matrices[1], quaternions[2]),  # Test case 2
+        (rotation_matrices[2], np.array([0.924, 0.383, 0.0, 0.0])),  # Test case 3
+    ],
+)
+def test_rotm2quat(R, expected):
+    result = rotm2quat(R)
 
-    # Test with invalid thresholds type
-    invalid_thresholds = "invalid"
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=sampling_frequency,
-            thresholds_mg=invalid_thresholds,
-            epoch_duration_sec=5,
-        )
 
+# Test function for quat2rotm function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[1], rotation_matrices[0]),  # Test case 1
+        (quaternions[2], rotation_matrices[1]),  # Test case 2
+        (np.array([0.924, 0.383, 0.0, 0.0]), rotation_matrices[2]),  # Test case 3
+    ],
+)
+def test_quat2rotm(q, expected):
+    result = quat2rotm(q)
 
-def test_invalid_epoch_duration():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
 
-    # Test with invalid epoch duration
-    invalid_epoch_duration = -1
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=sampling_frequency,
-            thresholds_mg={
-                "sedentary_threshold": 45,
-                "light_threshold": 100,
-                "moderate_threshold": 400,
-            },
-            epoch_duration_sec=invalid_epoch_duration,
-        )
+# Test function for quat2axang function
+@pytest.mark.parametrize(
+    "q, expected",
+    [
+        (quaternions[1], axis_angle_rep[1]),  # Test case 1
+        (quaternions[0], axis_angle_rep[0]),  # Test case 2
+        (quaternions[2], axis_angle_rep[2]),  # Test case 3
+    ],
+)
+def test_quat2axang(q, expected):
+    result = quat2axang(q)
 
 
-def test_invalid_plot_results_type_pam():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
+# Test function for axang2rotm function
+@pytest.mark.parametrize(
+    "axang, expected",
+    [
+        (axis_angle_rep[0], rotation_matrices[0]),  # Test case 1
+        (axis_angle_rep[1], rotation_matrices[1]),  # Test case 2
+        (axis_angle_rep[2], rotation_matrices[2]),  # Test case 3
+    ],
+)
+def test_axang2rotm(axang, expected):
+    result = axang2rotm(axang)
 
-    # Test with invalid plot_results type
-    invalid_plot_results = "invalid"
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=sampling_frequency,
-            thresholds_mg={
-                "sedentary_threshold": 45,
-                "light_threshold": 100,
-                "moderate_threshold": 400,
-            },
-            epoch_duration_sec=5,
-            plot_results=invalid_plot_results,
-        )
 
+# Test function for quatconj function with different configurations
+@pytest.mark.parametrize(
+    "q, scalar_first, channels_last, expected",
+    [
+        (
+            np.array([[1, 0, 0, 0]]),
+            True,
+            True,
+            np.array([[1, 0, 0, 0]]),
+        ),  # Identity quaternion
+        (
+            np.array([[0, 1, 0, 0]]),
+            True,
+            True,
+            np.array([[0, -1, 0, 0]]),
+        ),  # Pure imaginary quaternion
+        (
+            np.array([[0, 0, 1, 0]]),
+            True,
+            False,
+            np.array([[0, 0, -1, 0]]),
+        ),  # Pure imaginary quaternion, channels_last = False
+        (
+            np.array([[0, 0, 0, 1]]),
+            False,
+            True,
+            np.array([[0, 0, 0, -1]]),
+        ),  # Pure imaginary quaternion, scalar_last = True
+        (
+            np.array([[[0, 1, 0, 0], [0, 0, 1, 0]]]),
+            True,
+            True,
+            np.array([[[0, -1, 0, 0], [0, 0, -1, 0]]]),
+        ),  # Two quaternions
+    ],
+)
+def case_two_test_quatconj(q, scalar_first, channels_last, expected):
+    result = quatconj(q, scalar_first=scalar_first, channels_last=channels_last)
 
-def test_invalid_sampling_freq_type_error_handling():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
 
-    # Test with invalid sampling frequency type
-    invalid_sampling_freq = "invalid"
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=invalid_sampling_freq,
-            thresholds_mg={
-                "sedentary_threshold": 45,
-                "light_threshold": 100,
-                "moderate_threshold": 400,
-            },
-            epoch_duration_sec=5,
-            plot_results=True,
-        )
+# Test function for quatconj function
+def test_quatconj_transpose():
+    """Test quatconj with transposed quaternion."""
+    q = np.array([[[0, 1, 0, 0], [0, 0, 1, 0]]])
+    result = quatconj(q, scalar_first=True, channels_last=False)
+
+
+def test_quatconj_manipulation():
+    """Test quatconj with quaternion manipulation."""
+    q = np.array([[1, 2, 3, 4], [5, 6, 7, 8]])
+    q_tmp = q.copy()
+    q[..., 0] = q_tmp[..., -1]
+    q[..., 1:] = q_tmp[..., :-1]
+    del q_tmp
+    result = quatconj(q, scalar_first=False, channels_last=True)
+
+
+# Test function for quatmultiply function with different configurations
+@pytest.mark.parametrize(
+    "q1, q2",
+    [
+        (
+            np.array([[[1, 0, 0, 0]]]),
+            np.array([[[1, 0, 0, 0]]]),
+        ),  # Identity quaternion
+        (
+            np.array([[[0, 1, 0, 0]]]),
+            np.array([[[0, 0, 1, 0]]]),
+        ),  # Pure imaginary quaternions
+    ],
+)
+def test_quatmultiply(q1, q2):
+    result = quatmultiply(q1, q2)
 
 
-def test_invalid_thresholds_type_error_handling():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
+# Test function for quatmultiply function with channels_last=True
+@pytest.mark.parametrize(
+    "q1, q2",
+    [
+        (
+            np.array(
+                [[[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]]]
+            ),  # q1 with channels_last=True
+            np.array(
+                [[[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]]]
+            ),  # q2 with channels_last=True
+        ),
+        (
+            np.array(
+                [[[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]]]
+            ),  # q1 with channels_last=True
+            np.array(
+                [[[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0]]]
+            ),  # q2 with channels_last=True
+        ),
+    ],
+)
+def test_quatmultiply_channels_last(q1, q2):
 
-    # Test with invalid thresholds type
-    invalid_thresholds = "invalid"
-    with pytest.raises(ValueError):
-        pam.detect(
-            data=acceleration_data,
-            sampling_freq_Hz=sampling_frequency,
-            thresholds_mg=invalid_thresholds,
-            epoch_duration_sec=5,
-            plot_results=True,
-        )
+    # Determine channels_last based on the shape of q1
+    channels_last = q1.shape[-1]
 
+    result = quatmultiply(
+        q1, q2, channels_last=channels_last
+    )  # Pass channels_last accordingly
 
-def test_empty_input_data():
-    # Define empty_data with required columns
-    empty_data = pd.DataFrame(
-        {
-            "LARM_ACCEL_x": [],
-            "LARM_ACCEL_y": [],
-            "LARM_ACCEL_z": [],
-        }
-    )
 
-    # Initialize the PhysicalActivityMonitoring class
-    pam = PhysicalActivityMonitoring()
+# Test function for rotm2quat function with different methods
+def test_method_copysign():
+    """Test rotm2quat with method 'copysign'."""
+    R = np.array([[0, 1, 0], [-1, 0, 0], [0, 0, 1]])
+    expected = np.array([0.70710678, 0.70710678, 0, 0])
+    result = rotm2quat(R, method="copysign")
 
-    # Call the detect method with empty_data
-    with pytest.raises(ValueError):
-        pam.detect(data=empty_data, sampling_freq_Hz=sampling_frequency)
+
+def test_invalid_method():
+    """Test rotm2quat with an invalid method."""
+    R = np.eye(3)
+    with pytest.raises(
+        RuntimeError, match='invalid method, must be "copysign", "auto", 0, 1, 2 or 3'
+    ):
+        rotm2quat(R, method=4)
 
 
-def test_pam_detect_full_coverage():
-    # Initialize the class
-    pam = PhysicalActivityMonitoring()
-
-    # Call the detect method with plot_results=False to avoid plotting
-    pam.detect(
-        data=acceleration_data,
-        sampling_freq_Hz=sampling_frequency,
-        thresholds_mg={
-            "sedentary_threshold": 45,
-            "light_threshold": 100,
-            "moderate_threshold": 400,
-        },
-        epoch_duration_sec=5,
-        plot_results=False,
+# Test cases for quatmultiply function
+@pytest.mark.parametrize(
+    "q1_shape, q2_shape, scalar_first, channels_last",
+    [
+        ((3, 4), (3, 4), True, True),  # Basic case
+        ((3, 4), (3, 4), False, True),  # Test scalar_last=True
+        ((3, 4), None, True, True),  # Test self-multiplication
+        ((3, 1, 4), (3, 1, 4), True, True),  # Test broadcasting
+    ],
+)
+def test_quatmultiply(q1_shape, q2_shape, scalar_first, channels_last):
+    # Generate random quaternion arrays with given shapes
+    q1 = np.random.rand(*q1_shape)
+    q2 = None if q2_shape is None else np.random.rand(*q2_shape)
+
+    # Call the quatmultiply function
+    result = quatmultiply(
+        q1, q2, scalar_first=scalar_first, channels_last=channels_last
     )
-    physical_activities_ = pam.physical_activities_
 
-    # Assertions
-    assert isinstance(
-        physical_activities_, pd.DataFrame
-    ), "Physical activity information should be stored in a DataFrame."
 
-    # Check if the DataFrame has expected columns
-    expected_columns = [
-        "date",
-        "sedentary_mean_enmo",
-        "sedentary_time_min",
-        "light_mean_enmo",
-        "light_time_min",
-        "moderate_mean_enmo",
-        "moderate_time_min",
-        "vigorous_mean_enmo",
-        "vigorous_time_min",
-    ]
-    assert all(
-        col in physical_activities_.columns for col in expected_columns
-    ), "DataFrame should have the expected columns."
+# Test function for axang2rotm function
+@pytest.mark.parametrize(
+    "axang, expected",
+    [
+        (np.array([0.15, 0.25, 0.35, 0.0]), np.eye(3)),  # Test case with correct shape
+    ],
+)
+def test_axang2rotm(axang, expected):
+    # Reshape axang to have the required shape (..., 4)
+    axang = axang.reshape(-1, 4)
+    result = axang2rotm(axang)
+    assert np.allclose(result, expected)
 
 
 # Run the tests with pytest
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `ngmt-0.0.3/ngmt/utils/__pycache__/data_utils.cpython-311.pyc` & `ngmt-0.0.4/ngmt/utils/__pycache__/data_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/__pycache__/matlab_loader.cpython-311.pyc` & `ngmt-0.0.4/ngmt/utils/__pycache__/matlab_loader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/__pycache__/preprocessing.cpython-311.pyc` & `ngmt-0.0.4/ngmt/utils/__pycache__/preprocessing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/file_io.py` & `ngmt-0.0.4/ngmt/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/FIR_2_3Hz_40.mat` & `ngmt-0.0.4/ngmt/utils/FIR_2_3Hz_40.mat`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/matlab_loader.py` & `ngmt-0.0.4/ngmt/utils/matlab_loader.py`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/orientation_estimation/_madgwick.py` & `ngmt-0.0.4/ngmt/utils/orientation_estimation/_madgwick.py`

 * *Files identical despite different names*

### Comparing `ngmt-0.0.3/ngmt/utils/preprocessing.py` & `ngmt-0.0.4/ngmt/utils/preprocessing.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import matplotlib.pyplot as plt
 import scipy.interpolate
 import scipy.signal
 import scipy.io
 import scipy.integrate
 import scipy.ndimage
 import pywt
+from ngmt.utils import quaternion
+from ngmt.config import cfg_colors
+
 
 # use the importlib.resources package to access the FIR_2_3Hz_40.mat file
 with pkg_resources.path(
     "ngmt.utils", "FIR_2_3Hz_40.mat"
 ) as mat_filter_coefficients_file:
     pass
 
 
 def resample_interpolate(
-    input_signal, initial_sampling_frequency=100, target_sampling_frequency=40
+    input_signal, initial_sampling_frequency: float, target_sampling_frequency: float
 ):
     """
     Resample and interpolate a signal to a new sampling frequency.
 
     This function takes a signal `input_signal` sampled at an initial sampling frequency `initial_sampling_frequency`
     and resamples it to a target sampling frequency `target_sampling_frequency` using linear interpolation.
 
@@ -118,23 +121,27 @@
         filt_signal = scipy.signal.savgol_filter(
             signal, window_length, polynomial_order
         )
         return filt_signal
 
     elif method == "butter":
         # Extract parameters specific to butterworth filter
-        cutoff_freq_hz = kwargs.get("cutoff_freq_hz", 100.0)
-        sampling_rate_hz = kwargs.get("sampling_rate_hz", 1000.0)
+        cutoff_freq_hz = kwargs.get("cutoff_freq_hz", 5.0)
+        sampling_rate_hz = kwargs.get("sampling_rate_hz", 200.0)
 
         if order is None:
             raise ValueError("For Butterworth filter, 'order' must be specified.")
 
         # Apply butterworth lowpass filter
         b, a = scipy.signal.butter(
-            order, cutoff_freq_hz, btype="low", analog=False, fs=sampling_rate_hz
+            N=order,
+            Wn=cutoff_freq_hz / (sampling_rate_hz / 2),
+            btype="low",
+            analog=False,
+            fs=sampling_rate_hz,
         )
         filt_signal = scipy.signal.filtfilt(b, a, signal)
         return filt_signal
 
     elif method == "fir":
         # Update default parameters with any provided kwargs
         fir_params = {**default_fir_params, **kwargs}
@@ -234,17 +241,14 @@
             denominator_coefficient,
             signal,
             axis=0,
             padtype="odd",
             padlen=3
             * (max(len(numerator_coefficient), len(denominator_coefficient)) - 1),
         )
-    else:
-        # Define filter coefficients based on your specific requirements
-        pass
 
     # Return the filtered signal
 
     return filtered_signal
 
 
 def apply_continuous_wavelet_transform(
@@ -316,29 +320,28 @@
             filtered_signal, sigma=sigma, mode=mode, radius=round(gaussian_radius)
         )
 
     return filtered_signal
 
 
 def calculate_envelope_activity(
-    input_signal, smooth_window=20, threshold_style=1, duration=20, plot_results=0
+    input_signal, smooth_window=20, threshold_style=1, duration=20
 ):
     """
     Calculate envelope-based activity detection using the Hilbert transform.
 
     This function analyzes an input signal `input_signal` to detect periods of activity based on the signal's envelope.
     It calculates the analytical signal using the Hilbert transform, smoothes the envelope, and applies an
     adaptive threshold to identify active regions.
 
     Parameters:
         input_signal (array_like): The input signal.
         smooth_window (int): Window length for smoothing the envelope (default is 20).
         threshold_style (int): Threshold selection style: 0 for manual, 1 for automatic (default is 1).
         duration (int): Minimum duration of activity to be detected (default is 20).
-        plot_results (int): Set to 1 for plotting results, 0 otherwise (default is 0).
 
     Returns:
         tuple (ndarray, ndarray): A tuple containing:
         alarm (ndarray): Vector indicating active parts of the signal.
         env (ndarray): Smoothed envelope of the signal.
     """
     # Error handling for invalid input data
@@ -350,17 +353,14 @@
 
     if not isinstance(threshold_style, (int)) or threshold_style <= 0:
         raise ValueError("The threshold style must be a positive integer.")
 
     if not isinstance(duration, (int)) or duration <= 0:
         raise ValueError("The duration must be a positive integer.")
 
-    if not plot_results == 0 or plot_results == 1:
-        raise ValueError("The plotting results must be 0 or 1.")
-
     # Calculate the analytical signal and get the envelope
     input_signal = input_signal.flatten()
     # Compute the analytic signal, using the Hilbert transform form scipy.signal.
     analytic = scipy.signal.hilbert(input_signal)
     env = np.abs(analytic)  # Compute the envelope of the analytic signal.
 
     # Take the moving average of the analytic signal
@@ -368,21 +368,22 @@
         env, np.ones(smooth_window) / smooth_window, mode="full"
     )  # Returns the discrete, linear convolution of two one-dimensional sequences.
 
     env = env - np.mean(env)  # Remove the offset by subtracting the mean of 'env'
     env = env / np.max(env)  # Normalize the 'env' by dividing by its maximum value
 
     # Threshold the signal
-    if threshold_style == 0:
-        plt.plot(env)
-        plt.title("Select a threshold on the graph")
-        THR_SIG = plt.ginput(1)[0][1]
-        plt.close()
-    else:
-        THR_SIG = 4 * np.mean(env)
+    # if threshold_style == 0:
+    #     plt.plot(env)
+    #     plt.title("Select a threshold on the graph")
+    #     THR_SIG = plt.ginput(1)[0][1]
+    #     plt.close()
+    # else:
+    #     THR_SIG = 4 * np.mean(env)
+    THR_SIG = 4 * np.mean(env)
 
     # Set noise and signal levels
     noise = np.mean(env) / 3  # noise level
 
     # Signal level: It's used as a reference to distinguish between the background noise and the actual signal activity.
     threshold = np.mean(env)
 
@@ -425,46 +426,46 @@
             THR_SIG = noise + 0.50 * (
                 np.abs(threshold - noise)
             )  # Update the threshold using noise and threshold values.
         THR_buf[i] = (
             THR_SIG  # Store the updated threshold value in the threshold buffer.
         )
 
-    if plot_results == 1:
-        plt.figure()
-        ax = plt.subplot(2, 1, 1)
-        plt.plot(input_signal)
-        plt.plot(np.where(alarm != 0, np.max(input_signal), 0), "r", linewidth=2.5)
-        plt.plot(THR_buf, "--g", linewidth=2.5)
-        plt.title("Raw Signal and detected Onsets of activity")
-        plt.legend(
-            ["Raw Signal", "Detected Activity in Signal", "Adaptive Threshold"],
-            loc="upper left",
-        )
-        plt.grid(True)
-        plt.axis("tight")
-
-        ax2 = plt.subplot(2, 1, 2)
-        plt.plot(env)
-        plt.plot(THR_buf, "--g", linewidth=2.5)
-        plt.plot(thres_buf, "--r", linewidth=2)
-        plt.plot(noise_buf, "--k", linewidth=2)
-        plt.title("Smoothed Envelope of the signal (Hilbert Transform)")
-        plt.legend(
-            [
-                "Smoothed Envelope of the signal (Hilbert Transform)",
-                "Adaptive Threshold",
-                "Activity level",
-                "Noise Level",
-            ]
-        )
-        plt.grid(True)
-        plt.axis("tight")
-        plt.tight_layout()
-        plt.show()
+    # if plot_results == 1:
+    #     plt.figure()
+    #     ax = plt.subplot(2, 1, 1)
+    #     plt.plot(input_signal)
+    #     plt.plot(np.where(alarm != 0, np.max(input_signal), 0), "r", linewidth=2.5)
+    #     plt.plot(THR_buf, "--g", linewidth=2.5)
+    #     plt.title("Raw Signal and detected Onsets of activity")
+    #     plt.legend(
+    #         ["Raw Signal", "Detected Activity in Signal", "Adaptive Threshold"],
+    #         loc="upper left",
+    #     )
+    #     plt.grid(True)
+    #     plt.axis("tight")
+
+    #     ax2 = plt.subplot(2, 1, 2)
+    #     plt.plot(env)
+    #     plt.plot(THR_buf, "--g", linewidth=2.5)
+    #     plt.plot(thres_buf, "--r", linewidth=2)
+    #     plt.plot(noise_buf, "--k", linewidth=2)
+    #     plt.title("Smoothed Envelope of the signal (Hilbert Transform)")
+    #     plt.legend(
+    #         [
+    #             "Smoothed Envelope of the signal (Hilbert Transform)",
+    #             "Adaptive Threshold",
+    #             "Activity level",
+    #             "Noise Level",
+    #         ]
+    #     )
+    #     plt.grid(True)
+    #     plt.axis("tight")
+    #     plt.tight_layout()
+    #     plt.show()
 
     return alarm, env
 
 
 def find_consecutive_groups(input_signal):
     """
     Find consecutive groups of non-zero values in an input array.
@@ -558,17 +559,14 @@
             `start`: The index of the first value in the pulse train.
 
             `end`: The index of the last value in the pulse train.
 
             `steps`: The number of steps in the pulse train.
     """
     # Error handling for invalid input data
-    if not isinstance(signal, np.ndarray):
-        raise ValueError("Input signal must be a NumPy array.")
-
     if signal.size < 1:
         raise ValueError("Input signal must not be empty.")
 
     # Initialize an empty list to store detected pulse trains.
     pulse_trains = []
 
     # Initialize a flag to track whether we are within a pulse train.
@@ -1060,7 +1058,534 @@
     # Reset the index for the resulting DataFrame
     processed_data.reset_index(inplace=True)
 
     # Return a DataFrame with the time, averaged ENMO, and classes of sedentary, light, moderate and vigorous shown with 1 or 0.
     return processed_data[
         ["timestamp", "enmo", "sedentary", "light", "moderate", "vigorous"]
     ]
+
+
+# Function to plot results of the gait sequence detection algorithm
+def gsd_plot_results(
+    target_sampling_freq_Hz, detected_activity_signal, gait_sequences_
+):
+    """
+    Plot the detected gait sequences.
+
+    Args:
+        target_sampling_freq_Hz (float) : Target sampling frequency.
+        detected_activity_signal (np.array): Pre-processed acceleration signal.
+        gait_sequences_ (pd.DataFrame): Detected gait sequences.
+
+    Returns:
+        plot
+    """
+    plt.figure(figsize=(22, 14))
+    plt.plot(
+        np.arange(len(detected_activity_signal)) / (60 * target_sampling_freq_Hz),
+        detected_activity_signal,
+        label="Pre-processed acceleration signal",
+        color=cfg_colors["prep"][0],
+    )
+    plt.title("Detected gait sequences", fontsize=20)
+    plt.xlabel("Time (minutes)", fontsize=20)
+    plt.ylabel("Acceleration (g)", fontsize=20)
+
+    # Fill the area between start and end times
+    for index, sequence in gait_sequences_.iterrows():
+        onset = sequence["onset"] / 60  # Convert to minutes
+        end_time = (sequence["onset"] + sequence["duration"]) / 60  # Convert to minutes
+        plt.axvline(onset, color=cfg_colors["raw"][1])
+        plt.axvspan(onset, end_time, facecolor="grey", alpha=0.8)
+    plt.legend(
+        ["Pre-processed acceleration signal", "Gait onset", "Gait duration"],
+        fontsize=20,
+        loc="best",
+    )
+    plt.grid(visible=None, which="both", axis="both")
+    plt.xticks(fontsize=20)
+    plt.yticks(fontsize=20)
+    plt.show()
+
+
+# Function to plot results of the physical activity monitoring algorithm
+def pam_plot_results(hourly_average_data, thresholds_mg):
+    """
+    Plots the hourly averaged ENMO for each day along with activity level thresholds.
+
+    Args:
+        hourly_average_data (pd.DataFrame): DataFrame containing hourly averaged ENMO values.
+        thresholds_mg (dict): Dictionary containing threshold values for physical activity detection.
+    """
+    # Plotting
+    fig, ax = plt.subplots(figsize=(14, 8))
+
+    # Choose the 'turbo' colormap for coloring each day
+    colormap = plt.cm.turbo
+
+    # Plot thresholds
+    ax.axhline(
+        y=thresholds_mg.get("sedentary_threshold", 45),
+        color="y",
+        linestyle="--",
+        label="Sedentary threshold",
+    )
+    ax.axhline(
+        y=thresholds_mg.get("light_threshold", 100),
+        color="g",
+        linestyle="--",
+        label="Light physical activity threshold",
+    )
+    ax.axhline(
+        y=thresholds_mg.get("moderate_threshold", 400),
+        color="r",
+        linestyle="--",
+        label="Moderate physical activity threshold",
+    )
+
+    # Plot each day data with a different color
+    for i, date in enumerate(hourly_average_data.index):
+        color = colormap(i)
+        ax.plot(hourly_average_data.loc[date], label=str(date), color=color)
+
+    # Customize plot appearance
+    plt.xticks(range(24), [str(i).zfill(2) for i in range(24)])
+    plt.xlabel("Time (h)", fontsize=16)
+    plt.ylabel("ENMO (mg)", fontsize=16)
+    plt.title("Hourly averaged ENMO for each day along with activity level thresholds")
+    plt.legend(loc="upper left", fontsize=16)
+    plt.grid(visible=None, which="both", axis="both")
+    plt.xticks(fontsize=16)
+    plt.yticks(fontsize=16)
+    plt.tight_layout()
+    plt.show()
+
+
+# Function to estimate tilt angle
+def tilt_angle_estimation(data, sampling_frequency_hz):
+    """
+    Estimate tilt angle using simple method with gyro data.
+
+    Args:
+        data (ndarray, DataFrame): Array or DataFrame containing gyro data.
+        sampling_frequency_hz (float, int): Sampling frequency.
+
+    Returns:
+        tilt (ndarray): Tilt angle estimate (deg).
+    """
+    # Error handling for invalid input data
+    if isinstance(data, pd.DataFrame):
+        data = data.to_numpy()
+
+    # Check if data is a numpy array
+    if not isinstance(data, np.ndarray):
+        raise TypeError("Input data must be a numpy array or pandas DataFrame")
+
+    gyro_y = data[:, 1]
+
+    # Integrate gyro data over time to estimate tilt
+    tilt_angle = -np.cumsum(gyro_y) / sampling_frequency_hz
+
+    return tilt_angle
+
+
+#  Function for denoising using wavelet decomposition
+def wavelet_decomposition(data, level, wavetype):
+    """
+    Denoise a signal using wavelet decomposition and reconstruction.
+
+    Args:
+        data (ndarray): Input signal to denoise.
+        level (int): Order of wavelet decomposition.
+        wavetype (str): Wavelet type to use.
+
+    Returns:
+        denoised_signal (ndarray): Denoised signal.
+    """
+    # Perform wavelet decomposition
+    coeffs = pywt.wavedec(data, wavetype, mode="smooth", level=level)
+
+    # Zero out wavelet coefficients beyond specified order
+    for i in range(1, len(coeffs)):
+        if i != 0:  # Keep the first set of coefficients
+            coeffs[i][:] = 0
+
+    # Reconstruct signal from coefficients
+    denoised_signal = pywt.waverec(coeffs, wavetype, mode="smooth")
+
+    return denoised_signal
+
+
+# Function for computing moving variance
+def moving_var(data, window):
+    """
+    Compute the centered moving variance.
+
+    Args:
+        Data (int) : Data to take the moving variance on window
+        Window size (int) : Window size for the moving variance.
+
+    Returns
+        m_var (numpy.ndarray) : Moving variance
+    """
+
+    # Initialize an array to store the moving variance
+    m_var = np.zeros(data.shape)
+
+    # Calculate the padding required
+    pad = int(np.ceil(window / 2))
+
+    # Define the shape and strides for creating rolling windows
+    shape = data.shape[:-1] + (data.shape[-1] - window + 1, window)
+    strides = data.strides + (data.strides[-1],)
+
+    # Create rolling windows from the input data
+    rw_seq = np.lib.stride_tricks.as_strided(data, shape=shape, strides=strides)
+
+    # Compute the variance along the rolling windows and store it in m_var
+    n = rw_seq.shape[0]
+    m_var[pad : pad + n] = np.var(rw_seq, axis=-1, ddof=1)
+
+    # Copy the variance values to the padding regions
+    m_var[:pad], m_var[pad + n :] = m_var[pad], m_var[-pad - 1]
+
+    return m_var
+
+
+# Function to plot results of the gait sequence detection algorithm
+def pham_plot_results(accel, gyro, postural_transitions_, sampling_freq_Hz):
+    """
+    Plot results of the gait sequence detection algorithm.
+
+    Args:
+        accel (ndarray): Array of acceleration data.
+        gyro (ndarray): Array of gyroscope data.
+        postural_transitions_ (DataFrame): DataFrame containing postural transition information.
+        sampling_freq_Hz (float): Sampling frequency in Hertz.
+
+    Returns:
+        Plot postural transitions
+    """
+    # Figure
+    fig = plt.figure(figsize=(21, 10))
+
+    # Subplot 1: Acceleration data
+    ax1 = plt.subplot(211)
+    for i in range(3):
+        ax1.plot(
+            np.arange(len(accel)) / sampling_freq_Hz,
+            accel[:, i],
+        )
+    for i in range(len(postural_transitions_)):
+        onset = postural_transitions_["onset"][i]
+        duration = postural_transitions_["duration"][i]
+        ax1.axvline(x=onset, color="r")
+        ax1.axvspan(onset, (onset + duration), color="grey")
+    ax1.set_title("Detected Postural Transitions", fontsize=20)
+    ax1.set_ylabel(f"Acceleration (g)", fontsize=14)
+    ax1.set_xlabel(f"Time (sec)", fontsize=14)
+    ax1.legend(
+        ["Acc 1", "Acc 2", "Acc 3", "Event oset", "Event duration"],
+        loc="upper right",
+        fontsize=14,
+    )
+    ax1.set_ylim(-2, 2.5)
+    plt.xticks(fontsize=14)
+    plt.yticks(fontsize=14)
+
+    # Subplot 2: Gyro data
+    ax2 = plt.subplot(212)
+    for i in range(3):
+        ax2.plot(
+            np.arange(len(gyro)) / sampling_freq_Hz,
+            gyro[:, i],
+        )
+    for i in range(len(postural_transitions_)):
+        onset = postural_transitions_["onset"][i]
+        duration = postural_transitions_["duration"][i]
+        ax2.axvline(x=onset, color="r")
+        ax2.axvspan(onset, (onset + duration), color="grey")
+    ax1.set_title("Detected Postural Transitions", fontsize=20)
+    ax2.set_ylabel(f"Gyro (deg/s)", fontsize=14)
+    ax2.set_xlabel(f"Time (sec)", fontsize=14)
+    ax2.legend(
+        ["Gyr 1", "Gyr 2", "Gyr 3", "Event oset", "Event duration"],
+        loc="upper right",
+        fontsize=14,
+    )
+    ax2.set_ylim(-200, 200)
+    plt.xticks(fontsize=14)
+    plt.yticks(fontsize=14)
+    fig.tight_layout()
+    plt.show()
+
+
+# Function to detect postural transitions based on stationary periods
+def process_postural_transitions_stationary_periods(
+    time,
+    accel,
+    gyro,
+    stationary,
+    tilt_angle_deg,
+    sampling_period,
+    sampling_freq_Hz,
+    init_period,
+    local_peaks,
+):
+    """
+    Estimate orientation and analyze postural transitions based on sensor data.
+
+    Args:
+        time (ndarray): Array of timestamps.
+        accel (ndarray): Array of accelerometer data (3D).
+        gyro (ndarray): Array of gyroscope data (3D).
+        stationary (ndarray): Array indicating stationary periods.
+        tilt_angle_deg (ndarray): Array of tilt angle data.
+        sampling_period (float): Sampling period in seconds.
+        sampling_freq_Hz (float): Sampling frequency in Hz.
+        init_period (float): Initialization period in seconds.
+        local_peaks (ndarray): Array of indices indicating local peaks.
+
+    Returns:
+        tuple: A tuple containing:
+            time_pt (list): List of peak times.
+            pt_type (list): List of postural transition types.
+            pt_angle (list): List of postural transition angles.
+            duration (list): List of postural transition durations.
+            flexion_max_vel (list): List of maximum flexion velocities.
+            extension_max_vel (list): List of maximum extension velocities.
+    """
+    # If there is enough stationary data, perform sensor fusion using accelerometer and gyro data
+    # Initialize quaternion array for orientation estimation
+    quat = np.zeros((len(time), 4))
+
+    # Initial convergence: Update the quaternion using the mean accelerometer values over a certain period
+    # This helps in initializing the orientation for accurate estimation
+    index_sel = np.arange(0, np.where(time >= time[0] + init_period)[0][0] + 1)
+    mean_accel = np.mean(accel[index_sel], axis=0)
+    quat[0] = quaternion.rotm2quat(np.eye(3) + quaternion.axang2rotm(mean_accel))
+
+    # Update the quaternion for all data points
+    for t in range(1, len(time)):
+        # Calculate the rotation matrix from gyroscope data
+        dt = time[t] - time[t - 1]
+        ang_velocity = gyro[t] * dt
+        delta_rot = quaternion.axang2rotm(ang_velocity)
+
+        # Update the quaternion based on the rotation matrix
+        quat[t] = quaternion.quatmultiply(quat[t - 1], quaternion.rotm2quat(delta_rot))
+
+        # Normalize the quaternion to avoid drift
+        quat[t] = quaternion.quatnormalize(quat[t])
+
+    # Analyze gyro data to detect peak velocities and directional changes
+    # Zero-crossing method is used to define the beginning and the end of a PT in the gyroscope signal
+    iZeroCr = np.where((gyro[:, 1][:-1] * gyro[:, 1][1:]) < 0)[0]
+
+    # Calculate the difference between consecutive values
+    gyrY_diff = np.diff(gyro[:, 1])
+
+    # Beginning of a PT was defined as the first zero crossing point of themedio-lateral angular
+    # velocity (gyro[:,1]) on the left side of the PT event, with negative slope.
+    # Initialize left side indices with ones
+    ls = np.ones_like(local_peaks)
+
+    # Initialize right side indices with length of gyro data
+    # rs = len(gyro[:,1]) * np.ones_like(local_peaks)
+    rs = np.full_like(local_peaks, len(gyro[:, 1]))
+    for i in range(len(local_peaks)):
+        # Get the index of the current local peak
+        pt = local_peaks[i]
+
+        # Calculate distances to all zero-crossing points relative to the peak
+        dist2peak = iZeroCr - pt
+
+        # Extract distances to zero-crossing points on the left side of the peak
+        dist2peak_ls = dist2peak[dist2peak < 0]
+
+        # Extract distances to zero-crossing points on the right side of the peak
+        dist2peak_rs = dist2peak[dist2peak > 0]
+
+        # Iterate over distances to zero-crossing points on the left side of the peak (in reverse order)
+        for j in range(len(dist2peak_ls) - 1, -1, -1):
+            # Check if slope is down and the left side not too close to the peak (more than 200ms)
+            if gyrY_diff[pt + dist2peak_ls[j]] < 0 and -dist2peak_ls[j] > 25:
+                # Store the index of the left side
+                ls[i] = pt + dist2peak_ls[j]
+                break
+
+    # Further analysis to distinguish between different types of postural transitions (sit-to-stand or stand-to-sit)
+    # Rotate body accelerations to Earth frame
+    acc = quaternion.rotm2quat(
+        np.column_stack((accel[:, 0], accel[:, 1], accel[:, 2])), quat
+    )
+
+    # Remove gravity from measurements
+    acc -= np.array([[0, 0, 1]] * len(time))
+
+    # Convert acceletion data to m/s^2
+    acc *= 9.81
+
+    # Calculate velocities
+    vel = np.zeros_like(acc)
+
+    # Iterate over time steps
+    for t in range(1, len(vel)):
+        # Integrate acceleration to calculate velocity
+        vel[t, :] = vel[t - 1, :] + acc[t, :] * sampling_period
+        if stationary[t] == 1:
+            # Force zero velocity when stationary
+            vel[t, :] = [0, 0, 0]
+
+    # Compute and remove integral drift
+    velDrift = np.zeros_like(vel)
+
+    # Indices where stationary changes to non-stationary
+    activeStart = np.where(np.diff(stationary) == -1)[0]
+
+    # Indices where non-stationary changes to stationary
+    activeEnd = np.where(np.diff(stationary) == 1)[0]
+    if activeStart[0] > activeEnd[0]:
+        # Ensure start from index 0 if starts non-stationary
+        activeStart = np.insert(activeStart, 0, 0)
+
+    if activeStart[-1] > activeEnd[-1]:
+        # Ensure last segment ends properly
+        activeEnd = np.append(activeEnd, len(stationary))
+    for i in range(len(activeEnd)):
+        # Calculate drift rate
+        driftRate = vel[activeEnd[i] - 1] / (activeEnd[i] - activeStart[i])
+
+        # Enumerate time steps within the segment
+        enum = np.arange(1, activeEnd[i] - activeStart[i] + 1)
+
+        # Calculate drift for each time step
+        drift = np.column_stack(
+            (enum * driftRate[0], enum * driftRate[1], enum * driftRate[2])
+        )
+
+        # Store the drift for this segment
+        velDrift[activeStart[i] : activeEnd[i], :] = drift
+
+    # Remove integral drift from velocity
+    vel -= velDrift
+
+    # Compute translational position
+    pos = np.zeros_like(vel)
+
+    # Iterate over time steps
+    for t in range(1, len(pos)):
+        # Integrate velocity to yield position
+        pos[t, :] = pos[t - 1, :] + vel[t, :] * sampling_period
+
+    # Estimate vertical displacement and classify as actual PTs or Attempts
+    # Calculate vertical displacement
+    disp_z = pos[rs, 2] - pos[ls, 2]
+
+    # Initialize flag for actual PTs
+    pt_actual_flag = np.zeros_like(local_peaks)
+
+    for i in range(len(disp_z)):
+        # Displacement greater than 10cm and less than 1m
+        if 0.1 < abs(disp_z[i]) < 1:
+            # Flag as actual PT if displacement meets criteria
+            pt_actual_flag[i] = 1
+
+    # Initialize list for PT types
+    pt_type = []
+
+    # Distinguish between different types of postural transitions
+    for i in range(len(local_peaks)):
+        if pt_actual_flag[i] == 1:
+            if disp_z[i] == 0:
+                pt_type.append("NA")
+            elif disp_z[i] > 0:
+                pt_type.append("sit to stand")
+            else:
+                pt_type.append("stand to sit")
+        else:
+            pt_type.append("NA")
+
+    # Calculate maximum flexion velocity and maximum extension velocity
+    flexion_max_vel = np.zeros_like(local_peaks)
+    extension_max_vel = np.zeros_like(local_peaks)
+    for i in range(len(local_peaks)):
+        flexion_max_vel[i] = max(abs(gyro[:, 1][ls[i] : local_peaks[i]]))
+        extension_max_vel[i] = max(abs(gyro[:, 1][local_peaks[i] : rs[i]]))
+
+    # Calculate PT angle
+    pt_angle = np.abs(tilt_angle_deg[local_peaks] - tilt_angle_deg[ls])
+    if ls[0] == 0:
+        # Adjust angle for the first PT if necessary
+        pt_angle[0] = np.abs(tilt_angle_deg[local_peaks[0]] - tilt_angle_deg[rs[0]])
+
+    # Calculate duration of each PT
+    duration = (rs - ls) / sampling_freq_Hz
+
+    # Convert peak times to integers
+    time_pt = time[local_peaks]
+
+    # Initialize PTs list
+    # i.e., the participant was considered to perform a complete standing up or sitting down movement
+    PTs = [
+        [
+            "Time[s]",
+            "Type",
+            "Angle[°]",
+            "Duration[s]",
+            "Max flexion velocity[°/s]",
+            "Max extension velocity[°/s]",
+            "Vertical displacement[m]",
+        ]
+    ]
+
+    # Initialize Attempts list
+    # i.e., the participant was considered not to perform a complete PT, e.g., forward and backwards body motion
+    Attempts = [
+        [
+            "Time[s]",
+            "Type",
+            "Angle[°]",
+            "Duration[s]",
+            "Max flexion velocity[°/s]",
+            "Max extension velocity[°/s]",
+            "Vertical displacement[m]",
+        ]
+    ]
+
+    # Iterate over detected peaks
+    for i in range(len(local_peaks)):
+        if pt_actual_flag[i] == 1:
+            PTs.append(
+                [
+                    time_pt[i],
+                    pt_type[i],
+                    pt_angle[i],
+                    duration[i],
+                    flexion_max_vel[i],
+                    extension_max_vel[i],
+                    disp_z[i],
+                ]
+            )  # Append PT details to PTs list
+        else:
+            Attempts.append(
+                [
+                    time_pt[i],
+                    pt_type[i],
+                    pt_angle[i],
+                    duration[i],
+                    flexion_max_vel[i],
+                    extension_max_vel[i],
+                    disp_z[i],
+                ]
+            )  # Append PT details to Attempts list
+
+    # Extract postural transition information from PTs
+    time_pt = [pt[0] for pt in PTs[1:]]
+    pt_type = [pt[1] for pt in PTs[1:]]
+    pt_angle = [pt[2] for pt in PTs[1:]]
+    duration = [pt[3] for pt in PTs[1:]]
+    flexion_max_vel = [pt[4] for pt in PTs[1:]]
+    extension_max_vel = [pt[5] for pt in PTs[1:]]
+
+    # Return the necessary outputs
+    return time_pt, pt_type, pt_angle, duration, flexion_max_vel, extension_max_vel
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ngmt-0.0.3/ngmt/utils/quaternion.py` & `ngmt-0.0.4/ngmt/utils/quaternion.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,31 @@
 ) -> np.ndarray:
     """
     Compute the inverse of quaternions.
 
     This function calculates the inverse of quaternions by first computing the conjugate
     and then normalizing the conjugate.
 
-    Parameters:
-    - q (np.ndarray): Input array of quaternions with shape (..., 4).
-    - scalar_first (bool, optional): If True, assumes the scalar part is the first element.
-      If False, assumes the scalar part is the last element. Default is True.
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the second-to-last dimension. Default is True.
+    Args:
+        q (np.ndarray): Input array of quaternions with shape (..., 4).
+        scalar_first (bool, optional): If True, assumes the scalar part is the first element.
+            If False, assumes the scalar part is the last element. Default is True.
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the second-to-last dimension. Default is True.
 
     Returns:
-    - np.ndarray: Inverse of quaternions with the same shape as the input array.
+        np.ndarray: Inverse of quaternions with the same shape as the input array.
 
     Notes:
-    - The input array is cast to float before the computation.
-    - If channels_last is False, the input array is transposed to switch channels and time axis.
+        - The input array is cast to float before the computation.
+        - If channels_last is False, the input array is transposed to switch channels and time axis.
 
     Quaternion Inverse Calculation:
-    The inverse of a quaternion q is obtained by first calculating its conjugate and then normalizing it:
-    q_inv = normalize(conjugate(q))
+        >>> The inverse of a quaternion q is obtained by first calculating its conjugate and then normalizing it:
+        >>> q_inv = normalize(conjugate(q))
     """
 
     # Cast array to float
     q = np.asarray(q, float)
 
     # Compute the quaternion conjugate
     qconj = quatconj(q, scalar_first=scalar_first, channels_last=channels_last)
@@ -47,29 +47,29 @@
 def quatnormalize(q: np.ndarray, channels_last: bool = True) -> np.ndarray:
     """
     Normalize quaternions.
 
     This function normalizes quaternions by dividing each quaternion by its magnitude (norm).
     The result is a unit quaternion with the same orientation as the original quaternion.
 
-    Parameters:
-    - q (np.ndarray): Input array of quaternions with shape (..., 4).
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the second-to-last dimension. Default is True.
+    Args:
+        q (np.ndarray): Input array of quaternions with shape (..., 4).
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the second-to-last dimension. Default is True.
 
     Returns:
-    - np.ndarray: Normalized quaternions with the same shape as the input array.
+        np.ndarray: Normalized quaternions with the same shape as the input array.
 
     Notes:
-    - The input array is cast to float before the computation.
-    - If channels_last is False, the input array is transposed to switch channels and time axis.
+        - The input array is cast to float before the computation.
+        - If channels_last is False, the input array is transposed to switch channels and time axis.
 
     Quaternion Normalization:
-    The normalization of a quaternion q is performed by dividing each element of q by its norm:
-    q_normalized = q / norm(q)
+        >>> The normalization of a quaternion q is performed by dividing each element of q by its norm:
+        >>> q_normalized = q / norm(q)
     """
 
     # Cast array to float
     q = np.asarray(q, float)
 
     # Calculate the norm
     norm = quatnorm(q, channels_last=channels_last)
@@ -82,29 +82,29 @@
 def quatnorm(q: np.ndarray, channels_last: bool = True) -> np.ndarray:
     """
     Calculate the norm (magnitude) of quaternions.
 
     This function computes the norm (magnitude) of quaternions along the specified axis,
     which represents the length of the quaternion vector.
 
-    Parameters:
-    - q (np.ndarray): Input array of quaternions with shape (..., 4).
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the first dimension. Default is True.
+    Args:
+        q (np.ndarray): Input array of quaternions with shape (..., 4).
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the first dimension. Default is True.
 
     Returns:
-    - np.ndarray: Norm of quaternions along the specified axis with the same shape as the input array.
+        np.ndarray: Norm of quaternions along the specified axis with the same shape as the input array.
 
     Notes:
-    - The input array is cast to float before the computation.
-    - If channels_last is False, the input array is transposed to switch channels and time axis.
+        - The input array is cast to float before the computation.
+        - If channels_last is False, the input array is transposed to switch channels and time axis.
 
     Quaternion Norm Calculation:
-    The norm of a quaternion q is calculated as follows:
-    norm(q) = sqrt(w^2 + x^2 + y^2 + z^2)
+        >>> The norm of a quaternion q is calculated as follows:
+        >>> norm(q) = sqrt(w^2 + x^2 + y^2 + z^2)
     """
 
     # Cast array to float
     q = np.asarray(q, float)
 
     # Calculate the quaternion norm
     norm = (
@@ -120,31 +120,31 @@
 ) -> np.ndarray:
     """
     Compute the quaternion conjugate.
 
     This function calculates the conjugate of a quaternion, which is obtained by negating
     the imaginary (vector) parts while keeping the real (scalar) part unchanged.
 
-    Parameters:
-    - q (np.ndarray): Input array of quaternions with shape (..., 4).
-    - scalar_first (bool, optional): If True, assumes the scalar part is the first element.
-      If False, assumes the scalar part is the last element. Default is True.
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the second-to-last dimension. Default is True.
+    Args:
+        q (np.ndarray): Input array of quaternions with shape (..., 4).
+        scalar_first (bool, optional): If True, assumes the scalar part is the first element.
+            If False, assumes the scalar part is the last element. Default is True.
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the second-to-last dimension. Default is True.
 
     Returns:
-    - np.ndarray: Quaternion conjugate with the same shape as the input array.
+        np.ndarray: Quaternion conjugate with the same shape as the input array.
 
     Notes:
-    - The input array is cast to float before the computation.
-    - If channels_last is False, the input array is transposed to switch channels and time axis.
-    - If scalar_first is False, the scalar part is moved to the last element.
+        - The input array is cast to float before the computation.
+        - If channels_last is False, the input array is transposed to switch channels and time axis.
+        - If scalar_first is False, the scalar part is moved to the last element.
 
     Quaternion Conjugate Formula:
-    q_conj = [w, -x, -y, -z]
+        >>> q_conj = [w, -x, -y, -z]
     """
 
     # Cast array to float
     q = np.asarray(q, float)
 
     if not channels_last:
         # Take the tranpose, i.e. switch channels and time axis
@@ -183,39 +183,39 @@
     """
     Multiply two sets of quaternions.
 
     This function performs quaternion multiplication on two sets of quaternions.
     Quaternions are 4-dimensional vectors of the form [w, x, y, z], where 'w' is the
     scalar (real) part, and 'x', 'y', and 'z' are the vector (imaginary) parts.
 
-    Parameters:
-    - q1 (np.ndarray): Input array of quaternions with shape (..., 4).
-    - q2 (np.ndarray, optional): Input array of quaternions with shape (..., 4).
-      If None, q2 is set to q1, making it a self-multiplication. Default is None.
-    - scalar_first (bool, optional): If True, assumes the scalar part is the first element.
-      If False, assumes the scalar part is the last element. Default is True.
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the second-to-last dimension. Default is True.
+    Args:
+        q1 (np.ndarray): Input array of quaternions with shape (..., 4).
+        q2 (np.ndarray, optional): Input array of quaternions with shape (..., 4).
+            If None, q2 is set to q1, making it a self-multiplication. Default is None.
+        scalar_first (bool, optional): If True, assumes the scalar part is the first element.
+            If False, assumes the scalar part is the last element. Default is True.
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the second-to-last dimension. Default is True.
 
     Returns:
-    - np.ndarray: Result of quaternion multiplication with the same shape as the input arrays.
+        np.ndarray: Result of quaternion multiplication with the same shape as the input arrays.
 
     Raises:
-    - AssertionError: If the last dimension of q1 and q2 is not 4.
+        AssertionError: If the last dimension of q1 and q2 is not 4.
 
     Notes:
-    - If q2 is None, this function performs self-multiplication (q1 * q1).
-    - The input arrays are cast to float before the computation.
-    - If channels_last is False, the input arrays are transposed to switch channels and time axis.
-
-    Quaternion Multiplication Formula:
-    q3 = [w1w2 - x1x2 - y1y2 - z1z2,
-          w1x2 + x1w2 + y1z2 - z1y2,
-          w1y2 - x1z2 + y1w2 + z1x2,
-          w1z2 + x1y2 - y1x2 + z1w2]
+        - If q2 is None, this function performs self-multiplication (q1 * q1).
+        - The input arrays are cast to float before the computation.
+        - If channels_last is False, the input arrays are transposed to switch channels and time axis.
+
+    Quaternion Conjugate Formula:
+        >>> q3 = [w1w2 - x1x2 - y1y2 - z1z2,
+            w1x2 + x1w2 + y1z2 - z1y2,
+            w1y2 - x1z2 + y1w2 + z1x2,
+            w1z2 + x1y2 - y1x2 + z1w2]
     """
 
     # Parse input quaternions
     q2 = q1.copy() if q2 is None else q2
 
     # Cast arrays to float
     q1 = np.asarray(q1, float)
@@ -280,36 +280,37 @@
     if not channels_last:
         # Switch channels and time axis back
         q3 = q3.T
     return q3
 
 
 def rotm2quat(R: np.ndarray, method: int | str = "auto") -> np.ndarray:
-    """Convert a 3x3 rotation matrix to a quaternion.
+    """
+    Convert a 3x3 rotation matrix to a quaternion.
 
     Source:
     - https://github.com/dlaidig/qmt/blob/0fa8d32eb461e14d78e9ddbd569664ea59bcea19/qmt/functions/quaternion.py#L1004
 
-    Parameters:
-    - R (np.ndarray): A rotation matrix with shape (3, 3).
-    - scalar_first (bool, optional): If True, sets the first element as the scalar part.
-      If False, sets the last element as the scalar part is the last element. Default is True.
-    - channels_last (bool, optional): If True, assumes the channels are the last dimension.
-      If False, assumes the channels are the first dimension. Default is True.
+    Args:
+        R (np.ndarray): A rotation matrix with shape (3, 3).
+        scalar_first (bool, optional): If True, sets the first element as the scalar part.
+            If False, sets the last element as the scalar part is the last element. Default is True.
+        channels_last (bool, optional): If True, assumes the channels are the last dimension.
+            If False, assumes the channels are the first dimension. Default is True.
 
     Returns:
-    - np.ndarray: The quaternion corresponding to the rotation matrix.
+        np.ndarray: The quaternion corresponding to the rotation matrix.
 
     Raises:
-    - AssertionError: If the shape of R is not (3, 3).
+        AssertionError: If the shape of R is not (3, 3).
 
     Notes:
-    - If q2 is None, this function performs self-multiplication (q1 * q1).
-    - The input arrays are cast to float before the computation.
-    - If channels_last is False, the input arrays are transposed to switch channels and time axis.
+        - If q2 is None, this function performs self-multiplication (q1 * q1).
+        - The input arrays are cast to float before the computation.
+        - If channels_last is False, the input arrays are transposed to switch channels and time axis.
     """
 
     # Cast array to float
     R = np.asarray(R, float)
     assert R.ndim >= 2 and R.shape[-2:] == (3, 3)
 
     w_sq = (1 + R[..., 0, 0] + R[..., 1, 1] + R[..., 2, 2]) / 4
@@ -357,49 +358,38 @@
 
 def quat2rotm(
     q: np.ndarray, scalar_first: bool = True, channels_last: bool = True
 ) -> np.ndarray:
     """
     Convert quaternion(s) to rotation matrix.
 
-    Parameters
-    ----------
-    q : np.ndarray
-        Input quaternion(s) as a NumPy array. The last dimension must have size 4.
-    scalar_first : bool, optional
-        If True, the quaternion is assumed to be in scalar-first order (default is True).
-    channels_last : bool, optional
-        If True, the last dimension represents the quaternion channels (default is True).
-        If False, the quaternion channels are assumed to be in the first dimension.
-
-    Returns
-    -------
-    np.ndarray
-        Rotation matrix corresponding to the input quaternion(s).
-
-    Raises
-    ------
-    AssertionError
-        If the last dimension of the input array `q` does not have size 4.
-
-    Notes
-    -----
-    The conversion is based on the formula:
-    R = | 1 - 2*q2^2 - 2*q3^2    2*(q1*q2 - q3*q0)    2*(q1*q3 + q2*q0) |
-        | 2*(q1*q2 + q3*q0)    1 - 2*q1^2 - 2*q3^2    2*(q2*q3 - q1*q0) |
-        | 2*(q1*q3 - q2*q0)    2*(q1*q0 + q2*q3)    1 - 2*q1^2 - 2*q2^2 |
-
-    References
-    ----------
-    - Wikipedia: https://en.wikipedia.org/wiki/Rotation_matrix#Quaternion
-
-    Examples
-    --------
-    >>> quaternion = np.array([1.0, 0.0, 0.0, 0.0])
-    >>> rotation_matrix = quat2rotm(quaternion)
+    Args:
+        q (np.ndarray): Input quaternion(s) as a NumPy array. The last dimension must have size 4.
+        scalar_first (bool, optional): If True, the quaternion is assumed to be in scalar-first order (default is True).
+        channels_last (bool, optional): If True, the last dimension represents the quaternion channels (default is True).
+            If False, the quaternion channels are assumed to be in the first dimension.
+
+    Returns:
+        np.ndarray: Rotation matrix corresponding to the input quaternion(s).
+
+    Raises:
+        AssertionError: If the last dimension of the input array `q` does not have size 4.
+
+    Notes:
+        >>> The conversion is based on the formula:
+        >>> R = | 1 - 2*q2^2 - 2*q3^2    2*(q1*q2 - q3*q0)    2*(q1*q3 + q2*q0) |
+            | 2*(q1*q2 + q3*q0)    1 - 2*q1^2 - 2*q3^2    2*(q2*q3 - q1*q0) |
+            | 2*(q1*q3 - q2*q0)    2*(q1*q0 + q2*q3)    1 - 2*q1^2 - 2*q2^2 |
+
+    References:
+        Wikipedia: https://en.wikipedia.org/wiki/Rotation_matrix#Quaternion
+
+    Examples:
+        >>> quaternion = np.array([1.0, 0.0, 0.0, 0.0])
+        >>> rotation_matrix = quat2rotm(quaternion)
     """
 
     # Cast array to float
     q = np.asarray(q, float)
     assert q.shape[-1] == 4
 
     # Derive rotation matrix from quaternion
@@ -416,21 +406,21 @@
     return R
 
 
 def quat2axang(q: np.ndarray) -> np.ndarray:
     """
     Convert a quaternion to axis-angle representation.
 
-    Parameters:
-    - q (np.ndarray): Input quaternion array of shape (..., 4).
+    Args:
+        q (np.ndarray): Input quaternion array of shape (..., 4).
 
     Returns:
-    - np.ndarray: Axis-angle representation array of shape (..., 4),
-                  where the first three elements are the axis of rotation
-                  and the last element is the angle of rotation in radians.
+        np.ndarray: Axis-angle representation array of shape (..., 4),
+            where the first three elements are the axis of rotation
+            and the last element is the angle of rotation in radians.
 
     The function normalizes the input quaternion, calculates the angle of rotation,
     and computes the axis of rotation in the axis-angle representation.
 
     Note: The input quaternion array is expected to have the last dimension of size 4.
     """
 
@@ -446,7 +436,52 @@
     axang[..., 3] = 2.0 * np.arccos(q[..., 0])
     axang[..., :3] = np.where(
         np.sin(axang[..., 3] / 2.0) > _EPS,
         q[..., 1:] / np.sin(axang[..., 3] / 2.0),
         np.array([0.0, 0.0, 1.0]),
     )
     return axang
+
+
+def axang2rotm(axang: np.ndarray) -> np.ndarray:
+    """
+    Convert axis-angle representation to rotation matrix.
+
+    Args:
+        axang (np.ndarray): Input array of axis-angle representations with shape (..., 4),
+            where the first three elements are the axis of rotation
+            and the last element is the angle of rotation in radians.
+
+    Returns:
+        np.ndarray: Rotation matrix corresponding to the input axis-angle representations.
+
+    The function computes the rotation matrix using Rodrigues' rotation formula.
+    """
+
+    # Cast array to float
+    axang = np.asarray(axang, float)
+    assert axang.shape[-1] == 4
+
+    # Extract axis and angle
+    axis = axang[..., :3]
+    angle = axang[..., 3]
+
+    # Normalize axis
+    axis /= np.linalg.norm(axis, axis=-1, keepdims=True)
+
+    # Compute rotation matrix using Rodrigues' rotation formula
+    cos_theta = np.cos(angle)
+    sin_theta = np.sin(angle)
+    cross_prod_matrix = np.zeros((*axis.shape[:-1], 3, 3), dtype=float)
+    cross_prod_matrix[..., 0, 1] = -axis[..., 2]
+    cross_prod_matrix[..., 0, 2] = axis[..., 1]
+    cross_prod_matrix[..., 1, 0] = axis[..., 2]
+    cross_prod_matrix[..., 1, 2] = -axis[..., 0]
+    cross_prod_matrix[..., 2, 0] = -axis[..., 1]
+    cross_prod_matrix[..., 2, 1] = axis[..., 0]
+    rotation_matrix = (
+        np.eye(3, dtype=float) * cos_theta[..., None]
+        + sin_theta[..., None] * cross_prod_matrix
+        + (1 - cos_theta[..., None]) * np.einsum("...i,...j->...ij", axis, axis)
+    )
+
+    return rotation_matrix
```

### Comparing `ngmt-0.0.3/pyproject.toml` & `ngmt-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ngmt"
-version = "0.0.3"
+version = "0.0.4"
 description = "The NeuroGeriatricMotionToolbox (NGMT) is a Python-based toolbox for processing motion data."
 license = "MIT"
 readme = "README.md"
 homepage = "https://neurogeriatricskiel.github.io/NGMT/"
 repository = "https://github.com/neurogeriatricskiel/NGMT"
 documentation = "https://neurogeriatricskiel.github.io/NGMT"
 authors = [
@@ -18,17 +18,18 @@
     "Masoud Abedinifar <Masoud.Abedinifar@uksh.de>",
     "Julius Welzel <j.welzel@neurologie.uni-kiel.de>",
     "Robbin Romijnders <r.romijnders@neurologie.uni-kiel.de>"
 ]
 packages = [
     { include = "ngmt" },
 ]
+include = ["CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = ">=3.9.0,<3.13"
+python = ">=3.10.0,<3.13"
 pandas = ">=2"
 scipy = ">=1.11.0"
 numpy = ">=1.25"
 pytest = "^7.4.3"
 pywavelets = "^1.4.1"
 ipykernel = "^6.26.0"
 matplotlib = "^3.8.1"
@@ -36,14 +37,16 @@
 qmt = "^0.2.4"
 vqf = "^2.0.0"
 h5py = "^3.10.0"
 polars = "^0.20.5"
 seaborn = "^0.13.1"
 json-repair = "^0.8.0"
 pyarrow = "^15.0.0"
+bids-validator = "^1.14.4"
+actipy = "^3.0.5"
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-material", "pymdownx.superfences"]
 
 [tool.poetry.group.dev.dependencies]
 pytest-cov = "^4.1.0"
 pytest = "^7.4.3"
```

### Comparing `ngmt-0.0.3/README.md` & `ngmt-0.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 [![codecov](https://codecov.io/gh/neurogeriatricskiel/NGMT/graph/badge.svg?token=L578RHZ699)](https://codecov.io/gh/neurogeriatricskiel/NGMT)
 [![build docs](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/mkdocs.yml/badge.svg)](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/mkdocs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub issues](https://img.shields.io/github/issues-raw/neurogeriatricskiel/NGMT)
 ![GitHub contributors](https://img.shields.io/github/contributors/neurogeriatricskiel/NGMT)
 [![lint-and-test](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/test-and-lint.yml/badge.svg)](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/test-and-lint.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ngmt)
 
-# NGMT
-![NeurogeriatricsLogo](ng_logo.png)
+
+![NGMTLogo](ngmt_logo_transBG.png)
 
 Welcome to the NeuroGeriatricMotionToolbox (NGMT). We are a Python based toolbox for processing motion data.
 
-> The toolbox is currently under development and is not yet ready for use.
+!!! warning
+
+    The toolbox is currently under development and is not yet ready for use.
 
-The toolbox is aimed at a wide variety of motion researchers who want to use open souce software to process their data.
-We have implemented a wide variety of functions to process motion data, such as:
--   Gait sequence detection (GSD)
--   Inital contact detection (ICD)
--   More to follow ...
 
-The idea is that various motion data can be loaded into our dedicated dataclasses which rely on principles from the [Motion-BIDS](https://bids-specification.readthedocs.io/en/latest/modality-specific-files/motion.html) standard.
+The toolbox is aimed at motion researchers who want to use python based open source software to process their data.
+We have implemented validated algorithms in modules to process motion data, such as:
+   - Gait sequence detection (GSD)
+   - Inital contact detection (ICD)
+   - Physical activity monitoring (PAM)
+   - Postural transition detection (SSD)
+   - More to follow ...
+
+The idea is that various motion data can be loaded into our dedicated dataclass which rely on principles from the [Motion-BIDS](https://bids-specification.readthedocs.io/en/latest/modality-specific-files/motion.html) standard.
 
 ## Data classes
 ### Data classes: conceptual framework
 
 Motion data is recorded with many different systems and modalities, each with their own proprietary data format. NGMT deals with this by organizing both data and metadata in a [BIDS-like format](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html). The BIDS format suggests that [motion recording data](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html#motion-recording-data) from a single tracking system is organized in a single `*_tracksys-<label>_motion.tsv` file. 
 
-> [!NOTE]  
-> A tracking system is defined as a group of motion channels that share hardware properties (the recording device) and software properties (the recording duration and number of samples).
+!!! note
+
+    A tracking system is defined as a group of motion channels that share hardware properties (the recording device) and software properties (the recording duration and number of samples).
 
 In NGMT, data from a single tracking system is therefore loaded into a single `pandas.DataFrame`. The column headers of this `pandas.DataFrame` refer to the channels, and the corresponding [channels information](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html#channels-description-_channelstsv) is likewise available as a `pandas.DataFrame`.
 
-Similarly, if any [events](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/task-events.html) are available for the given recording, these are loaded into a single `pandas.DataFrame` for each tracking system as well.
+Similarly, if any [events](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/task-events.html) are available for the given recording, these are loaded into a single `pandas.DataFrame` for each tracking system as well. The events derived from the toolbox can be exported to a BIDS like '*_events.tsv' file.
 
 ### Data classes: in practice
 These concepts are translated into a NGMT dataclass for each recording: `NGMTRecording`:
 ```mermaid
 classDiagram
    class NGMTRecording {
       data: dict[str, pd.DataFrame]
       channels: dict[str, pd.DataFrame]
       info: None | dict[str, Any] = None
       events: None | dict[str, pd.DataFrame] = None
       events_info: None | dict[str, Any] = None
+      add_events(tracking_system, new_events)
+      add_info(key, value)
+      export_events(file_path, tracking_system=None, file_name=None, bids_compatible_fname=False)
    }
 
 ```
  A recording consists of the motion data from one or more tracking systems, where each tracking system may consist motion data from one or more tracked points. Therefore, the motion data (`NGMTRecording.data`) are organized as a dictionary where the dictionary keys refer to the tracking systems, and the corresponding values the actual (raw) data as a `pandas.DataFrame`. The description of data channels (`NGMTRecording.channels`) is availabe as a dictionary with the same keys, and the values contain the channels description.
 ```python
 >>> from ngmt.datasets import mobilised
 >>> file_name = "/mnt/neurogeriatrics_data/Mobilise-D/rawdata/sub-3011/Free-living/data.mat"
@@ -54,54 +64,65 @@
 {'SU':         LowerBack_ACCEL_x  ...  LowerBack_BARO_n/a
 0                0.967784  ...         1011.628100
 1                0.969667  ...         1011.628400
 ...                   ...  ...                 ...
 993022           0.970579  ...         1012.078703
 993023           0.960542  ...         1002.580321
 
-[993024 rows x 10 columns], 'SU_INDIP':         LowerBack_ACCEL_x  ...  LowerBack_MAGN_z
+[993024 rows x 10 columns], 
+
+'SU_INDIP':      LowerBack_ACCEL_x  ... LowerBack_MAGN_z
 0                0.967986  ...         -5.902833
 1                0.963671  ...          9.501037
 ...                   ...  ...               ...
 993022           0.951656  ...        -17.987983
 993023           0.955107  ...        -18.050600
 
-[993024 rows x 9 columns]}
+[993024 rows x 9 columns]
+}
+
 >>> recording.channels
-{'SU':                  name type component tracked_point  units  sampling_frequency
-0   LowerBack_ACCEL_x  Acc         x     LowerBack      g               100.0
-1   LowerBack_ACCEL_y  Acc         y     LowerBack      g               100.0
-2   LowerBack_ACCEL_z  Acc         z     LowerBack      g               100.0
-3  LowerBack_ANGVEL_x  Gyr         x     LowerBack  deg/s               100.0
-4  LowerBack_ANGVEL_y  Gyr         y     LowerBack  deg/s               100.0
-5  LowerBack_ANGVEL_z  Gyr         z     LowerBack  deg/s               100.0
-6    LowerBack_MAGN_x  Mag         x     LowerBack     µT               100.0
-7    LowerBack_MAGN_y  Mag         y     LowerBack     µT               100.0
-8    LowerBack_MAGN_z  Mag         z     LowerBack     µT               100.0
-9  LowerBack_BARO_n/a  Bar       n/a     LowerBack    hPa               100.0, 'SU_INDIP':                  name type component tracked_point  units  sampling_frequency
-0   LowerBack_ACCEL_x  Acc         x     LowerBack      g               100.0
-1   LowerBack_ACCEL_y  Acc         y     LowerBack      g               100.0
-2   LowerBack_ACCEL_z  Acc         z     LowerBack      g               100.0
-3  LowerBack_ANGVEL_x  Gyr         x     LowerBack  deg/s               100.0
-4  LowerBack_ANGVEL_y  Gyr         y     LowerBack  deg/s               100.0
-5  LowerBack_ANGVEL_z  Gyr         z     LowerBack  deg/s               100.0
-6    LowerBack_MAGN_x  Mag         x     LowerBack     µT               100.0
-7    LowerBack_MAGN_y  Mag         y     LowerBack     µT               100.0
-8    LowerBack_MAGN_z  Mag         z     LowerBack     µT               100.0}
+{'SU':                  
+   name                 type  component   tracked_point  units    sampling_frequency
+0  LowerBack_ACCEL_x    Acc   x           LowerBack      g        100.0
+1  LowerBack_ACCEL_y    Acc   y           LowerBack      g        100.0
+2  LowerBack_ACCEL_z    Acc   z           LowerBack      g        100.0
+3  LowerBack_ANGVEL_x   Gyr   x           LowerBack      deg/s    100.0
+4  LowerBack_ANGVEL_y   Gyr   y           LowerBack      deg/s    100.0
+5  LowerBack_ANGVEL_z   Gyr   z           LowerBack      deg/s    100.0
+6  LowerBack_MAGN_x     Mag   x           LowerBack      µT       100.0
+7  LowerBack_MAGN_y     Mag   y           LowerBack      µT       100.0
+8  LowerBack_MAGN_z     Mag   z           LowerBack      µT       100.0
+9  LowerBack_BARO_n/a   Bar   n/a         LowerBack      hPa      100.0, 
+
+'SU_INDIP':
+   name                 type  component   tracked_point  units    sampling_frequency
+0  LowerBack_ACCEL_x    Acc   x           LowerBack      g        100.0
+1  LowerBack_ACCEL_y    Acc   y           LowerBack      g        100.0
+2  LowerBack_ACCEL_z    Acc   z           LowerBack      g        100.0
+3  LowerBack_ANGVEL_x   Gyr   x           LowerBack      deg/s    100.0
+4  LowerBack_ANGVEL_y   Gyr   y           LowerBack      deg/s    100.0
+5  LowerBack_ANGVEL_z   Gyr   z           LowerBack      deg/s    100.0
+6  LowerBack_MAGN_x     Mag   x           LowerBack      µT       100.0
+7  LowerBack_MAGN_y     Mag   y           LowerBack      µT       100.0
+8  LowerBack_MAGN_z     Mag   z           LowerBack      µT       100.0
+9  LowerBack_BARO_n/a   Bar   n/a         LowerBack      hPa      100.0,
+}
 ```
 
-> [!NOTE]  
-> In the examples you find a [tutorial (the basics of NGMT)](https://neurogeriatricskiel.github.io/NGMT/00_tutorial_basics/) that explains the basics of the dataclass and how to work with them.
+!!! note
+
+    In the examples you find a [tutorial (the basics of NGMT)](https://neurogeriatricskiel.github.io/NGMT/examples/00_tutorial_basics/) that explains the basics of the dataclass and how to work with them.
 
-## Documentation
-The full documentation can be found [here](https://neurogeriatricskiel.github.io/NGMT/).
 
 ## Installation
 The toolbox has been released on [pypi](https://pypi.org/project/ngmt/) and can be installed via pip:
 ```bash
 pip install ngmt
 ```
 It requires Python 3.10 or higher.
 
 ## Authors
 
 [Masoud Abedinifar](https://github.com/masoudabedinifar), [Julius Welzel](https://github.com/JuliusWelzel), [Walter Maetzler](mailto:w.maetzler@neurologie.uni-kiel.de), [Clint Hansen](mailto:c.hansen@neurologie.uni-kiel.de) & [Robbin Romijnders](https://github.com/rmndrs89)
+
+![NeurogeriatricsLogo](ng_logo.png)
```

### Comparing `ngmt-0.0.3/PKG-INFO` & `ngmt-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ngmt
-Version: 0.0.3
+Version: 0.0.4
 Summary: The NeuroGeriatricMotionToolbox (NGMT) is a Python-based toolbox for processing motion data.
 Home-page: https://neurogeriatricskiel.github.io/NGMT/
 License: MIT
 Author: Masoud Abedinifar
 Author-email: Masoud.Abedinifar@uksh.de
 Maintainer: Masoud Abedinifar
 Maintainer-email: Masoud.Abedinifar@uksh.de
-Requires-Python: >=3.9.0,<3.13
+Requires-Python: >=3.10.0,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Requires-Dist: actipy (>=3.0.5,<4.0.0)
+Requires-Dist: bids-validator (>=1.14.4,<2.0.0)
 Requires-Dist: h5py (>=3.10.0,<4.0.0)
 Requires-Dist: ipykernel (>=6.26.0,<7.0.0)
 Requires-Dist: json-repair (>=0.8.0,<0.9.0)
 Requires-Dist: matplotlib (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.25)
 Requires-Dist: pandas (>=2)
 Requires-Dist: polars (>=0.20.5,<0.21.0)
@@ -36,52 +37,62 @@
 
 [![codecov](https://codecov.io/gh/neurogeriatricskiel/NGMT/graph/badge.svg?token=L578RHZ699)](https://codecov.io/gh/neurogeriatricskiel/NGMT)
 [![build docs](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/mkdocs.yml/badge.svg)](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/mkdocs.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![GitHub issues](https://img.shields.io/github/issues-raw/neurogeriatricskiel/NGMT)
 ![GitHub contributors](https://img.shields.io/github/contributors/neurogeriatricskiel/NGMT)
 [![lint-and-test](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/test-and-lint.yml/badge.svg)](https://github.com/neurogeriatricskiel/NGMT/actions/workflows/test-and-lint.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ngmt)
 
-# NGMT
-![NeurogeriatricsLogo](ng_logo.png)
+
+![NGMTLogo](ngmt_logo_transBG.png)
 
 Welcome to the NeuroGeriatricMotionToolbox (NGMT). We are a Python based toolbox for processing motion data.
 
-> The toolbox is currently under development and is not yet ready for use.
+!!! warning
+
+    The toolbox is currently under development and is not yet ready for use.
 
-The toolbox is aimed at a wide variety of motion researchers who want to use open souce software to process their data.
-We have implemented a wide variety of functions to process motion data, such as:
--   Gait sequence detection (GSD)
--   Inital contact detection (ICD)
--   More to follow ...
 
-The idea is that various motion data can be loaded into our dedicated dataclasses which rely on principles from the [Motion-BIDS](https://bids-specification.readthedocs.io/en/latest/modality-specific-files/motion.html) standard.
+The toolbox is aimed at motion researchers who want to use python based open source software to process their data.
+We have implemented validated algorithms in modules to process motion data, such as:
+   - Gait sequence detection (GSD)
+   - Inital contact detection (ICD)
+   - Physical activity monitoring (PAM)
+   - Postural transition detection (SSD)
+   - More to follow ...
+
+The idea is that various motion data can be loaded into our dedicated dataclass which rely on principles from the [Motion-BIDS](https://bids-specification.readthedocs.io/en/latest/modality-specific-files/motion.html) standard.
 
 ## Data classes
 ### Data classes: conceptual framework
 
 Motion data is recorded with many different systems and modalities, each with their own proprietary data format. NGMT deals with this by organizing both data and metadata in a [BIDS-like format](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html). The BIDS format suggests that [motion recording data](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html#motion-recording-data) from a single tracking system is organized in a single `*_tracksys-<label>_motion.tsv` file. 
 
-> [!NOTE]  
-> A tracking system is defined as a group of motion channels that share hardware properties (the recording device) and software properties (the recording duration and number of samples).
+!!! note
+
+    A tracking system is defined as a group of motion channels that share hardware properties (the recording device) and software properties (the recording duration and number of samples).
 
 In NGMT, data from a single tracking system is therefore loaded into a single `pandas.DataFrame`. The column headers of this `pandas.DataFrame` refer to the channels, and the corresponding [channels information](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/motion.html#channels-description-_channelstsv) is likewise available as a `pandas.DataFrame`.
 
-Similarly, if any [events](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/task-events.html) are available for the given recording, these are loaded into a single `pandas.DataFrame` for each tracking system as well.
+Similarly, if any [events](https://bids-specification.readthedocs.io/en/stable/modality-specific-files/task-events.html) are available for the given recording, these are loaded into a single `pandas.DataFrame` for each tracking system as well. The events derived from the toolbox can be exported to a BIDS like '*_events.tsv' file.
 
 ### Data classes: in practice
 These concepts are translated into a NGMT dataclass for each recording: `NGMTRecording`:
 ```mermaid
 classDiagram
    class NGMTRecording {
       data: dict[str, pd.DataFrame]
       channels: dict[str, pd.DataFrame]
       info: None | dict[str, Any] = None
       events: None | dict[str, pd.DataFrame] = None
       events_info: None | dict[str, Any] = None
+      add_events(tracking_system, new_events)
+      add_info(key, value)
+      export_events(file_path, tracking_system=None, file_name=None, bids_compatible_fname=False)
    }
 
 ```
  A recording consists of the motion data from one or more tracking systems, where each tracking system may consist motion data from one or more tracked points. Therefore, the motion data (`NGMTRecording.data`) are organized as a dictionary where the dictionary keys refer to the tracking systems, and the corresponding values the actual (raw) data as a `pandas.DataFrame`. The description of data channels (`NGMTRecording.channels`) is availabe as a dictionary with the same keys, and the values contain the channels description.
 ```python
 >>> from ngmt.datasets import mobilised
 >>> file_name = "/mnt/neurogeriatrics_data/Mobilise-D/rawdata/sub-3011/Free-living/data.mat"
@@ -90,55 +101,66 @@
 {'SU':         LowerBack_ACCEL_x  ...  LowerBack_BARO_n/a
 0                0.967784  ...         1011.628100
 1                0.969667  ...         1011.628400
 ...                   ...  ...                 ...
 993022           0.970579  ...         1012.078703
 993023           0.960542  ...         1002.580321
 
-[993024 rows x 10 columns], 'SU_INDIP':         LowerBack_ACCEL_x  ...  LowerBack_MAGN_z
+[993024 rows x 10 columns], 
+
+'SU_INDIP':      LowerBack_ACCEL_x  ... LowerBack_MAGN_z
 0                0.967986  ...         -5.902833
 1                0.963671  ...          9.501037
 ...                   ...  ...               ...
 993022           0.951656  ...        -17.987983
 993023           0.955107  ...        -18.050600
 
-[993024 rows x 9 columns]}
+[993024 rows x 9 columns]
+}
+
 >>> recording.channels
-{'SU':                  name type component tracked_point  units  sampling_frequency
-0   LowerBack_ACCEL_x  Acc         x     LowerBack      g               100.0
-1   LowerBack_ACCEL_y  Acc         y     LowerBack      g               100.0
-2   LowerBack_ACCEL_z  Acc         z     LowerBack      g               100.0
-3  LowerBack_ANGVEL_x  Gyr         x     LowerBack  deg/s               100.0
-4  LowerBack_ANGVEL_y  Gyr         y     LowerBack  deg/s               100.0
-5  LowerBack_ANGVEL_z  Gyr         z     LowerBack  deg/s               100.0
-6    LowerBack_MAGN_x  Mag         x     LowerBack     µT               100.0
-7    LowerBack_MAGN_y  Mag         y     LowerBack     µT               100.0
-8    LowerBack_MAGN_z  Mag         z     LowerBack     µT               100.0
-9  LowerBack_BARO_n/a  Bar       n/a     LowerBack    hPa               100.0, 'SU_INDIP':                  name type component tracked_point  units  sampling_frequency
-0   LowerBack_ACCEL_x  Acc         x     LowerBack      g               100.0
-1   LowerBack_ACCEL_y  Acc         y     LowerBack      g               100.0
-2   LowerBack_ACCEL_z  Acc         z     LowerBack      g               100.0
-3  LowerBack_ANGVEL_x  Gyr         x     LowerBack  deg/s               100.0
-4  LowerBack_ANGVEL_y  Gyr         y     LowerBack  deg/s               100.0
-5  LowerBack_ANGVEL_z  Gyr         z     LowerBack  deg/s               100.0
-6    LowerBack_MAGN_x  Mag         x     LowerBack     µT               100.0
-7    LowerBack_MAGN_y  Mag         y     LowerBack     µT               100.0
-8    LowerBack_MAGN_z  Mag         z     LowerBack     µT               100.0}
+{'SU':                  
+   name                 type  component   tracked_point  units    sampling_frequency
+0  LowerBack_ACCEL_x    Acc   x           LowerBack      g        100.0
+1  LowerBack_ACCEL_y    Acc   y           LowerBack      g        100.0
+2  LowerBack_ACCEL_z    Acc   z           LowerBack      g        100.0
+3  LowerBack_ANGVEL_x   Gyr   x           LowerBack      deg/s    100.0
+4  LowerBack_ANGVEL_y   Gyr   y           LowerBack      deg/s    100.0
+5  LowerBack_ANGVEL_z   Gyr   z           LowerBack      deg/s    100.0
+6  LowerBack_MAGN_x     Mag   x           LowerBack      µT       100.0
+7  LowerBack_MAGN_y     Mag   y           LowerBack      µT       100.0
+8  LowerBack_MAGN_z     Mag   z           LowerBack      µT       100.0
+9  LowerBack_BARO_n/a   Bar   n/a         LowerBack      hPa      100.0, 
+
+'SU_INDIP':
+   name                 type  component   tracked_point  units    sampling_frequency
+0  LowerBack_ACCEL_x    Acc   x           LowerBack      g        100.0
+1  LowerBack_ACCEL_y    Acc   y           LowerBack      g        100.0
+2  LowerBack_ACCEL_z    Acc   z           LowerBack      g        100.0
+3  LowerBack_ANGVEL_x   Gyr   x           LowerBack      deg/s    100.0
+4  LowerBack_ANGVEL_y   Gyr   y           LowerBack      deg/s    100.0
+5  LowerBack_ANGVEL_z   Gyr   z           LowerBack      deg/s    100.0
+6  LowerBack_MAGN_x     Mag   x           LowerBack      µT       100.0
+7  LowerBack_MAGN_y     Mag   y           LowerBack      µT       100.0
+8  LowerBack_MAGN_z     Mag   z           LowerBack      µT       100.0
+9  LowerBack_BARO_n/a   Bar   n/a         LowerBack      hPa      100.0,
+}
 ```
 
-> [!NOTE]  
-> In the examples you find a [tutorial (the basics of NGMT)](https://neurogeriatricskiel.github.io/NGMT/00_tutorial_basics/) that explains the basics of the dataclass and how to work with them.
+!!! note
+
+    In the examples you find a [tutorial (the basics of NGMT)](https://neurogeriatricskiel.github.io/NGMT/examples/00_tutorial_basics/) that explains the basics of the dataclass and how to work with them.
 
-## Documentation
-The full documentation can be found [here](https://neurogeriatricskiel.github.io/NGMT/).
 
 ## Installation
 The toolbox has been released on [pypi](https://pypi.org/project/ngmt/) and can be installed via pip:
 ```bash
 pip install ngmt
 ```
 It requires Python 3.10 or higher.
 
 ## Authors
 
 [Masoud Abedinifar](https://github.com/masoudabedinifar), [Julius Welzel](https://github.com/JuliusWelzel), [Walter Maetzler](mailto:w.maetzler@neurologie.uni-kiel.de), [Clint Hansen](mailto:c.hansen@neurologie.uni-kiel.de) & [Robbin Romijnders](https://github.com/rmndrs89)
 
+![NeurogeriatricsLogo](ng_logo.png)
+
```

