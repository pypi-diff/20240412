# Comparing `tmp/actipy-3.0.5.tar.gz` & `tmp/actipy-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-3.0.5.tar", last modified: Fri Dec 29 13:05:16 2023, max compression
+gzip compressed data, was "actipy-3.0.6.tar", last modified: Fri Apr 12 06:14:33 2024, max compression
```

## Comparing `actipy-3.0.5.tar` & `actipy-3.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:05:16.453636 actipy-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2023-12-29 13:04:35.000000 actipy-3.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-29 13:04:35.000000 actipy-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-12-29 13:05:16.453636 actipy-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-29 13:04:35.000000 actipy-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2023-12-29 13:04:35.000000 actipy-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 13:05:16.453636 actipy-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-12-29 13:04:35.000000 actipy-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:05:16.449635 actipy-3.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:05:16.453636 actipy-3.0.5/src/actipy/
--rw-r--r--   0 runner    (1001) docker     (127)    12407 2023-12-29 13:04:39.000000 actipy-3.0.5/src/actipy/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (127)    32239 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2023-12-29 13:04:39.000000 actipy-3.0.5/src/actipy/AxivityReader$BlockParser.class
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2023-12-29 13:04:39.000000 actipy-3.0.5/src/actipy/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-29 13:04:39.000000 actipy-3.0.5/src/actipy/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (127)    10962 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (127)     8748 2023-12-29 13:04:39.000000 actipy-3.0.5/src/actipy/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-29 13:05:16.453636 actipy-3.0.5/src/actipy/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22147 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13690 2023-12-29 13:04:35.000000 actipy-3.0.5/src/actipy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 13:05:16.453636 actipy-3.0.5/src/actipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-12-29 13:05:16.000000 actipy-3.0.5/src/actipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-29 13:05:16.000000 actipy-3.0.5/src/actipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 13:05:16.000000 actipy-3.0.5/src/actipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2023-12-29 13:05:16.000000 actipy-3.0.5/src/actipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-29 13:05:16.000000 actipy-3.0.5/src/actipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2023-12-29 13:04:35.000000 actipy-3.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:14:33.510337 actipy-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-12 06:14:16.000000 actipy-3.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 06:14:16.000000 actipy-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-12 06:14:33.510337 actipy-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-12 06:14:16.000000 actipy-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-04-12 06:14:16.000000 actipy-3.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:14:33.510337 actipy-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-12 06:14:16.000000 actipy-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:14:33.506337 actipy-3.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:14:33.510337 actipy-3.0.6/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-12 06:14:20.000000 actipy-3.0.6/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (127)    32112 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-12 06:14:20.000000 actipy-3.0.6/src/actipy/AxivityReader$BlockParser.class
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-12 06:14:20.000000 actipy-3.0.6/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-12 06:14:20.000000 actipy-3.0.6/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-12 06:14:20.000000 actipy-3.0.6/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 06:14:33.510337 actipy-3.0.6/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22153 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13690 2024-04-12 06:14:16.000000 actipy-3.0.6/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:14:33.510337 actipy-3.0.6/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-12 06:14:33.000000 actipy-3.0.6/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 06:14:33.000000 actipy-3.0.6/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:14:33.000000 actipy-3.0.6/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-12 06:14:33.000000 actipy-3.0.6/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 06:14:33.000000 actipy-3.0.6/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-12 06:14:16.000000 actipy-3.0.6/versioneer.py
```

### Comparing `actipy-3.0.5/LICENSE.md` & `actipy-3.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/PKG-INFO` & `actipy-3.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-3.0.5/README.md` & `actipy-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/pyproject.toml` & `actipy-3.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/setup.py` & `actipy-3.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/ActigraphReader.class` & `actipy-3.0.6/src/actipy/ActigraphReader.class`

 * *Files 11% similar despite different names*

#### procyon -ec {}

```diff
@@ -281,21 +281,20 @@
                 if (++n6 == 9) {
                     accelPair = readAccelPair(array, n3);
                     i = 2;
                 }
                 while (i > 0) {
                     --i;
                     n6 = 0;
-                    final long n7 = Math.round(1000.0 * n5 / n2) + n4;
-                    final double n8 = accelPair[3 - i * 3];
-                    final double n9 = accelPair[4 - i * 3];
-                    final double n10 = accelPair[5 - i * 3];
-                    final long trueUnixTime = getTrueUnixTime(n7, s);
+                    final long duration = Math.round(1000.0 * n5 / n2) + n4;
+                    final double n7 = accelPair[3 - i * 3];
+                    final double n8 = accelPair[4 - i * 3];
+                    final double n9 = accelPair[5 - i * 3];
                     try {
-                        npyWriter.write((Map)toItems(TimeUnit.MILLISECONDS.toNanos(trueUnixTime), n8, n9, n10));
+                        npyWriter.write((Map)toItems(TimeUnit.MILLISECONDS.toNanos(duration), n7, n8, n9));
                     }
                     catch (final Exception ex) {
                         System.err.println("Line write error: " + ex.toString());
                     }
                     ++n5;
                 }
             }
@@ -334,18 +333,18 @@
                     }
                     if (n10 > 2047) {
                         n10 += 61440;
                     }
                     array[j] = (short)n10 / n6;
                     array[j] = Math.round(array[j] * 1000.0) / 1000.0;
                 }
+                final long duration = Math.round(1000.0 * n8 / n) + n2 * 1000L;
                 ++n8;
-                final long trueUnixTime = getTrueUnixTime(Math.round(1000.0 * n8 / n) + n2 * 1000L, s);
                 try {
-                    npyWriter.write((Map)toItems(trueUnixTime, array[1], array[0], array[2]));
+                    npyWriter.write((Map)toItems(TimeUnit.MILLISECONDS.toNanos(duration), array[1], array[0], array[2]));
                 }
                 catch (final Exception ex) {
                     System.err.println("Line write error: " + ex.toString());
                 }
             }
         }
         catch (final IOException ex2) {
@@ -380,18 +379,18 @@
                     b = (byte)inputStream.read();
                     n4 ^= b;
                     final int n9 = n8 | (b & 0xFF) << 8;
                     i += 2;
                     array[j] = (short)n9 / n6;
                     array[j] = Math.round(array[j] * 1000.0) / 1000.0;
                 }
+                final long duration = Math.round(1000.0 * n7 / n) + n2 * 1000L;
                 ++n7;
-                final long trueUnixTime = getTrueUnixTime(Math.round(1000.0 * n7 / n) + n2 * 1000L, s);
                 try {
-                    npyWriter.write((Map)toItems(trueUnixTime, array[0], array[1], array[2]));
+                    npyWriter.write((Map)toItems(TimeUnit.MILLISECONDS.toNanos(duration), array[0], array[1], array[2]));
                 }
                 catch (final Exception ex) {
                     System.err.println("Line write error: " + ex.toString());
                 }
             }
         }
         catch (final IOException ex2) {
```

### Comparing `actipy-3.0.5/src/actipy/ActigraphReader.java` & `actipy-3.0.6/src/actipy/ActigraphReader.java`

 * *Files 2% similar despite different names*

```diff
@@ -433,15 +433,14 @@
                     i=0;
 
                     long t = Math.round((1000d*samples)/sampleRate) + firstSampleTime;
                     double x = twoSamples[3-twoSampleCounter*3];
                     double y = twoSamples[4-twoSampleCounter*3];
                     double z = twoSamples[5-twoSampleCounter*3];
                     // double temp = 1.0d; // don't know temp yet
-                    t = getTrueUnixTime(t, infoTimeShift);
 
                     try {
                         writer.write(toItems(TimeUnit.MILLISECONDS.toNanos(t), x, y, z));
                     } catch (Exception e) {
                         System.err.println("Line write error: " + e.toString());
                     }
 
@@ -508,21 +507,21 @@
                     sample[axis] = axis_val / accelerationScale;
                     sample[axis] = (double) Math.round(sample[axis] * 1000d) / 1000d; // round to 3rd decimal
                 }
                 // logger.log(Level.FINER, "i: " + i);
                 // logger.log(Level.FINER, "x y z: " + sample[1] + " " + sample[0] + " " + sample[2]);
 
                 // double temp = 1.0d; // don't know temp yet
-                samples += 1;
                 long myTime = Math.round((1000d*samples)/sampleRate) + firstSampleTime*1000; // in Miliseconds
-                myTime = getTrueUnixTime(myTime, infoTimeShift);
+                samples += 1;
+
 
                 // Yes, sample[1] and sample[0] are swapped. Not the case elsewhere.
                 try {
-                    writer.write(toItems(myTime, sample[1], sample[0], sample[2]));
+                    writer.write(toItems(TimeUnit.MILLISECONDS.toNanos(myTime), sample[1], sample[0], sample[2]));
                 } catch (Exception e) {
                     System.err.println("Line write error: " + e.toString());
                 }
 
             }
         } catch (IOException ex) {
             ex.printStackTrace(System.err);
@@ -582,24 +581,22 @@
                     axis_val = (short) shifter;
 
                     sample[axis] = axis_val / accelerationScale;
                     sample[axis] = (double) Math.round(sample[axis] * 1000d) / 1000d; // round to 3rd decimal
                 }
 
                 // double temp = 1.0d; // don't know temp yet
-                samples += 1;
-
                 long myTime = Math.round((1000d*samples)/sampleRate) + firstSampleTime*1000; // in Miliseconds
-                myTime = getTrueUnixTime(myTime, infoTimeShift);
+                samples += 1;
 
                 // logger.log(Level.FINER, "i: " + i + "\nx y z: " + sample[0] + " " + sample[1] + " " + sample[2] +
                 //         "\nTime:" + myTime);
 
                 try {
-                    writer.write(toItems(myTime, sample[0], sample[1], sample[2]));
+                    writer.write(toItems(TimeUnit.MILLISECONDS.toNanos(myTime), sample[0], sample[1], sample[2]));
                 } catch (Exception e) {
                     System.err.println("Line write error: " + e.toString());
                 }
 
             }
         } catch (IOException ex) {
             ex.printStackTrace(System.err);
```

### Comparing `actipy-3.0.5/src/actipy/AxivityReader$BlockParser.class` & `actipy-3.0.6/src/actipy/AxivityReader$BlockParser.class`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/AxivityReader.class` & `actipy-3.0.6/src/actipy/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/AxivityReader.java` & `actipy-3.0.6/src/actipy/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/GENEActivReader.class` & `actipy-3.0.6/src/actipy/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/GENEActivReader.java` & `actipy-3.0.6/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/NpyWriter.class` & `actipy-3.0.6/src/actipy/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/NpyWriter.java` & `actipy-3.0.6/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy/processing.py` & `actipy-3.0.6/src/actipy/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     :param data: A pandas.DataFrame of acceleration time-series. The index must be a DateTimeIndex.
     :type data: pandas.DataFrame.
     :param sample_rate: Target sample rate (Hz) to achieve.
     :type sample_rate: int or float
     :param dropna: Whether to drop NaN values after resampling. Defaults to False.
     :type dropna: bool, optional
-    :param chunksize: Chunk size. Defaults to 1_000_000.
+    :param chunksize: Chunk size for chunked processing. Defaults to 1_000_000 rows.
     :type chunksize: int, optional
     :return: Processed data and processing info.
     :rtype: (pandas.DataFrame, dict)
     """
 
     info = {}
 
@@ -95,15 +95,15 @@
 
     :param data: A pandas.DataFrame of acceleration time-series. The index must be a DateTimeIndex.
     :type data: pandas.DataFrame.
     :param data_sample_rate: The data's original sample rate.
     :type data_sample_rate: int or float
     :param cutoff_rate: Cutoff (Hz) for low-pass filter. Defaults to 20.
     :type cutoff_rate: int, optional
-    :param chunksize: Chunk size. Defaults to 1_000_000.
+    :param chunksize: Chunk size for chunked processing. Defaults to 1_000_000 rows.
     :type chunksize: int, optional
     :return: Processed data and processing info.
     :rtype: (pandas.DataFrame, dict)
     """
 
     info = {}
 
@@ -165,26 +165,22 @@
     return data, info
 
 
 def detect_nonwear(data, patience='90m', window='10s', stdtol=15 / 1000):
     """
     Detect nonwear episodes based on long periods of no movement.
 
-    :param data: A pandas.DataFrame of acceleration time-series. The index must be a DateTimeIndex.
+    :param pandas.DataFrame data: A pandas.DataFrame of acceleration time-series. The index must be a DateTimeIndex.
     :type data: pandas.DataFrame.
-    :param patience: Minimum length of the stationary period to be flagged as
-        non-wear. Defaults to 90 minutes ("90m").
+    :param patience: Minimum length of the stationary period to be flagged as non-wear. Defaults to 90 minutes ("90m").
     :type patience: str, optional
-    :param stationary_indicator: A boolean pandas.Series indexed as `data`
-        indicating stationary (low movement) periods. If None, it will be
-        automatically inferred. Defaults to None.
-    :type stationary_indicator: pandas.Series, optional
-    :param drop: Wheter to drop the non-wear periods. If False, the non-wear
-        periods will be filled with NaNs. Defaults to False.
-    :type drop: bool, optional
+    :param window: Rolling window to use to check for stationary periods. Defaults to 10 seconds ("10s").
+    :type window: str, optional
+    :param stdtol: Standard deviation under which the window is considered stationary. Defaults to 15 milligravity (0.015).
+    :type stdtol: float, optional
     :return: Processed data and processing info.
     :rtype: (pandas.DataFrame, dict)
     """
 
     info = {}
 
     stationary_indicator = (  # this is more memory friendly than data[['x', 'y', 'z']].std()
@@ -240,19 +236,19 @@
     :param data: A pandas.DataFrame of acceleration time-series. It must contain
         at least columns `x,y,z` and the index must be a DateTimeIndex.
     :type data: pandas.DataFrame.
     :param calib_cube: Calibration cube criteria. See van Hees et al. 2014 for details. Defaults to 0.3.
     :type calib_cube: float, optional.
     :param calib_min_samples: Minimum number of stationary samples required to run calibration. Defaults to 50.
     :type calib_min_samples: int, optional.
-    :param stationary_indicator: A boolean pandas.Series indexed as `data`
-        indicating stationary (low movement) periods. If None, it will be
-        automatically inferred. Defaults to None.
-    :type stationary_indicator: pandas.Series, optional
-    :param chunksize: Chunk size. Defaults to 1_000_000.
+    :param window: Rolling window to use to check for stationary periods. Defaults to 10 seconds ("10s").
+    :type window: str, optional
+    :param stdtol: Standard deviation under which the window is considered stationary. Defaults to 15 milligravity (0.015).
+    :type stdtol: float, optional
+    :param chunksize: Chunk size for chunked processing. Defaults to 1_000_000 rows.
     :type chunksize: int, optional
     :return: Processed data and processing info.
     :rtype: (pandas.DataFrame, dict)
     """
 
     info = {}
```

### Comparing `actipy-3.0.5/src/actipy/reader.py` & `actipy-3.0.6/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/src/actipy.egg-info/PKG-INFO` & `actipy-3.0.6/src/actipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 3.0.5
+Version: 3.0.6
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-3.0.5/src/actipy.egg-info/SOURCES.txt` & `actipy-3.0.6/src/actipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actipy-3.0.5/versioneer.py` & `actipy-3.0.6/versioneer.py`

 * *Files identical despite different names*

