# Comparing `tmp/DLMS_Firmware_updater-0.1.4.tar.gz` & `tmp/DLMS_Firmware_updater-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_Firmware_updater-0.1.4.tar", last modified: Tue Apr  9 11:27:47 2024, max compression
+gzip compressed data, was "DLMS_Firmware_updater-0.2.0.tar", last modified: Fri Apr 12 13:20:16 2024, max compression
```

## Comparing `DLMS_Firmware_updater-0.1.4.tar` & `DLMS_Firmware_updater-0.2.0.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.984218 DLMS_Firmware_updater-0.1.4/
--rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      569 2024-04-09 11:27:47.983222 DLMS_Firmware_updater-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.1.4/README.md
--rw-rw-rw-   0        0        0     1115 2024-04-09 11:26:30.000000 DLMS_Firmware_updater-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 11:27:47.984218 DLMS_Firmware_updater-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.585021 DLMS_Firmware_updater-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.651256 DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/__init__.py
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/config.toml
--rw-rw-rw-   0        0        0     3361 2024-04-09 11:25:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/main.py
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.673220 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/
--rw-rw-rw-   0        0        0      569 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-09 11:27:47.000000 DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.683219 DLMS_Firmware_updater-0.1.4/test/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.686221 DLMS_Firmware_updater-0.1.4/test/Firmwares/
--rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.1.4/test/Firmwares/firmwares.dat
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.591018 DLMS_Firmware_updater-0.1.4/test/Types/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.587020 DLMS_Firmware_updater-0.1.4/test/Types/101/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.740252 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/
--rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.14.typ
--rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.16.typ
--rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.26.typ
--rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.39.typ
--rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.43.typ
--rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.45.typ
--rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.46.typ
--rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.48.typ
--rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.49.typ
--rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.53.typ
--rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.54.typ
--rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.1.0.typ
--rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.2.0.typ
--rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.0.typ
--rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.30.typ
--rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.7.typ
--rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.9.typ
--rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.4.0.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.588018 DLMS_Firmware_updater-0.1.4/test/Types/102/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.781217 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/
--rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.20.typ
--rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.26.typ
--rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.39.typ
--rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.41.typ
--rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.43.typ
--rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.45.typ
--rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.48.typ
--rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.49.typ
--rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.53.typ
--rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.1.0.typ
--rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.2.0.typ
--rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.0.typ
--rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.30.typ
--rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.5.typ
--rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.7.typ
--rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.589017 DLMS_Firmware_updater-0.1.4/test/Types/103/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.819219 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/
--rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.16.typ
--rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.26.typ
--rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.39.typ
--rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.43.typ
--rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.45.typ
--rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.48.typ
--rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.49.typ
--rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.1.0.typ
--rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.2.0.typ
--rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.0.typ
--rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.30.typ
--rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.7.typ
--rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.590017 DLMS_Firmware_updater-0.1.4/test/Types/104/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.858221 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/
--rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.20.typ
--rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.26.typ
--rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.39.typ
--rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.43.typ
--rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.45.typ
--rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.48.typ
--rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.49.typ
--rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.53.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.1.0.typ
--rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.1.9.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.2.0.typ
--rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.2.5.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.0.typ
--rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.30.typ
--rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.7.typ
--rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.9.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.860217 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.888219 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.0.typ
--rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.15.typ
--rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.16.typ
--rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.17.typ
--rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.0.typ
--rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.3.typ
--rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.7.typ
--rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.6.1.typ
--rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.913218 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.0.typ
--rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.10.typ
--rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.12.typ
--rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.15.typ
--rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.16.typ
--rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.17.typ
--rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.5.0.typ
--rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.5.7.typ
--rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.935219 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
--rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
--rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
--rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
--rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
--rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
--rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.956217 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
--rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
--rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
--rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
--rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
--rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
--rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
-drwxrwxrwx   0        0        0        0 2024-04-09 11:27:47.980219 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/
--rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
--rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
--rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
--rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
--rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
--rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
--rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
--rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
--rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
--rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.1.4/test/Types/KPZ/image_transfer_1.typ
--rw-rw-rw-   0        0        0    24980 2024-04-05 12:32:20.000000 DLMS_Firmware_updater-0.1.4/test/client_log.txt
--rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.1.4/test/config.toml
--rw-rw-rw-   0        0        0      129 2024-04-08 11:48:52.000000 DLMS_Firmware_updater-0.1.4/test/test_updater.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.234088 DLMS_Firmware_updater-0.2.0/
+-rw-rw-rw-   0        0        0      141 2024-04-08 12:09:56.000000 DLMS_Firmware_updater-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      569 2024-04-12 13:20:16.234088 DLMS_Firmware_updater-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-04-05 11:46:13.000000 DLMS_Firmware_updater-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1115 2024-04-12 13:00:21.000000 DLMS_Firmware_updater-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:20:16.235089 DLMS_Firmware_updater-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       45 2024-04-08 11:38:51.000000 DLMS_Firmware_updater-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.898094 DLMS_Firmware_updater-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.923095 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:48:37.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/__init__.py
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/config.toml
+-rw-rw-rw-   0        0        0     3612 2024-04-12 13:09:16.000000 DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.938092 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/
+-rw-rw-rw-   0        0        0      569 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5345 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-12 13:20:15.000000 DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.946094 DLMS_Firmware_updater-0.2.0/test/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.949094 DLMS_Firmware_updater-0.2.0/test/Firmwares/
+-rw-rw-rw-   0        0        0  1766884 2024-02-16 08:53:58.000000 DLMS_Firmware_updater-0.2.0/test/Firmwares/firmwares.dat
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.905098 DLMS_Firmware_updater-0.2.0/test/Types/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.900095 DLMS_Firmware_updater-0.2.0/test/Types/101/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.004092 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/
+-rw-rw-rw-   0        0        0    57842 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.14.typ
+-rw-rw-rw-   0        0        0    50536 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.16.typ
+-rw-rw-rw-   0        0        0    52759 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.26.typ
+-rw-rw-rw-   0        0        0    34300 2023-12-21 03:55:07.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.39.typ
+-rw-rw-rw-   0        0        0    52661 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.43.typ
+-rw-rw-rw-   0        0        0    58232 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.45.typ
+-rw-rw-rw-   0        0        0    57145 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.46.typ
+-rw-rw-rw-   0        0        0    75612 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.48.typ
+-rw-rw-rw-   0        0        0    34417 2023-12-21 04:16:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.49.typ
+-rw-rw-rw-   0        0        0   116670 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.53.typ
+-rw-rw-rw-   0        0        0    81183 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.54.typ
+-rw-rw-rw-   0        0        0     3996 2023-11-27 13:04:23.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.0.typ
+-rw-rw-rw-   0        0        0   105296 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.0.typ
+-rw-rw-rw-   0        0        0   104149 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.0.typ
+-rw-rw-rw-   0        0        0   110418 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.30.typ
+-rw-rw-rw-   0        0        0   109427 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.7.typ
+-rw-rw-rw-   0        0        0   113952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.9.typ
+-rw-rw-rw-   0        0        0     2940 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.4.0.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.901094 DLMS_Firmware_updater-0.2.0/test/Types/102/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.049091 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/
+-rw-rw-rw-   0        0        0    52751 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.20.typ
+-rw-rw-rw-   0        0        0    54303 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.26.typ
+-rw-rw-rw-   0        0        0    36789 2023-12-20 11:05:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.39.typ
+-rw-rw-rw-   0        0        0    54404 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.41.typ
+-rw-rw-rw-   0        0        0    54502 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.43.typ
+-rw-rw-rw-   0        0        0    60174 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.45.typ
+-rw-rw-rw-   0        0        0    78025 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.48.typ
+-rw-rw-rw-   0        0        0    37934 2023-12-20 11:30:16.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.49.typ
+-rw-rw-rw-   0        0        0   115968 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.53.typ
+-rw-rw-rw-   0        0        0     3974 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.0.typ
+-rw-rw-rw-   0        0        0   114434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.0.typ
+-rw-rw-rw-   0        0        0   114952 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.0.typ
+-rw-rw-rw-   0        0        0   133762 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.30.typ
+-rw-rw-rw-   0        0        0   116367 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.5.typ
+-rw-rw-rw-   0        0        0   128811 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.7.typ
+-rw-rw-rw-   0        0        0   136629 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.903093 DLMS_Firmware_updater-0.2.0/test/Types/103/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.088091 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/
+-rw-rw-rw-   0        0        0    50538 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.16.typ
+-rw-rw-rw-   0        0        0    52761 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.26.typ
+-rw-rw-rw-   0        0        0    34302 2023-12-20 11:53:57.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.39.typ
+-rw-rw-rw-   0        0        0    52960 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.43.typ
+-rw-rw-rw-   0        0        0    58627 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.45.typ
+-rw-rw-rw-   0        0        0    75853 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.48.typ
+-rw-rw-rw-   0        0        0    34419 2023-12-21 03:44:07.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.49.typ
+-rw-rw-rw-   0        0        0   117000 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.0.typ
+-rw-rw-rw-   0        0        0   105032 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.0.typ
+-rw-rw-rw-   0        0        0   104156 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.0.typ
+-rw-rw-rw-   0        0        0   110280 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.30.typ
+-rw-rw-rw-   0        0        0   109434 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.7.typ
+-rw-rw-rw-   0        0        0   113959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:15.904094 DLMS_Firmware_updater-0.2.0/test/Types/104/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.123090 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/
+-rw-rw-rw-   0        0        0    52848 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.20.typ
+-rw-rw-rw-   0        0        0    54310 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.26.typ
+-rw-rw-rw-   0        0        0    36791 2023-12-20 10:26:34.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.39.typ
+-rw-rw-rw-   0        0        0    54724 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.43.typ
+-rw-rw-rw-   0        0        0    60391 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.45.typ
+-rw-rw-rw-   0        0        0    78146 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.48.typ
+-rw-rw-rw-   0        0        0    37935 2023-12-20 10:46:38.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.49.typ
+-rw-rw-rw-   0        0        0   118764 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.53.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.0.typ
+-rw-rw-rw-   0        0        0   114441 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.9.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.0.typ
+-rw-rw-rw-   0        0        0   114959 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.5.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.0.typ
+-rw-rw-rw-   0        0        0   133694 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.30.typ
+-rw-rw-rw-   0        0        0   128818 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.7.typ
+-rw-rw-rw-   0        0        0   136636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.9.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.126092 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.150091 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ
+-rw-rw-rw-   0        0        0   147549 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ
+-rw-rw-rw-   0        0        0   146973 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ
+-rw-rw-rw-   0        0        0   146964 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ
+-rw-rw-rw-   0        0        0   145262 2023-10-31 09:20:28.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ
+-rw-rw-rw-   0        0        0    87888 2023-11-16 05:19:14.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ
+-rw-rw-rw-   0        0        0    88315 2023-11-29 12:34:20.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ
+-rw-rw-rw-   0        0        0    88966 2023-12-15 08:12:51.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ
+-rw-rw-rw-   0        0        0    89042 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.174090 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ
+-rw-rw-rw-   0        0        0   173570 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ
+-rw-rw-rw-   0        0        0   172860 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ
+-rw-rw-rw-   0        0        0    96832 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ
+-rw-rw-rw-   0        0        0   170726 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ
+-rw-rw-rw-   0        0        0   170785 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ
+-rw-rw-rw-   0        0        0   168739 2023-10-31 11:55:04.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ
+-rw-rw-rw-   0        0        0   102599 2023-11-29 12:38:13.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ
+-rw-rw-rw-   0        0        0   103542 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.192089 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ
+-rw-rw-rw-   0        0        0   147636 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ
+-rw-rw-rw-   0        0        0   147060 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ
+-rw-rw-rw-   0        0        0   147052 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ
+-rw-rw-rw-   0        0        0   145337 2023-10-31 11:55:11.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ
+-rw-rw-rw-   0        0        0    88727 2023-11-29 12:38:31.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ
+-rw-rw-rw-   0        0        0    89162 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.211090 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ
+-rw-rw-rw-   0        0        0   172819 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ
+-rw-rw-rw-   0        0        0   170738 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ
+-rw-rw-rw-   0        0        0   170642 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ
+-rw-rw-rw-   0        0        0   168751 2023-10-31 12:05:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ
+-rw-rw-rw-   0        0        0   102731 2023-11-29 12:38:38.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ
+-rw-rw-rw-   0        0        0   103458 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ
+drwxrwxrwx   0        0        0        0 2024-04-12 13:20:16.231089 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/
+-rw-rw-rw-   0        0        0     3996 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ
+-rw-rw-rw-   0        0        0   171345 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ
+-rw-rw-rw-   0        0        0   172600 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ
+-rw-rw-rw-   0        0        0   170800 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ
+-rw-rw-rw-   0        0        0   170867 2023-11-21 08:08:15.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ
+-rw-rw-rw-   0        0        0   168765 2023-10-31 14:32:35.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ
+-rw-rw-rw-   0        0        0     3789 2023-11-16 12:32:41.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ
+-rw-rw-rw-   0        0        0   102803 2023-11-29 12:38:49.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ
+-rw-rw-rw-   0        0        0   103828 2023-12-20 06:08:22.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ
+-rw-rw-rw-   0        0        0     3936 2023-11-24 05:19:52.000000 DLMS_Firmware_updater-0.2.0/test/Types/KPZ/image_transfer_1.typ
+-rw-rw-rw-   0        0        0    35431 2024-04-12 13:19:19.000000 DLMS_Firmware_updater-0.2.0/test/client_log.txt
+-rw-rw-rw-   0        0        0    74536 2024-04-04 09:14:27.000000 DLMS_Firmware_updater-0.2.0/test/config.toml
+-rw-rw-rw-   0        0        0      387 2024-04-12 13:11:37.000000 DLMS_Firmware_updater-0.2.0/test/test_updater.py
```

### Comparing `DLMS_Firmware_updater-0.1.4/PKG-INFO` & `DLMS_Firmware_updater-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_Firmware_updater
-Version: 0.1.4
+Version: 0.2.0
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.1.4/pyproject.toml` & `DLMS_Firmware_updater-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 [tool.setuptools.package-data]
 DLMSFirmwareUpdater = ["*.toml", "*.dat", "*.typ"]
 #exclude = ["test*", "dummy"]  # alternatively: `exclude = ["additional*"]`
 #namespaces = false
 
 [project]
 name = "DLMS_Firmware_updater"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS_SPODES_client == 0.7.2",
+    "DLMS_SPODES_client == 0.7.6",
     "pyinstaller >= 6.2",
     "build >= 1.2.1"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=["dlms", "spodes", "client", "firmware", "update"]
```

### Comparing `DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/config.toml` & `DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/config.toml`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/src/DLMSFirmwareUpdater/main.py` & `DLMS_Firmware_updater-0.2.0/src/DLMSFirmwareUpdater/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import argparse
 import time
 
 from DLMS_SPODES_client.servers import TransactionServer, Result
-from DLMS_SPODES_client import task
+from DLMS_SPODES_client import task, services
 from DLMS_SPODES_client.client import Client, logL
 from DLMS_SPODES_communications import AsyncSerial, AsyncNetwork
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Update Firmware Program for DLMS meters")
     parser.add_argument(
         '-t', '--type',
-        choices=("Serial", "Net"),
+        choices=("File", "Serial", "Net"),
         required=True,
         help="Communication type")
     parser.add_argument(
         "-p",
         nargs='*',
         help="connection parameters")
     parser.add_argument(
         "-T", "--timeout",
         type=int,
         default=60,
-        help="connection parameters")
+        help="communication timeout")
     parser.add_argument(
         "-s", "--secret",
         type=lambda value: str.encode(value, "ascii"),
-        required=True,
+        default="0000000000000000",
         help="DLMS association secret")
     parser.add_argument(
         "-sap",
         type=int,
         default=0x30,
         help="DLMS SAP")
     parser.add_argument(
@@ -65,50 +65,51 @@
     parser.add_argument(
         "-f", "--file",
         type=str,
         default=".//output.txt",
         help="output result file"
     )
     args = parser.parse_args()
-    match args.type:
-        case "Serial":
-            c_t = AsyncSerial
-        case "Net":
-            c_t = AsyncNetwork
-        case communication_type:
-            raise ValueError(F"unknown {communication_type=}")
+    if (source := args.type) in ("Serial", "Net"):
+        clients = [c := Client(
+                        SAP=args.sap,
+                        secret=args.secret.hex(),
+                        addr_size=-1)]
+        c.m_id.set(args.mechanism_id)
+        c.device_address.set(args.da)
+        c_t = AsyncSerial if source == "Serial" else AsyncNetwork
+        c.media = c_t(*args.p)
+        c.media.inactivity_timeout = args.timeout
+    elif source == "File":
+        if len(args.p) == 1:
+            clients = services.get_client_from_csv(file_name=args.p[0])
+        else:
+            raise ValueError("-p for \"File\" must have 1 file name")
+    else:
+         raise ValueError(F"unknown {source=}")
     t_server = TransactionServer(
-        clients=[
-            c := Client(
-                SAP=args.sap,
-                secret=args.secret.hex(),
-                addr_size=-1)
-        ],
+        clients=clients,
         tsk=task.Loop(
             task=task.UpdateFirmware(),
             func=lambda res: res,
             delay=args.loop_delay,
             attempt_amount=args.n_loops
         )
     )
-    c.m_id.set(args.mechanism_id)
-    c.device_address.set(args.da)
-    c.media = c_t(*args.p)
-    c.media.inactivity_timeout = args.timeout
     t_server.start()
     results = list(t_server.results)
     with open(
             file=args.file,
             mode="w+",
             encoding="utf-8") as file:
         while results:
             time.sleep(3)
             for res in results:
                 res: Result
                 if res.complete:
                     results.remove(res)
-                    c.log(logL.INFO, F"Для {res.client} обновление: {'Удачно' if res.value else 'Неудачно'}")
+                    res.client.log(logL.INFO, F"Для {res.client} обновление: {'Удачно' if res.value else 'Неудачно'}")
                     file.write(F"{res.client} {res.value}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/PKG-INFO` & `DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-Firmware-updater
-Version: 0.1.4
+Version: 0.2.0
 Summary: dlms-spodes
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/DLMSFirmwareUpdater_project
 Keywords: dlms,spodes,client,firmware,update
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DLMS_Firmware_updater-0.1.4/src/DLMS_Firmware_updater.egg-info/SOURCES.txt` & `DLMS_Firmware_updater-0.2.0/src/DLMS_Firmware_updater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Firmwares/firmwares.dat` & `DLMS_Firmware_updater-0.2.0/test/Firmwares/firmwares.dat`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.14.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.14.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.26.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.39.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.43.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.45.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.46.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.46.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.48.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.49.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.53.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/0.0.54.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/0.0.54.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.1.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.1.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.2.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.2.5.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.30.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.3.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/101/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/101/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.20.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.26.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.39.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.41.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.41.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.43.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.45.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.48.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.49.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/0.0.53.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.1.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.1.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.2.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.2.5.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.30.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.5.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/102/09054d324d5f33/1.3.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/102/09054d324d5f33/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.26.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.39.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.43.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.45.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.48.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.49.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/0.0.53.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.1.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.1.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.2.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.2.5.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.30.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/103/09064d324d5f3153/1.3.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/103/09064d324d5f3153/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.20.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.20.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.26.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.26.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.39.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.39.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.43.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.43.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.45.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.45.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.48.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.48.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.49.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.49.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/0.0.53.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/0.0.53.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.1.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.1.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.1.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.2.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.2.5.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.2.5.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.30.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.30.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/104/09064d324d5f3353/1.3.9.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/104/09064d324d5f3353/1.3.9.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.15.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.17.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.4.22.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.3.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.3.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.5.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.6.1.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f31/1.6.2.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f31/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.10.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.10.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.12.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.15.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.17.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.4.22.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.5.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.5.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09054d324d5f33/1.6.2.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09054d324d5f33/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.15.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.17.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.4.22.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.5.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.5.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3153/1.6.2.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3153/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.15.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.17.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.4.22.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.5.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.5.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3353/1.6.2.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3353/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.12.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.12.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.15.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.15.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.16.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.16.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.17.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.17.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.4.22.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.4.22.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.5.0.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.0.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.5.7.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.5.7.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/09064d324d5f3354/1.6.2.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/09064d324d5f3354/1.6.2.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/Types/KPZ/image_transfer_1.typ` & `DLMS_Firmware_updater-0.2.0/test/Types/KPZ/image_transfer_1.typ`

 * *Files identical despite different names*

### Comparing `DLMS_Firmware_updater-0.1.4/test/client_log.txt` & `DLMS_Firmware_updater-0.2.0/test/client_log.txt`

 * *Files 18% similar despite different names*

```diff
@@ -171,7 +171,75 @@
 101000017410: 05.04 15:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - DisconnectRequest
 101000017410: 05.04 15:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1 SA:16 
 101000017410: 05.04 15:31 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:16 SA:1  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
 101000017410: 05.04 15:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close communication channel: AsyncSerial(port='COM13', inactivity_timeout=3)
 101000017410: 05.04 15:31 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close media: AsyncSerial(port='COM13', inactivity_timeout=3)
 #common: 05.04 15:32 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
 #common: 05.04 15:32 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:02 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:04 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:04 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:04 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:05 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:05 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:06 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#common: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - Open port communication channel: AsyncSerial(port='COM13', inactivity_timeout=1)
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=16, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:16  Info[11]:81 80 08 05 02 07 ee 06 02 07 ee
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:16 SA:1/16  Info[10]:81 80 07 05 01 ef 06 02 04 00
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:16  Info[34]:e6 e6 00 60 1d a1 09 06 07 60 85 74 05 08 01 01 be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:16 SA:1/16  Info[46]:e6 e7 00 61 29 a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 00 be 10 04 0e 08 00 06 5f 1f 04 00 00 10 10 04 00 00 07
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001000000010000
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - Authentication success
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:16 SA:1/16  Info[24]:e6 e7 00 c4 01 c1 00 09 0f 4b 50 5a 31 30 31 30 30 30 30 31 37 34 31 30
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 60 01 01 ff 02 00
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:16 SA:1/16  Info[14]:e6 e7 00 c4 01 c1 00 09 05 4d 32 4d 5f 31
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:16  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 00 02 01 ff 02 00
+#0: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:16 SA:1/16  Info[15]:e6 e7 00 c4 01 c1 00 09 06 31 2e 36 2e 31 34
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - added 253 DLMS objects
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - DisconnectRequest
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: DISC_P DA:1/16 SA:16 
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:16 SA:1/16  Info[22]:81 80 13 05 01 ef 06 02 04 00 07 04 00 00 00 01 08 04 00 00 00 01
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close communication channel: AsyncSerial(port='COM13', inactivity_timeout=1)
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - c.SA=Address(upper_address=48, lower_address=None) c.DA=Address(upper_address=1, lower_address=16)
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: SNRM_P DA:1/16 SA:48  Info[10]:81 80 07 05 02 04 00 06 01 ef
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: UA_F DA:48 SA:1/16  Info[10]:81 80 07 05 01 ef 06 02 04 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - negotiation setup: NEGOTIATION: 1024->[info_size]->239 1->[window]->1
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[67]:e6 e6 00 60 3e a1 09 06 07 60 85 74 05 08 01 01 8a 02 07 80 8b 07 60 85 74 05 08 02 02 ac 12 80 10 d9 25 43 23 0f fc c3 34 3d 5b 4c c4 be c5 96 a8 be 10 04 0e 01 00 00 00 06 5f 1f 04 00 7f ff ff 04 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[79]:e6 e7 00 61 4a a1 09 06 07 60 85 74 05 08 01 01 a2 03 02 01 00 a3 05 a1 03 02 01 0e 88 02 07 80 89 07 60 85 74 05 08 02 02 aa 12 80 10 0a ca ad 2e b4 c1 1f d8 75 0e 51 92 49 1d 56 b1 be 10 04 0e 08 00 06 5f 1f 04 00 00 18 9d 04 00 00 07
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - SET CONFORMANCE: 000000000001100010011101
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[34]:e6 e6 00 c3 01 c1 00 0f 00 00 28 00 03 ff 01 01 09 10 2e 24 45 93 cb 55 93 10 dc c1 e5 da f9 5c 68 e2
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c7 01 c1 00 01 00 09 10 c0 03 58 cf 9c 0c f4 a6 da ea 04 4d 22 2d 4c 32
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 2a 00 00 ff 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S2_R3_PF DA:48 SA:1/16  Info[24]:e6 e7 00 c4 01 c1 00 09 0f 4b 50 5a 31 30 31 30 30 30 30 31 37 34 31 30
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S3_R3_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 80 64 00 ff 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S3_R4_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c4 01 c1 00 0a 12 30 30 30 38 50 57 52 4d 5f 4d 32 4d 5f 31 5f 46 34 5f
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S4_R4_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S4_R5_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S5_R5_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 06 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S5_R6_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 06
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S6_R6_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 80 ff 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S6_R7_PF DA:48 SA:1/16  Info[12]:e6 e7 00 c4 01 c1 00 06 00 00 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - set image to update suitable_firmware=AppVersion(1, 3, 30)
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - boot_version=8 is actual
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S7_R7_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 01 00 00 80 64 00 ff 02 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S7_R0_PF DA:48 SA:1/16  Info[27]:e6 e7 00 c4 01 c1 00 0a 12 30 30 30 38 50 57 52 4d 5f 4d 32 4d 5f 31 5f 46 34 5f
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S0_R0_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 06 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S0_R1_PF DA:48 SA:1/16  Info[9]:e6 e7 00 c4 01 c1 00 16 06
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S1_R1_PF DA:1/16 SA:48  Info[16]:e6 e6 00 c0 01 c1 00 12 00 00 2c 00 00 ff 07 00
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - RX: S1_R2_PF DA:48 SA:1/16  Info[52]:e6 e7 00 c4 01 c1 00 01 01 02 03 06 00 02 bb 9c 09 10 83 c3 b5 c9 f0 28 f5 67 10 87 39 2b 3b dc b8 50 09 10 83 c3 b5 c9 f0 28 f5 67 10 87 39 2b 3b dc b8 50
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - TX: S2_R2_PF DA:1/16 SA:48  Info[41]:e6 e6 00 c3 01 c1 00 12 00 00 2c 00 00 ff 01 01 02 02 09 10 46 5e 30 85 76 84 d1 41 c0 f2 32 e9 f5 02 b5 e1 06 00 02 f9 6c
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - WARNING - Data send failed.  Try to resend 2/3. RX_buffer: 
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - WARNING - Data send failed.  Try to resend 3/3. RX_buffer: 
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Close media: AsyncSerial(port='COM13', inactivity_timeout=1)
+KPZ101000017410: 12.04 16:09 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для KPZ101000017410 обновление: Неудачно
+#common: 12.04 16:11 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#0: 12.04 16:11 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 0 обновление: Неудачно
+#1: 12.04 16:12 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 1 обновление: Неудачно
+#2: 12.04 16:12 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 2 обновление: Неудачно
+#common: 12.04 16:18 - DLMSClient.DLMS_SPODES_client.logger - DEBUG - Start <Logger DLMSClient.DLMS_SPODES_client.logger (DEBUG)>
+#0: 12.04 16:18 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 0 обновление: Неудачно
+#1: 12.04 16:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 1 обновление: Неудачно
+#2: 12.04 16:19 - DLMSClient.DLMS_SPODES_client.logger - INFO - Для 2 обновление: Неудачно
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `DLMS_Firmware_updater-0.1.4/test/config.toml` & `DLMS_Firmware_updater-0.2.0/test/config.toml`

 * *Files identical despite different names*

