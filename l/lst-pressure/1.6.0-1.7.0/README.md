# Comparing `tmp/lst-pressure-1.6.0.tar.gz` & `tmp/lst-pressure-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lst-pressure-1.6.0.tar", last modified: Tue Apr  9 12:58:42 2024, max compression
+gzip compressed data, was "lst-pressure-1.7.0.tar", last modified: Fri Apr 12 10:27:39 2024, max compression
```

## Comparing `lst-pressure-1.6.0.tar` & `lst-pressure-1.7.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/cli/apps/AppInterface.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/aggregate/
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/aggregate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/cli/apps/observables/
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/cli/apps/observables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/conf/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/logger/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/lst_pressure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-09 12:58:42.000000 lst-pressure-1.6.0/lst_pressure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.287570 lst-pressure-1.6.0/lstpressure/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lst/
--rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/LST.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lst/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lst/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lstcalendar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/lstindex/
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTInterval.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/lstindex/LSTIntervalType.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/lstindex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/observable/
--rw-r--r--   0 runner    (1001) docker     (127)     6388 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observable/Observable.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/observable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.291570 lst-pressure-1.6.0/lstpressure/observation/
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observation/Observation.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/observation/is_observable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/LocationProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/planets.json
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/sun/location_providers/normalize_intervals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/lstpressure/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/lstpressure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/normalize_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/lstpressure/utils/time_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.295570 lst-pressure-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/lstcalendar/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/lstcalendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendarDate.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/lstcalendar/test_LSTInterval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/observation/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/observation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/observation/test_Observation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/sun/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.303570 lst-pressure-1.6.0/tests/sun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/sun/test_Sun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/test_lib_astral.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/test_lib_meerkat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:58:42.299570 lst-pressure-1.6.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 12:58:42.307570 lst-pressure-1.6.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_normalize_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_normalize_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 12:57:57.000000 lst-pressure-1.6.0/tests/utils/test_time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/cli/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/cli/apps/AppInterface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/cli/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/cli/apps/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/cli/apps/aggregate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/cli/apps/observables/
+-rw-r--r--   0 runner    (1001) docker     (127)    10563 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/cli/apps/observables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/lst_pressure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-12 10:27:39.000000 lst-pressure-1.7.0/lst_pressure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-12 10:27:39.000000 lst-pressure-1.7.0/lst_pressure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:27:39.000000 lst-pressure-1.7.0/lst_pressure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 10:27:39.000000 lst-pressure-1.7.0/lst_pressure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/lstpressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/lstpressure/lst/
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lst/LST.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/lst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/lstpressure/lst/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/lst/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lst/helpers/calculate_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lst/helpers/calculate_observations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.300012 lst-pressure-1.7.0/lstpressure/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lstcalendar/LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lstcalendar/LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/lstcalendar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/lstindex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lstindex/LSTIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lstindex/LSTInterval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/lstindex/LSTIntervalType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/lstindex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/observable/
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/observable/Observable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/observable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/observation/Observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/observation/is_observable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/sun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/sun/location_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/LocationProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/sun/location_providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.308013 lst-pressure-1.7.0/lstpressure/sun/location_providers/astral_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/sun/location_providers/astral_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.312013 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/planets.json
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/sun/location_providers/normalize_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.312013 lst-pressure-1.7.0/lstpressure/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/lstpressure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/utils/normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/utils/normalize_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/lstpressure/utils/time_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.312013 lst-pressure-1.7.0/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.312013 lst-pressure-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/tests/lstcalendar/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/tests/lstcalendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/lstcalendar/test_LSTCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/lstcalendar/test_LSTCalendarDate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/lstcalendar/test_LSTInterval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/tests/observation/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/tests/observation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/observation/test_Observation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/tests/sun/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 10:27:39.320012 lst-pressure-1.7.0/tests/sun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/sun/test_Sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/test_lib_astral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/test_lib_meerkat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:27:39.316012 lst-pressure-1.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 10:27:39.324012 lst-pressure-1.7.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/utils/test_normalize_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/utils/test_normalize_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 10:26:49.000000 lst-pressure-1.7.0/tests/utils/test_time_conversions.py
```

### Comparing `lst-pressure-1.6.0/LICENSE` & `lst-pressure-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/PKG-INFO` & `lst-pressure-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lst-pressure
-Version: 1.6.0
+Version: 1.7.0
 Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
 Home-page: https://github.com/ska-sa/lst-pressure
 Author: Zach Smith
 Author-email: zsmith@sarao.ac.za
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -144,14 +144,17 @@
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
 # ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
 cat observations.csv | lstpressure obs --pretty
 
+# ... By default --pretty will truncate long values. If you want the full output specify --no-trunc
+cat observations.csv | lstpressure obs --pretty --no-trunc
+
 # Get a list of schedulable observations over the next 3 months (including this month)
 cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
 cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
```

### Comparing `lst-pressure-1.6.0/README.md` & `lst-pressure-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,17 @@
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
 # ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
 cat observations.csv | lstpressure obs --pretty
 
+# ... By default --pretty will truncate long values. If you want the full output specify --no-trunc
+cat observations.csv | lstpressure obs --pretty --no-trunc
+
 # Get a list of schedulable observations over the next 3 months (including this month)
 cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
 cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
```

### Comparing `lst-pressure-1.6.0/cli/__init__.py` & `lst-pressure-1.7.0/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,8 @@
         parser.print_help()
         return
 
     # Otherwise execute the application
     app.parse(args).exe()
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/cli/apps/AppInterface.py` & `lst-pressure-1.7.0/cli/apps/AppInterface.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/cli/apps/aggregate/__init__.py` & `lst-pressure-1.7.0/cli/apps/aggregate/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ..AppInterface import AppInterface
 from typing import Self
 import os
 import subprocess
 from logger import error
 import sys
+import csv
+from io import StringIO
 
 
 SQL_FOLDER_PATH = os.path.join(os.path.dirname(__file__), "sql")
 existing_reports = [
     f.replace(".sql", "")
     for f in os.listdir(SQL_FOLDER_PATH)
     if os.path.isfile(os.path.join(SQL_FOLDER_PATH, f))
@@ -42,14 +44,21 @@
             "--pretty",
             required=False,
             default=False,
             action="store_true",
             help=f"Format CSV output using the csvlook tool (included in this CLI)",
         )
         self.parser.add_argument(
+            "--no-trunc",
+            required=False,
+            default=False,
+            action="store_true",
+            help=f"When using --pretty, long values are truncated by default. Disable this behaviour via this flag",
+        )
+        self.parser.add_argument(
             "--echo",
             required=False,
             default=False,
             action="store_true",
             help=f"Echo the aggregation query back - useful for evaluating .sql file contents that would otherwise be opaque. For example: --echo --query {existing_reports[0]}",
         )
 
@@ -57,14 +66,20 @@
 
     def parse(self, args) -> Self:
         self.args = args
         self.echo = args.echo
         self.input = args.input
         self.query = parse_sql_query(args.query)
         self.pretty = args.pretty
+        self.no_trunc = args.no_trunc if args.no_trunc else False
+
+        if self.no_trunc:
+            if not self.pretty:
+                error("--no-trunc is only applicable when --pretty flag is used")
+                exit(1)
 
         if self.echo and self.pretty:
             error("Don't use --pretty and --echo together.")
             exit(1)
 
         return self
 
@@ -82,15 +97,15 @@
                 )
                 exit(1)
         else:
             with open(self.input, "r") as file:
                 input_csv = file.read()
 
         result = execute_csvsql(input_csv, self.query, self.args.query)
-        result = execute_csvlook(result) if self.pretty else result
+        result = execute_csvlook(result, self.no_trunc) if self.pretty else result
 
         # Print result to stdout
         print(result)
         exit()
 
 
 def parse_sql_query(str_input):
@@ -112,43 +127,74 @@
         with open(path + ".sql", "r") as file:
             return file.read().strip()
 
     # If not a file, assume it's a SQL string
     return str_input
 
 
-def execute_csvlook(input_content):
-    csvlook_opts = [
-        "-I",
-        "--null-value",
-        "0",
-    ]
+def truncate_cols_to_max_chars(max_chars, line):
+    # Use StringIO to simulate file I/O which csv.reader expects
+    input_line = StringIO(line)
+    output_line = StringIO()
+    reader = csv.reader(input_line)
+    writer = csv.writer(output_line)
+
+    # Read the line with csv.reader which handles commas, quotes correctly
+    for row in reader:
+        # Truncate each field to max_chars and append ellipsis if truncated
+        truncated_row = [
+            (field[: max_chars - 3] + " ...") if len(field) > max_chars else field
+            for field in row
+        ]
+        # Write the truncated row to the output_line
+        writer.writerow(truncated_row)
 
-    command = ["csvlook", *csvlook_opts]
+    # Get the content of output_line and remove the trailing newline
+    return output_line.getvalue().strip()
 
-    try:
-        # Use subprocess.Popen to run the command
-        process = subprocess.Popen(
-            command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, text=True
-        )
 
-        # Pass input content to the subprocess
-        output, _ = process.communicate(input=input_content)
+def execute_csvlook(input_content, no_trunc=False):
+    csvlook_opts = ["-I", "--null-value", "0"]
+    command = ["csvlook", *csvlook_opts]
 
-        # Wait for the process to finish and get the return code
-        return_code = process.wait()
+    try:
+        # Start the subprocess with pipes for stdin and stdout
+        with subprocess.Popen(
+            command,
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            text=True,
+        ) as process:
+            # Check if input is string and split into lines if necessary
+            if isinstance(input_content, str):
+                input_content = input_content.splitlines()
+
+            # Process each line, writing to stdin and logging
+            for line in input_content:
+                line = truncate_cols_to_max_chars(18, line) if not no_trunc else line
+                process.stdin.write(line + "\n")
+                process.stdin.flush()  # Ensure the line is sent to the process
+
+            # Read the output
+            output, errors = process.communicate()
+
+            # Check for errors
+            if process.returncode != 0:
+                print(
+                    f"csvlook process returned a non-zero exit code: {process.returncode}"
+                )
+                print(f"Errors: {errors}")
+                return None
 
-        if return_code == 0:
             return output
-        else:
-            error(f"csvlook process returned a non-zero exit code: {return_code}")
-            error(f"Command output: {output}")
-            return None
+
     except Exception as e:
-        raise e
+        print(f"An error occurred: {e}")
+        raise
 
 
 def execute_csvsql(input_content, sql, query_name=""):
     duck_opts = (
         [
             "--db",
             "duckdb:///:memory:",
@@ -158,31 +204,34 @@
         else []
     )
 
     command = ["csvsql", "--query", sql, *duck_opts]
 
     try:
         # Use subprocess.Popen to run the command
-        process = subprocess.Popen(
-            command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, text=True
-        )
-
-        # Pass input content to the subprocess
-        output, _ = process.communicate(input=input_content)
+        with subprocess.Popen(
+            command,
+            stdin=subprocess.PIPE,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            text=True,
+        ) as process:
+            # Pass input content to the subprocess
+            output, _ = process.communicate(input=input_content)
 
-        # Wait for the process to finish and get the return code
-        return_code = process.wait()
+            # Wait for the process to finish and get the return code
+            return_code = process.wait()
 
-        if return_code == 0:
-            return output
-        else:
-            error(f"csvsql process returned a non-zero exit code: {return_code}")
-            error(f"Command output: {output}")
-            return None
+            if return_code == 0:
+                return output
+            else:
+                error(f"csvsql process returned a non-zero exit code: {return_code}")
+                error(f"Command output: {output}")
+                return None
     except Exception as e:
         raise e
 
 
 __all__ = ["parse_sql_query", "Aggregate", "execute_csvsql", "execute_csvlook"]
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/cli/apps/observables/__init__.py` & `lst-pressure-1.7.0/cli/apps/observables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,14 +202,22 @@
             "--pretty",
             required=False,
             default=False,
             action="store_true",
             help=f"Format CSV output using the csvlook tool (included in this CLI)",
         )
 
+        self.parser.add_argument(
+            "--no-trunc",
+            required=False,
+            default=False,
+            action="store_true",
+            help=f"When using --pretty, long values are truncated by default. Disable this behaviour via this flag",
+        )
+
         return self
 
     def parse(self, args) -> Self:
         if args.lat or args.long:
             if LocationProviderType[args.loc_provider] == LocationProviderType.MEERKAT:
                 error(
                     "The MEERKAT provider has set lat/long coordinates that can't be overriden. Either use a different loc-provider or don't specify --lat and --long"
@@ -237,14 +245,20 @@
         self.filter_value = (
             None if not filter_name else filter_mapping.get(filter_name.upper(), None)
         )
 
         self.output = args.output if args.output else None
         self.aggregate = args.aggregate if args.aggregate else None
         self.pretty = args.pretty if args.pretty else None
+        self.no_trunc = args.no_trunc if args.no_trunc else False
+
+        if self.no_trunc:
+            if not self.pretty:
+                error("--no-trunc is only applicable when --pretty flag is used")
+                exit(1)
         return self
 
     def exe(self) -> None:
         sql = parse_sql_query(self.aggregate) if self.aggregate else None
 
         def observation_filter(observation: Observation):
             if self.filter_value in observation.utc_constraints:
@@ -274,17 +288,21 @@
 
         output_string = (
             execute_csvsql(output_csv_string, sql, self.aggregate)
             if sql
             else output_csv_string
         )
 
-        output_string = execute_csvlook(output_string) if self.pretty else output_string
+        output_string = (
+            execute_csvlook(output_string, self.no_trunc)
+            if self.pretty
+            else output_string
+        )
 
         if self.output:
             with open(self.output, "w") as f:
                 f.write(output_string)
         else:
             print(output_string)
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/conf/__init__.py` & `lst-pressure-1.7.0/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     def PY_ENV(self, value):
         self._py_env = value
 
 
 __all__ = ["Conf", "LogLevel"]
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/logger/__init__.py` & `lst-pressure-1.7.0/logger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 def error(*args, **kwargs):
     print("ERROR", *args, **kwargs, file=sys.stderr)
 
 
 __all__ = ["debug", "info", "warn", "error"]
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/lst_pressure.egg-info/PKG-INFO` & `lst-pressure-1.7.0/lst_pressure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lst-pressure
-Version: 1.6.0
+Version: 1.7.0
 Summary: Determine periods of "LST pressure" by querying for intersections between LST/Solar intervals
 Home-page: https://github.com/ska-sa/lst-pressure
 Author: Zach Smith
 Author-email: zsmith@sarao.ac.za
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -144,14 +144,17 @@
 
 # Get a list of today's schedulable observations
 cat observations.csv | lstpressure obs
 
 # ... And format the result nicely using csvlook. It's hard to imaging using this tool without --pretty. To use csvlook with custom args, just omit the --pretty flag
 cat observations.csv | lstpressure obs --pretty
 
+# ... By default --pretty will truncate long values. If you want the full output specify --no-trunc
+cat observations.csv | lstpressure obs --pretty --no-trunc
+
 # Get a list of schedulable observations over the next 3 months (including this month)
 cat observations.csv | lstpressure obs --end="+2M" --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months
 cat observations.csv | lstpressure obs --end="+2M" --filter night --pretty
 
 # Get a list of schedulable NIGHT observations over the next 3 months, aggregated by opportunities per month
```

### Comparing `lst-pressure-1.6.0/lst_pressure.egg-info/SOURCES.txt` & `lst-pressure-1.7.0/lst_pressure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/__init__.py` & `lst-pressure-1.7.0/lstpressure/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,8 @@
     "Sun",
     "utils",
     "LSTConf",
     "LocationProviderType",
 ]
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/lstpressure/lst/LST.py` & `lst-pressure-1.7.0/lstpressure/lst/LST.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 lstpressure.lst.LST
 """
+
 import pandas as pd
 from pandas import DataFrame
 from datetime import datetime
 from typing import Optional, Callable
 from ..observation import Observation
 from ..observable import Observable
 from .helpers import calculate_observations, calculate_observables
 from collections import defaultdict
 from io import StringIO
 from perf import track_total_runtime, decorate_all
 from conf import Conf, LogLevel, LocationProviderType
 from logger import info, warn
+import json
 
 conf = Conf()
 
 
 @decorate_all(track_total_runtime)
 class LST:
     """
@@ -253,27 +255,33 @@
         for record in data:
             (
                 id,
                 proposal_id,
                 date,
                 constraint,
                 duration,
+                tags,
+                preferred_dates,
+                avoid_dates,
                 lst_window_start,
                 lst_window_end,
                 lst_interval_start,
                 lst_interval_end,
                 utc_interval_start,
                 utc_interval_end,
             ) = record
             grouped_data[date].append(
                 [
                     id,
                     proposal_id,
                     constraint,
                     duration,
+                    tags,
+                    preferred_dates,
+                    avoid_dates,
                     lst_window_start,
                     lst_window_end,
                     lst_interval_start,
                     lst_interval_end,
                     utc_interval_start,
                     utc_interval_end,
                 ]
@@ -289,17 +297,22 @@
                 "Duration": duration,
                 "Observation window start (LST)": lst_window_start,
                 "Observation window end (LST)": lst_window_end,
                 "Interval start (LST)": lst_interval_start,
                 "Interval end (LST)": lst_interval_end,
                 "Interval start (UTC)": utc_interval_start,
                 "Interval end (UTC)": utc_interval_end,
+                "Tags": json.dumps(tags) if len(tags) else None,
+                "Preferred dates": json.dumps(preferred_dates)
+                if len(preferred_dates)
+                else None,
+                "Avoid dates": json.dumps(avoid_dates) if len(avoid_dates) else None,
             }
             for date, id_value in grouped_data.items()
-            for id, proposal_id, constraint, duration, lst_window_start, lst_window_end, lst_interval_start, lst_interval_end, utc_interval_start, utc_interval_end in id_value
+            for id, proposal_id, constraint, duration, tags, preferred_dates, avoid_dates, lst_window_start, lst_window_end, lst_interval_start, lst_interval_end, utc_interval_start, utc_interval_end in id_value
         ]
 
         # Construct the DataFrame
         df = pd.DataFrame(data_list)
         return df
 
     def to_csv_buffer(self) -> StringIO:
```

### Comparing `lst-pressure-1.6.0/lstpressure/lst/helpers/calculate_observables.py` & `lst-pressure-1.7.0/lstpressure/lst/helpers/calculate_observables.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendar.py` & `lst-pressure-1.7.0/lstpressure/lstcalendar/LSTCalendar.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/lstcalendar/LSTCalendarDate.py` & `lst-pressure-1.7.0/lstpressure/lstcalendar/LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/lstindex/LSTIndex.py` & `lst-pressure-1.7.0/lstpressure/lstindex/LSTIndex.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/lstindex/LSTInterval.py` & `lst-pressure-1.7.0/lstpressure/lstindex/LSTInterval.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/lstindex/LSTIntervalType.py` & `lst-pressure-1.7.0/lstpressure/lstindex/LSTIntervalType.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/observable/Observable.py` & `lst-pressure-1.7.0/lstpressure/observable/Observable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 observable.Observable
 """
+
 from datetime import datetime
 from typing import Any, Self
 from ..observation import Observation
 from ..lstindex import LSTInterval, LSTIntervalType
 from perf import track_total_runtime, decorate_all
 
 
@@ -90,14 +91,44 @@
 
         Returns:
             float: The duration of the observation in hours.
         """
         return self.observation.duration
 
     @property
+    def tags(self) -> list[str]:
+        """
+        Returns the observation tags
+
+        Returns:
+            list[str]: List of observation tags
+        """
+        return self.observation.tags
+
+    @property
+    def preferred_dates(self) -> list:
+        """
+        Returns the user-specified preferred dates of their observation block
+
+        Returns:
+            list: List of preferred dates
+        """
+        return self.observation.preferred_dates
+
+    @property
+    def avoid_dates(self) -> list:
+        """
+        Returns the user-specified dates to avoid when scheduling their observation block
+
+        Returns:
+            list: List of dates to avoid
+        """
+        return self.observation.avoid_dates
+
+    @property
     def utc_constraint(self) -> LSTIntervalType:
         """
         Returns the UTC constraint type of the observation interval.
 
         Returns:
             LSTIntervalType: The UTC constraint type of the interval.
         """
@@ -118,37 +149,52 @@
 
         return (
             self.id,
             self.proposal_id,
             self.dt.strftime("%Y-%m-%d"),
             self.utc_constraint,
             round(self.duration, 2),
+            self.tags,
+            self.preferred_dates,
+            self.avoid_dates,
             self.observation.lst_window_start,
             self.observation.lst_window_end,
             round(self.interval.start, 2),
             round(lst_window_end, 2),
             self.interval.start_utc,
             self.interval.end_utc,
         )
 
     def __lt__(self, other) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
-        return (self.id, self.dt, self.utc_constraint, self.duration, self.interval.start) < (
+        return (
+            self.id,
+            self.dt,
+            self.utc_constraint,
+            self.duration,
+            self.interval.start,
+        ) < (
             other.id,
             other.dt,
             other.utc_constraint,
             other.duration,
             other.interval.start,
         )
 
     def __le__(self, other) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
-        return (self.id, self.dt, self.utc_constraint, self.duration, self.interval.start) <= (
+        return (
+            self.id,
+            self.dt,
+            self.utc_constraint,
+            self.duration,
+            self.interval.start,
+        ) <= (
             other.id,
             other.dt,
             other.utc_constraint,
             other.duration,
             other.interval.start,
         )
 
@@ -170,39 +216,54 @@
             other.interval.end,
             other.observation.id,
         )
 
     def __ge__(self, other) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
-        return (self.id, self.dt, self.utc_constraint, self.duration, self.interval.start) >= (
+        return (
+            self.id,
+            self.dt,
+            self.utc_constraint,
+            self.duration,
+            self.interval.start,
+        ) >= (
             other.id,
             other.dt,
             other.utc_constraint,
             other.duration,
             other.interval.start,
         )
 
     def __gt__(self, other) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
-        return (self.id, self.dt, self.utc_constraint, self.duration, self.interval.start) > (
+        return (
+            self.id,
+            self.dt,
+            self.utc_constraint,
+            self.duration,
+            self.interval.start,
+        ) > (
             other.id,
             other.dt,
             other.utc_constraint,
             other.duration,
             other.interval.start,
         )
 
     def __hash__(self) -> int:
         return hash(
             (
                 self.interval.dt,
                 self.utc_constraint,
                 self.duration,
+                "".join(self.tags),
+                "".join(["".join(d) for d in self.preferred_dates]),
+                "".join(["".join(d) for d in self.avoid_dates]),
                 self.interval.start,
                 self.interval.end,
                 self.observation.id,
             )
         )
 
     def __str__(self) -> int:
```

### Comparing `lst-pressure-1.6.0/lstpressure/observation/Observation.py` & `lst-pressure-1.7.0/lstpressure/observation/Observation.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,17 @@
         self,
         id: any,
         lst_window_start: float,
         lst_window_end: float,
         utc_constraints: LSTIntervalType | list[LSTIntervalType] = None,
         duration: float = None,
         proposal_id: str = None,
+        tags: list[str] = None,
+        preferred_dates: list = None,
+        avoid_dates: list = None,
     ) -> None:
         """
         Initializes an instance of Block.
 
         Parameters
         ----------
         id: any
@@ -59,14 +62,17 @@
                     if utc_constraints and isinstance(utc_constraints, list)
                     else [utc_constraints]
                 ),
             )
         )
         self.proposal_id = proposal_id
         self._duration = duration if duration else 0
+        self._tags = tags if tags else []
+        self._preferred_dates = preferred_dates if preferred_dates else []
+        self._avoid_dates = avoid_dates if avoid_dates else []
         self._cal: Optional[LSTCalendar] = None  # Reference to the calendar
         self._intervals = []
         self._intervals.append(
             LSTInterval(
                 *normalize_interval(self.lst_window_start, self.lst_window_end),
                 None,
                 None,
@@ -83,14 +89,35 @@
     def duration(self) -> float:
         """
         Required observation duration in hours (decimal)
         """
         return self._duration
 
     @property
+    def tags(self) -> list[str]:
+        """
+        List of tags associated with an observation
+        """
+        return self._tags
+
+    @property
+    def preferred_dates(self) -> list:
+        """
+        List of preferred dates of an observation
+        """
+        return self._preferred_dates
+
+    @property
+    def avoid_dates(self) -> list:
+        """
+        List of dates to avoid for an observation
+        """
+        return self._avoid_dates
+
+    @property
     def intervals(self) -> list[LSTInterval]:
         return self._intervals
 
     @property
     def calendar(self) -> LSTCalendar:
         if not self._cal:
             raise ValueError("Block has not been added to any LSTCalendar.")
```

### Comparing `lst-pressure-1.6.0/lstpressure/observation/is_observable.py` & `lst-pressure-1.7.0/lstpressure/observation/is_observable.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/Sun.py` & `lst-pressure-1.7.0/lstpressure/sun/Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py` & `lst-pressure-1.7.0/lstpressure/sun/location_providers/astral_provider/AstralProvider.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py` & `lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/AstroUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py` & `lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/DateTimeUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py` & `lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/MeerKATProvider.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py` & `lst-pressure-1.7.0/lstpressure/sun/location_providers/meerkat_provider/SolarSystemUtils.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/utils/normalize_coordinates.py` & `lst-pressure-1.7.0/lstpressure/utils/normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/utils/normalize_date.py` & `lst-pressure-1.7.0/lstpressure/utils/normalize_date.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/lstpressure/utils/time_conversions.py` & `lst-pressure-1.7.0/lstpressure/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/perf/__init__.py` & `lst-pressure-1.7.0/perf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,8 +106,8 @@
 
     return decorate
 
 
 __all__ = ["monitor_perf", "track_total_runtime", "decorate_all"]
 
 # Automatically added by katversion
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `lst-pressure-1.6.0/setup.py` & `lst-pressure-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendar.py` & `lst-pressure-1.7.0/tests/lstcalendar/test_LSTCalendar.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/lstcalendar/test_LSTCalendarDate.py` & `lst-pressure-1.7.0/tests/lstcalendar/test_LSTCalendarDate.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/lstcalendar/test_LSTInterval.py` & `lst-pressure-1.7.0/tests/lstcalendar/test_LSTInterval.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/sun/test_Sun.py` & `lst-pressure-1.7.0/tests/sun/test_Sun.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/test_lib_astral.py` & `lst-pressure-1.7.0/tests/test_lib_astral.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from conf import LocationProviderType
 
 # 20231030 LST dusk is about 2130
 
 tests = [
     # (lst_window_start, lst_window_end, utc_constraints, duration, dt_range, observables_count)
     (8, 20, [I.NIGHT], 2, ["20231030"], 0),
-    (8, 20, [], 2, ["20231030"], 2),
+    (8, 20, [], 2, ["20231030"], 3),
     (2, 20, [I.NIGHT], 0.5, ["20231030"], 1),
     (20, 1, [I.NIGHT], 2, ["20231030"], 2),
     (20, 1, [I.NIGHT], 2, ["20231030", "20231031"], 4),
     (20, 1, [], 2, ["20231030", "20231031"], 10),
     (20, 1, [], 2, ["20231106"], 5),
     (20, 1, [I.SUNRISE_SUNSET], 2, ["20231030", "20231031"], 0),
     (20, 1, [I.SUNSET_SUNRISE], 2, ["20231030", "20231031"], 4),
-    (12.5, 15.5, None, None, ["20231107"], 2),  # FROM OPT
+    (12.5, 15.5, None, None, ["20231107"], 3),  # FROM OPT
     (
         3.75,
         5.25,
         [I.NIGHT],
         5.655,
         ["20240501", "20240701"],
         0,
```

### Comparing `lst-pressure-1.6.0/tests/test_lib_meerkat.py` & `lst-pressure-1.7.0/tests/test_lib_meerkat.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from conf import LocationProviderType
 
 # 20231030 LST dusk is about 2130
 
 tests = [
     # (lst_window_start, lst_window_end, utc_constraints, duration, dt_range, observables_count)
     (8, 20, [I.NIGHT], 2, ["20231030"], 0),
-    (8, 20, [], 2, ["20231030"], 2),
+    (8, 20, [], 2, ["20231030"], 3),
     (2, 20, [I.NIGHT], 0.5, ["20231030"], 1),
     (20, 1, [I.NIGHT], 2, ["20231030"], 2),
     (20, 1, [I.NIGHT], 2, ["20231030", "20231031"], 4),
     (20, 1, [], 2, ["20231030", "20231031"], 10),
     (20, 1, [], 2, ["20231106"], 5),
     (20, 1, [I.SUNRISE_SUNSET], 2, ["20231030", "20231031"], 0),
     (20, 1, [I.SUNSET_SUNRISE], 2, ["20231030", "20231031"], 4),
-    (12.5, 15.5, None, None, ["20231107"], 2),  # FROM OPT
+    (12.5, 15.5, None, None, ["20231107"], 3),  # FROM OPT
     (
         3.75,
         5.25,
         [I.NIGHT],
         5.655,
         ["20240501", "20240701"],
         0,
@@ -88,14 +88,24 @@
     duration,
     dt_range,
     observables_count,
 ):
     assert (
         len(
             sorted(
-                LSTCalendar(*dt_range, provider=LocationProviderType.MEERKAT).observables(
-                    [Observation("~", lst_window_start, lst_window_end, utc_constraints, duration)]
+                LSTCalendar(
+                    *dt_range, provider=LocationProviderType.MEERKAT
+                ).observables(
+                    [
+                        Observation(
+                            "~",
+                            lst_window_start,
+                            lst_window_end,
+                            utc_constraints,
+                            duration,
+                        )
+                    ]
                 )
             )
         )
         == observables_count
     )
```

### Comparing `lst-pressure-1.6.0/tests/utils/test_normalize_coordinates.py` & `lst-pressure-1.7.0/tests/utils/test_normalize_coordinates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/utils/test_normalize_dates.py` & `lst-pressure-1.7.0/tests/utils/test_normalize_dates.py`

 * *Files identical despite different names*

### Comparing `lst-pressure-1.6.0/tests/utils/test_time_conversions.py` & `lst-pressure-1.7.0/tests/utils/test_time_conversions.py`

 * *Files identical despite different names*

