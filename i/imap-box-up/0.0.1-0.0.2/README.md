# Comparing `tmp/imap_box_up-0.0.1.tar.gz` & `tmp/imap_box_up-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imap_box_up-0.0.1.tar", last modified: Fri Apr 12 01:36:48 2024, max compression
+gzip compressed data, was "imap_box_up-0.0.2.tar", last modified: Fri Apr 12 09:04:03 2024, max compression
```

## Comparing `imap_box_up-0.0.1.tar` & `imap_box_up-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/
--rw-rw-rw-   0        0        0    11359 2023-08-06 03:53:35.000000 imap_box_up-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    11358 2024-04-11 18:16:19.000000 imap_box_up-0.0.1/LICENSE-2.0.txt
--rw-rw-rw-   0        0        0     4895 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4120 2024-04-11 18:34:36.000000 imap_box_up-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap/
--rw-rw-rw-   0        0        0       30 2024-04-10 03:49:25.000000 imap_box_up-0.0.1/imap/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/editor.py
--rw-rw-rw-   0        0        0      949 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/global_var.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap/lib/
--rw-rw-rw-   0        0        0        0 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/__init__.py
--rw-rw-rw-   0        0        0     3299 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/common.py
--rw-rw-rw-   0        0        0    30089 2024-04-12 00:38:05.000000 imap_box_up-0.0.1/imap/lib/convertor.py
--rw-rw-rw-   0        0        0     1980 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/convex_hull.py
--rw-rw-rw-   0        0        0     2223 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/draw.py
--rw-rw-rw-   0        0        0     6642 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/odr_spiral.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap/lib/opendrive/
--rw-rw-rw-   0        0        0        0 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/__init__.py
--rw-rw-rw-   0        0        0      962 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/common.py
--rw-rw-rw-   0        0        0     2450 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/header.py
--rw-rw-rw-   0        0        0     3302 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/junction.py
--rw-rw-rw-   0        0        0    15653 2024-04-10 06:51:57.000000 imap_box_up-0.0.1/imap/lib/opendrive/lanes.py
--rw-rw-rw-   0        0        0     4401 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/map.py
--rw-rw-rw-   0        0        0     8140 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/plan_view.py
--rw-rw-rw-   0        0        0     2681 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/profile.py
--rw-rw-rw-   0        0        0     6348 2024-04-10 07:08:00.000000 imap_box_up-0.0.1/imap/lib/opendrive/road.py
--rw-rw-rw-   0        0        0     4576 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/signals.py
--rw-rw-rw-   0        0        0      771 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/opendrive/user_data.py
--rw-rw-rw-   0        0        0      988 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/polynoms.py
--rw-rw-rw-   0        0        0     2173 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/proj_helper.py
--rw-rw-rw-   0        0        0     4528 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/proto_utils.py
--rw-rw-rw-   0        0        0     1910 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/imap/lib/transform.py
--rw-rw-rw-   0        0        0     5128 2024-04-10 03:40:45.000000 imap_box_up-0.0.1/imap/main.py
--rw-rw-rw-   0        0        0     4808 2024-04-10 02:41:29.000000 imap_box_up-0.0.1/imap/map.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/
--rw-rw-rw-   0        0        0     4895 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/imap_box_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-08-06 03:53:36.000000 imap_box_up-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 01:36:48.000000 imap_box_up-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1175 2024-04-11 18:31:01.000000 imap_box_up-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:03.540062 imap_box_up-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-12 09:04:03.540062 imap_box_up-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:03.536062 imap_box_up-0.0.2/imap/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/global_var.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:03.536062 imap_box_up-0.0.2/imap/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30241 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/convex_hull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/odr_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:03.540062 imap_box_up-0.0.2/imap/lib/opendrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/junction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/lanes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/plan_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/road.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/opendrive/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/polynoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/proj_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/lib/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/imap/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:04:03.540062 imap_box_up-0.0.2/imap_box_up.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 09:04:03.000000 imap_box_up-0.0.2/imap_box_up.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:04:03.544062 imap_box_up-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-12 09:03:24.000000 imap_box_up-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imap_box_up-0.0.1/LICENSE` & `imap_box_up-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/README.md` & `imap_box_up-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # imap
 
 [![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
 
-**[imap](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo. 
+**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap), the imap tool is very useful. 
 
-I called the modified with **imap_box_up** , Just to differentiate it from imap_box
+The name of **imap_box_up** , Just to modified from imap_box
 
-imap_box_up code: https://github.com/porterpan/imap_box_up
+The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
+
+imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
 
 **Note:**
 
-Modified on project [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
+The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
 
 > I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
 
+## now(fix junction bug)
+
+![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
+
+![junction detail](https://img2.imgtp.com/2024/04/12/Ct9V2l51.png)
+
+## the old tool bug
 
+![invalid junction](https://img2.imgtp.com/2024/04/12/hOWOvqyr.jpg)
+
+![junction error](https://imap.readthedocs.io/en/latest/_images/map_show.jpg)
 
-![example]([eg1.png](https://private-user-images.githubusercontent.com/30954452/321745045-d23d05d2-66a4-4690-bf17-073c7fd4bbe3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI4NjA3NjQsIm5iZiI6MTcxMjg2MDQ2NCwicGF0aCI6Ii8zMDk1NDQ1Mi8zMjE3NDUwNDUtZDIzZDA1ZDItNjZhNC00NjkwLWJmMTctMDczYzdmZDRiYmUzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDExVDE4MzQyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTE4NDYyY2ZkZjQxMjQ2YTZiZmVmMWI2YTg3ZTA3NGZlMzNjNTY3ZTIxZDFhZDY1NjdlZWFiYWM1YTk2YjI0MTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.GhurdLnE04-8-OwlWQF2VWgymB4e-EX-hAONUX1pQaM))
 
 **Supported features**:
 1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
 2. Find lane by id
 3. Convert format: Opendrive to Apollo format.
 
 | os      | support                 | remark |
@@ -42,61 +53,52 @@
 pip3 install imap_box_up
 ```
 
 ## Example
 #### 1. Visualization
 After the installation is complete, you can view the map with the following command.
 ```shell
-imap -m data/borregas_ave.txt
+imap_box_up -m data/borregas_ave.txt
 // or
-imap -m data/town.xodr
+imap_box_up -m data/town.xodr
 ```
 Currently supported formats:
 * Apollo map
 * OpenDrive map
 
 #### 2. Find lane by id
 You can use below command to find lane by id, Found lane is shown in **Red**.
 ```shell
-imap -m data/borregas_ave.txt -l lane_35
+imap_box_up -m data/borregas_ave.txt -l lane_35
 ```
 
 #### 3. Format conversion
 Now you can convert OpenDrive map to Apollo map by following command.
-```shell
-imap -f -i data/town.xodr -o data/apollo_map.txt
-```
-you should better reference follow command to convert apollo map to OpenDrive map.
-
- 1.show appollo map by id:
-
- ```shell
- imap -m data/borregas_ave.txt -l lane_35
- ```
-
-2.Format conversion with UTM map(opendrive->appollo): 
 
+- save as utm world coordinates(**world map** for old feature)
 ```shell
-imap -f -i data/town.xodr -o data/apollo_map.txt
+imap_box_up -f -i data/town.xodr -o data/apollo_map.txt
 ```
-3.Format conversion with inertial map(opendrive->appollo.inertial map):
+
+- save as inertial system coordinates (**relative map** for new feature)
 
 ```shell
-imap -f -r -i data/town.xodr -o data/apollo_map.txt
+imap_box_up -f -r -i data/town.xodr -o data/apollo_map.txt
 ```
 
 
-
 The following is the display of the hd-map in `data\borregas_ave.txt`.You can click on the lane you want to display more detail info, which will display the current lane's id, as well as the predecessor and successor lane's id in the upper left corner.
 
-![map_show](docs/_static/map_show.jpg)
+![imap_box_up convert map load to rviz display](https://img2.imgtp.com/2024/04/12/a1QPsCb2.png)
 
 
 ## Questions
-1. After running the command `imap -m data/your_map_file`, nothing display and no errors!!!
+1. After running the command `imap_box_up -m data/your_map_file`, nothing display and no errors!!!
 
 A: Check the permissions of the map file, if the current user does not have permissions, modify the permissions with the following commands.
 ```shell
 sudo chmod 777 data/your_map_file
 ```
 2. Map data permission checking has no problem, still nothing display and no errors!
 A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
+
+> If you have any questions, please feel free to contact me.
```

### Comparing `imap_box_up-0.0.1/imap/editor.py` & `imap_box_up-0.0.2/imap/editor.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/global_var.py` & `imap_box_up-0.0.2/imap/global_var.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/common.py` & `imap_box_up-0.0.2/imap/lib/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/convertor.py` & `imap_box_up-0.0.2/imap/lib/convertor.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   write_pb_to_bin_file
 )
 
 from imap.lib.draw import draw_line, show
 from imap.lib.convex_hull import convex_hull, aabb_box
 from imap.lib.proj_helper import latlon2utm
 from concave_hull import concave_hull as concave_hull_lib
-from scipy.spatial import ConvexHull, Delaunay
+from scipy.spatial import ConvexHull as ConvexHull_lib
 import numpy as np
 
 
 # Distance between stop line and pedestrian crossing
 STOP_LINE_DISTANCE = 1.0
 
 
@@ -586,63 +586,63 @@
     if not self._is_valid_junction(xodr_junction):
       return []
 
     points = []
     # TODO:: junction boundry 
     if type == "box":
       for road, relation in xodr_junction.connected_roads:
-          start, end = road.get_cross_section(relation)
+        cross_section = road.get_cross_section(relation)
+        if cross_section:
+          start, end = cross_section
           points.append([start.x, start.y])
           points.append([end.x, end.y])
 
           # when point <= 4 convex_hull will not fully covered, so we change to aabb_box
-          if len(points) <= 4:
-            return aabb_box(points)
-          else:
-            return convex_hull(points)
+      if len(points) <= 4:
+        return aabb_box(points)
+      else:
+        return convex_hull(points)
     
-    elif type == "boundry":  
+    elif type == "boundry": 
       left_incomroadlist = []  
       right_incomroadlist = []  
  
       boundary_point_temp=[]
       for junction_connecting_lane in xodr_junction.connections:  
         # connecting_road 
         for lanesection_ in self.xodr_map.roads[junction_connecting_lane.connecting_road].lanes.lane_sections: 
           junction_id = self.xodr_map.roads[junction_connecting_lane.connecting_road].junction_id 
           if junction_id == "-1":
             continue 
           link_name = self.xodr_map.roads[junction_connecting_lane.connecting_road].link
-          print("junction_id: ", junction_id)
-          print("pre: {} sub: {}".format(link_name.predecessor.contact_point, link_name.successor.contact_point))          
+          # print("junction_id: ", junction_id)
+          # print("pre: {} sub: {}".format(link_name.predecessor.contact_point, link_name.successor.contact_point))          
           incomRoadID = junction_connecting_lane.connecting_road #incoming_road
           left_boundary_points = []
           right_boundary_points = []  
-          # if link_name.predecessor.contact_point !="end" and link_name.successor.contact_point !="start":
-          #   continue
           
           for lanesectionright in lanesection_.right: # -            
             if  lanesectionright.lane_type != "driving" and lanesectionright.lane_type != "shoulder": 
-              print("laneleft.lane_id.right: ", lanesectionright.lane_id)
-              print("laneleft.type: ", lanesectionright.lane_type)
+              # print("laneleft.lane_id.right: ", lanesectionright.lane_id)
+              # print("laneleft.type: ", lanesectionright.lane_type)
               if incomRoadID in right_incomroadlist:
                 break
               right_incomroadlist.append(incomRoadID) 
               if len(lanesection_.right)>0 and len(lanesection_.left)>0:   
                 for points in lanesectionright.right_boundary:              
                       right_boundary_points.append([points.x, points.y])  
               else:
                 for points in lanesectionright.right_boundary:              
                       right_boundary_points.append([points.x, points.y])          
                      
                              
           for lanesectionleft in lanesection_.left: # + 
             if lanesectionleft.lane_type != "driving" and lanesectionleft.lane_type != "shoulder":
-              print("laneleft.lane_id.left: ", lanesectionleft.lane_id)
-              print("laneleft.type: ", lanesectionleft.lane_type)  
+              # print("laneleft.lane_id.left: ", lanesectionleft.lane_id)
+              # print("laneleft.type: ", lanesectionleft.lane_type)  
               if incomRoadID in left_incomroadlist:
                 break
               left_incomroadlist.append(incomRoadID)
               if len(lanesection_.right)>0 and len(lanesection_.left)>0:                
                 for points in lanesectionleft.left_boundary:                           
                     left_boundary_points.append([points.x, points.y])
               else:
@@ -692,20 +692,22 @@
               boundary_point_temp[j][1] = temp_name_
           boundary_points.extend(boundary_point_temp[i][0])
         boundary_points.extend(boundary_point_temp[3][0])
       else:
         for points, _, _ in boundary_point_temp:
           boundary_points.extend(points)
       
-      hull = ConvexHull(np.array(boundary_points))
+      hull = ConvexHull_lib(np.array(boundary_points))
 
 
       # return boundary_points
       return concave_hull_lib(boundary_points, length_threshold=0, concavity=5, convex_hull_indexes=hull.vertices)
-      
+    else:
+      print("---------------------convert method error---------------------")
+      return   
 
   def convert_junctions(self, method="boundry"):
     for _, xodr_junction in self.xodr_map.junctions.items():
       polygon = self.construct_junction_polygon(xodr_junction, method)
       if len(polygon) < 3:
         logging.warning(
           "junction {} polygon size < 3.".format(xodr_junction.junction_id))
@@ -713,19 +715,22 @@
 
       pb_junction = self.pb_map.junction.add()
       pb_junction.id.id = xodr_junction.junction_id
       for x, y in polygon:
         pb_point = pb_junction.polygon.point.add()
         pb_point.x, pb_point.y, pb_point.z = x, y, 0
 
-  def convert(self, relative=False):
+  def convert(self, relative=False, junctionbox=False):
     self.convert_header(relative)
     # Don't change the order. "convert_roads" must before "convert_junctions"
     self.convert_roads()
-    self.convert_junctions(method="boundry")
+    if junctionbox == False:      
+      self.convert_junctions(method="boundry")
+    else:      
+      self.convert_junctions(method="box")
 
     # Todo(zero): display xodr map
     if self.output_file_name is None:
       show(need_save=global_var.get_element_value("need_save_figure"), path=self.input_file_name.replace(".xodr", ".png"))
 
 
   def save_map(self):
```

### Comparing `imap_box_up-0.0.1/imap/lib/convex_hull.py` & `imap_box_up-0.0.2/imap/lib/convex_hull.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/draw.py` & `imap_box_up-0.0.2/imap/lib/draw.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/odr_spiral.py` & `imap_box_up-0.0.2/imap/lib/odr_spiral.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/common.py` & `imap_box_up-0.0.2/imap/lib/opendrive/common.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/header.py` & `imap_box_up-0.0.2/imap/lib/opendrive/header.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/junction.py` & `imap_box_up-0.0.2/imap/lib/opendrive/junction.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/lanes.py` & `imap_box_up-0.0.2/imap/lib/opendrive/lanes.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,14 @@
       return []
 
   
       
   def get_cross_section_points(self, relation):
     # qian
     if relation == "predecessor":
-      return self.lane_sections[0].get_cross_section_points_("start")
+      return self.lane_sections[0].get_cross_section("start")
     # hou
     elif relation == "successor":
-      return self.lane_sections[-1].get_cross_section_points_("end")
+      return self.lane_sections[-1].get_cross_section("end")
     else:
       print("Unknown relation!")
       return []
```

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/map.py` & `imap_box_up-0.0.2/imap/lib/opendrive/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/plan_view.py` & `imap_box_up-0.0.2/imap/lib/opendrive/plan_view.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/profile.py` & `imap_box_up-0.0.2/imap/lib/opendrive/profile.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/road.py` & `imap_box_up-0.0.2/imap/lib/opendrive/road.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/signals.py` & `imap_box_up-0.0.2/imap/lib/opendrive/signals.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/opendrive/user_data.py` & `imap_box_up-0.0.2/imap/lib/opendrive/user_data.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/polynoms.py` & `imap_box_up-0.0.2/imap/lib/polynoms.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/proj_helper.py` & `imap_box_up-0.0.2/imap/lib/proj_helper.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/lib/proto_utils.py` & `imap_box_up-0.0.2/imap/lib/proto_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-#!/usr/bin/env python
-
-# Copyright 2021 daohu527 <daohu527@gmail.com>
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-###############################################################################
-# Copyright 2017 The Apollo Authors. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-# http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-###############################################################################
-"""Protobuf utils."""
-
-import traceback
-
-import google.protobuf.text_format as text_format
-
-
-def write_pb_to_text_file(topic_pb, file_path):
-    """write pb message to file"""
-    file_name = "{}.txt".format(file_path)
-    with open(file_name, 'w') as f:
-        f.write(str(topic_pb))
-        print("File success saved in: {}".format(file_name))
-
-def write_pb_to_bin_file(topic_pb, file_path):
-    """write pb message to file
-
-    Args:
-        topic_pb ([object]): [protobuf file]
-        file_path ([string]): [file path]
-    """
-    file_name = "{}.bin".format(file_path)
-    with open(file_name, 'wb') as f:
-        f.write(topic_pb.SerializeToString())
-        print("File success saved in: {}".format(file_name))
-
-
-def get_pb_from_text_file(filename, pb_value):
-    """Get a proto from given text file."""
-    with open(filename, 'r') as file_in:
-        return text_format.Merge(file_in.read(), pb_value)
-
-
-def get_pb_from_bin_file(filename, pb_value):
-    """Get a proto from given binary file."""
-    with open(filename, 'rb') as file_in:
-        pb_value.ParseFromString(file_in.read())
-    return pb_value
-
-
-def get_pb_from_file(filename, pb_value):
-    """Get a proto from given file by trying binary mode and text mode."""
-    try:
-        return get_pb_from_bin_file(filename, pb_value)
-    except:
-        try:
-            return get_pb_from_text_file(filename, pb_value)
-        except:
-            traceback.print_exc()
-            print('Error: Cannot parse %s as binary or text proto', filename)
-    return None
-
-
-def flatten(pb_value, selectors):
-    """
-    Get a flattened tuple from pb_value. Selectors is a list of sub-fields.
-
-    Usage:
-    For a pb_value of:
-        total_pb = {
-            me: { name: 'myself' }
-            children: [{ name: 'child0' }, { name: 'child1' }]
-        }
-    my_name, child0_name = flatten(total_pb, ['me.name', 'children[0].name'])
-    # You get (my_name='myself', child0_name='child0')
-
-    children_names = flatten(total_pb, 'children.name')
-    # You get (children_names=['child0', 'child1'])
-    """
-
-    def __select_field(val, field):
-        if hasattr(val, '__len__'):
-            # Flatten repeated field.
-            return [__select_field(elem, field) for elem in val]
-        if not field.endswith(']'):
-            # Simple field.
-            return val.__getattribute__(field)
-        # field contains index: "field[index]".
-        field, index = field.split('[')
-        val = val.__getattribute__(field)
-        index = int(index[:-1])
-        return val[index] if index < len(val) else None
-
-    def __select(val, selector):
-        for field in selector.split('.'):
-            val = __select_field(val, field)
-            if val is None:
-                return None
-        return val
-
-    # Return the single result for single selector.
-    if isinstance(selectors, str):
-        return __select(pb_value, selectors)
-    # Return tuple result for multiple selectors.
-    return tuple((__select(pb_value, selector) for selector in selectors))
+#!/usr/bin/env python
+
+# Copyright 2021 daohu527 <daohu527@gmail.com>
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+###############################################################################
+# Copyright 2017 The Apollo Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+# http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+###############################################################################
+"""Protobuf utils."""
+
+import traceback
+
+import google.protobuf.text_format as text_format
+
+
+def write_pb_to_text_file(topic_pb, file_path):
+    """write pb message to file"""
+    file_name = "{}.txt".format(file_path)
+    with open(file_name, 'w') as f:
+        f.write(str(topic_pb))
+        print("File success saved in: {}".format(file_name))
+
+def write_pb_to_bin_file(topic_pb, file_path):
+    """write pb message to file
+
+    Args:
+        topic_pb ([object]): [protobuf file]
+        file_path ([string]): [file path]
+    """
+    file_name = "{}.bin".format(file_path)
+    with open(file_name, 'wb') as f:
+        f.write(topic_pb.SerializeToString())
+        print("File success saved in: {}".format(file_name))
+
+
+def get_pb_from_text_file(filename, pb_value):
+    """Get a proto from given text file."""
+    with open(filename, 'r') as file_in:
+        return text_format.Merge(file_in.read(), pb_value)
+
+
+def get_pb_from_bin_file(filename, pb_value):
+    """Get a proto from given binary file."""
+    with open(filename, 'rb') as file_in:
+        pb_value.ParseFromString(file_in.read())
+    return pb_value
+
+
+def get_pb_from_file(filename, pb_value):
+    """Get a proto from given file by trying binary mode and text mode."""
+    try:
+        return get_pb_from_bin_file(filename, pb_value)
+    except:
+        try:
+            return get_pb_from_text_file(filename, pb_value)
+        except:
+            traceback.print_exc()
+            print('Error: Cannot parse %s as binary or text proto', filename)
+    return None
+
+
+def flatten(pb_value, selectors):
+    """
+    Get a flattened tuple from pb_value. Selectors is a list of sub-fields.
+
+    Usage:
+    For a pb_value of:
+        total_pb = {
+            me: { name: 'myself' }
+            children: [{ name: 'child0' }, { name: 'child1' }]
+        }
+    my_name, child0_name = flatten(total_pb, ['me.name', 'children[0].name'])
+    # You get (my_name='myself', child0_name='child0')
+
+    children_names = flatten(total_pb, 'children.name')
+    # You get (children_names=['child0', 'child1'])
+    """
+
+    def __select_field(val, field):
+        if hasattr(val, '__len__'):
+            # Flatten repeated field.
+            return [__select_field(elem, field) for elem in val]
+        if not field.endswith(']'):
+            # Simple field.
+            return val.__getattribute__(field)
+        # field contains index: "field[index]".
+        field, index = field.split('[')
+        val = val.__getattribute__(field)
+        index = int(index[:-1])
+        return val[index] if index < len(val) else None
+
+    def __select(val, selector):
+        for field in selector.split('.'):
+            val = __select_field(val, field)
+            if val is None:
+                return None
+        return val
+
+    # Return the single result for single selector.
+    if isinstance(selectors, str):
+        return __select(pb_value, selectors)
+    # Return tuple result for multiple selectors.
+    return tuple((__select(pb_value, selector) for selector in selectors))
```

### Comparing `imap_box_up-0.0.1/imap/lib/transform.py` & `imap_box_up-0.0.2/imap/lib/transform.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap/main.py` & `imap_box_up-0.0.2/imap/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,38 +23,39 @@
 
 import imap.global_var as global_var
 
 from imap.lib.draw import add_editor, show_map
 from imap.lib.convertor import Opendrive2Apollo
 
 
-def convert_map_format(input_path, output_path, relative):
+def convert_map_format(input_path, output_path, relative, junctionbox=False):
     opendrive2apollo = Opendrive2Apollo(input_path, output_path)
     # todo(zero): only lane type is driving add relationship!!!
     opendrive2apollo.set_parameters(only_driving=False)
-    opendrive2apollo.convert(relative)
+    opendrive2apollo.convert(relative, junctionbox)
     opendrive2apollo.save_map()
 
 
 def show_open_drive_map(map_file):
     opendrive2apollo = Opendrive2Apollo(map_file)
     opendrive2apollo.set_parameters(only_driving=False)
     opendrive2apollo.convert()
 
 
 def main(args=sys.argv):
     parser = argparse.ArgumentParser(
         description="Imap is a tool to display hdmap info on a map.",
-        prog="main.py",
+        prog="imap_box_up",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog='eg:\n \
-    1.show appollo map by id: imap -m data/borregas_ave.txt -l lane_35 \n \
-    2.Format conversion with UTM map(opendrive->appollo): imap -f -i data/town.xodr -o data/apollo_map.txt \n \
-    3.Format conversion with relative map(opendrive->appollo.relative map): imap -f -r -i data/town.xodr -o data/apollo_map.txt \n \
-    Notice:\
+    1.show appollo map by id: imap_box_up -m data/borregas_ave.txt -l lane_35 \n \
+    2.Format conversion with UTM map(opendrive->appollo): imap_box_up -f -i data/town.xodr -o data/apollo_map.txt \n \
+    3.Format conversion with relative map(opendrive->appollo.relative map, recommend): imap_box_up -f -r -i data/town.xodr -o data/apollo_map.txt \n \
+    4.if you want convert map junction with box(not recommend): imap_box_up -f -r -b -i data/town.xodr -o data/apollo_map.txt \n \
+    Notice:\n \
     1.After running the command imap -m data/your_map_file, nothing display and no errors!!! \n \
         step1:Check the permissions: sudo chmod 777 data/your_map_file \n \
     if step1 no solve the problem, you can try sudo pip install xxx again. \n \
     2.Other Problem you can contact porter.pan@outlook.com \n \
     3.code modified from: https://github.com/daohu527/imap '
         )
 
@@ -85,15 +86,17 @@
         default=1.0, help="sampling length")
     parser.add_argument(
         "-d", "--debug", action="store", type=bool, required=False,
         nargs='?', const=True, default=False, help="debug mode")
     parser.add_argument(
         "-r", "--relative", action="store", type=bool, required=False,
         nargs='?', default=False, help="convert opendrive map to appollo map without GIS projection")
-
+    parser.add_argument(
+        "-b", "--box", action="store", type=bool, required=False,
+        nargs='?', default=False, help="convert opendrive map to appollo map junction with box(not recommend)")
     args = parser.parse_args(args[1:])
 
     # 1. Init global var
     global_var._init()
     global_var.set_element_vaule("sampling_length", args.sampling)
     global_var.set_element_vaule("debug_mode", args.debug)
     global_var.set_element_vaule("enable_z_axis", args.enable_z_axis)
@@ -116,11 +119,11 @@
 
     # 3. convert opendrive map to apollo
     if args.format is not None:
         map_file = Path(args.input)
         if not map_file.is_file():
             logging.error("File not exist! '{}'".format(args.input))
             return
-        convert_map_format(args.input, args.output, args.relative)
+        convert_map_format(args.input, args.output, args.relative, args.box)
 
 if __name__ == '__main__':
   main(args=sys.argv)
```

### Comparing `imap_box_up-0.0.1/imap/map.py` & `imap_box_up-0.0.2/imap/map.py`

 * *Files identical despite different names*

### Comparing `imap_box_up-0.0.1/imap_box_up.egg-info/PKG-INFO` & `imap_box_up-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,125 @@
-Metadata-Version: 2.1
-Name: imap-box-up
-Version: 0.0.1
-Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
-Home-page: https://github.com/porterpan/imap_box_up
-Author: porter
-Author-email: porter.pan@outlook.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE-2.0.txt
-
-# imap
-
-[![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
-
-**[imap](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo. 
-
-I called the modified with **imap_box_up** , Just to differentiate it from imap_box
-
-imap_box_up code: https://github.com/porterpan/imap_box_up
-
-**Note:**
-
-Modified on project [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
-
-> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
-
-
-
-![example]([eg1.png](https://private-user-images.githubusercontent.com/30954452/321745045-d23d05d2-66a4-4690-bf17-073c7fd4bbe3.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI4NjA3NjQsIm5iZiI6MTcxMjg2MDQ2NCwicGF0aCI6Ii8zMDk1NDQ1Mi8zMjE3NDUwNDUtZDIzZDA1ZDItNjZhNC00NjkwLWJmMTctMDczYzdmZDRiYmUzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA0MTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNDExVDE4MzQyNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTE4NDYyY2ZkZjQxMjQ2YTZiZmVmMWI2YTg3ZTA3NGZlMzNjNTY3ZTIxZDFhZDY1NjdlZWFiYWM1YTk2YjI0MTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.GhurdLnE04-8-OwlWQF2VWgymB4e-EX-hAONUX1pQaM))
-
-**Supported features**:
-1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
-2. Find lane by id
-3. Convert format: Opendrive to Apollo format.
-
-| os      | support                 | remark |
-|---------|-------------------------|--------|
-| ubuntu  | :heavy_check_mark:      |        |
-| mac     | :heavy_check_mark:      |        |
-| windows | :heavy_check_mark:      |        |
-
-## Related work
-- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
-- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
-- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
-
-## Quick start
-
-#### Install
-You can install imap by following cmd.
-```shell
-pip3 install imap_box_up
-```
-
-## Example
-#### 1. Visualization
-After the installation is complete, you can view the map with the following command.
-```shell
-imap -m data/borregas_ave.txt
-// or
-imap -m data/town.xodr
-```
-Currently supported formats:
-* Apollo map
-* OpenDrive map
-
-#### 2. Find lane by id
-You can use below command to find lane by id, Found lane is shown in **Red**.
-```shell
-imap -m data/borregas_ave.txt -l lane_35
-```
-
-#### 3. Format conversion
-Now you can convert OpenDrive map to Apollo map by following command.
-```shell
-imap -f -i data/town.xodr -o data/apollo_map.txt
-```
-you should better reference follow command to convert apollo map to OpenDrive map.
-
- 1.show appollo map by id:
-
- ```shell
- imap -m data/borregas_ave.txt -l lane_35
- ```
-
-2.Format conversion with UTM map(opendrive->appollo): 
-
-```shell
-imap -f -i data/town.xodr -o data/apollo_map.txt
-```
-3.Format conversion with inertial map(opendrive->appollo.inertial map):
-
-```shell
-imap -f -r -i data/town.xodr -o data/apollo_map.txt
-```
-
-
-
-The following is the display of the hd-map in `data\borregas_ave.txt`.You can click on the lane you want to display more detail info, which will display the current lane's id, as well as the predecessor and successor lane's id in the upper left corner.
-
-![map_show](docs/_static/map_show.jpg)
-
-
-## Questions
-1. After running the command `imap -m data/your_map_file`, nothing display and no errors!!!
-
-A: Check the permissions of the map file, if the current user does not have permissions, modify the permissions with the following commands.
-```shell
-sudo chmod 777 data/your_map_file
-```
-2. Map data permission checking has no problem, still nothing display and no errors!
-A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
-
-
+Metadata-Version: 2.1
+Name: imap_box_up
+Version: 0.0.2
+Summary: High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!
+Home-page: https://github.com/porterpan/imap_box_up
+Author: porter
+Author-email: porter.pan@outlook.com
+Project-URL: Bug Tracker, https://github.com/porterpan/imap_box_up/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: protobuf<=3.19.4
+Requires-Dist: matplotlib
+Requires-Dist: pyproj
+Requires-Dist: record_msg<=0.1.1
+Requires-Dist: concave-hull<=0.0.7
+Requires-Dist: scipy<=1.13.0
+
+# imap
+
+[![Documentation Status](https://readthedocs.org/projects/imap/badge/?version=latest)](https://imap.readthedocs.io/en/latest/?badge=latest)
+
+**[imap_box_up](https://imap.readthedocs.io/en/latest/)** is a tool for visualize and convert format of the hd-map. This project was inspired by Apollo, modified by [imap](https://github.com/daohu527/imap), the imap tool is very useful. 
+
+The name of **imap_box_up** , Just to modified from imap_box
+
+The modified tool is named **imap_box_up** just to distinguish it from **imap_box**
+
+imap_box_up source code: [https://github.com/porterpan/imap_box_up](https://github.com/porterpan/imap_box_up)
+
+**Note:**
+
+The project is Modify on project of [https://github.com/daohu527/imap](https://github.com/daohu527/imap)
+
+> I found that imap_box had the problem of inaccurate junction drawing, which could not meet the needs of my project. Therefore, I modified imap_box based on it to adapt to appollo hdmap code. 
+
+## now(fix junction bug)
+
+![valid junction](https://img2.imgtp.com/2024/04/12/aHEcAl7a.png)
+
+![junction detail](https://img2.imgtp.com/2024/04/12/Ct9V2l51.png)
+
+## the old tool bug
+
+![invalid junction](https://img2.imgtp.com/2024/04/12/hOWOvqyr.jpg)
+
+![junction error](https://imap.readthedocs.io/en/latest/_images/map_show.jpg)
+
+
+**Supported features**:
+1. Visualize the hd-map, supported formats: Apollo, OpenDrive.
+2. Find lane by id
+3. Convert format: Opendrive to Apollo format.
+
+| os      | support                 | remark |
+|---------|-------------------------|--------|
+| ubuntu  | :heavy_check_mark:      |        |
+| mac     | :heavy_check_mark:      |        |
+| windows | :heavy_check_mark:      |        |
+
+## Related work
+- [odrviewer.io](https://odrviewer.io/) is an excellent interactive online OpenDRIVE viewer.
+- [esmini](https://github.com/esmini/esmini) is a basic OpenSCENARIO player.
+- [apollo_map](https://github.com/Flycars/apollo_map) convert carla map to apollo
+
+## Quick start
+
+#### Install
+You can install imap by following cmd.
+```shell
+pip3 install imap_box_up
+```
+
+## Example
+#### 1. Visualization
+After the installation is complete, you can view the map with the following command.
+```shell
+imap_box_up -m data/borregas_ave.txt
+// or
+imap_box_up -m data/town.xodr
+```
+Currently supported formats:
+* Apollo map
+* OpenDrive map
+
+#### 2. Find lane by id
+You can use below command to find lane by id, Found lane is shown in **Red**.
+```shell
+imap_box_up -m data/borregas_ave.txt -l lane_35
+```
+
+#### 3. Format conversion
+Now you can convert OpenDrive map to Apollo map by following command.
+
+- save as utm world coordinates(**world map** for old feature)
+```shell
+imap_box_up -f -i data/town.xodr -o data/apollo_map.txt
+```
+
+- save as inertial system coordinates (**relative map** for new feature)
+
+```shell
+imap_box_up -f -r -i data/town.xodr -o data/apollo_map.txt
+```
+
+
+The following is the display of the hd-map in `data\borregas_ave.txt`.You can click on the lane you want to display more detail info, which will display the current lane's id, as well as the predecessor and successor lane's id in the upper left corner.
+
+![imap_box_up convert map load to rviz display](https://img2.imgtp.com/2024/04/12/a1QPsCb2.png)
+
+
+## Questions
+1. After running the command `imap_box_up -m data/your_map_file`, nothing display and no errors!!!
+
+A: Check the permissions of the map file, if the current user does not have permissions, modify the permissions with the following commands.
+```shell
+sudo chmod 777 data/your_map_file
+```
+2. Map data permission checking has no problem, still nothing display and no errors!
+A: It's better to install imap_box by running "sudo pip3 install imap_box", then run "imap -m xxx.txt".
+
+> If you have any questions, please feel free to contact me.
```

### Comparing `imap_box_up-0.0.1/setup.py` & `imap_box_up-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imap_box_up",
-    version="0.0.1",
+    version="0.0.2",
     author="porter",
     author_email="porter.pan@outlook.com",
     description="High-resolution map visualization and conversion tool, opendrive hdmap convert to appollo base map!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/porterpan/imap_box_up",
     project_urls={
```

