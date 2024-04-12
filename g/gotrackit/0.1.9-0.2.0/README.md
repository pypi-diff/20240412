# Comparing `tmp/gotrackit-0.1.9.tar.gz` & `tmp/gotrackit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotrackit-0.1.9.tar", last modified: Thu Mar 28 03:54:39 2024, max compression
+gzip compressed data, was "gotrackit-0.2.0.tar", last modified: Fri Apr 12 07:59:26 2024, max compression
```

## Comparing `gotrackit-0.1.9.tar` & `gotrackit-0.2.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.135253 gotrackit-0.1.9/
--rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     4857 2024-03-28 03:54:39.134256 gotrackit-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     4111 2024-03-28 00:46:46.000000 gotrackit-0.1.9/README.md
--rw-rw-rw-   0        0        0      795 2024-03-28 03:51:17.000000 gotrackit-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-28 03:54:39.135253 gotrackit-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.047440 gotrackit-0.1.9/src/
--rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.1.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.052427 gotrackit-0.1.9/src/gotrackit/
--rw-rw-rw-   0        0        0    15214 2024-03-27 01:02:12.000000 gotrackit-0.1.9/src/gotrackit/GlobalVal.py
--rw-rw-rw-   0        0        0     9387 2024-03-27 16:13:09.000000 gotrackit-0.1.9/src/gotrackit/MapMatch.py
--rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.1.9/src/gotrackit/WrapsFunc.py
--rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.1.9/src/gotrackit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.060405 gotrackit-0.1.9/src/gotrackit/generation/
--rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.1.9/src/gotrackit/generation/GpsGen.py
--rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.1.9/src/gotrackit/generation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.064394 gotrackit-0.1.9/src/gotrackit/gps/
--rw-rw-rw-   0        0        0     4261 2024-03-27 05:40:59.000000 gotrackit-0.1.9/src/gotrackit/gps/GpsArray.py
--rw-rw-rw-   0        0        0     5518 2024-03-26 05:31:59.000000 gotrackit-0.1.9/src/gotrackit/gps/GpsTrip.py
--rw-rw-rw-   0        0        0    21313 2024-03-27 15:05:04.000000 gotrackit-0.1.9/src/gotrackit/gps/LocGps.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.1.9/src/gotrackit/gps/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.069382 gotrackit-0.1.9/src/gotrackit/map/
--rw-rw-rw-   0        0        0    19541 2024-03-27 12:44:31.000000 gotrackit-0.1.9/src/gotrackit/map/Link.py
--rw-rw-rw-   0        0        0    23155 2024-03-28 03:18:55.000000 gotrackit-0.1.9/src/gotrackit/map/Net.py
--rw-rw-rw-   0        0        0     4589 2024-03-27 12:44:31.000000 gotrackit-0.1.9/src/gotrackit/map/Node.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.1.9/src/gotrackit/map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.071376 gotrackit-0.1.9/src/gotrackit/model/
--rw-rw-rw-   0        0        0    44664 2024-03-28 03:49:29.000000 gotrackit-0.1.9/src/gotrackit/model/Markov.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.1.9/src/gotrackit/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.076362 gotrackit-0.1.9/src/gotrackit/netreverse/
--rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.1.9/src/gotrackit/netreverse/GlobalVal.py
--rw-rw-rw-   0        0        0    23983 2024-03-28 03:42:10.000000 gotrackit-0.1.9/src/gotrackit/netreverse/NetGen.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.078357 gotrackit-0.1.9/src/gotrackit/netreverse/Parse/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Parse/__init__.py
--rw-rw-rw-   0        0        0    19074 2024-03-17 13:01:30.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Parse/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.084342 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/
--rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/GeoProcess.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/GraphAna.py
--rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/IndexAna.py
--rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/MapProcess.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/__init__.py
--rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/od.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.085339 gotrackit-0.1.9/src/gotrackit/netreverse/Request/
--rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.088331 gotrackit-0.1.9/src/gotrackit/netreverse/Request/api/
--rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/api/WebApi.py
--rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/api/__init__.py
--rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/request_path.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.090362 gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/
--rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/__init__.py
--rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/bd_ts.py
--rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/gd_car_path.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.096357 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.098352 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/DupProcess/
--rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.104342 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/
--rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.109322 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.114309 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
--rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
--rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/get_merged_link_seq.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.120293 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
--rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
--rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
--rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
--rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
--rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links.py
--rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_short.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.122287 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/SaveStreets/
--rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
--rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.124282 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Split/
--rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.126277 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Tools/
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
--rw-rw-rw-   0        0        0     5047 2024-03-05 02:20:24.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Tools/process.py
--rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/__init__.py
--rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/conn.py
--rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/increment.py
--rw-rw-rw-   0        0        0     8807 2024-03-28 03:28:26.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/net_reverse.py
--rw-rw-rw-   0        0        0     4452 2024-03-16 12:30:07.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/optimize_net.py
--rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/save_file.py
--rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.1.9/src/gotrackit/netreverse/__init__.py
--rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.1.9/src/gotrackit/netreverse/book_mark.py
--rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.1.9/src/gotrackit/netreverse/format_od.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.128271 gotrackit-0.1.9/src/gotrackit/solver/
--rw-rw-rw-   0        0        0     9181 2024-03-25 06:12:09.000000 gotrackit-0.1.9/src/gotrackit/solver/Viterbi.py
--rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.1.9/src/gotrackit/solver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.132264 gotrackit-0.1.9/src/gotrackit/tools/
--rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.1.9/src/gotrackit/tools/__init__.py
--rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.1.9/src/gotrackit/tools/coord_trans.py
--rw-rw-rw-   0        0        0    11487 2024-03-28 03:42:10.000000 gotrackit-0.1.9/src/gotrackit/tools/geo_process.py
--rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.1.9/src/gotrackit/tools/save_file.py
--rw-rw-rw-   0        0        0     4996 2024-03-27 15:41:55.000000 gotrackit-0.1.9/src/gotrackit/visualization.py
-drwxrwxrwx   0        0        0        0 2024-03-28 03:54:39.133258 gotrackit-0.1.9/src/gotrackit.egg-info/
--rw-rw-rw-   0        0        0     4857 2024-03-28 03:54:39.000000 gotrackit-0.1.9/src/gotrackit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3694 2024-03-28 03:54:39.000000 gotrackit-0.1.9/src/gotrackit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 03:54:39.000000 gotrackit-0.1.9/src/gotrackit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-03-28 03:54:39.000000 gotrackit-0.1.9/src/gotrackit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-28 03:54:39.000000 gotrackit-0.1.9/src/gotrackit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.428638 gotrackit-0.2.0/
+-rw-rw-rw-   0        0        0     1085 2024-01-01 15:23:01.000000 gotrackit-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4886 2024-04-12 07:59:26.427641 gotrackit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4140 2024-04-12 07:45:08.000000 gotrackit-0.2.0/README.md
+-rw-rw-rw-   0        0        0      795 2024-04-12 03:50:07.000000 gotrackit-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:59:26.428638 gotrackit-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.339875 gotrackit-0.2.0/src/
+-rw-rw-rw-   0        0        0      101 2023-12-09 00:21:11.000000 gotrackit-0.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.345859 gotrackit-0.2.0/src/gotrackit/
+-rw-rw-rw-   0        0        0    15398 2024-04-04 05:30:17.000000 gotrackit-0.2.0/src/gotrackit/GlobalVal.py
+-rw-rw-rw-   0        0        0    11426 2024-04-12 07:23:48.000000 gotrackit-0.2.0/src/gotrackit/MapMatch.py
+-rw-rw-rw-   0        0        0      624 2023-12-31 13:24:06.000000 gotrackit-0.2.0/src/gotrackit/WrapsFunc.py
+-rw-rw-rw-   0        0        0      102 2024-01-18 03:53:10.000000 gotrackit-0.2.0/src/gotrackit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.351843 gotrackit-0.2.0/src/gotrackit/generation/
+-rw-rw-rw-   0        0        0    25084 2024-03-27 15:57:38.000000 gotrackit-0.2.0/src/gotrackit/generation/GpsGen.py
+-rw-rw-rw-   0        0        0      103 2023-12-30 07:52:41.000000 gotrackit-0.2.0/src/gotrackit/generation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.354836 gotrackit-0.2.0/src/gotrackit/gps/
+-rw-rw-rw-   0        0        0     4291 2024-04-10 08:42:29.000000 gotrackit-0.2.0/src/gotrackit/gps/GpsArray.py
+-rw-rw-rw-   0        0        0     8007 2024-04-12 03:06:11.000000 gotrackit-0.2.0/src/gotrackit/gps/GpsTrip.py
+-rw-rw-rw-   0        0        0    21814 2024-04-11 02:47:55.000000 gotrackit-0.2.0/src/gotrackit/gps/LocGps.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/gps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.360824 gotrackit-0.2.0/src/gotrackit/map/
+-rw-rw-rw-   0        0        0    19202 2024-04-11 02:00:49.000000 gotrackit-0.2.0/src/gotrackit/map/Link.py
+-rw-rw-rw-   0        0        0    23292 2024-04-11 01:53:49.000000 gotrackit-0.2.0/src/gotrackit/map/Net.py
+-rw-rw-rw-   0        0        0     4607 2024-04-09 00:43:47.000000 gotrackit-0.2.0/src/gotrackit/map/Node.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.362814 gotrackit-0.2.0/src/gotrackit/model/
+-rw-rw-rw-   0        0        0    52888 2024-04-12 02:40:08.000000 gotrackit-0.2.0/src/gotrackit/model/Markov.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.367801 gotrackit-0.2.0/src/gotrackit/netreverse/
+-rw-rw-rw-   0        0        0     1657 2024-01-31 02:46:45.000000 gotrackit-0.2.0/src/gotrackit/netreverse/GlobalVal.py
+-rw-rw-rw-   0        0        0    26881 2024-04-12 03:06:11.000000 gotrackit-0.2.0/src/gotrackit/netreverse/NetGen.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.368798 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/__init__.py
+-rw-rw-rw-   0        0        0    19151 2024-04-10 05:04:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Parse/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.377774 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/
+-rw-rw-rw-   0        0        0     3697 2024-01-27 14:10:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GeoProcess.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GraphAna.py
+-rw-rw-rw-   0        0        0     1649 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/IndexAna.py
+-rw-rw-rw-   0        0        0      221 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/MapProcess.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/__init__.py
+-rw-rw-rw-   0        0        0     4362 2024-03-07 05:54:15.000000 gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/od.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.378772 gotrackit-0.2.0/src/gotrackit/netreverse/Request/
+-rw-rw-rw-   0        0        0        0 2023-12-12 03:03:06.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.380766 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/
+-rw-rw-rw-   0        0        0     3812 2024-01-29 14:05:19.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/WebApi.py
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:05:25.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/__init__.py
+-rw-rw-rw-   0        0        0     3093 2024-01-29 11:43:10.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/request_path.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.382760 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/
+-rw-rw-rw-   0        0        0      103 2023-12-12 04:10:22.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/__init__.py
+-rw-rw-rw-   0        0        0     7809 2024-01-28 14:46:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/bd_ts.py
+-rw-rw-rw-   0        0        0    11231 2024-01-31 07:13:59.000000 gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/gd_car_path.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.390740 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.393736 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/
+-rw-rw-rw-   0        0        0    21741 2024-03-18 03:07:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.397720 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/
+-rw-rw-rw-   0        0        0      103 2023-12-18 12:14:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/__init__.py
+-rw-rw-rw-   0        0        0     6874 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.401710 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     9459 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    12225 2024-03-06 12:24:39.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py
+-rw-rw-rw-   0        0        0    15086 2024-01-27 08:21:05.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.403705 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/
+-rw-rw-rw-   0        0        0      102 2024-03-17 11:27:43.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.410686 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
+-rw-rw-rw-   0        0        0    18675 2024-01-27 07:25:52.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
+-rw-rw-rw-   0        0        0    11592 2024-01-31 01:26:21.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
+-rw-rw-rw-   0        0        0     2865 2024-01-27 07:40:20.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
+-rw-rw-rw-   0        0        0     8948 2024-04-08 05:51:27.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
+-rw-rw-rw-   0        0        0    21559 2024-04-12 02:47:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.412680 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/
+-rw-rw-rw-   0        0        0      134 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
+-rw-rw-rw-   0        0        0    21115 2024-03-15 13:54:11.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.413678 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/
+-rw-rw-rw-   0        0        0     4266 2024-01-29 13:44:04.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.415672 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/__init__.py
+-rw-rw-rw-   0        0        0     5745 2024-04-08 08:18:36.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/process.py
+-rw-rw-rw-   0        0        0      133 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/__init__.py
+-rw-rw-rw-   0        0        0     9629 2024-03-27 15:52:33.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/conn.py
+-rw-rw-rw-   0        0        0    18855 2024-03-09 13:07:40.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/increment.py
+-rw-rw-rw-   0        0        0     9043 2024-04-08 07:19:18.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/net_reverse.py
+-rw-rw-rw-   0        0        0     5765 2024-04-12 02:47:41.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/optimize_net.py
+-rw-rw-rw-   0        0        0     1188 2024-03-05 08:17:38.000000 gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/save_file.py
+-rw-rw-rw-   0        0        0        0 2023-12-16 09:25:56.000000 gotrackit-0.2.0/src/gotrackit/netreverse/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-01-29 14:01:55.000000 gotrackit-0.2.0/src/gotrackit/netreverse/book_mark.py
+-rw-rw-rw-   0        0        0     1868 2024-01-27 14:19:15.000000 gotrackit-0.2.0/src/gotrackit/netreverse/format_od.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.417668 gotrackit-0.2.0/src/gotrackit/netxfer/
+-rw-rw-rw-   0        0        0    17197 2024-03-31 15:04:35.000000 gotrackit-0.2.0/src/gotrackit/netxfer/SumoConvert.py
+-rw-rw-rw-   0        0        0      101 2024-03-30 00:52:12.000000 gotrackit-0.2.0/src/gotrackit/netxfer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.418665 gotrackit-0.2.0/src/gotrackit/solver/
+-rw-rw-rw-   0        0        0     9181 2024-04-03 02:13:18.000000 gotrackit-0.2.0/src/gotrackit/solver/Viterbi.py
+-rw-rw-rw-   0        0        0      103 2023-12-31 04:37:58.000000 gotrackit-0.2.0/src/gotrackit/solver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.425646 gotrackit-0.2.0/src/gotrackit/tools/
+-rw-rw-rw-   0        0        0      102 2024-01-10 02:23:14.000000 gotrackit-0.2.0/src/gotrackit/tools/__init__.py
+-rw-rw-rw-   0        0        0    10646 2024-03-05 06:26:07.000000 gotrackit-0.2.0/src/gotrackit/tools/coord_trans.py
+-rw-rw-rw-   0        0        0    12119 2024-04-08 08:18:36.000000 gotrackit-0.2.0/src/gotrackit/tools/geo_process.py
+-rw-rw-rw-   0        0        0      812 2024-04-12 02:40:08.000000 gotrackit-0.2.0/src/gotrackit/tools/group.py
+-rw-rw-rw-   0        0        0     1121 2024-01-31 04:02:14.000000 gotrackit-0.2.0/src/gotrackit/tools/save_file.py
+-rw-rw-rw-   0        0        0     5360 2024-04-04 06:01:58.000000 gotrackit-0.2.0/src/gotrackit/visualization.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:59:26.426643 gotrackit-0.2.0/src/gotrackit.egg-info/
+-rw-rw-rw-   0        0        0     4886 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3666 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-12 07:59:26.000000 gotrackit-0.2.0/src/gotrackit.egg-info/top_level.txt
```

### Comparing `gotrackit-0.1.9/LICENSE` & `gotrackit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/PKG-INFO` & `gotrackit-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,48 +16,74 @@
 Requires-Dist: shapely
 Requires-Dist: networkx
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: keplergl
 Requires-Dist: geopy
 
-# GoTrackIt
+
+![car_gps.png](docs/_static/images/gotrackit.png)
+
+
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
-
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**2024.03.29即将更新: v0.1.9**
+**04.12已更新: v0.2.0**
 
-- 增加GPS增密功能
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 引入GPS点差分方向向量来修正发射概率
+- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
 
-- 地图匹配接口升级，使用更加简单，暴露了更多的[可调参数](https://gotrackit.readthedocs.io/en/latest/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8.html#id36)
+- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
 
-- 构建Net对象限制为：输入的link和node的数据必须为WGS-84 EPSG:4326地理坐标，平面投影坐标系不再需要手动指定，可自动进行6度带的确定
+- 增加GPS点停留点识别功能
 
-- 增加了路网处理函数：路段划分功能
+- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
 
-- 增加了路网处理函数：路段-link_id字段、from_node字段、to_node字段，节点-node_id字段重映射函数
+- 增加依据GPS数据提取带途径点OD的功能
 
-- 修复GPS生成接口中速度为负数的BUG
+- 增加了路网处理函数：路段、节点重塑
 
-- 修复Net初始化过程中由于节点ID过大导致内存溢出的问题
+- 修复了部分BUG
 
-- 新增路径缓存开关、ID缓存开关参数
 
 遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
+<div align="center">
+    <img src="docs/_static/images/l_f.gif" />
+</div>
+
+<div align="center">
+    <img src="docs/_static/images/m_h_f.gif" />
+</div>
+
+稀疏轨迹增密匹配：
+
+<div align="center">
+    <img src="docs/_static/images/dense_gps.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/taxi_xishu.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/xa_sample.gif" />
+</div>
+
+
 ![car_gps.png](docs/_static/images/wxq.jpg)
 
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
@@ -76,22 +102,23 @@
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
-- geopandas(0.14.1)
 - geopy(2.4.1)
 - gdal(3.4.3)
+- shapely(2.0.3)
+- fiona(1.9.5)
+- pyproj(3.6.1)
+- geopandas(0.14.3)
 - networkx(3.2.1)
-- shapely(2.0.2)
 - pandas(2.0.3)
 - numpy(1.26.2)
-- pyproj(3.6.1)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
 geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
 
 #### __使用pip安装__
@@ -103,45 +130,37 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册
+### 1.2 用户手册与视频教程
+
+[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+
+[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+
+[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)、
-[视频教程1](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)、
-[视频教程2](https://www.bilibili.com/video/BV1nC411z7Vg/?share_source=copy_web&vd_source=9b4518c7de4757ad3b99e18456efbaa6)
+[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
 
 __如何依据GPS数据推算车辆的实际路径？__
 
-## 3. 地图匹配算法动画演示
-
-想了解算法过程的可以参考B站视频:
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)
-
 ![main.png](docs/_static/images/single_p.png)
 
 ![main.png](docs/_static/images/transition.png)
 
 ![main.png](docs/_static/images/viterbi.png)
 
 ![main.png](docs/_static/images/trace.png)
 
 
-## 4. 匹配结果可视化
-
-中高频GPS匹配效果:
-
-![main.png](docs/_static/images/m_h_f.gif)
-
-低频GPS匹配效果:
-
-![main.png](docs/_static/images/l_f.gif)
```

### Comparing `gotrackit-0.1.9/README.md` & `gotrackit-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,67 @@
-# GoTrackIt
+
+![car_gps.png](docs/_static/images/gotrackit.png)
+
+
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
-
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**2024.03.29即将更新: v0.1.9**
+**04.12已更新: v0.2.0**
 
-- 增加GPS增密功能
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 引入GPS点差分方向向量来修正发射概率
+- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
 
-- 地图匹配接口升级，使用更加简单，暴露了更多的[可调参数](https://gotrackit.readthedocs.io/en/latest/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8.html#id36)
+- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
 
-- 构建Net对象限制为：输入的link和node的数据必须为WGS-84 EPSG:4326地理坐标，平面投影坐标系不再需要手动指定，可自动进行6度带的确定
+- 增加GPS点停留点识别功能
 
-- 增加了路网处理函数：路段划分功能
+- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
 
-- 增加了路网处理函数：路段-link_id字段、from_node字段、to_node字段，节点-node_id字段重映射函数
+- 增加依据GPS数据提取带途径点OD的功能
 
-- 修复GPS生成接口中速度为负数的BUG
+- 增加了路网处理函数：路段、节点重塑
 
-- 修复Net初始化过程中由于节点ID过大导致内存溢出的问题
+- 修复了部分BUG
 
-- 新增路径缓存开关、ID缓存开关参数
 
 遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
+<div align="center">
+    <img src="docs/_static/images/l_f.gif" />
+</div>
+
+<div align="center">
+    <img src="docs/_static/images/m_h_f.gif" />
+</div>
+
+稀疏轨迹增密匹配：
+
+<div align="center">
+    <img src="docs/_static/images/dense_gps.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/taxi_xishu.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/xa_sample.gif" />
+</div>
+
+
 ![car_gps.png](docs/_static/images/wxq.jpg)
 
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
@@ -54,22 +80,23 @@
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
-- geopandas(0.14.1)
 - geopy(2.4.1)
 - gdal(3.4.3)
+- shapely(2.0.3)
+- fiona(1.9.5)
+- pyproj(3.6.1)
+- geopandas(0.14.3)
 - networkx(3.2.1)
-- shapely(2.0.2)
 - pandas(2.0.3)
 - numpy(1.26.2)
-- pyproj(3.6.1)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
 geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
 
 #### __使用pip安装__
@@ -81,45 +108,37 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册
+### 1.2 用户手册与视频教程
+
+[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+
+[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+
+[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)、
-[视频教程1](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)、
-[视频教程2](https://www.bilibili.com/video/BV1nC411z7Vg/?share_source=copy_web&vd_source=9b4518c7de4757ad3b99e18456efbaa6)
+[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
 
 __如何依据GPS数据推算车辆的实际路径？__
 
-## 3. 地图匹配算法动画演示
-
-想了解算法过程的可以参考B站视频:
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)
-
 ![main.png](docs/_static/images/single_p.png)
 
 ![main.png](docs/_static/images/transition.png)
 
 ![main.png](docs/_static/images/viterbi.png)
 
 ![main.png](docs/_static/images/trace.png)
 
 
-## 4. 匹配结果可视化
-
-中高频GPS匹配效果:
-
-![main.png](docs/_static/images/m_h_f.gif)
-
-低频GPS匹配效果:
-
-![main.png](docs/_static/images/l_f.gif)
```

### Comparing `gotrackit-0.1.9/pyproject.toml` & `gotrackit-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotrackit"
-version = "0.1.9"
+version = "0.2.0"
 dependencies = ["geopandas>=0.14.1", "shapely", "networkx", "pandas", "numpy", "keplergl", "geopy"]
 requires-python = ">=3.8"
 authors = [
   { name="Kai Tang", email="794568794@qq.com" },
 ]
 description = "A Python Package for Map Matching Algorithm Based on Hidden Markov Model"
 readme = "README.md"
```

### Comparing `gotrackit-0.1.9/src/gotrackit/GlobalVal.py` & `gotrackit-0.2.0/src/gotrackit/GlobalVal.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,30 +39,33 @@
         self.FROM_GPS_SEQ = 'from_seq'
         self.TO_GPS_SEQ = 'to_seq'
 
         self.GROUP_FIELD = 'group'
         self.SUB_GROUP_FIELD = 'sub_group'
         self.NEXT_P = 'next_p'
         self.PRE_P = 'pre_p'
+        self.NEXT_SEQ = 'next_seq'
         self.NEXT_TIME = 'next_time'
         self.ADJ_TIME_GAP = 'time_gap'
-        self.ADJ_DIS = 'dis_gap'
+        self.ADJ_DIS = 'gps_adj_dis'
         self.ADJ_SPEED = 'adj_speed'
 
         self.DENSE_GEO = '__dens_geo__'
         self.N_SEGMENTS = '__n__'
 
         self.DIFF_VEC = 'diff_vec'
 
 
 class MarkovField(object):
     """HMM模型字段"""
     def __init__(self):
         self.FROM_STATE = 'from_state'
         self.TO_STATE = 'to_state'
+        self.FROM_SEQ = 'from_seq'
+        self.TO_SEQ = 'to_seq'
         self.FROM_STATE_N = 'from_state_node'
         self.TO_STATE_N = 'to_state_node'
         self.ROUTE_LENGTH = 'route_l'
         self.ROUTE_ITEM = 'route_item'
         self.STRAIGHT_LENGTH = 'straight_l'
         self.DIS_GAP = 'dis_gap'
         self.PRJ_L = 'prj_dis'
@@ -376,14 +379,16 @@
                 "radiusScale": "linear"
             }
         }
 
         self.BASE_LINK_NAME = 'base_link'
         self.BASE_NODE_NAME = 'base_node'
         self.MIX_NAME = 'mix'
+        self.GPS_NAME = 'gps'
+        self.MATCH_LINK_NAME = 'match_link'
     def get_base_config(self):
         return copy.deepcopy(self.__BASE_CONFIG)
 
     def get_polygon_config(self):
         return copy.deepcopy(self.__POLYGON_CONFIG)
 
 class PrjConst(object):
```

### Comparing `gotrackit-0.1.9/src/gotrackit/MapMatch.py` & `gotrackit-0.2.0/src/gotrackit/MapMatch.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,78 +17,94 @@
 agent_if_field = gps_field.AGENT_ID_FIELD
 node_id_field = net_field.NODE_ID_FIELD
 
 
 class MapMatch(object):
     def __init__(self, flag_name: str = 'test', net: Net = None, use_sub_net: bool = True, gps_df: pd.DataFrame = None,
                  time_format: str = "%Y-%m-%d %H:%M:%S", time_unit: str = 's',
-                 gps_buffer: float = 90, gps_route_buffer_gap: float = 25.0,
-                 max_increment_times: int = 2, increment_buffer: bool = 20.0,
+                 gps_buffer: float = 100, gps_route_buffer_gap: float = 25.0,
+                 max_increment_times: int = 2, increment_buffer: float = 20.0,
                  beta: float = 20.0, gps_sigma: float = 20.0, dis_para: float = 0.1,
                  is_lower_f: bool = False, lower_n: int = 2,
                  use_heading_inf: bool = False, heading_para_array: np.ndarray = None,
-                 dense_gps: bool = True, dense_interval: float = 25.0,
+                 dense_gps: bool = True, dense_interval: float = 50.0,
+                 dwell_l_length: float = 10.0, dwell_n: int = 3, del_dwell: bool = True,
+                 dup_threshold: float = 10.0,
                  is_rolling_average: bool = False, window: int = 2,
                  export_html: bool = False, use_gps_source: bool = False, html_fldr: str = None,
                  export_geo_res: bool = False, geo_res_fldr: str = None,
-                 node_num_threshold: int = 2000):
+                 node_num_threshold: int = 2000, top_k: int = 20, omitted_l: float = 6.0, multi_core: bool = True,
+                 core_num: int = 1, link_width: float = 1.5, node_radius: float = 1.5,
+                 match_link_width: float = 5.0, gps_radius: float = 6.0):
         """
 
         :param flag_name: 标记字符名称, 会用于标记输出的可视化文件, 默认"test"
         :param net: gotrackit路网对象, 必须指定
         :param use_sub_net: 是否在子网络上进行计算, 默认True
         :param gps_df: GPS数据, 必须指定
         :param time_format: GPS数据中时间列的格式, 默认"%Y-%m-%d %H:%M:%S"
         :param time_unit: GPS数据中时间列的单位, 如果时间列是数值(秒或者毫秒), 默认's'
-        :param gps_buffer: GPS的搜索半径, 单位米, 意为只选取每个gps_buffer点附近100米范围内的路段作为候选路段, 默认90.0
+        :param gps_buffer: GPS的搜索半径, 单位米, 意为只选取每个gps_buffer点附近100米范围内的路段作为候选路段, 默认100.0
         :param gps_route_buffer_gap: 半径增量, gps_buffer + gps_route_buffer_gap 的半径范围用于计算子网络, 默认25.0
         :param max_increment_times: 增量搜索次数, 默认2
         :param increment_buffer: 增量半径, 默认20.0
         :param beta: 该值越大, 状态转移概率对于距离越不敏感, 默认20m
         :param gps_sigma: 该值越大, 发射概率对距离越不敏感, 默认20m
         :param dis_para: 距离的折减系数, 默认0.1
         :param is_lower_f: 是否对GPS数据进行数据降频率, 适用于: 高频-高定位误差 GPS数据, 默认False
         :param lower_n: 频率倍率, 默认2
         :param use_heading_inf: 是否利用GPS的差分方向向量修正发射概率, 适用于: 低定位误差 GPS数据 或者低频定位数据(配合加密参数), 默认False
         :param heading_para_array: 差分方向修正参数, 默认np.array([1.0, 1.0, 1.0, 0.1, 0.00001, 0.000001, 0.00001, 0.000001, 0.000001])
         :param dense_gps: 是否对GPS数据进行加密, 默认False
         :param dense_interval: 当前后GPS点的直线距离l超过dense_interval即进行加密, 进行 int(l / dense_interval) + 1 等分加密, 默认25.0
+        :param dup_threshold: 利用GPS轨迹计算sub_net时, 先对GPS点原始轨迹做简化, 重复点检测阈值, 默认5m
         :param is_rolling_average: 是否启用滑动窗口平均对GPS数据进行降噪, 默认False
         :param window: 滑动窗口大小, 默认2
         :param export_html: 是否输出网页可视化结果html文件, 默认True
         :param use_gps_source: 是否在可视化结果中使用GPS源数据进行展示, 默认False
         :param html_fldr: 保存网页可视化结果的文件目录, 默认当前目录
         :param export_geo_res: 是否输出匹配结果的几何可视化文件, 默认False
         :param geo_res_fldr: 存储几何可视化文件的目录, 默认当前目录
         :param node_num_threshold: 默认2000
+        :param omitted_l: 当某GPS点与前后GPS点的平均距离小于该距离(m)时, 该GPS点的方向限制作用被取消
+        :param multi_core: 是否启用多核匹配, 默认True
+        :param core_num: 用几个核, 默认1
+        :param gps_radius: HTML可视化中GPS点的半径大小，单位米，默认8米
         """
         # 坐标系投影
         self.plain_crs = net.planar_crs
         self.geo_crs = net.geo_crs
 
         # 用于自动确定是否使用全局路网的指标
         self.node_num_threshold = node_num_threshold
 
         # gps参数
         self.gps_df = gps_df
         self.time_format = time_format  # 时间列格式
         self.time_unit = time_unit  # 时间列单位
         self.is_lower_f = is_lower_f  # 是否降频率
         self.lower_n = lower_n  # 降频倍数
+        self.del_dwell = del_dwell
+        self.dwell_n = dwell_n
+        self.dwell_l_length = dwell_l_length
         self.is_rolling_average = is_rolling_average  # 是否启用滑动窗口平均
         self.rolling_window = window  # 窗口大小
         self.dense_gps = dense_gps  # 是否加密GPS
         self.dense_interval = dense_interval  # 加密阈值(前后GPS点直线距离超过该值就会启用线性加密)
         self.gps_buffer = gps_buffer  # gps的关联范围(m)
         self.use_sub_net = use_sub_net  # 是否启用子网络
         self.max_increment_times = max_increment_times
         self.increment_buffer = increment_buffer
         self.gps_route_buffer_gap = gps_route_buffer_gap
         self.use_heading_inf = use_heading_inf
         self.heading_para_array = heading_para_array
+        self.omitted_l = omitted_l
+        self.top_k = top_k
+        self.dup_threshold = dup_threshold
+        assert dup_threshold < (self.gps_buffer + self.gps_route_buffer_gap) / 3
 
         self.beta = beta  # 状态转移概率参数, 概率与之成正比
         self.gps_sigma = gps_sigma  # 发射概率参数, 概率与之成正比
         self.flag_name = flag_name
         self.dis_para = dis_para
 
         self.export_html = export_html
@@ -97,14 +113,23 @@
         self.html_fldr = html_fldr
 
         self.may_error_list = dict()
 
         self.my_net = net
         self.not_conn_cost = self.my_net.not_conn_cost
         self.use_gps_source = use_gps_source
+        assert omitted_l < dense_interval / 2, 'omitted_l 必须小于 dense_interval / 2'
+        self.multi_core = multi_core
+        self.core_num = core_num
+
+        # 网页可视化参数
+        self.link_width = link_width
+        self.node_radius = node_radius
+        self.match_link_width = match_link_width
+        self.gps_radius = gps_radius
 
     def execute(self):
 
         match_res_df = pd.DataFrame()
         if len(self.my_net.get_node_data()[node_id_field].unique()) <= self.node_num_threshold:
             self.use_sub_net = False
 
@@ -113,16 +138,21 @@
             file_name = '-'.join([self.flag_name, str(agent_id)])
             print(rf'agent: {agent_id}')
             _gps_df.reset_index(inplace=True, drop=True)
             gps_obj = GpsPointsGdf(gps_points_df=_gps_df, time_format=self.time_format,
                                    buffer=self.gps_buffer, time_unit=self.time_unit,
                                    plane_crs=self.plain_crs,
                                    max_increment_times=self.max_increment_times, increment_buffer=self.increment_buffer,
-                                   dense_gps=self.dense_gps, dense_interval=self.dense_interval)
+                                   dense_gps=self.dense_gps, dense_interval=self.dense_interval,
+                                   dwell_l_length=self.dwell_l_length, dwell_n=self.dwell_n)
             del _gps_df
+
+            if self.del_dwell:
+                gps_obj.del_dwell_points()
+
             # 降频处理
             if self.is_lower_f:
                 print(rf'lower {self.lower_n} - frequency')
                 gps_obj.lower_frequency(n=self.lower_n)
 
             if self.is_rolling_average:
                 print(rf'rolling average by window size - {self.rolling_window}')
@@ -131,25 +161,27 @@
             if self.dense_gps:
                 print(rf'dense gps by interval - {self.dense_interval}m')
                 gps_obj.dense()
 
             # 依据当前的GPS数据(源数据)做一个子网络
             if self.use_sub_net:
                 print(rf'using sub net')
-                sub_net = self.my_net.create_computational_net(
-                    gps_array_buffer=gps_obj.get_gps_array_buffer(buffer=self.gps_buffer + self.gps_route_buffer_gap))
-                # 初始化一个隐马尔可夫模型
-                hmm_obj = HiddenMarkov(net=sub_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
-                                       not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
-                                       heading_para_array=self.heading_para_array, dis_para=self.dis_para)
+                used_net = self.my_net.create_computational_net(
+                    gps_array_buffer=gps_obj.get_gps_array_buffer(buffer=self.gps_buffer + self.gps_route_buffer_gap,
+                                                                  dup_threshold=self.dup_threshold))
             else:
+                used_net = self.my_net
                 print(rf'using whole net')
-                hmm_obj = HiddenMarkov(net=self.my_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
-                                       not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
-                                       heading_para_array=self.heading_para_array, dis_para=self.dis_para)
+
+            # 初始化一个隐马尔可夫模型
+            hmm_obj = HiddenMarkov(net=used_net, gps_points=gps_obj, beta=self.beta, gps_sigma=self.gps_sigma,
+                                   not_conn_cost=self.not_conn_cost, use_heading_inf=self.use_heading_inf,
+                                   heading_para_array=self.heading_para_array, dis_para=self.dis_para,
+                                   top_k=self.top_k, omitted_l=self.omitted_l, multi_core=self.multi_core,
+                                   core_num=self.core_num)
 
             # 求解参数
             hmm_obj.generate_markov_para()
             hmm_obj.solve()
             _match_res_df = hmm_obj.acquire_res()
             if hmm_obj.is_warn:
                 self.may_error_list[agent_id] = hmm_obj.warn_info
@@ -160,12 +192,18 @@
 
             match_res_df = pd.concat([match_res_df, _match_res_df])
 
             if self.export_html:
                 # 4.初始化一个匹配结果管理器
                 vc = VisualizationCombination(use_gps_source=self.use_gps_source)
                 vc.collect_hmm(hmm_obj)
-                vc.visualization(zoom=15, out_fldr=self.html_fldr,
-                                 file_name=file_name)
+                try:
+                    vc.visualization(zoom=15, out_fldr=self.html_fldr,
+                                     file_name=file_name, link_width=self.link_width,
+                                     node_radius=self.node_radius, match_link_width=self.match_link_width,
+                                     gps_radius=self.gps_radius)
+                except Exception as e:
+                    print(repr(e))
+                    print(rf'输出HTML可视化文件, 出现某些错误, 输出失败...')
                 del vc
         match_res_df.reset_index(inplace=True, drop=True)
         return match_res_df, self.may_error_list
```

### Comparing `gotrackit-0.1.9/src/gotrackit/WrapsFunc.py` & `gotrackit-0.2.0/src/gotrackit/WrapsFunc.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/generation/GpsGen.py` & `gotrackit-0.2.0/src/gotrackit/generation/GpsGen.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/gps/GpsArray.py` & `gotrackit-0.2.0/src/gotrackit/gps/GpsArray.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,37 +52,38 @@
                 pd.to_datetime(self.gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
         self.gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.gps_points_gdf.copy()
+        self.check()
 
     def check(self):
         _gap = {agent_field, lng_field, lat_field, time_field} - set(self.gps_gdf.columns)
         assert _gap == set(), rf'GPS数据缺少{_gap}字段'
 
     @property
     def gps_gdf(self) -> gpd.GeoDataFrame:
         return self.gps_points_gdf.copy()
 
     @property
     def crs(self):
         return self.__crs
 
     def to_plane_prj(self) -> None:
-        if self.gps_points_gdf.crs == self.plane_crs:
+        if self.gps_points_gdf.crs.srs == self.plane_crs:
             self.__crs = self.plane_crs
             pass
         else:
             self.gps_points_gdf = self.gps_points_gdf.to_crs(self.plane_crs)
             self.__crs = self.plane_crs
 
     def to_geo_prj(self) -> None:
-        if self.gps_points_gdf.crs == self.geo_crs:
+        if self.gps_points_gdf.crs.srs == self.geo_crs:
             self.__crs = self.geo_crs
             pass
         else:
             self.gps_points_gdf = self.gps_points_gdf.to_crs(self.geo_crs)
             self.__crs = self.geo_crs
 
     @property
```

### Comparing `gotrackit-0.1.9/src/gotrackit/gps/LocGps.py` & `gotrackit-0.2.0/src/gotrackit/gps/LocGps.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,66 +8,72 @@
 import datetime
 import numpy as np
 import pandas as pd
 import geopandas as gpd
 from ..map.Net import Net
 from datetime import timedelta
 from ..tools.geo_process import prj_inf
-from ..GlobalVal import GpsField, NetField, PrjConst
-from ..WrapsFunc import function_time_cost
 from ..tools.geo_process import segmentize
-from ..tools.geo_process import angle_base_north
+from ..GlobalVal import GpsField, NetField, PrjConst
 from shapely.geometry import Point, Polygon, LineString
 
 
 gps_field = GpsField()
 net_field = NetField()
 prj_const = PrjConst()
 
 lng_field = gps_field.LNG_FIELD
 lat_field = gps_field.LAT_FIELD
 next_p_field = gps_field.NEXT_P
+next_seq_field = gps_field.NEXT_SEQ
 pre_p_field = gps_field.PRE_P
 time_field = gps_field.TIME_FIELD
 next_time_field = gps_field.NEXT_TIME
 agent_field = gps_field.AGENT_ID_FIELD
 geometry_field = gps_field.GEOMETRY_FIELD
 time_gap_field = gps_field.ADJ_TIME_GAP
 dis_gap_field = gps_field.ADJ_DIS
 adj_speed_field = gps_field.ADJ_SPEED
 dense_geo_field = gps_field.DENSE_GEO
 n_seg_field = gps_field.N_SEGMENTS
 diff_vec = gps_field.DIFF_VEC
 geo_crs = prj_const.PRJ_CRS
+sub_group_field = gps_field.SUB_GROUP_FIELD
+
 
 class GpsPointsGdf(object):
 
     def __init__(self, gps_points_df: pd.DataFrame = None,
                  buffer: float = 200.0, increment_buffer: float = 20.0, max_increment_times: int = 10,
                  time_format: str = '%Y-%m-%d %H:%M:%S', time_unit: str = 's',
-                 plane_crs: str = 'EPSG:32649', dense_gps: bool = True, dense_interval: float = 25.0):
+                 plane_crs: str = 'EPSG:32649', dense_gps: bool = True, dense_interval: float = 25.0,
+                 dwell_l_length: float = 10.0, dwell_n: int = 3):
         """
 
         :param gps_points_df: gps数据dataframe, agent_id, lng, lat, time
         :param buffer: GPS点的buffer半径大小(用于生成候选路段), m
         :param increment_buffer: 使用buffer进行关联, 可能会存在部分GPS点仍然关联不到任何路段, 对于这部分路段, 将启用增量buffer进一步关联
         :param max_increment_times: 增量搜索的最大次数
         :param time_format: 时间列的字符格式
         :param plane_crs: 平面投影坐标系
         :param dense_gps: 是否加密GPS点
+        :param dwell_l_length: 停留点识别距离阈值
+        :param dwell_n: 连续dwell_n个点的距离小于dwell_l_length就被识别为停留点
         :param dense_interval: 加密间隔(相邻GPS点的直线距离小于dense_interval即会进行加密)
         """
         self.geo_crs = geo_crs
         self.buffer = buffer
         self.__crs = self.geo_crs
         self.plane_crs = plane_crs
         self.increment_buffer = increment_buffer
         self.dense_gps = dense_gps
         self.dense_interval = dense_interval
         self.max_increment_times = 1 if max_increment_times <= 0 else max_increment_times
+        self.dwell_l_length = dwell_l_length
+        self.dwell_n = dwell_n
         self.__gps_point_dis_dict = dict()
         self.__gps_points_gdf = gps_points_df
         self.check()
         if gps_field.HEADING_FIELD not in self.__gps_points_gdf.columns:
             self.__gps_points_gdf[gps_field.HEADING_FIELD] = 0.0
         self.__gps_points_gdf[gps_field.GEOMETRY_FIELD] = self.__gps_points_gdf.apply(
             lambda item: Point(item[gps_field.LNG_FIELD], item[gps_field.LAT_FIELD]), axis=1)
@@ -79,15 +85,14 @@
         except Exception as e:
             print(repr(e))
             self.__gps_points_gdf[gps_field.TIME_FIELD] = \
                 pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD], unit=time_unit)
         self.__gps_points_gdf.sort_values(by=[gps_field.TIME_FIELD], ascending=[True], inplace=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
         self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
-
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.to_plane_prj()
         # self.calc_gps_point_dis()
 
         # 存储最原始的GPS信息
         self.__source_gps_points_gdf = self.__gps_points_gdf.copy()
 
@@ -98,22 +103,16 @@
                 gps_field.AGENT_ID_FIELD, gps_field.TIME_FIELD}.issubset(
             set(self.__gps_points_gdf.columns)), \
             rf'GPS数据字段有误, 请至少包含如下字段: {gps_field.AGENT_ID_FIELD, gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD}'
 
     def dense(self):
 
         # 时间差和距离差
-        self.__gps_points_gdf[next_time_field] = self.__gps_points_gdf[time_field].shift(-1).fillna(
-            self.__gps_points_gdf[time_field])
-        self.__gps_points_gdf[next_p_field] = self.__gps_points_gdf[geometry_field].shift(-1).fillna(
-            self.__gps_points_gdf[geometry_field])
-        self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf.apply(
-            lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
-        self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf.apply(
-            lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
+        self.calc_adj_dis_gap()
+        self.calc_adj_time_gap()
 
         should_be_dense_gdf = self.__gps_points_gdf[self.__gps_points_gdf[dis_gap_field] > self.dense_interval].copy()
         if should_be_dense_gdf.empty:
             return None
         self.__gps_points_gdf.drop(columns=[next_time_field, next_p_field, time_gap_field, dis_gap_field], axis=1,
                                    inplace=True)
 
@@ -143,27 +142,46 @@
 
         self.__gps_points_gdf = pd.concat([self.__gps_points_gdf, should_be_dense_gdf])
         self.__gps_points_gdf.sort_values(by=time_field, ascending=True, inplace=True)
         self.__gps_points_gdf.reset_index(inplace=True, drop=True)
         self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
         self.__gps_points_gdf[gps_field.ORIGIN_POINT_SEQ_FIELD] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD]
 
+    def calc_adj_dis_gap(self) -> None:
+        # 距离差
+        self.__gps_points_gdf[next_p_field] = self.__gps_points_gdf[geometry_field].shift(-1).fillna(
+            self.__gps_points_gdf[geometry_field])
+        self.__gps_points_gdf[dis_gap_field] = self.__gps_points_gdf.apply(
+            lambda row: row[next_p_field].distance(row[geometry_field]), axis=1)
+
+    def calc_adj_time_gap(self) -> None:
+        # 时间差
+        self.__gps_points_gdf[next_time_field] = self.__gps_points_gdf[time_field].shift(-1).fillna(
+            self.__gps_points_gdf[time_field])
+        self.__gps_points_gdf[time_gap_field] = self.__gps_points_gdf.apply(
+            lambda row: (row[next_time_field] - row[time_field]).seconds, axis=1)
+
+    def calc_pre_next_dis(self) -> pd.DataFrame():
+        self.calc_adj_dis_gap()
+        # next_seq
+        res = self.__gps_points_gdf.copy()
+        res[next_seq_field] = res[gps_field.POINT_SEQ_FIELD].shift(-1)
+        res.dropna(subset=[next_seq_field], inplace=True)
+        res[next_seq_field] = res[next_seq_field].astype(int)
+        return res[[gps_field.POINT_SEQ_FIELD, next_seq_field, gps_field.ADJ_DIS]]
+
     def lower_frequency(self, n: int = 5):
         """
         GPS数据降频
         :param n: 降频倍数
         :return:
         """
-        self.__gps_points_gdf['label'] = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].apply(lambda x: x % n)
-        self.__gps_points_gdf = self.__gps_points_gdf[self.__gps_points_gdf['label'] == 0].copy()
-        # self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
-        # self.__gps_points_gdf.reset_index(inplace=True, drop=True)
-        # self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD] = [i for i in range(len(self.__gps_points_gdf))]
+        self.__gps_points_gdf['label'] = pd.Series([i for i in range(len(self.__gps_points_gdf))]) % n
+        self.__gps_points_gdf = self.__gps_points_gdf[self.__gps_points_gdf['label'].eq(0)].copy()
         self.__gps_points_gdf.drop(columns=['label'], axis=1, inplace=True)
-        # self.calc_gps_point_dis()
 
     def rolling_average(self, window: int = 2):
         """
         滑动窗口降噪
         :param window: 窗口大小
         :return:
         """
@@ -201,27 +219,18 @@
         self.__gps_points_gdf[net_field.GEOMETRY_FIELD] = self.__gps_points_gdf[
             [gps_field.LNG_FIELD, gps_field.LAT_FIELD]].apply(
             lambda item: Point(item), axis=1)
         self.__gps_points_gdf[gps_field.TIME_FIELD] = pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD],
                                                                      unit='s')
         self.__gps_points_gdf[gps_field.TIME_FIELD] = pd.to_datetime(self.__gps_points_gdf[gps_field.TIME_FIELD],
                                                                      format='%Y-%m-%d %H:%M:%S')
-        # print(self.__gps_points_gdf.crs)
-        # self.calc_gps_point_dis()
-
-    def dwell_point_processing(self, buffer: float = 25.0):
-        """识别停留点, 去除多余的停留点GPS信息"""
-        if self.__source_gps_points_gdf is None:
-            self.__source_gps_points_gdf = self.__gps_points_gdf.copy()
-        # TO DO ......
-        self.calc_gps_point_dis()
-        pass
 
     def calc_gps_point_dis(self) -> None:
         seq_list = self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].to_list()
+        # {(from_seq, to_seq): dis, ...}
         self.__gps_point_dis_dict = {
             (seq_list[i], seq_list[i + 1]): self.__gps_points_gdf.at[seq_list[i], gps_field.GEOMETRY_FIELD].distance(
                 self.__gps_points_gdf.at[seq_list[i + 1], gps_field.GEOMETRY_FIELD]) for i in
             range(len(self.__gps_points_gdf) - 1)}
 
     def get_gps_point_dis(self, adj_gps_seq: tuple = None) -> float:
         try:
@@ -229,14 +238,17 @@
         # some gps points do not have any candidate links
         except KeyError:
             dis = self.__gps_points_gdf.at[adj_gps_seq[0], gps_field.GEOMETRY_FIELD].distance(
                 self.__gps_points_gdf.at[adj_gps_seq[1], gps_field.GEOMETRY_FIELD])
             self.__gps_point_dis_dict[adj_gps_seq] = dis
         return dis
 
+    def get_adj_gps_dis_df(self):
+        return self.__gps_point_dis_dict
+
     def plot_point(self):
         pass
 
     def get_gps_buffer_gdf(self):
         pass
 
     def calc_diff_heading(self):
@@ -248,114 +260,98 @@
         self.__gps_points_gdf[pre_p_field] = self.__gps_points_gdf[geometry_field].shift(1).fillna(
             self.__gps_points_gdf[geometry_field])
 
         self.__gps_points_gdf['next_loc'] = self.__gps_points_gdf.apply(
             lambda row: np.array([row[next_p_field].x, row[next_p_field].y]), axis=1)
         self.__gps_points_gdf['pre_loc'] = self.__gps_points_gdf.apply(
             lambda row: np.array([row[pre_p_field].x, row[pre_p_field].y]), axis=1)
-        self.__gps_points_gdf['loc'] = self.__gps_points_gdf.apply(
-            lambda row: np.array([row[geometry_field].x, row[geometry_field].y]), axis=1)
-        self.__gps_points_gdf[diff_vec] = self.__gps_points_gdf.apply(
-            lambda row: row['next_loc'] - row['loc'] + row['loc'] - row['pre_loc'],
-            axis=1)
 
-        self.__gps_points_gdf.drop(
-            columns=[next_p_field, pre_p_field, 'next_loc', 'pre_loc', 'loc', ], axis=1,
-            inplace=True)
-        self.done_diff_heading = True
+        # self.__gps_points_gdf['loc'] = self.__gps_points_gdf.apply(
+        #     lambda row: np.array([row[geometry_field].x, row[geometry_field].y]), axis=1)
+        # self.__gps_points_gdf[diff_vec] = self.__gps_points_gdf.apply(
+        #     lambda row: (row['next_loc'] - row['loc'] + row['loc'] - row['pre_loc']) / 2,
+        #     axis=1)
 
-    @staticmethod
-    def calc_angle(vec1: np.ndarray = None, vec2: np.ndarray = None):
-        a, b = False, False
-
-        if np.linalg.norm(vec1) == 0:
-            a = True
-        vec1 = vec1 / np.linalg.norm(vec1)
-
-        if np.linalg.norm(vec2) == 0:
-            b = True
-        vec2 = vec2 / np.linalg.norm(vec2)
-
-        c_vec = np.ndarray
-
-        if a and b:
-            return -1
-
-        if a or b:
-            if a:
-                c_vec = vec2
-            elif b:
-                c_vec = vec1
-        else:
-            c_vec = vec1 + vec2
+        self.__gps_points_gdf[diff_vec] = (self.__gps_points_gdf['next_loc'] - self.__gps_points_gdf['pre_loc']) / 2
 
-        res = angle_base_north(v=c_vec)
-        return res
+        self.__gps_points_gdf.drop(
+            columns=[next_p_field, pre_p_field, 'next_loc', 'pre_loc'], axis=1, inplace=True)
+        self.done_diff_heading = True
 
     @property
     def gps_gdf(self) -> gpd.GeoDataFrame:
         return self.__gps_points_gdf.copy()
 
     @property
     def crs(self):
         return self.__crs
 
-    def get_gps_array_buffer(self, buffer: float = 200.0) -> Polygon:
+    def get_gps_array_buffer(self, buffer: float = 200.0, dup_threshold: float = 10.0) -> Polygon:
         """输出gps路径的buffer范围面域"""
-        gps_array_buffer = LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()).buffer(buffer)
+        gps_route_l = gpd.GeoSeries(LineString(self.__gps_points_gdf[gps_field.GEOMETRY_FIELD].to_list()))
+        simplify_gps_route_l = gps_route_l.remove_repeated_points(dup_threshold)
+        gps_array_buffer = simplify_gps_route_l[0].buffer(buffer)
         return gps_array_buffer
 
-    @function_time_cost
     def generate_candidate_link(self, net: Net = None) -> tuple[pd.DataFrame, list[int]]:
         """
         计算GPS观测点的候选路段
         :param net:
         :return: GPS候选路段信息, 未匹配到候选路段的gps点id
         """
         gps_buffer_gdf = self.__gps_points_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.GEOMETRY_FIELD]].copy()
-        if gps_buffer_gdf.crs != self.plane_crs:
+        if gps_buffer_gdf.crs.srs != self.plane_crs:
             gps_buffer_gdf = gps_buffer_gdf.to_crs(self.plane_crs)
 
         single_link_gdf = net.get_link_data()[[net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                                net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD,
                                                net_field.LENGTH_FIELD, net_field.GEOMETRY_FIELD]]
-
+        single_link_gdf.reset_index(inplace=True, drop=True)
         candidate_link = pd.DataFrame()
         remain_gps_list = []
         for i in [i for i in range(0, self.max_increment_times)]:
             now_buffer = self.buffer + i * self.increment_buffer
             print(rf'buffer: {now_buffer}m...')
 
             gps_buffer_gdf['gps_buffer'] = gps_buffer_gdf[net_field.GEOMETRY_FIELD].apply(lambda p: p.buffer(now_buffer))
             gps_buffer_gdf.set_geometry('gps_buffer', inplace=True, crs=gps_buffer_gdf.crs)
             join_df = gpd.sjoin(gps_buffer_gdf, single_link_gdf, how='left')
 
             _candidate_link = join_df[~join_df[net_field.SINGLE_LINK_ID_FIELD].isna()]
             candidate_link = pd.concat([candidate_link, _candidate_link])
-
+            del _candidate_link
             remain_gps_list = list(join_df[join_df[net_field.SINGLE_LINK_ID_FIELD].isna()][gps_field.POINT_SEQ_FIELD].unique())
             if not remain_gps_list:
                 break
 
             gps_buffer_gdf = gps_buffer_gdf[gps_buffer_gdf[gps_field.POINT_SEQ_FIELD].isin(remain_gps_list)].copy()
-        candidate_link.drop(columns=['index_right', net_field.GEOMETRY_FIELD, 'gps_buffer'], axis=1, inplace=True)
-        candidate_link.reset_index(inplace=True, drop=True)
-
+        if not candidate_link.empty:
+            candidate_link.drop(columns=['index_right', 'gps_buffer'], axis=1, inplace=True)
+            for col in [net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD,
+                        net_field.SINGLE_LINK_ID_FIELD, net_field.DIRECTION_FIELD]:
+                candidate_link[col] = candidate_link[col].astype(int)
+            # add link geo
+            single_link_gdf.rename(columns={net_field.GEOMETRY_FIELD: 'single_link_geo'}, inplace=True)
+            candidate_link = pd.merge(candidate_link,
+                                      single_link_gdf[[net_field.SINGLE_LINK_ID_FIELD, 'single_link_geo',
+                                                       net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]],
+                                      on=net_field.SINGLE_LINK_ID_FIELD, how='left')
+            candidate_link.reset_index(inplace=True, drop=True)
         return candidate_link, remain_gps_list
 
     def to_plane_prj(self) -> None:
-        if self.__gps_points_gdf.crs == self.plane_crs:
+        if self.__gps_points_gdf.crs.srs == self.plane_crs:
             self.__crs = self.plane_crs
             pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.plane_crs)
             self.__crs = self.plane_crs
 
     def to_geo_prj(self) -> None:
-        if self.__gps_points_gdf.crs == self.geo_crs:
+        if self.__gps_points_gdf.crs.srs == self.geo_crs:
             self.__crs = self.geo_crs
             pass
         else:
             self.__gps_points_gdf = self.__gps_points_gdf.to_crs(self.geo_crs)
             self.__crs = self.geo_crs
 
     def get_point(self, seq: int = 0):
@@ -391,56 +387,48 @@
         :param gps_point:
         :param line:
         :return: (GPS投影点坐标, GPS点到投影点的直线距离, GPS投影点到line拓扑起点的路径距离, line的长度)
         """
         prj_p, p_prj_l, prj_route_l, line_length, _, prj_vec = prj_inf(p=gps_point, line=line)
         return prj_p, p_prj_l, prj_route_l, line_length, prj_vec
 
-        # distance = line.project(gps_point)
-        #
-        # if distance <= 0.0:
-        #     prj_p = Point(list(line.coords)[0])
-        #     return prj_p, prj_p.distance(gps_point), distance, line.length
-        # elif distance >= line.length:
-        #     prj_p = Point(list(line.coords)[-1])
-        #     return prj_p, prj_p.distance(gps_point), distance, line.length
-        # else:
-        #     coords = list(line.coords)
-        #     for i, p in enumerate(coords):
-        #         xd = line.project(Point(p))
-        #         if xd == distance:
-        #             prj_p = Point(coords[i])
-        #             return prj_p, prj_p.distance(gps_point), distance, line.length
-        #         if xd > distance:
-        #             cp = line.interpolate(distance)
-        #             prj_p = Point((cp.x, cp.y))
-        #             return prj_p, prj_p.distance(gps_point), distance, line.length
-
     @property
     def gps_list_length(self) -> int:
         return len(self.__gps_points_gdf)
 
     @property
     def used_observation_seq_list(self) -> list[int]:
         return self.__gps_points_gdf[gps_field.POINT_SEQ_FIELD].to_list()
 
+    def del_dwell_points(self) -> None:
+        # add field = dis_gap_field
+        self.calc_adj_dis_gap()
+        self.__gps_points_gdf['dwell_label'] = \
+            (self.__gps_points_gdf[dis_gap_field] > self.dwell_l_length).astype(int)
 
-if __name__ == '__main__':
-    from datetime import timedelta
+        self.__gps_points_gdf = self.del_consecutive_zero(df=self.__gps_points_gdf, col='dwell_label', n=self.dwell_n)
+        self.__gps_points_gdf.drop(columns=[sub_group_field], axis=1, inplace=True)
+
+    @staticmethod
+    def del_consecutive_zero(df: pd.DataFrame or gpd.GeoDataFrame = None,
+                             col: str = None, n: int = 3) -> pd.DataFrame or gpd.GeoDataFrame:
+        """
+        标记超过连续n行为0的行, 并且只保留最后一行
+        :param df:
+        :param col:
+        :param n:
+        :return:
+        """
+        m = df[col].ne(0)
+        df['__del__'] = (df.groupby(m.cumsum())[col]
+                         .transform('count').gt(n + 1)
+                         & (~m)
+                         )
+        df['__a__'] = df['__del__'].ne(1).cumsum()
+        df['__cut__'] = df['__a__'] & df['__del__']
+        df.drop_duplicates(subset=['__a__'], keep='last', inplace=True)
+        df[sub_group_field] = df['__cut__'].ne(0).cumsum()
+        df.drop(columns=['__del__', '__a__', '__cut__'], axis=1, inplace=True)
+        return df
 
-    df = pd.DataFrame({'val': [1,2,3,4,5,6,7]})
-    df['val1'] = [1,2,3,4,5,6,7]
-    df['time'] = [datetime.datetime.now() + timedelta(seconds=i * 10) for i in range(1, len(df) + 1)]
-    result = df[['val', 'val1']].rolling(window=2).mean()
-    print(result)
-    print(result.at[1, 'val'])
-    # print(df)
-    # df['time'] = df['time'].apply(lambda x: x.timestamp())
-    # result = df['val'].rolling(window=2).mean()
-    # result = df['time'].rolling(window=2).mean()
-    # print(result)
-    #
-    # df['time'] = result
-    # df['time'] = pd.to_datetime(df['time'], unit='s')
-    # print(df)
```

### Comparing `gotrackit-0.1.9/src/gotrackit/map/Link.py` & `gotrackit-0.2.0/src/gotrackit/map/Link.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,55 +27,43 @@
 from_node_field = net_field.FROM_NODE_FIELD
 to_node_field = net_field.TO_NODE_FIELD
 length_field = net_field.LENGTH_FIELD
 geometry_field = net_field.GEOMETRY_FIELD
 link_vec_field = net_field.LINK_VEC_FIELD
 
 
-
 class Link(object):
     def __init__(self, link_gdf: gpd.GeoDataFrame = None, planar_crs: str = None,
                  weight_field: str = None, is_check: bool = True, not_conn_cost: float = 999.0,
                  init_available_link: bool = True):
 
         self.not_conn_cost = not_conn_cost
         self.geo_crs = geo_crs
         self.planar_crs = planar_crs
-
-        _gap = {link_id_field, dir_field, from_node_field, to_node_field, length_field, geometry_field} - set(
-            link_gdf.columns)
-        if _gap:
-            raise ValueError(rf'缺少必须字段:{_gap}')
-        for col in [net_field.LINK_ID_FIELD, net_field.DIRECTION_FIELD,
-                    net_field.FROM_NODE_FIELD, net_field.TO_NODE_FIELD]:
-            link_gdf[col] = link_gdf[col].astype(int)
         self.link_gdf = link_gdf.copy()
         self.link_gdf.index = self.link_gdf[link_id_field]
-        for col in [net_field.DIRECTION_FIELD, net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
-                    net_field.TO_NODE_FIELD]:
-            link_gdf[col] = link_gdf[col].astype(int)
         self.weight_field = weight_field
         self.__available_link_id = []
         if is_check:
             self.check()
-        self.max_link_id = None
+        self.max_link_id = 999
         if init_available_link:
             self.init_available_link_id()
         self.__single_link_gdf = gpd.GeoDataFrame()
         self.__double_single_mapping: dict[int, tuple[int, int, int, int]] = dict()
         self.__ft_link_mapping: dict[tuple[int, int], int] = dict()
 
         self.__graph = nx.DiGraph()
         self.__ud_graph = nx.Graph()
         self.__one_out_degree_nodes = None
         self.__link_ft_mapping: dict[int, tuple[int, int]] = dict()
         self.done_link_vec = False
 
     def check(self):
-        assert self.link_gdf.crs == self.geo_crs, rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs}'
+        assert self.link_gdf.crs.srs == self.geo_crs, rf'Link层数据必须为WGS84 - EPSG:4326, 实际输入: {self.link_gdf.crs.srs}'
         gap_set = {net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                    net_field.TO_NODE_FIELD, net_field.DIRECTION_FIELD, self.weight_field,
                    net_field.GEOMETRY_FIELD} - set(self.link_gdf.columns)
         assert len(gap_set) == 0, rf'线层Link缺少以下字段:{gap_set}'
         assert len(self.link_gdf[net_field.LINK_ID_FIELD]) == len(self.link_gdf[net_field.LINK_ID_FIELD].unique()), \
             rf'字段{net_field.LINK_ID_FIELD}不唯一...'
         assert set(self.link_gdf[net_field.DIRECTION_FIELD]).issubset({0, 1}), \
@@ -91,14 +79,19 @@
         :return:
         """
         self.create_single_link(link_gdf=self.link_gdf)
         self.__single_link_gdf.set_index(net_field.SINGLE_LINK_ID_FIELD, inplace=True)
         self.__single_link_gdf[net_field.SINGLE_LINK_ID_FIELD] = list(self.__single_link_gdf.index)
 
     def renew_length(self):
+        _idx = list(self.link_gdf.index)[0]
+        length_a, length_b = \
+            self.link_gdf.at[_idx, net_field.GEOMETRY_FIELD].length, self.link_gdf.at[_idx, net_field.LENGTH_FIELD]
+        if 0.8 <= length_a / length_b <= 1.2:
+            return None
         self.link_gdf[length_field] = self.link_gdf.apply(lambda row: row[geometry_field].length, axis=1)
 
     def init_link_from_existing_single_link(self, single_link_gdf: gpd.GeoDataFrame = None):
         """通过给定的single_link_gdf初始化link, 用在子net的初始化上"""
         self.__single_link_gdf = single_link_gdf.copy()
         self.__double_single_mapping = {single_link_id: (link_id, int(direction), f, t) for
                                         single_link_id, link_id, direction, f, t in
@@ -208,19 +201,19 @@
         assert set(dir_val).issubset({0, 1})
         length_list = [l.length for l in geo]
         attr_dict = {link_id_field: link_id, from_node_field: from_node, to_node_field: to_node,
                      length_field: length_list,
                      dir_field: dir_val, geometry_field: geo}
         attr_dict.update(kwargs)
         self.link_gdf = pd.concat(
-            [self.link_gdf, gpd.GeoDataFrame(attr_dict, geometry=geometry_field, crs=self.link_gdf.crs)])
+            [self.link_gdf, gpd.GeoDataFrame(attr_dict, geometry=geometry_field, crs=self.link_gdf.crs.srs)])
         self.link_gdf.index = self.link_gdf[link_id_field]
 
     def append_link_gdf(self, link_gdf: gpd.GeoDataFrame = None) -> None:
-        assert link_gdf.crs == self.crs
+        assert link_gdf.crs.srs == self.crs
         assert set(link_gdf[link_id_field]) & set(self.link_gdf[link_id_field]) == set()
         self.link_gdf = pd.concat(
             [self.link_gdf, link_gdf])
         self.link_gdf.index = self.link_gdf[link_id_field]
 
     def renew_single_link(self):
         pass
@@ -326,45 +319,45 @@
     def get_geo_by_ft(self, from_node: int = None, to_node: int = None) -> LineString:
         return self.__single_link_gdf.at[self.__ft_link_mapping[(from_node, to_node)], net_field.GEOMETRY_FIELD]
 
     def get_ft_link_mapping(self) -> dict[tuple[int, int], int]:
         return self.__ft_link_mapping
 
     def to_plane_prj(self) -> None:
-        if self.link_gdf.crs == self.planar_crs:
+        if self.link_gdf.crs.srs == self.planar_crs:
             pass
         else:
             if self.__single_link_gdf is None or self.__single_link_gdf.empty:
                 pass
             else:
                 self.__single_link_gdf = self.__single_link_gdf.to_crs(self.planar_crs)
             self.link_gdf = self.link_gdf.to_crs(self.planar_crs)
 
     def to_geo_prj(self) -> None:
-        if self.link_gdf.crs == self.geo_crs:
+        if self.link_gdf.crs.srs == self.geo_crs:
             pass
         else:
             if self.__single_link_gdf is None or self.__single_link_gdf.empty:
                 pass
             else:
                 self.__single_link_gdf = self.__single_link_gdf.to_crs(self.geo_crs)
             self.link_gdf = self.link_gdf.to_crs(self.geo_crs)
 
     @property
     def crs(self):
-        return self.link_gdf.crs
+        return self.link_gdf.crs.srs
 
     @property
     def bilateral_unidirectional_mapping(self) -> dict[int, tuple[int, int, int, int]]:
         return self.__double_single_mapping.copy()
 
     def init_available_link_id(self) -> None:
         max_link = self.link_gdf[link_id_field].max()
         self.max_link_id = max_link
-        if self.max_link_id >= 10000000:
+        if self.max_link_id >= 100000:
             return None
         self.__available_link_id = list({i for i in range(1, max_link + 1)} - set(self.link_gdf[link_id_field]))
 
     @property
     def available_link_id(self) -> int:
         if self.__available_link_id:
             now_link_id = self.__available_link_id.pop()
```

### Comparing `gotrackit-0.1.9/src/gotrackit/map/Net.py` & `gotrackit-0.2.0/src/gotrackit/map/Net.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,32 +66,33 @@
         if node_gdf is None:
             self.__node = Node(node_gdf=gpd.read_file(node_path), is_check=is_check, init_available_node=self.cache_id)
         else:
             self.__node = Node(node_gdf=node_gdf, is_check=is_check, init_available_node=self.cache_id)
 
         if link_gdf is None:
             self.__link = Link(link_gdf=gpd.read_file(link_path), weight_field=self.weight_field, is_check=is_check,
-                               planar_crs=self.__node.planar_crs, init_available_link=self.cache_id)
+                               planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
+                               not_conn_cost=self.not_conn_cost)
         else:
             self.__link = Link(link_gdf=link_gdf, weight_field=self.weight_field, is_check=is_check,
-                               planar_crs=self.__node.planar_crs, init_available_link=self.cache_id)
+                               planar_crs=self.__node.planar_crs, init_available_link=self.cache_id,
+                               not_conn_cost=self.not_conn_cost)
         self.__planar_crs = self.__node.planar_crs
         self.to_plane_prj()
         self.__link.renew_length()
         if not init_from_existing:
             if create_single:
                 self.__link.init_link()
         else:
             if create_single:
                 self.__link.init_link_from_existing_single_link(single_link_gdf=link_gdf)
         if not init_from_existing:
             self.__node.init_node()
         else:
             pass
-
         if is_check:
             self.check()
     @property
     def planar_crs(self):
         return self.__planar_crs
 
     @planar_crs.setter
@@ -153,23 +154,21 @@
         :param o_node:
         :param d_node:
         :return:
         """
         return self.__link.get_shortest_path_length(o_node=o_node, d_node=d_node)
 
     def calc_shortest_path(self, source: int = None, method: str = 'dijkstra') -> None:
-        if source in self.__stp_cache.keys():
+
+        try:
+            self.__done_path_cost[source], self.__stp_cache[source] = self._single_source_path(
+                self.__link.get_graph(), source=source,
+                method=method, weight_field=self.weight_field)
+        except nx.NetworkXNoPath:
             pass
-        else:
-            try:
-                self.__done_path_cost[source], self.__stp_cache[source] = self._single_source_path(
-                    self.__link.get_graph(), source=source,
-                    method=method, weight_field=self.weight_field)
-            except nx.NetworkXNoPath:
-                pass
 
     @staticmethod
     def _single_source_path(g: nx.DiGraph = None, source: int = None, method: str = 'dijkstra',
                             weight_field: str = None) -> tuple[dict[int, int], dict[int, list]]:
         if method == 'dijkstra':
             return nx.single_source_dijkstra(g, source, weight=weight_field)
         else:
@@ -270,15 +269,16 @@
         sub_node_list = list(set(sub_single_link_gdf[net_field.FROM_NODE_FIELD]) | \
                              set(sub_single_link_gdf[net_field.TO_NODE_FIELD]))
         sub_node_gdf = self.__node.get_node_data().loc[sub_node_list, :].copy()
         sub_net = Net(link_gdf=sub_single_link_gdf,
                       node_gdf=sub_node_gdf,
                       weight_field=self.weight_field,
                       init_from_existing=True, is_check=False,
-                      search_method=self.search_method)
+                      search_method=self.search_method, cache_path=self.cache_path, cache_id=self.cache_id,
+                      not_conn_cost=self.not_conn_cost)
         sub_net.init_net()
         return sub_net
 
     @property
     def graph(self) -> nx.DiGraph:
         return self.__link.get_graph()
```

### Comparing `gotrackit-0.1.9/src/gotrackit/map/Node.py` & `gotrackit-0.2.0/src/gotrackit/map/Node.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 node_id_field = net_field.NODE_ID_FIELD
 geometry_field = net_field.GEOMETRY_FIELD
 
 
 class Node(object):
     def __init__(self, node_gdf: gpd.GeoDataFrame = None, is_check: bool = True, init_available_node: bool = True):
         self.geo_crs = geo_crs
-        self.planar_crs = node_gdf.crs
+        self.planar_crs = node_gdf.crs.srs
         self.__node_gdf = node_gdf.copy()
-        self.max_node_id = None
-        self.__available_node_id = None
+        self.max_node_id = 999
+        self.__available_node_id = []
         if is_check:
             self.planar_crs = judge_plain_crs_based_on_node(node_gdf=self.__node_gdf)
             self.check()
         if init_available_node:
             self.init_available_node_id()
 
     def check(self):
-        assert self.__node_gdf.crs == self.geo_crs, rf'Node层数据必须为WGS84 - EPSG:4326, 实际输入: {self.__node_gdf.crs}'
+        assert self.__node_gdf.crs.srs == self.geo_crs, rf'Node层数据必须为WGS84 - EPSG:4326, 实际输入: {self.__node_gdf.crs.srs}'
         gap_set = {node_id_field, geometry_field} - set(self.__node_gdf.columns)
         assert len(gap_set) == 0, rf'线层Link缺少以下字段:{gap_set}'
         assert len(self.__node_gdf[node_id_field]) == len(self.__node_gdf[node_id_field].unique()), \
             rf'字段{node_id_field}不唯一...'
         for col in [node_id_field]:
             assert len(self.__node_gdf[self.__node_gdf[col].isna()]) == 0, rf'点层Node字段{col}有空值...'
             self.__node_gdf[col] = self.__node_gdf[col].astype(int)
@@ -61,32 +61,32 @@
         return self.__node_gdf.copy()
 
     def modify_node_gdf(self, node_id_list: list[int], attr_field_list:list[str], val_list: list[list] = None):
         self.__node_gdf.loc[node_id_list, attr_field_list] = val_list
 
     @property
     def crs(self):
-        return self.__node_gdf.crs
+        return self.__node_gdf.crs.srs
 
     def to_plane_prj(self) -> None:
-        if self.__node_gdf.crs == self.planar_crs:
+        if self.__node_gdf.crs.srs == self.planar_crs:
             pass
         else:
             self.__node_gdf = self.__node_gdf.to_crs(self.planar_crs)
 
     def to_geo_prj(self) -> None:
-        if self.__node_gdf.crs == self.geo_crs:
+        if self.__node_gdf.crs.srs == self.geo_crs:
             pass
         else:
             self.__node_gdf = self.__node_gdf.to_crs(self.geo_crs)
 
     def init_available_node_id(self) -> None:
         max_node = self.__node_gdf[node_id_field].max()
         self.max_node_id = max_node
-        if self.max_node_id >= 10000000:
+        if self.max_node_id >= 10000:
             return None
         self.__available_node_id = list({i for i in range(1, max_node + 1)} - set(self.__node_gdf[node_id_field]))
 
     @property
     def available_node_id(self) -> int:
         if self.__available_node_id:
             now_node_id = self.__available_node_id.pop()
```

### Comparing `gotrackit-0.1.9/src/gotrackit/model/Markov.py` & `gotrackit-0.2.0/src/gotrackit/model/Markov.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # -- coding: utf-8 --
 # @Time    : 2023/12/9 8:29
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 """Markov Model Class"""
 
-
 import time
 import os.path
 import datetime
 import warnings
-import itertools
 import numpy as np
 import pandas as pd
 import networkx as nx
+import multiprocessing
 import geopandas as gpd
 from ..map.Net import Net
+from itertools import chain
 from datetime import timedelta
+from ..tools.group import cut_group
 from ..solver.Viterbi import Viterbi
 from ..gps.LocGps import GpsPointsGdf
+from ..tools.geo_process import prj_inf
 from ..WrapsFunc import function_time_cost
 from shapely.geometry import Point, LineString
 from ..GlobalVal import NetField, GpsField, MarkovField
-from ..tools.geo_process import n_equal_points, vector_angle
+from ..tools.geo_process import n_equal_points, hmm_vector_angle
 
 
 gps_field = GpsField()
 net_field = NetField()
 markov_field = MarkovField()
 
 from_link_f, to_link_f = markov_field.FROM_STATE, markov_field.TO_STATE
@@ -36,15 +38,16 @@
 
 
 class HiddenMarkov(object):
     """隐马尔可夫模型类"""
 
     def __init__(self, net: Net, gps_points: GpsPointsGdf, beta: float = 30.1, gps_sigma: float = 20.0,
                  not_conn_cost: float = 999.0, use_heading_inf: bool = True, heading_para_array: np.ndarray = None,
-                 dis_para: float = 0.1):
+                 dis_para: float = 0.1, top_k: int = 25, omitted_l: float = 6.0, multi_core: bool = True,
+                 core_num: int = 1):
         self.gps_points = gps_points
         self.net = net
         # (gps_seq, single_link_id): (prj_p, prj_dis, route_dis)
         self.__done_prj_dict: dict[tuple[int, int]: tuple[Point, float, float, float, np.ndarray]] = dict()
         self.__adj_seq_path_dict: dict[tuple[int, int], list[int, int]] = dict()
         self.__ft_transition_dict = dict()
         self.__ft_mapping_dict = dict()
@@ -58,51 +61,48 @@
         self.__s2s_route_l = dict()
         self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf = None, None, None
         self.path_cost_df = pd.DataFrame()
         self.is_warn = False
         self.not_conn_cost = not_conn_cost
         self.use_heading_inf = use_heading_inf
         if heading_para_array is None:
-            self.heading_para_array = np.array([1.0, 1.0, 1.0, 0.1, 0.00001, 0.000001, 0.00001, 0.000001, 0.000001])
+            self.heading_para_array = np.array([1.0, 1.0, 1.0, 0.1, 0.00001, 0.00001, 0.00001, 0.000001, 0.000001])
+        else:
+            self.heading_para_array = heading_para_array
         self.angle_slice = 180 / len(self.heading_para_array)
         self.dis_para = dis_para
         self.warn_info = list()
+        self.top_k = top_k
+        self.omitted_l = omitted_l
+        self.multi_core = multi_core
+        self.core_num = int(core_num) if int(core_num) <= os.cpu_count() else os.cpu_count()
+        self.gps_candidate_link = None
 
     def generate_markov_para(self):
 
         # self.__generate_markov_para()
-        self.__generate_transition_mat()
+        if self.multi_core and self.core_num >= 1:
+            self.__generate_transition_mat_alpha_multi()
+        else:
+            self.__generate_transition_mat()
         self.__generate_emission_mat()
 
     @function_time_cost
     def __generate_transition_mat(self):
 
-        # 依据一辆车的时序gps点和和底层路网生成转移概率矩阵和生成概率矩阵
-        # seq, geometry, single_link_id, from_node, to_node, dir, length
-        gps_candidate_link, _gap = self.gps_points.generate_candidate_link(net=self.net)
-
-        if _gap:
-            warnings.warn(rf'seq为: {_gap}的GPS点没有关联到任何候选路段..., 不会用于路径匹配计算...')
-
-            # 删除关联不到任何路段的gps点
-            self.gps_points.delete_target_gps(target_seq_list=list(_gap))
-
-        # 一定要排序
-        seq_list = sorted(list(gps_candidate_link[gps_field.POINT_SEQ_FIELD].unique()))
-
-        if len(seq_list) <= 1:
-            raise ValueError(r'GPS数据样本点不足2个, 请检查...')
+        # 计算 初步候选
+        seq_list = self.__generate_candidates()
 
         self.gps_points.calc_gps_point_dis()
-
+        # _ = pd.DataFrame()
         # 计算状态转移概率矩阵
         for i in range(0, len(seq_list) - 1):
-            from_link = gps_candidate_link[gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i]][
+            from_link = self.gps_candidate_link[self.gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i]][
                 net_field.SINGLE_LINK_ID_FIELD].to_list()
-            to_link = gps_candidate_link[gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i + 1]][
+            to_link = self.gps_candidate_link[self.gps_candidate_link[gps_field.POINT_SEQ_FIELD] == seq_list[i + 1]][
                 net_field.SINGLE_LINK_ID_FIELD].to_list()
 
             transition_df = pd.DataFrame([[int(f), int(t)] for f in from_link for t in to_link],
                                          columns=[markov_field.FROM_STATE,
                                                   markov_field.TO_STATE])
 
             transition_df[markov_field.ROUTE_LENGTH] = \
@@ -111,14 +111,15 @@
                                                         to_gps_seq=seq_list[i + 1],
                                                         from_link_id=item[markov_field.FROM_STATE],
                                                         to_link_id=item[markov_field.TO_STATE]), axis=1)
 
             transition_df[markov_field.DIS_GAP] = np.abs(-transition_df[
                 markov_field.ROUTE_LENGTH] + self.gps_points.get_gps_point_dis((seq_list[i], seq_list[i + 1])))
 
+            # _ = pd.concat([_, transition_df])
             self.__s2s_route_l[(seq_list[i], seq_list[i + 1])] = transition_df[
                 [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.ROUTE_LENGTH]].copy().set_index(
                 [markov_field.FROM_STATE, markov_field.TO_STATE])
 
             # 转成matrix
             transition_mat = transition_df[
                 [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.DIS_GAP]].set_index(
@@ -129,14 +130,16 @@
                 {i: t for i, t in zip(range(len(to_link)), sorted(to_link))}
             transition_mat = self.transition_probability(self.beta, transition_mat, self.dis_para)
 
             self.__ft_transition_dict[seq_list[i]] = transition_mat
             self.__ft_mapping_dict[seq_list[i]] = f_mapping
             self.__ft_mapping_dict[seq_list[i + 1]] = t_mapping
 
+        # print(_)
+
     @function_time_cost
     def __generate_emission_mat(self):
 
         # 计算每个观测点的生成概率, 这是在计算状态转移概率之后, 已经将关联不到的GPS点删除了
         # 这里的向量是候选路段的投影点的方向向量
         emission_p_df = pd.DataFrame(self.__done_prj_dict).T.reset_index(drop=False).rename(
             columns={'level_0': gps_field.POINT_SEQ_FIELD, 'level_1': net_field.SINGLE_LINK_ID_FIELD,
@@ -146,15 +149,16 @@
         if self.use_heading_inf:
             self.gps_points.calc_diff_heading()
             emission_p_df = pd.merge(emission_p_df, self.gps_points.gps_gdf[[gps_field.POINT_SEQ_FIELD,
                                                                              gps_field.DIFF_VEC]], how='left',
                                      on=gps_field.POINT_SEQ_FIELD)
             emission_p_df[markov_field.HEADING_GAP] = \
                 emission_p_df.apply(
-                    lambda row: vector_angle(v1=row[gps_field.DIFF_VEC], v2=row[net_field.LINK_VEC_FIELD]),
+                    lambda row: hmm_vector_angle(gps_diff_vec=row[gps_field.DIFF_VEC],
+                                                 link_dir_vec=row[net_field.LINK_VEC_FIELD], omitted_l=self.omitted_l),
                     axis=1)
         else:
             emission_p_df[markov_field.HEADING_GAP] = 0
         emission_p_df[markov_field.HEADING_GAP] = emission_p_df[markov_field.HEADING_GAP].astype(object)
         emission_p_df[markov_field.PRJ_L] = emission_p_df[markov_field.PRJ_L].astype(object)
         emission_p_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
                                   ascending=[True, True], inplace=True)
@@ -165,14 +169,65 @@
         self.__emission_mat_dict = {
             int(row[gps_field.POINT_SEQ_FIELD]): self.emission_probability(dis=row[markov_field.PRJ_L],
                                                                            sigma=self.gps_sigma,
                                                                            heading_gap=row[markov_field.HEADING_GAP])
             for _, row in
             emission_p_df.iterrows()}
 
+    def __generate_candidates(self) -> list[int]:
+        # 初步依据gps点buffer得到候选路段, 关联不到的GPS点删除掉
+        # seq, geometry, single_link_id, from_node, to_node, dir, length
+        gps_candidate_link, _gap = self.gps_points.generate_candidate_link(net=self.net)
+
+        if gps_candidate_link.empty:
+            raise ValueError(r'GPS数据样本点无法关联到任何路段, 请检查路网完整性或者增加gps_buffer参数...')
+
+        if _gap:
+            warnings.warn(rf'seq为: {_gap}的GPS点没有关联到任何候选路段..., 不会用于路径匹配计算...')
+            # 删除关联不到任何路段的gps点
+            self.gps_points.delete_target_gps(target_seq_list=list(_gap))
+
+        # 一定要排序
+        seq_list = sorted(list(gps_candidate_link[gps_field.POINT_SEQ_FIELD].unique()))
+        if len(seq_list) <= 1:
+            raise ValueError(
+                r'经过路段关联, 删除掉无法关联到路段的GPS点后, GPS数据样本点不足2个, 请检查路网完整性或者增加gps_buffer参数...')
+        self.gps_candidate_link = gps_candidate_link
+        return seq_list
+
+    @staticmethod
+    def filter_k_candidates(preliminary_candidate_link: gpd.GeoDataFrame or pd.DataFrame = None,
+                            top_k: int = 10) -> tuple[gpd.GeoDataFrame or pd.DataFrame, dict]:
+        """
+        对Buffer范围内的初步候选路段进行二次筛选, 需按照投影距离排名前K位, 并且得到计算发射概率需要的数据
+        :param preliminary_candidate_link:
+        :param top_k
+        :return:
+        """
+        preliminary_candidate_link[
+            ['prj_p', 'prj_dis', 'route_dis', 'l_length', 'split_line', 'p_vec']] = preliminary_candidate_link.apply(
+            lambda row: prj_inf(p=row[gps_field.GEOMETRY_FIELD], line=row['single_link_geo']), axis=1,
+            result_type='expand')
+        del preliminary_candidate_link['split_line']
+        preliminary_candidate_link.sort_values(by=[gps_field.POINT_SEQ_FIELD, 'prj_dis'], ascending=[True, True],
+                                               inplace=True)
+        k_candidate_link = preliminary_candidate_link.groupby(gps_field.POINT_SEQ_FIELD).head(top_k)
+        k_candidate_link.reset_index(inplace=True, drop=True)
+        done_prj_dict = {
+            (gps_seq, single_link_id): (prj_p, prj_dis, route_dis, l_length, p_vec) for
+            gps_seq, single_link_id, prj_p, prj_dis, route_dis, l_length, p_vec in
+            zip(k_candidate_link[gps_field.POINT_SEQ_FIELD],
+                k_candidate_link[net_field.SINGLE_LINK_ID_FIELD],
+                k_candidate_link['prj_p'],
+                k_candidate_link['prj_dis'],
+                k_candidate_link['route_dis'],
+                k_candidate_link['l_length'],
+                k_candidate_link['p_vec'])}
+        return k_candidate_link, done_prj_dict
+
     def solve(self, use_lop_p: bool = True):
         """
 
         :param use_lop_p: 是否使用对数概率, 避免浮点数精度下溢
         :return:
         """
 
@@ -181,14 +236,174 @@
                                 o_mat_dict=self.__emission_mat_dict,
                                 t_mat_dict=self.__ft_transition_dict, use_log_p=use_lop_p)
         self.__solver.init_model()
         self.index_state_list = self.__solver.iter_model()
 
         print(self.index_state_list)
 
+    @function_time_cost
+    def __generate_transition_mat_alpha_multi(self):
+        n = self.core_num
+
+        # 计算 初步候选, 经过这一步, 实际匹配用到的GPS点已经完全确定
+        # 得到self.gps_candidate_link
+        seq_list = self.__generate_candidates()
+
+        # 已经删除了关联不到任何路段的GPS点, 基于新的序列计算相邻GPS点距离
+        # gps_field.POINT_SEQ_FIELD, gps_field.NEXT_SEQ, gps_field.ADJ_DIS
+        gps_pre_next_dis_df = self.gps_points.calc_pre_next_dis()
+        gps_pre_next_dis_df.rename(columns={gps_field.POINT_SEQ_FIELD: gps_field.FROM_GPS_SEQ,
+                                            gps_field.NEXT_SEQ: gps_field.TO_GPS_SEQ}, inplace=True)
+
+        single_link_ft_df = self.net.get_link_data()[[net_field.SINGLE_LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
+                                                      net_field.TO_NODE_FIELD]].copy()
+        single_link_ft_df.reset_index(inplace=True, drop=True)
+
+        ft_list = [[i, i + 1, seq_list[i], seq_list[i + 1]] for i in range(0, len(seq_list) - 1)]
+        g = self.net.graph
+        if n > 1:
+            print(f'using multiprocessing - {n} cores')
+            ft_group = cut_group(obj_list=ft_list, n=n)
+            del ft_list
+            pool = multiprocessing.Pool(processes=len(ft_group))
+            result_list = []
+            for i in range(0, len(ft_group)):
+                result = pool.apply_async(self.generate_transition_mat_alpha,
+                                          args=(ft_group[i], single_link_ft_df, self.gps_candidate_link,
+                                                gps_pre_next_dis_df, g,
+                                                self.net.search_method, self.net.weight_field, self.net.cache_path,
+                                                self.net.not_conn_cost))
+                result_list.append(result)
+            pool.close()
+            pool.join()
+            adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict = \
+                dict(), dict(), dict(), dict(), dict()
+            for res in result_list:
+                _adj_seq_path_dict, _ft_transition_dict, _ft_mapping_dict, _s2s_route_l, _prj_done_dict = res.get()
+                adj_seq_path_dict.update(_adj_seq_path_dict)
+                ft_transition_dict.update(_ft_transition_dict)
+                ft_mapping_dict.update(_ft_mapping_dict)
+                s2s_route_l.update(_s2s_route_l)
+                prj_done_dict.update(_prj_done_dict)
+        else:
+            adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict = \
+                self.generate_transition_mat_alpha(
+                    ft_list, single_link_ft_df, self.gps_candidate_link, gps_pre_next_dis_df, g,
+                    self.net.search_method, self.net.weight_field, self.net.cache_path,
+                    self.net.not_conn_cost)
+
+        self.__adj_seq_path_dict = adj_seq_path_dict
+        self.__ft_mapping_dict = ft_mapping_dict
+        self.__ft_transition_dict = ft_transition_dict
+        self.__s2s_route_l = s2s_route_l
+        self.__done_prj_dict = prj_done_dict
+
+    def generate_transition_mat_alpha(self, gps_ft_list: list = None, single_link_ft_df: pd.DataFrame = None,
+                                      pre_seq_candidate: pd.DataFrame = None,
+                                      gps_pre_next_dis_df: pd.DataFrame = None,
+                                      g: nx.DiGraph = None,
+                                      method: str = None, weight_field: str = 'length',
+                                      cache_path: bool = True, not_conn_cost: float = 999.0) -> \
+            tuple[dict, dict, dict, dict, dict]:
+        done_stp_cache, done_cost_cache, adj_seq_path_dict, s2s_route_l = dict(), dict(), dict(), dict()
+        ft_transition_dict, ft_mapping_dict = dict(), dict()
+        # seq_candidate这里是初步的
+        gps_ft_df = pd.DataFrame(gps_ft_list, columns=['idx', 'next_idx', 'f_gps_seq', 't_gps_seq'])
+        del gps_ft_df['idx']
+        del gps_ft_df['next_idx']
+        used_gps_seq = list(set(gps_ft_df['f_gps_seq']) | set(gps_ft_df['t_gps_seq']))
+        # p_name = os.getpid()
+        # print(rf'{p_name}:{used_gps_seq}')
+        # print(rf'{p_name}:{len(used_gps_seq)}')
+        pre_seq_candidate = pre_seq_candidate[
+                pre_seq_candidate[gps_field.POINT_SEQ_FIELD].isin(used_gps_seq)].copy()
+        seq_k_candidate, prj_done_dict = \
+            self.filter_k_candidates(preliminary_candidate_link=pre_seq_candidate,
+                                     top_k=self.top_k)
+        # print(rf'{p_name}:{seq_k_candidate}')
+        del pre_seq_candidate
+        del used_gps_seq
+        seq_k_candidate = seq_k_candidate.groupby(gps_field.POINT_SEQ_FIELD).agg({net_field.SINGLE_LINK_ID_FIELD: list})
+
+        all_ft_state_list = list(chain(*[[[idx, next_idx, f_gps_seq, t_gps_seq, from_link, to_link]
+                                          for from_link in seq_k_candidate.at[f_gps_seq, net_field.SINGLE_LINK_ID_FIELD]
+                                          for to_link in seq_k_candidate.at[t_gps_seq, net_field.SINGLE_LINK_ID_FIELD]]
+                                         for idx, next_idx, f_gps_seq, t_gps_seq in gps_ft_list]))
+        # print(rf'{p_name}: {len(all_ft_state_list)}')
+        transition_df = pd.DataFrame(all_ft_state_list, columns=['idx', 'next_idx',
+                                                                 gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ,
+                                                                 markov_field.FROM_STATE, markov_field.TO_STATE])
+        # print(transition_df)
+        del all_ft_state_list
+        transition_df = self.diy_merge(left_df=transition_df,
+                                       right_df=single_link_ft_df,
+                                       left_key=markov_field.FROM_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
+                                       label='from')
+        transition_df = self.diy_merge(left_df=transition_df,
+                                       right_df=single_link_ft_df,
+                                       left_key=markov_field.TO_STATE, right_key=net_field.SINGLE_LINK_ID_FIELD,
+                                       label='to')
+        del single_link_ft_df
+        transition_df[markov_field.ROUTE_LENGTH] = \
+            transition_df.apply(
+                lambda item: self.calc_route_length_alpha(from_gps_seq=item[gps_field.FROM_GPS_SEQ],
+                                                          to_gps_seq=item[gps_field.TO_GPS_SEQ],
+                                                          from_link_id=item[markov_field.FROM_STATE],
+                                                          to_link_id=item[markov_field.TO_STATE],
+                                                          from_link_ft=(item['from_link_f'], item['from_link_t']),
+                                                          to_link_ft=(item['to_link_f'], item['to_link_t']),
+                                                          di_g=g,
+                                                          weight_field=weight_field,
+                                                          method=method,
+                                                          prj_done_dict=prj_done_dict,
+                                                          done_stp_cache=done_stp_cache,
+                                                          done_cost_cache=done_cost_cache,
+                                                          cache_path=cache_path,
+                                                          not_conn_cost=not_conn_cost,
+                                                          adj_seq_path_dict=adj_seq_path_dict), axis=1)
+        del done_cost_cache, done_stp_cache, g
+        transition_df = pd.merge(transition_df, gps_pre_next_dis_df, on=[gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ],
+                                 how='left')
+
+        transition_df[markov_field.DIS_GAP] = np.abs(
+            -transition_df[markov_field.ROUTE_LENGTH] + transition_df[gps_field.ADJ_DIS])
+
+        for (idx, next_idx, f_gps_seq, t_gps_seq), df in transition_df.groupby(
+                ['idx', 'next_idx', gps_field.FROM_GPS_SEQ, gps_field.TO_GPS_SEQ]):
+            s2s_route_l[(f_gps_seq, t_gps_seq)] = df[
+                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.ROUTE_LENGTH]].copy().set_index(
+                [markov_field.FROM_STATE, markov_field.TO_STATE])
+
+            # 转成matrix
+            transition_mat = df[
+                [markov_field.FROM_STATE, markov_field.TO_STATE, markov_field.DIS_GAP]].set_index(
+                [markov_field.FROM_STATE, markov_field.TO_STATE]).unstack().values
+            from_link, to_link = list(set(df[markov_field.FROM_STATE])), list(set(df[markov_field.TO_STATE]))
+            # 索引映射
+            f_mapping, t_mapping = {i: f for i, f in zip(range(len(from_link)), sorted(from_link))}, \
+                {i: t for i, t in zip(range(len(to_link)), sorted(to_link))}
+            transition_mat = self.transition_probability(self.beta, transition_mat, self.dis_para)
+
+            ft_transition_dict[f_gps_seq] = transition_mat
+            ft_mapping_dict[f_gps_seq] = f_mapping
+            ft_mapping_dict[t_gps_seq] = t_mapping
+
+        return adj_seq_path_dict, ft_transition_dict, ft_mapping_dict, s2s_route_l, prj_done_dict
+
+    @staticmethod
+    def diy_merge(left_df: pd.DataFrame, right_df: pd.DataFrame or gpd.GeoDataFrame = None, left_key: str = None,
+                  right_key: str = None, label: str = 'from'):
+        df = pd.merge(left_df, right_df, left_on=left_key, right_on=right_key, how='left')
+
+        df.rename(columns={net_field.FROM_NODE_FIELD: label + '_link_f',
+                           net_field.TO_NODE_FIELD: label + '_link_t'}, inplace=True)
+
+        df.drop(columns=[right_key], axis=1, inplace=True)
+        return df
+
     def calc_route_length(self, from_gps_seq: int = None, to_gps_seq: int = None, from_link_id: int = None,
                           to_link_id: int = None) -> float:
         """
         :param from_gps_seq: 上一观测时刻的gps点序号
         :param to_gps_seq: 当前观测时刻的gps点序号
         :param from_link_id: 上一观测时刻候选link_id
         :param to_link_id: 当前观测时刻候选link_id
@@ -197,30 +412,14 @@
         # prj_p, prj_dis, route_dis
         (from_prj_p, from_prj_dis, from_route_dis, from_l_length, from_p_vec) = \
             self.cache_emission_data(gps_seq=from_gps_seq, single_link_id=from_link_id)
 
         (to_prj_p, to_prj_dis, to_route_dis, to_l_length, to_p_vec) = \
             self.cache_emission_data(gps_seq=to_gps_seq, single_link_id=to_link_id)
 
-        # if (from_gps_seq, from_link_id) in self.__done_prj_dict.keys():
-        #     (from_prj_p, from_prj_dis, from_route_dis, from_l_length) = self.__done_prj_dict[
-        #         (from_gps_seq, from_link_id)]
-        # else:
-        #     (from_prj_p, from_prj_dis, from_route_dis, from_l_length) = self.get_gps_prj_info(
-        #         target_link_id=from_link_id,
-        #         gps_seq=from_gps_seq)
-        #     self.__done_prj_dict.update(
-        #         {(from_gps_seq, from_link_id): (from_prj_p, from_prj_dis, from_route_dis, from_l_length)})
-        # if (to_gps_seq, to_link_id) in self.__done_prj_dict.keys():
-        #     (to_prj_p, to_prj_dis, to_route_dis, to_l_length) = self.__done_prj_dict[(to_gps_seq, to_link_id)]
-        # else:
-        #     (to_prj_p, to_prj_dis, to_route_dis, to_l_length) = self.get_gps_prj_info(target_link_id=to_link_id,
-        #                                                                               gps_seq=to_gps_seq)
-        #     self.__done_prj_dict.update({(to_gps_seq, to_link_id): (to_prj_p, to_prj_dis, to_route_dis, to_l_length)})
-
         # 基于投影信息计算路径长度
         from_link_ft, to_link_ft = self.net.get_link_from_to(from_link_id, _type='single'), \
             self.net.get_link_from_to(to_link_id, _type='single')
 
         # same link
         if from_link_id == to_link_id:
             route_l = np.absolute(from_route_dis - to_route_dis)
@@ -263,230 +462,156 @@
                 route_l2 = to_route_dis
 
             route_l = np.absolute(route_l1 + route_l2)
             return route_l
         else:
             return self.not_conn_cost
 
+    def calc_route_length_alpha(self, from_gps_seq: int = None, to_gps_seq: int = None,
+                                from_link_id: int = None, to_link_id: int = None,
+                                from_link_ft=None, to_link_ft=None,
+                                done_stp_cache: dict = None, done_cost_cache: dict = None,
+                                prj_done_dict: dict = None,
+                                adj_seq_path_dict: dict = None,
+                                di_g: nx.DiGraph = None,
+                                method: str = None, weight_field: str = 'length',
+                                cache_path: bool = True, not_conn_cost: float = 999.0) -> float:
+        """"""
+        from_prj_p, from_prj_dis, from_route_dis, from_l_length, from_p_vec = prj_done_dict[
+            (from_gps_seq, from_link_id)]
+        to_prj_p, to_prj_dis, to_route_dis, to_l_length, to_p_vec = prj_done_dict[
+            (to_gps_seq, to_link_id)]
+
+        # same link
+        if from_link_id == to_link_id:
+            route_l = np.absolute(from_route_dis - to_route_dis)
+            return route_l
+
+        # one same node
+        dup_node_list = list(set(from_link_ft) & set(to_link_ft))
+        if len(dup_node_list) == 1:
+            dup_node = dup_node_list[0]
+            if (dup_node == from_link_ft[1]) and (dup_node == to_link_ft[0]):
+                route_l = from_l_length - from_route_dis + to_route_dis
+                return np.absolute(route_l)
+            else:
+                return self.not_conn_cost
+        # 正好相反的f-t
+        elif len(dup_node_list) == 2:
+            route_l = from_l_length - from_route_dis + to_route_dis
+            return np.absolute(route_l)
+        o_node,  d_node = from_link_ft[0], to_link_ft[0]
+        route_item = self.get_od_cost_alpha(g=di_g, o_node=o_node, d_node=d_node,
+                                            done_stp_cache=done_stp_cache, done_cost_cache=done_cost_cache,
+                                            method=method,
+                                            weight_field=weight_field, cache_path=cache_path,
+                                            not_conn_cost=not_conn_cost)
+        if len(route_item[0]) > 2:
+            adj_seq_path_dict[(from_link_id, to_link_id)] = route_item[0]
+        if route_item[0]:
+            if route_item[0][1] != from_link_ft[1]:
+                return not_conn_cost
+            else:
+                route_l1 = route_item[1] - from_route_dis
+
+            if route_item[0][-2] == to_link_ft[1]:
+                # abnormal
+                return not_conn_cost
+            else:
+                route_l2 = to_route_dis
+
+            route_l = np.absolute(route_l1 + route_l2)
+            return route_l
+        else:
+            return not_conn_cost
+
+    def get_od_cost_alpha(self, g: nx.DiGraph = None, o_node: int = None, d_node: int = None,
+                          cache_path: bool = True, done_stp_cache: dict = None,
+                          done_cost_cache: dict = None, method: str = None,
+                          weight_field: str = 'length', not_conn_cost: float = 999.0) -> tuple[list, float]:
+        """"""
+
+        if o_node in done_stp_cache.keys():
+            try:
+                node_path = done_stp_cache[o_node][d_node]
+                cost = done_cost_cache[o_node][d_node]
+            except KeyError:
+                return [], not_conn_cost
+        else:
+            self.calc_shortest_path_alpha(g=g, source=o_node, method=method, done_cost_cache=done_cost_cache,
+                                          done_stp_cache=done_stp_cache, weight_field=weight_field)
+            try:
+                node_path = done_stp_cache[o_node][d_node]
+                cost = done_cost_cache[o_node][d_node]
+                if not cache_path:
+                    del done_stp_cache[o_node]
+                    del done_cost_cache[o_node]
+            except KeyError:
+                return [], not_conn_cost
+
+        return node_path, cost
+
+    def calc_shortest_path_alpha(self, g: nx.DiGraph = None, source: int = None, done_stp_cache: dict = None,
+                                 done_cost_cache: dict = None, method: str = None,
+                                 weight_field: str = 'length'):
+        """
+
+        :param g:
+        :param source:
+        :param done_stp_cache:
+        :param done_cost_cache:
+        :param method:
+        :param weight_field:
+        :return:
+        """
+        try:
+            done_cost_cache[source], done_stp_cache[source] = self._single_source_path_alpha(
+                g, source=source,
+                method=method, weight_field=weight_field)
+        except nx.NetworkXNoPath:
+            pass
+
+    @staticmethod
+    def _single_source_path_alpha(g: nx.DiGraph = None, source: int = None, method: str = 'dijkstra',
+                                  weight_field: str = None) -> tuple[dict[int, int], dict[int, list]]:
+        if method == 'dijkstra':
+            return nx.single_source_dijkstra(g, source, weight=weight_field)
+        else:
+            return nx.single_source_bellman_ford(g, source, weight=weight_field)
+
     def cache_emission_data(self, gps_seq: int = None, single_link_id: int = None) -> \
             tuple[Point, float, float, float, np.ndarray]:
         """
         :param gps_seq:
         :param single_link_id:
         :return:
         """
         if (gps_seq, single_link_id) in self.__done_prj_dict.keys():
             # already calculated
             (prj_p, prj_dis, route_dis, l_length, p_vec) = self.__done_prj_dict[
                 (gps_seq, single_link_id)]
         else:
             # new calc and cache
+            print('# new calc and cache')
             (prj_p, prj_dis, route_dis, l_length, p_vec) = self.get_gps_prj_info(
                 target_link_id=single_link_id,
                 gps_seq=gps_seq)
             self.__done_prj_dict.update(
                 {(gps_seq, single_link_id): (prj_p, prj_dis, route_dis, l_length, p_vec)})
         return prj_p, prj_dis, route_dis, l_length, p_vec
 
-
-    # @function_time_cost
-    # def __generate_markov_para(self, use_swifter: bool = False):
-    #     # 依据一辆车的时序gps点和和底层路网生成转移概率矩阵和生成概率矩阵
-    #     # seq, geometry, single_link_id, from_node, to_node, dir, length
-    #     gps_candidate_link, _gap = self.gps_points.generate_candidate_link(net=self.net)
-    #
-    #     # {seq1: {'single_link_id': [candidate_link]}, seq2: ...}
-    #     gps_candidate_link_dict = gps_candidate_link.groupby([gps_field.POINT_SEQ_FIELD]).agg(
-    #         {net_field.SINGLE_LINK_ID_FIELD: list}).to_dict(orient='index')
-    #
-    #     if _gap:
-    #         warnings.warn(rf'seq为: {_gap}的GPS点没有关联到任何候选路段..., 不会用于路径匹配计算...')
-    #
-    #         # 删除关联不到任何路段的gps点
-    #         self.gps_points.delete_target_gps(target_seq_list=list(_gap))
-    #
-    #     # 一定要排序
-    #     seq_list = sorted(list(gps_candidate_link_dict.keys()))
-    #
-    #     if len(seq_list) <= 1:
-    #         raise ValueError(r'GPS数据样本点不足2个, 请检查...')
-    #
-    #     self.gps_points.calc_gps_point_dis()
-    #
-    #     ft_gps_candidate = \
-    #         {(seq_list[i], seq_list[i + 1]): [
-    #             list(itertools.product(gps_candidate_link_dict[seq_list[i]][net_field.SINGLE_LINK_ID_FIELD],
-    #                                    gps_candidate_link_dict[seq_list[i + 1]][net_field.SINGLE_LINK_ID_FIELD]))]
-    #             for i in range(0, len(seq_list) - 1)}
-    #
-    #     seq_link_df = gps_candidate_link.groupby([gps_field.POINT_SEQ_FIELD]).agg(
-    #         {net_field.SINGLE_LINK_ID_FIELD: list})
-    #     self.__ft_mapping_dict = {
-    #         seq: {i: link for i, link in enumerate(sorted(seq_link_df.at[seq, net_field.SINGLE_LINK_ID_FIELD]))} for seq
-    #         in seq_link_df.index}
-    #
-    #     # print(self.__ft_mapping_dict)
-    #     transit_df = pd.DataFrame(ft_gps_candidate).T.reset_index(drop=False).rename(
-    #         columns={'level_0': from_gps_f, 'level_1': to_gps_f, 0: 'ft_link'})
-    #
-    #     transit_df = transit_df.explode(column='ft_link', ignore_index=True)
-    #
-    #     all_required_source_list = \
-    #         gps_candidate_link[gps_candidate_link[gps_field.POINT_SEQ_FIELD].isin(seq_list[:-1])][
-    #             net_field.FROM_NODE_FIELD].unique()
-    #
-    #     # 提前计算最短路信息
-    #     path_cost_df = pd.DataFrame({'source': all_required_source_list})
-    #     if not use_swifter:
-    #         path_cost_df['path'] = path_cost_df.apply(lambda row:
-    #                                                   self.net._single_source_path(g=self.net.graph,
-    #                                                                                source=row['source'],
-    #                                                                                method=self.net.search_method,
-    #                                                                                weight_field=self.net.weight_field),
-    #                                                   axis=1)
-    #     else:
-    #         path_cost_df['path'] = path_cost_df.swifter.apply(lambda row:
-    #                                                            self.net._single_source_path(g=self.net.graph,
-    #                                                                                         source=row['source'],
-    #                                                                                         method=self.net.search_method,
-    #                                                                                         weight_field=self.net.weight_field),
-    #                                                            axis=1)
-    #
-    #     # 计算发射概率
-    #
-    #     print(path_cost_df)
-    #     path_cost_df.set_index('source', inplace=True)
-    #     self.path_cost_df = path_cost_df
-    #
-    #
-    #     # dis of (gps, prj_gps)
-    #     gps_candidate_link[['prj_p', markov_field.PRJ_L, 'route_dis', 'l_length']] = gps_candidate_link.apply(
-    #         lambda row: self.get_gps_prj_info(target_link_id=row[net_field.SINGLE_LINK_ID_FIELD],
-    #                                           gps_seq=row[gps_field.POINT_SEQ_FIELD]), axis=1, result_type='expand')
-    #
-    #     # 计算done_prj_dict
-    #     self.__done_prj_dict = {(row[gps_field.POINT_SEQ_FIELD], row[net_field.SINGLE_LINK_ID_FIELD]):
-    #                                 (row['prj_p'], row[markov_field.PRJ_L], row['route_dis'], row['l_length']) for
-    #                             _, row in
-    #                             gps_candidate_link.iterrows()}
-    #
-    #
-    #     emission_p_df = gps_candidate_link[
-    #         [gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD, markov_field.PRJ_L]].copy()
-    #
-    #     emission_p_df.sort_values(by=[gps_field.POINT_SEQ_FIELD, net_field.SINGLE_LINK_ID_FIELD],
-    #                               ascending=[True, True], inplace=True)
-    #
-    #     emission_p_df = \
-    #         emission_p_df.groupby([gps_field.POINT_SEQ_FIELD])[markov_field.PRJ_L].agg(
-    #             lambda x: list(x)).reset_index(drop=False)
-    #     # emission_p_df[markov_field.PRJ_L] = emission_p_df[markov_field.PRJ_L].swifter.apply(lambda row: np.array(row))
-    #     emission_p_df[markov_field.PRJ_L] = emission_p_df[markov_field.PRJ_L].apply(lambda row: np.array(row))
-    #
-    #     self.__emission_mat_dict = {
-    #         int(row[gps_field.POINT_SEQ_FIELD]): self.emission_probability(dis=row[markov_field.PRJ_L],
-    #                                                                        sigma=self.gps_sigma) for _, row in
-    #         emission_p_df.iterrows()}
-    #
-    #     def ft_link_path_item(from_link, to_link):
-    #         try:
-    #             source_item = path_cost_df.at[from_link, 'path']
-    #             return source_item[1][to_link], source_item[0][to_link]
-    #         except KeyError:
-    #             return [], NOT_CONN_COST
-    #
-    #     # 计算转移概率
-    #     transit_df[markov_field.ROUTE_LENGTH] = \
-    #         transit_df.apply(
-    #             lambda item: self._calc_route_length(from_link_id=item['ft_link'][0],
-    #                                                  to_link_id=item['ft_link'][1],
-    #                                                  from_route_dis=self.__done_prj_dict[
-    #                                                      (item[from_gps_f], item['ft_link'][0])][1],
-    #                                                  to_route_dis=self.__done_prj_dict[
-    #                                                      (item[to_gps_f], item['ft_link'][1])][1],
-    #                                                  from_l_length=self.__done_prj_dict[
-    #                                                      (item[from_gps_f], item['ft_link'][0])][3]
-    #                                                  ), axis=1)
-    #
-    #
-    #     # transit_df[markov_field.ROUTE_LENGTH] = \
-    #     #     transit_df.swifter.apply(
-    #     #         lambda item: self._calc_route_length(from_link_id=item['ft_link'][0],
-    #     #                                              to_link_id=item['ft_link'][1],
-    #     #                                              from_route_dis=self.__done_prj_dict[
-    #     #                                                  (item[from_gps_f], item['ft_link'][0])][1],
-    #     #                                              to_route_dis=self.__done_prj_dict[
-    #     #                                                  (item[to_gps_f], item['ft_link'][1])][1],
-    #     #                                              from_l_length=self.__done_prj_dict[
-    #     #                                                  (item[from_gps_f], item['ft_link'][0])][3]
-    #     #                                              ), axis=1)
-    #     print(transit_df)
-    #
-    # def _calc_route_length(self, from_route_dis: float = None, to_route_dis: float = None,
-    #                        from_l_length: float = None,
-    #                        from_link_id: int = None, to_link_id: int = None) -> float:
-    #     """
-    #     :param from_route_dis: 上一观测时刻的gps点序号
-    #     :param to_route_dis: 当前观测时刻的gps点序号
-    #     :param from_link_id: 上一观测时刻候选link_id
-    #     :param to_link_id: 当前观测时刻候选link_id
-    #     :return:
-    #     """
-    #     # 基于投影信息计算路径长度
-    #     from_link_ft, to_link_ft = self.net.get_link_from_to(from_link_id), self.net.get_link_from_to(to_link_id)
-    #
-    #     # same link
-    #     if from_link_id == to_link_id:
-    #         route_l = np.absolute(from_route_dis - to_route_dis)
-    #         return route_l
-    #
-    #     # one same node
-    #     dup_node_list = list(set(from_link_ft) & set(to_link_ft))
-    #     if len(dup_node_list) == 1:
-    #         dup_node = dup_node_list[0]
-    #         if (dup_node == from_link_ft[1]) and (dup_node == to_link_ft[0]):
-    #             route_l = from_l_length - from_route_dis + to_route_dis
-    #             return np.absolute(route_l)
-    #         else:
-    #             return NOT_CONN_COST
-    #     # 正好相反的f-t
-    #     elif len(dup_node_list) == 2:
-    #         route_l = from_l_length - from_route_dis + to_route_dis
-    #         return np.absolute(route_l)
-    #
-    #     try:
-    #         source_item = self.path_cost_df.at[from_link_ft[0], 'path']
-    #         route_item = [source_item[1][to_link_ft[0]], source_item[0][to_link_ft[0]]]
-    #     except KeyError:
-    #         route_item = [], NOT_CONN_COST
-    #
-    #     if len(route_item[0]) > 2:
-    #         self.__adj_seq_path_dict[(from_link_id, to_link_id)] = route_item[0]
-    #     if route_item[0]:
-    #         if route_item[0][1] != from_link_ft[1]:
-    #             return NOT_CONN_COST
-    #         else:
-    #             route_l1 = route_item[1] - from_route_dis
-    #
-    #         if route_item[0][-2] == to_link_ft[1]:
-    #             # abnormal
-    #             return NOT_CONN_COST
-    #         else:
-    #             route_l2 = to_route_dis
-    #
-    #         route_l = np.absolute(route_l1 + route_l2)
-    #         return route_l
-    #     else:
-    #         return NOT_CONN_COST
-    #
-    #
     def get_gps_prj_info(self, gps_seq: int = None, target_link_id: int = None) -> \
             tuple[Point, float, float, float, np.ndarray]:
         return self.gps_points.get_prj_inf(line=self.net.get_link_geo(target_link_id, _type='single'), seq=gps_seq)
 
+    def get_gps_prj_info_alpha(self, gps_geo: Point = None, target_link_geo: LineString = None) -> \
+            tuple[Point, float, float, float, np.ndarray]:
+        (prj_p, prj_dis, route_dis, l_length, _, p_vec) = prj_inf(gps_geo, target_link_geo)
+        return prj_p, prj_dis, route_dis, l_length, p_vec
+
     @staticmethod
     def transition_probability(beta: float = 30.2, dis_gap: float or np.ndarray = None, dis_para: float = 0.1):
         """
         dis_gap = straight_l - route_l
         :param beta:
         :param dis_gap:
         :param dis_para
@@ -562,23 +687,38 @@
             gps_link_state_df.reset_index(inplace=True, drop=True)
 
         # 给每个gps点打上路网link标签, 存在GPS匹配不到路段的情况(比如buffer范围内无候选路段)
         gps_match_res_gdf = pd.merge(gps_match_res_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.AGENT_ID_FIELD,
                                                         gps_field.LNG_FIELD, gps_field.LAT_FIELD, gps_field.TIME_FIELD,
                                                         gps_field.GEOMETRY_FIELD]],
                                      gps_link_state_df, on=gps_field.POINT_SEQ_FIELD, how='right')
+        del gps_link_state_df
         gps_match_res_gdf.loc[gps_match_res_gdf[gps_field.NEXT_LINK_FIELD].isna(), net_field.GEOMETRY_FIELD] = \
             omitted_gps_state_df[net_field.GEOMETRY_FIELD].to_list()
         gps_match_res_gdf.loc[gps_match_res_gdf[gps_field.NEXT_LINK_FIELD].isna(), gps_field.TIME_FIELD] = \
             omitted_gps_state_df[gps_field.TIME_FIELD].to_list()
 
         gps_match_res_gdf.drop(columns=[gps_field.NEXT_LINK_FIELD], axis=1, inplace=True)
-        gps_match_res_gdf = gpd.GeoDataFrame(gps_match_res_gdf, geometry=net_field.GEOMETRY_FIELD,
+        gps_match_res_gdf = gpd.GeoDataFrame(gps_match_res_gdf, geometry=gps_field.GEOMETRY_FIELD,
                                              crs=self.gps_points.crs)
-        self.gps_match_res_gdf = gps_match_res_gdf.to_crs(self.gps_points.geo_crs)
+        gps_match_res_gdf = gps_match_res_gdf.to_crs(self.gps_points.geo_crs)
+        gps_match_res_gdf[[gps_field.LNG_FIELD, gps_field.LAT_FIELD]] = gps_match_res_gdf.apply(
+            lambda row: (row[gps_field.GEOMETRY_FIELD].x, row[gps_field.GEOMETRY_FIELD].y), axis=1,
+            result_type='expand')
+        prj_gdf = gps_match_res_gdf[[markov_field.PRJ_GEO]].copy()
+        del gps_match_res_gdf[markov_field.PRJ_GEO]
+        prj_gdf.dropna(subset=[markov_field.PRJ_GEO], inplace=True)
+        prj_gdf = gpd.GeoDataFrame(prj_gdf, geometry=markov_field.PRJ_GEO, crs=self.gps_points.plane_crs)
+        prj_gdf = prj_gdf.to_crs(self.gps_points.geo_crs)
+        prj_gdf[['prj_lng', 'ptj_lat']] = prj_gdf.apply(
+            lambda row: (row[markov_field.PRJ_GEO].x, row[markov_field.PRJ_GEO].y), axis=1,
+            result_type='expand')
+        gps_match_res_gdf = pd.merge(gps_match_res_gdf, prj_gdf, how='left', left_index=True, right_index=True)
+        del prj_gdf
+        self.gps_match_res_gdf = gps_match_res_gdf
         return self.gps_match_res_gdf
 
     @function_time_cost
     def acquire_omitted_match_item(self, gps_link_state_df: pd.DataFrame = None) -> pd.DataFrame:
         """
         推算补全不完整的路径之间的path以及GPS点
         :param gps_link_state_df: 初步的匹配结果, 可能存在断掉的路径
@@ -657,15 +797,18 @@
         del omitted_gps_state_item
 
         omitted_gps_state_df[gps_field.TIME_FIELD] = omitted_gps_points_time
         omitted_gps_state_df[net_field.GEOMETRY_FIELD] = [Point(loc) for loc in omitted_gps_points]
 
         return omitted_gps_state_df
 
-    def acquire_visualization_res(self, use_gps_source: bool = False) -> tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
+    def acquire_visualization_res(self, use_gps_source: bool = False,
+                                  link_width: float = 1.5, node_radius: float = 1.5,
+                                  match_link_width: float = 5.0, gps_radius: float = 3.0) -> tuple[
+                                        gpd.GeoDataFrame, gpd.GeoDataFrame, gpd.GeoDataFrame]:
         """获取可视化结果"""
         if self.__plot_mix_gdf is None:
             single_link_gdf = self.net.get_link_data()
             node_gdf = self.net.get_node_data()
             net_crs = self.net.crs
             plain_crs = self.net.planar_crs
             is_geo_crs = self.net.is_geo_crs()
@@ -686,46 +829,47 @@
                                              gps_field.LAT_FIELD, gps_field.TIME_FIELD,
                                              gps_field.GEOMETRY_FIELD]].copy()
 
             # GPS点转化为circle polygon
             plot_gps_gdf.drop(columns=[gps_field.LNG_FIELD, gps_field.LAT_FIELD], axis=1, inplace=True)
             if plot_gps_gdf.crs != plain_crs:
                 plot_gps_gdf = plot_gps_gdf.to_crs(plain_crs)
-            plot_gps_gdf[net_field.GEOMETRY_FIELD] = plot_gps_gdf[net_field.GEOMETRY_FIELD].apply(lambda p: p.buffer(3.0))
+            plot_gps_gdf[net_field.GEOMETRY_FIELD] = \
+                plot_gps_gdf[net_field.GEOMETRY_FIELD].apply(lambda p: p.buffer(gps_radius))
             plot_gps_gdf[gps_field.TYPE_FIELD] = 'gps'
 
             # 匹配路段GDF
             plot_match_link_gdf = self.gps_match_res_gdf.copy()
             plot_match_link_gdf.drop(columns=[markov_field.PRJ_GEO], axis=1, inplace=True)
             plot_match_link_gdf[gps_field.TYPE_FIELD] = 'link'
             plot_match_link_gdf[net_field.GEOMETRY_FIELD] = plot_match_link_gdf[net_field.LINK_ID_FIELD].apply(
                 lambda x: double_link_geo[x])
             plot_match_link_gdf.crs = net_crs
             plot_match_link_gdf.drop_duplicates(subset=net_field.LINK_ID_FIELD, keep='first', inplace=True)
             plot_match_link_gdf.reset_index(drop=True, inplace=True)
             if is_geo_crs:
                 plot_match_link_gdf = plot_match_link_gdf.to_crs(plain_crs)
             plot_match_link_gdf[net_field.GEOMETRY_FIELD] = plot_match_link_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda l: l.buffer(5.0))
+                lambda l: l.buffer(match_link_width))
             plot_match_link_gdf.drop(columns=[gps_field.LNG_FIELD, gps_field.LAT_FIELD], axis=1, inplace=True)
 
             plot_gps_gdf = plot_gps_gdf.to_crs(self.net.geo_crs)
             plot_match_link_gdf = plot_match_link_gdf.to_crs(self.net.geo_crs)
             gps_link_gdf = pd.concat([plot_gps_gdf, plot_match_link_gdf])
             gps_link_gdf.reset_index(inplace=True, drop=True)
 
             # 路网底图
             origin_link_gdf = single_link_gdf.drop_duplicates(subset=[net_field.LINK_ID_FIELD], keep='first').copy()
             if is_geo_crs:
                 origin_link_gdf = origin_link_gdf.to_crs(plain_crs)
                 node_gdf = node_gdf.to_crs(plain_crs)
             origin_link_gdf[net_field.GEOMETRY_FIELD] = origin_link_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda x: x.buffer(1.5))
+                lambda x: x.buffer(link_width))
             node_gdf[net_field.GEOMETRY_FIELD] = node_gdf[net_field.GEOMETRY_FIELD].apply(
-                lambda x: x.buffer(1.5))
+                lambda x: x.buffer(node_radius))
 
             origin_link_gdf = origin_link_gdf.to_crs(self.net.geo_crs)
             node_gdf = node_gdf.to_crs(self.net.geo_crs)
 
             self.__plot_mix_gdf, self.__base_link_gdf, self.__base_node_gdf = gps_link_gdf, origin_link_gdf, node_gdf
             return gps_link_gdf, origin_link_gdf, node_gdf
 
@@ -737,54 +881,48 @@
         out_fldr = r'./' if out_fldr is None else out_fldr
         if self.gps_match_res_gdf is None:
             self.acquire_res()
 
         # gps
         gps_layer = self.gps_match_res_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.SUB_SEQ_FIELD,
                                             gps_field.GEOMETRY_FIELD]].copy()
-        gps_layer = gps_layer.to_crs(self.net.geo_crs)
 
         # prj_point
         prj_p_layer = self.gps_match_res_gdf[
             [gps_field.POINT_SEQ_FIELD, gps_field.SUB_SEQ_FIELD, net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
              net_field.TO_NODE_FIELD, markov_field.DIS_TO_NEXT, markov_field.PRJ_GEO, gps_field.GEOMETRY_FIELD]].copy()
         prj_p_layer.dropna(subset=[markov_field.PRJ_GEO], inplace=True)
-        prj_p_layer.set_geometry(markov_field.PRJ_GEO, inplace=True, crs=self.gps_points.plane_crs)
-        prj_p_layer = prj_p_layer.to_crs(self.gps_points.geo_crs)
+        prj_p_layer.set_geometry(markov_field.PRJ_GEO, inplace=True, crs=self.gps_points.geo_crs)
 
         prj_p_layer['__geo'] = prj_p_layer.apply(
             lambda item: LineString((item[gps_field.GEOMETRY_FIELD], item[markov_field.PRJ_GEO])), axis=1)
 
         # prj_line
         prj_l_layer = prj_p_layer[['__geo']].copy()
         prj_l_layer.rename(columns={'__geo': gps_field.GEOMETRY_FIELD}, inplace=True)
         prj_l_layer = gpd.GeoDataFrame(prj_l_layer, geometry=gps_field.GEOMETRY_FIELD, crs=prj_p_layer.crs)
 
         prj_p_layer.set_geometry(markov_field.PRJ_GEO, inplace=True, crs=prj_p_layer.crs)
 
         prj_p_layer.drop(columns=['__geo', gps_field.GEOMETRY_FIELD], axis=1, inplace=True)
 
-        prj_l_layer = prj_l_layer.to_crs(self.net.geo_crs)
-        prj_p_layer = prj_p_layer.to_crs(self.net.geo_crs)
-
         # match_link
         match_link_gdf = self.gps_match_res_gdf[[gps_field.POINT_SEQ_FIELD, gps_field.SUB_SEQ_FIELD,
                                                 net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                                 net_field.TO_NODE_FIELD]].copy()
         match_link_gdf.drop_duplicates(subset=[net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                                net_field.TO_NODE_FIELD], keep='first', inplace=True)
         match_link_gdf.reset_index(inplace=True, drop=True)
         match_link_gdf = pd.merge(match_link_gdf,
                                   self.net.get_link_data()[[net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                                             net_field.TO_NODE_FIELD, net_field.GEOMETRY_FIELD]],
                                   on=[net_field.LINK_ID_FIELD, net_field.FROM_NODE_FIELD,
                                       net_field.TO_NODE_FIELD],
                                   how='left')
-        match_link_gdf = gpd.GeoDataFrame(match_link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=self.net.crs)
-
+        match_link_gdf = gpd.GeoDataFrame(match_link_gdf, geometry=net_field.GEOMETRY_FIELD, crs=self.net.planar_crs)
         match_link_gdf = match_link_gdf.to_crs(self.net.geo_crs)
 
         for gdf, name in zip([gps_layer, prj_p_layer, prj_l_layer, match_link_gdf],
                              ['gps', 'prj_p', 'prj_l', 'match_link']):
             gdf.to_file(os.path.join(out_fldr, '-'.join([flag_name, name]) + '.geojson'), driver='GeoJSON')
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/GlobalVal.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/GlobalVal.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/NetGen.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/NetGen.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 # @Time    : 2023/7/31 0031 9:52
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 
 """生产路网的相关方法"""
 
-
-
 import time
 import os.path
 import pandas as pd
 import geopandas as gpd
 from ..map.Net import Net
 from .RoadNet.conn import Conn
 from .GlobalVal import NetField
 from .format_od import FormatOD
 from .RoadNet import net_reverse
+from ..gps.GpsTrip import GpsTrip
 from .RoadNet.increment import increment
 from .RoadNet.save_file import save_file
 from .Request.request_path import CarPath
 from .RoadNet.optimize_net import optimize
 from ..WrapsFunc import function_time_cost
 from .Parse.gd_car_path import ParseGdPath
+from .RoadNet.Split.SplitPath import split_path
 from .PublicTools.GeoProcess import generate_region
 from .RoadNet.Split.SplitPath import split_path_main
-from .RoadNet.Tools.process import merge_double_link
 from ..tools.geo_process import clean_link_geo, remapping_id
+from .RoadNet.Tools.process import merge_double_link, create_single_link
 from .RoadNet.SaveStreets.streets import generate_node_from_link, modify_minimum
 
 
 net_field = NetField()
 
 
 class Reverse(object):
@@ -49,19 +49,20 @@
                  cut_slice: bool = False, slice_num: int = 5, generate_rod: bool = False, min_rod_length: float = 5.0,
                  restrict_region_gdf: gpd.GeoDataFrame = None, save_split_link: bool = False,
                  modify_minimum_buffer: float = 0.8, save_streets_before_modify_minimum: bool = False,
                  save_streets_after_modify_minimum: bool = False, save_tpr_link: bool = False,
                  limit_col_name: str = 'road_name', ignore_dir: bool = False,
                  allow_ring: bool = False, restrict_angle: bool = True, restrict_length: bool = True,
                  accu_l_threshold: float = 200.0, angle_threshold: float = 35.0, min_length: float = 50.0,
+                 multi_core_merge: bool = False, merge_core_num: int = 2,
                  save_preliminary: bool = False, save_done_topo: bool = False,
                  is_process_dup_link: bool = True, process_dup_link_buffer: float = 0.8,
                  dup_link_buffer_ratio: float = 60.0, net_out_fldr: str = None, net_file_type: str = 'shp',
                  is_modify_conn: bool = True, conn_buffer: float = 0.8, conn_period: str = 'final',
-                 is_multi_core: bool = False, used_core_num: int = 2):
+                 multi_core_parse: bool = False, parse_core_num: int = 2):
         """
         :param flag_name: 标志字符(项目名称)
         :param plain_prj: 平面投影坐标系
         :param net_out_fldr: 输出路网的存储目录
         :return:
         """
         # overall
@@ -90,14 +91,16 @@
         self.restrict_angle = restrict_angle
         self.restrict_length = restrict_length
         self.accu_l_threshold = accu_l_threshold
         self.angle_threshold = angle_threshold
         self.min_length = min_length
         self.save_preliminary = save_preliminary
         self.save_done_topo = save_done_topo
+        self.multi_core_merge = multi_core_merge
+        self.merge_core_num = merge_core_num
 
         # process dup
         self.is_process_dup_link = is_process_dup_link
         self.process_dup_link_buffer = process_dup_link_buffer
         self.dup_link_buffer_ratio = dup_link_buffer_ratio
 
         # conn
@@ -107,16 +110,16 @@
         self.conn_period = conn_period
 
         # attrs
         self.__od_df = pd.DataFrame()
         self.__region_gdf = gpd.GeoDataFrame()
 
         # if uses multi core
-        self.is_multi_core = is_multi_core
-        self.used_core_num = used_core_num
+        self.multi_core_parse = multi_core_parse
+        self.parse_core_num = parse_core_num
 
     def generate_net_from_request(self, key_list: list[str] = None, binary_path_fldr: str = None,
                                   od_file_path: str = None, od_df: pd.DataFrame = None,
                                   region_gdf: gpd.GeoDataFrame = None, od_type='rand_od', boundary_buffer: float = 2000,
                                   cache_times: int = 300, ignore_hh: bool = True, remove_his: bool = True,
                                   log_fldr: str = None, save_log_file: bool = False,
                                   min_lng: float = None, min_lat: float = None, w: float = 2000, h: float = 2000,
@@ -152,16 +155,16 @@
                           is_slice=self.cut_slice,
                           slice_num=self.slice_num,
                           restrict_region_gdf=self.restrict_region_gdf,
                           attr_name_list=attr_name_list,
                           ignore_head_tail=self.ignore_head_tail,
                           check=False, generate_rod=self.generate_rod,
                           min_rod_length=self.min_rod_length,
-                          is_multi_core=self.is_multi_core,
-                          used_core_num=self.used_core_num)
+                          is_multi_core=self.multi_core_parse,
+                          used_core_num=self.parse_core_num)
 
         split_path_gdf = pgd.parse_path_main_multi()
 
         self.__generate_net_from_split_path(split_path_gdf=split_path_gdf)
 
     def generate_net_from_path_gdf(self, path_gdf: gpd.GeoDataFrame = None,
                                    restrict_region_gdf: gpd.GeoDataFrame = None,
@@ -224,15 +227,16 @@
                                                      restrict_length=self.restrict_length,
                                                      restrict_angle=self.restrict_angle,
                                                      save_preliminary=False,
                                                      out_fldr=self.net_out_fldr,
                                                      is_process_dup_link=False,
                                                      process_dup_link_buffer=self.process_dup_link_buffer,
                                                      min_length=self.min_length,
-                                                     dup_link_buffer_ratio=self.dup_link_buffer_ratio)
+                                                     dup_link_buffer_ratio=self.dup_link_buffer_ratio,
+                                                     multi_core=self.multi_core_merge, core_num=self.merge_core_num)
         if out_fldr is not None:
             save_file(data_item=link_gdf, out_fldr=out_fldr, file_type=self.net_file_type, file_name='opt_link')
             save_file(data_item=node_gdf, out_fldr=out_fldr, file_type=self.net_file_type, file_name='opt_node')
         return link_gdf, node_gdf, dup_info_dict
 
     def get_od_df(self) -> pd.DataFrame:
         return self.__od_df.copy()
@@ -294,15 +298,15 @@
                      od_num: int = 100, gap_n: int = 1000, min_od_length: float = 1200.0) -> tuple[bool, list[str]]:
         """构造OD -> 请求 -> 二进制存储"""
         assert binary_path_fldr is not None
 
         assert od_type in ['rand_od', 'region_od', 'diy_od', 'gps_based']
         fmod = FormatOD(plain_crs=self.plain_prj)
         if isinstance(region_gdf, gpd.GeoDataFrame) and not region_gdf.empty:
-            assert region_gdf.crs == 'EPSG:4326', '面域文件必须是EPSG:4326"'
+            assert region_gdf.crs.srs == 'EPSG:4326', '面域文件必须是EPSG:4326"'
         if od_type == 'rand_od':
             if region_gdf is None or region_gdf.empty:
                 region_gdf = generate_region(min_lng=min_lng, min_lat=min_lat, w=w, h=h, plain_crs=self.plain_prj)
 
             od_df = fmod.format_region_rnd_od(region_gdf=region_gdf, flag_name=self.flag_name, od_num=od_num,
                                               gap_n=gap_n, length_limit=min_od_length,
                                               boundary_buffer=boundary_buffer)
@@ -353,35 +357,37 @@
                                  save_streets_after_modify_minimum=self.save_streets_after_modify_minimum,
                                  is_process_dup_link=self.is_process_dup_link,
                                  process_dup_link_buffer=self.process_dup_link_buffer,
                                  dup_link_buffer_ratio=self.dup_link_buffer_ratio,
                                  net_file_type=self.net_file_type,
                                  modify_conn=self.is_modify_conn,
                                  conn_buffer=self.conn_buffer,
-                                 conn_period=self.conn_period)
+                                 conn_period=self.conn_period,
+                                 multi_core_merge=self.multi_core_merge,
+                                 core_num=self.merge_core_num)
 
     def modify_conn(self, link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None,
                     book_mark_name: str = 'test', link_name_field: str = 'road_name', generate_mark: bool = False) -> \
             tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
         """
 
         :param link_gdf:
         :param node_gdf:
         :param book_mark_name:
         :param link_name_field:
         :param generate_mark
         :return:
         """
-        geo_crs = link_gdf.crs
+        geo_crs = link_gdf.crs.srs
         assert geo_crs == 'EPSG:4326'
         link_gdf, node_gdf = self.fix_minimum_gap(node_gdf=node_gdf, link_gdf=link_gdf)
         net = Net(link_gdf=link_gdf, node_gdf=node_gdf, create_single=False)
         conn = Conn(net=net, check_buffer=self.conn_buffer)
         conn.execute(out_fldr=self.net_out_fldr, file_name=book_mark_name, generate_mark=generate_mark)
-        net.export_net(export_crs=link_gdf.crs, out_fldr=self.net_out_fldr, file_type=self.net_file_type,
+        net.export_net(export_crs=link_gdf.crs.srs, out_fldr=self.net_out_fldr, file_type=self.net_file_type,
                        flag_name='modifiedConn')
         net.to_geo_prj()
         link_gdf, node_gdf = net.get_bilateral_link_data(), net.get_node_data()
         link_gdf.reset_index(inplace=True, drop=True)
         node_gdf.reset_index(inplace=True, drop=True)
         return link_gdf, node_gdf
 
@@ -389,16 +395,17 @@
             tuple[gpd.GeoDataFrame, gpd.GeoDataFrame]:
         link_gdf, node_gdf, _ = modify_minimum(plain_prj=self.plain_prj, link_gdf=link_gdf, node_gdf=node_gdf,
                                                buffer=self.modify_minimum_buffer,
                                                ignore_merge_rule=True)
         return link_gdf, node_gdf
 
     @staticmethod
-    def clean_link_geo(gdf: gpd.GeoDataFrame = None, plain_crs: str = 'EPSG:32650') -> gpd.GeoDataFrame:
-        return clean_link_geo(gdf=gdf, plain_crs=plain_crs)
+    def clean_link_geo(gdf: gpd.GeoDataFrame = None, plain_crs: str = 'EPSG:32650',
+                       l_threshold: float = 0.5) -> gpd.GeoDataFrame:
+        return clean_link_geo(gdf=gdf, plain_crs=plain_crs, l_threshold=l_threshold)
 
     @staticmethod
     def remapping_link_node_id(link_gdf: gpd.GeoDataFrame or pd.DataFrame, node_gdf: gpd.GeoDataFrame or pd.DataFrame):
         """
         :param link_gdf:
         :param node_gdf:
         :return:
@@ -423,7 +430,49 @@
         # 执行划分路网
         # divide_l: 所有长度大于divide_l的路段都将按照divide_l进行划分
         # min_l: 划分后如果剩下的路段长度小于min_l, 那么此次划分将不被允许
         # is_init_link: 划分后是否重新初始化路网对象
         # method: alpha 或者 beta, 前一种方法可保留与划分前的link的映射关系(_parent_link字段)
         my_net.divide_links(divide_l=divide_l, min_l=min_l, is_init_link=False, method='alpha')
         return my_net.get_bilateral_link_data().reset_index(drop=True), my_net.get_node_data().reset_index(drop=True)
+
+    def redivide_link_node(self, link_gdf: gpd.GeoDataFrame = None):
+        """
+        对link进行线层和点层的重新划分
+        :param link_gdf: gpd.GeoDataFrame, 要求至少有geometry字段
+        """
+        link_gdf = link_gdf.to_crs('EPSG:4326')
+
+        if net_field.DIRECTION_FIELD not in link_gdf.columns:
+            print(rf'link层数据缺少dir字段, 自动填充为0')
+            link_gdf[net_field.DIRECTION_FIELD] = 0
+        link_gdf[net_field.DIRECTION_FIELD] = link_gdf[net_field.DIRECTION_FIELD].astype(int)
+        try:
+            del link_gdf[net_field.FROM_NODE_FIELD]
+            del link_gdf[net_field.TO_NODE_FIELD]
+            del link_gdf[net_field.LINK_ID_FIELD]
+            del link_gdf[net_field.LENGTH_FIELD]
+        except Exception as e:
+            print(repr(e))
+        assert set(link_gdf[net_field.DIRECTION_FIELD]).issubset({0, 1}), 'dir字段中有异常值, 只允许0,1出现'
+
+        # 创建single_link
+        single_link_gdf = create_single_link(link_gdf=link_gdf)
+        if self.limit_col_name not in single_link_gdf.columns:
+            single_link_gdf[self.limit_col_name] = 'XX路'
+        single_link_gdf = split_path(path_gdf=single_link_gdf)
+        single_link_gdf.drop(columns=['ft_loc'], axis=1, inplace=True)
+        del link_gdf
+        self.__generate_net_from_split_path(split_path_gdf=single_link_gdf)
+
+    @staticmethod
+    def generate_od_by_gps(gps_df: pd.DataFrame = None, time_format: str = '%Y-%m-%d %H:%M:%S', time_unit: str = 's',
+                           plain_crs: str = 'EPSG:32650', group_gap_threshold: float = 360.0, n: int = 5,
+                           min_distance_threshold: float = 10.0, way_points_num: int = 5,
+                           dwell_accu_time: float = 60.0) -> tuple[pd.DataFrame, gpd.GeoDataFrame]:
+        gtp = GpsTrip(gps_df=gps_df, time_unit=time_unit, time_format=time_format, plain_crs=plain_crs,
+                      group_gap_threshold=group_gap_threshold, n=n, min_distance_threshold=min_distance_threshold,
+                      way_points_num=way_points_num, dwell_accu_time=dwell_accu_time)
+        gtp.add_main_group()
+        od_df, od_line = gtp.generate_od()
+        return od_df, od_line
+
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/Parse/gd_car_path.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/Parse/gd_car_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,16 @@
                                                  cut_slice=self.is_slice, drop_ft_loc=False)
                 all_split_link_gdf = pd.concat([all_split_link_gdf, split_path_gdf])
                 all_split_link_gdf.reset_index(inplace=True, drop=True)
                 all_split_link_gdf.drop_duplicates(subset=['ft_loc'], keep='first', inplace=True)
             except:
                 print(rf'##########   Skip File {file}')
         all_split_link_gdf.reset_index(inplace=True, drop=True)
+        if all_split_link_gdf.empty:
+            return gpd.GeoDataFrame()
         all_split_link_gdf = gpd.GeoDataFrame(all_split_link_gdf, geometry='geometry', crs='EPSG:4326')
         if drop_ft:
             all_split_link_gdf.drop(columns=['ft_loc'], axis=1, inplace=True)
         return all_split_link_gdf
 
     def parse_path_main(self, out_type: str = 'dict', pickle_file_name_list: list[str] = None):
         """
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/GeoProcess.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GeoProcess.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/GraphAna.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/GraphAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/IndexAna.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/IndexAna.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/PublicTools/od.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/PublicTools/od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/Request/api/WebApi.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/Request/api/WebApi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/Request/request_path.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/Request/request_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/bd_ts.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/bd_ts.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/Request/usage/gd_car_path.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/Request/usage/gd_car_path.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/DupProcess/DupLinks.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/get_merged_link_seq.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_links.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Merge/merge_short.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,46 +78,36 @@
 #                 return merged_df
 #         else:
 #             merged_df['dir_list'] = merged_df['link_seq'].apply(lambda x: [0] * len(x))
 #             return merged_df
 
 
 # 主模块, 找出2度路段组
-def get_two_degrees_node_seq(ud_graph=None, allow_ring=False, d_graph=None):
+def get_two_degrees_node_seq(ud_graph=None, allow_ring=False, sub_graph_node_group=None, two_degrees_sub_graph=None):
     """
     找出2度节点组
     :param ud_graph: nx.net, 无向图
-    :param d_graph: nx.net, 有向图
     :param allow_ring: bool, 是否允许出现环
+    :param sub_graph_node_group:
+    :param two_degrees_sub_graph
     :return:
 
       group              link_seq(sorted...)
         1     [(2, 10), (10, 99), (8, 99)]
         2     [(13, 14), (14, 15), (15, 16), (16, 17)]
         3     [(1, 7), (7, 9), (3, 9), (3, 4), (4, 5), (5, 1)]
     """
-    # 找出度为2的节点id
-    degree_dict = dict(nx.degree(ud_graph))  # 无向图的度
-    d_degree_dict = dict(d_graph.degree)  # 有向图的度
     # 用于存储所有的链组
     all_seq_list = []
 
     # 用于存储所有的环组
     all_cycle_list = []
 
-    # 找出2度节点
-    # 无向图中度为2的节点,(且在有向图中的入度和出度之和为2或者4)
-    two_degree_node_list = [node for node in list(degree_dict.keys()) if
-                            (degree_dict[node] == 2) and d_degree_dict[node] in [2, 4]]
-
-    # 使用度为2的节点建立子图
-    two_degrees_sub_graph = nx.subgraph(ud_graph, two_degree_node_list)
-
     # 度为2的节点组成子图中也包含很多不连通的子图, all_seq_list: [[12, 23, 34], [1, 234, 2], ...]
-    for sub_graph_node in nx.connected_components(two_degrees_sub_graph):
+    for sub_graph_node in sub_graph_node_group:
         seq_list = []
 
         # 如果大于等于两个节点
         if len(sub_graph_node) >= 2:
             sub_graph = nx.subgraph(two_degrees_sub_graph, list(sub_graph_node))
 
             # 先找度节点
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links.py` & `gotrackit-0.2.0/src/gotrackit/tools/geo_process.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,275 +1,341 @@
 # -- coding: utf-8 --
 # @Time    : 2023/7/31 0031 9:52
 # @Author  : TangKai
 # @Team    : ZheChengData
 
 
-"""路网拓扑优化"""
-import time
-
+import numpy as np
 import pandas as pd
-import networkx as nx
 import geopandas as gpd
-from itertools import chain
-from ...GlobalVal import NetField
-from shapely.ops import linemerge
-from geopy.distance import distance
-from shapely.geometry import Point, LineString, MultiLineString
-from .get_merged_link_seq import get_merged_link_seq
-from .limit.same_head_tail_limit import same_ht_limit
-from .limit.same_head_tail_limit import get_head_tail_root
+from ..GlobalVal import NetField
+from .coord_trans import LngLatTransfer
+from shapely.geometry import LineString, Point
+from shapely.geometry import Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon, LinearRing
+from ..WrapsFunc import function_time_cost
 
 net_field = NetField()
-
-length_field = net_field.LENGTH_FIELD
+geometry_field = net_field.GEOMETRY_FIELD
 node_id_field = net_field.NODE_ID_FIELD
 link_id_field = net_field.LINK_ID_FIELD
-geometry_field = net_field.GEOMETRY_FIELD
-to_node_id_field = net_field.TO_NODE_FIELD
-direction_field = net_field.DIRECTION_FIELD
-from_node_id_field = net_field.FROM_NODE_FIELD
-required_field_list = [link_id_field, length_field, direction_field,
-                       from_node_id_field, to_node_id_field, geometry_field]
-
-
-def merge_two_degrees_node(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None,
-                           ignore_dir: bool = False, limit_col_name: str = None,
-                           allow_ring: bool = False, plain_prj: str = 'EPSG:32650', accu_l_threshold: float = 200.0,
-                           angle_threshold: float = 15.0,
-                           restrict_length: bool = True, restrict_angle: bool = True, min_length: float = 50.0) \
-        -> (gpd.GeoDataFrame, gpd.GeoDataFrame):
-    """
-    按照限制规则合并2度节点
-    :param link_gdf: 路网线层
-    :param node_gdf: 路网点层
-    :param ignore_dir: 是否忽略方向进行路段合并
-    :param limit_col_name: 限制字段名称
-    :param allow_ring: 是否允许合并后出现环
-    :param plain_prj: 平面投影坐标系
-    :param accu_l_threshold: 合并后的路段最长不能超过多少m
-    :param angle_threshold: 当路段转角超过多少度则划分节点
-    :param restrict_length: 是否启用路段长度限制
-    :param restrict_angle: 是否启用路段转交限制
-    :param min_length: 路段最短不能短于多少米
+from_node_field = net_field.FROM_NODE_FIELD
+to_node_field = net_field.TO_NODE_FIELD
+
+
+def n_equal_points(n, from_loc: tuple = None, to_loc=None,
+                   from_point: Point = None, to_point: Point = None, add_noise: bool = False,
+                   noise_frac: float = 0.3) -> list[list]:
+    """
+
+    :param n:
+    :param from_loc:
+    :param to_loc:
+    :param from_point:
+    :param to_point:
+    :param add_noise:
+    :param noise_frac:
     :return:
     """
-    # 1.找出可以合并的2度节点组
-    for col in [link_id_field, from_node_id_field, to_node_id_field, direction_field]:
-        link_gdf[col] = link_gdf[col].astype(int)
-    merged_link_df = get_merged_link_seq(link_gdf=link_gdf, judge_col_name=limit_col_name, ignore_dir=ignore_dir,
-                                         allow_ring=allow_ring,
-                                         node_gdf=node_gdf,
-                                         plain_prj=plain_prj, accu_l_threshold=accu_l_threshold,
-                                         angle_threshold=angle_threshold,
-                                         restrict_length=restrict_length, restrict_angle=restrict_angle,
-                                         min_length=min_length)
-    # 2.进行合并
-    if merged_link_df is not None:
-        new_link, new_node, info_dict = merge_links(link_gdf=link_gdf, node_gdf=node_gdf, merge_link_df=merged_link_df)
+    assert n > 1
+    if from_point is None or to_point is None:
+        line = LineString([from_loc, to_loc])
     else:
-        new_link, new_node, info_dict = link_gdf, node_gdf, dict()
+        line = LineString([from_point, to_point])
+    line_length = line.length
+
+    try:
+        dense_line = segmentize(line=line, n=n)
+    except AttributeError:
+        raise AttributeError(r'请升级geopandas到最新版本0.14.1')
+
+    equal_points = list(dense_line.coords)[1:-1]
+    if add_noise:
+        base_noise = 0.707106 * noise_frac * line_length / n
+        equal_points = [[loc[0] + np.random.normal(loc=0, scale=base_noise),
+                         loc[1] + np.random.normal(loc=0, scale=base_noise)] for loc in equal_points]
+    return equal_points
+
+
+def cut_line_in_nearest_point(line, point) -> list[LineString]:
+    """
+
+    :param line:
+    :param point:
+    :return:
+    """
+    xd = line.project(point)
+    return cut(line, xd)
 
-    origin_crs = new_link.crs
-    if origin_crs == plain_prj:
-        pass
+
+def cut(line: LineString = None, dis: float = None) -> list[LineString]:
+    """
+
+    :param line:
+    :param dis:
+    :return:
+    """
+    if dis <= 0.0 or dis >= line.length:
+        return [LineString(line)]
+    coords = list(line.coords)
+    for i, p in enumerate(coords):
+        xd = line.project(Point(p))
+        if xd == dis:
+            return [
+                LineString(coords[:i + 1]),
+                LineString(coords[i:])]
+        if xd > dis:
+            cp = line.interpolate(dis)
+            return [
+                LineString(coords[:i] + [(cp.x, cp.y)]),
+                LineString([(cp.x, cp.y)] + coords[i:])]
+
+
+def calc_link_angle(link_geo1=None, link_geo2=None) -> float:
+    """
+
+    :param link_geo1:
+    :param link_geo2:
+    :return:
+    """
+    coord_list_a = list(link_geo1.coords)
+    coord_list_b = list(link_geo2.coords)
+
+    vec_a = np.array(coord_list_a[-1]) - np.array(coord_list_a[0])
+    vec_b = np.array(coord_list_b[-1]) - np.array(coord_list_b[0])
+    cos_res = np.dot(vec_a, vec_b) / (np.linalg.norm(vec_a) * np.linalg.norm(vec_b))
+
+    if cos_res > 0:
+        if cos_res >= 1:
+            cos_res = 0.99999
+        return 180 * np.arccos(cos_res) / np.pi
+    elif cos_res < 0:
+        if cos_res < -1.0:
+            cos_res = -0.99999
+    return 180 * np.arccos(cos_res) / np.pi
+
+
+def segmentize(line: LineString = None, n: int = None) -> LineString:
+    """
+    将直线对象line进行n等分加密
+    :param line: 直线
+    :param n:
+    :return:
+    """
+    coord_list = list(line.coords)
+    s, e = coord_list[0], coord_list[-1]
+    try:
+        k = (e[1] - s[1]) / (e[0] - s[0])
+    except ZeroDivisionError:
+        gap = line.length / n
+        return LineString([s] + [(s[0], s[1] + (i + 1) * gap) for i in range(n - 1)] + [e])
+
+    b = e[1] - k * e[0]
+    gap_x = (e[0] - s[0]) / n
+    sample_x_list = [s[0] + (i + 1) * gap_x for i in range(n - 1)]
+    return LineString([s] + [(sample_x, k * sample_x + b) for sample_x in sample_x_list] + [e])
+
+
+def prj_inf(p: Point = None, line: LineString = None) -> tuple[Point, float, float, float, list[LineString], np.ndarray]:
+    """
+    # 返回 某point到line的(投影点坐标, 点到投影点的直线距离, 投影点到line拓扑起点的路径距离, line的长度, 投影点打断line后的geo list)
+    :param p:
+    :param line:
+    :return: (投影点坐标, 点到投影点的直线距离, 投影点到line拓扑起点的路径距离, line的长度, 投影点打断line后的geo list, 投影点的方向向量)
+    """
+
+    distance = line.project(p)
+
+    if distance <= 0.0:
+        line_cor = list(line.coords)
+        prj_p = Point(line_cor[0])
+        prj_vec = np.array(line_cor[1]) - np.array(line_cor[0])
+        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], prj_vec
+    elif distance >= line.length:
+        line_cor = list(line.coords)
+        prj_p = Point(line_cor[-1])
+        prj_vec = np.array(line_cor[-1]) - np.array(line_cor[-2])
+        return prj_p, prj_p.distance(p), distance, line.length, [LineString(line)], prj_vec
     else:
-        new_link = new_link.to_crs(plain_prj)
-        new_link[length_field] = new_link[geometry_field].apply(lambda x: x.length)
-        new_link = new_link.to_crs(origin_crs)
-
-    return new_link, new_node, info_dict
+        coords = list(line.coords)
+        for i, _p in enumerate(coords):
+            xd = line.project(Point(_p))
+            if xd == distance:
+                prj_p = Point(coords[i])
+                prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                return prj_p, prj_p.distance(p), distance, line.length, \
+                    [LineString(coords[:i + 1]), LineString(coords[i:])], prj_vec
+            if xd > distance:
+                cp = line.interpolate(distance)
+                prj_p = Point((cp.x, cp.y))
+                prj_vec = np.array(coords[i]) - np.array(coords[i - 1])
+                return prj_p, prj_p.distance(p), distance, line.length, [LineString(coords[:i] + [(cp.x, cp.y)]),
+                                                                         LineString(
+                                                                             [(cp.x, cp.y)] + coords[i:])], prj_vec
 
 
-# 逻辑子模块, 只记录合并信息, 并不修改传入的数据
-def merge_links(link_gdf=None, node_gdf=None, merge_link_df=None) -> (gpd.GeoDataFrame, gpd.GeoDataFrame, dict):
-    """传入可合并的路段组, 直接在线层数据, 点层数据上修改
-    :param link_gdf: gpd.GeoDataFrame, 线层数据
-    :param node_gdf: gpd.GeoDataFrame, 点层数据
-    :param merge_link_df: pd.oDataFrame, 合并路段信息
+def clean_link_geo(gdf: gpd.GeoDataFrame = None, plain_crs: str = 'EPSG:32650', l_threshold: float = 0.5) -> gpd.GeoDataFrame:
+    """
+    将geometry列中的Multi对象处理为single对象
+    :param gdf:
+    :param plain_crs
     :return:
+    """
+    assert geometry_field in gdf.columns
+    origin_crs = gdf.crs.srs
+    con = LngLatTransfer()
+
+    gdf[geometry_field] = gdf.apply(lambda row: con.obj_convert(geo_obj=row[geometry_field], con_type='None'), axis=1)
+    gdf = pd.DataFrame(gdf)
+    gdf[[geometry_field, 'is_multi']] = \
+        gdf.apply(lambda row:
+                  (list(row[geometry_field].geoms), 1)
+                  if isinstance(row[geometry_field], (MultiPolygon, MultiLineString, MultiPoint))
+                  else (row[geometry_field], 0), axis=1, result_type='expand')
+
+    is_multi_index = gdf['is_multi'] == 1
+    multi_gdf = gdf[is_multi_index].copy()
+    gdf.drop(index=gdf[is_multi_index].index, axis=0, inplace=True)
+
+    multi_gdf = multi_gdf.explode(column=[geometry_field], ignore_index=True)
+    multi_gdf.dropna(subset=[geometry_field], axis=0, inplace=True)
+
+    gdf = pd.concat([gdf, multi_gdf])
+    gdf.reset_index(inplace=True, drop=True)
+
+    gdf.drop(columns=['is_multi'], axis=1, inplace=True)
+    gdf = gpd.GeoDataFrame(gdf, geometry=geometry_field, crs=origin_crs)
+    gdf = gdf.to_crs(plain_crs)
+    gdf[geometry_field] = gdf[geometry_field].remove_repeated_points(l_threshold)
+    gdf = gdf.to_crs(origin_crs)
+    return gdf
 
-    ~~Input~~:
-    merge_link_df:
-       group              link_seq                                           dir_list         attr_list
-        1     [(2, 10), (10, 99), (8, 99)]                                   [1,1,1]      [XX路,XX路,XX路]
-        2     [(13, 14), (14, 15), (15, 16), (16, 17)]                       [0,0,0]      [XX路,XX路,XX路]
-        3     [(1, 7), (7, 9), (3, 9), (3, 4), (4, 5), (5, 99)]               [0,1,0]      [XX路,XX路,XX路]
-    """
-
-    # 直接修改传入的link_gdf
-    print(r'##########   Merge Road Sections')
-    node_gdf.set_index(node_id_field, inplace=True)
-    origin_crs = link_gdf.crs
-    link_gdf['sorted_ft'] = link_gdf[[from_node_id_field, to_node_id_field]].apply(lambda x: tuple(sorted(x)), axis=1)
-
-    origin_sorted_ft_list = link_gdf['sorted_ft'].to_list()
-
-    # 用于记录合并信息
-    merge_info_dict = dict()
-
-    # 计算head_node, tail_node, root_node
-
-    merge_link_df['head_tail_root_ring'] = merge_link_df['link_seq'].apply(lambda x: get_head_tail_root(x))
-
-    # 不允许组内合并后首尾节点一致
-    merge_link_df = same_ht_limit(origin_link_sorted_ft_list=origin_sorted_ft_list, merge_link_df=merge_link_df)
-
-    sum_del_node_list = []
-    sum_merge_link_list = []
-    sum_link_data_list = []
-
-    for row in merge_link_df.itertuples():
-        link_seq_list = getattr(row, 'link_seq')
-        head_tail_root_ring = getattr(row, 'head_tail_root_ring')
-        dir_list = getattr(row, 'dir_list')
-
-        ring = head_tail_root_ring[0]
-        root = head_tail_root_ring[1]
-        head = head_tail_root_ring[2]
-        tail = head_tail_root_ring[3]
-
-        # 选出要合并的线层索引
-        to_be_merge_link_gdf = link_gdf[link_gdf['sorted_ft'].isin(link_seq_list)].copy()
-
-        # 修正线型(保证相接的点的坐标一致)
-        to_be_merge_link_gdf['geometry'] = to_be_merge_link_gdf.apply(
-            lambda item: LineString([node_gdf.at[item[from_node_id_field], geometry_field]] +
-                                    list(item['geometry'].coords)[1:-1] +
-                                    [node_gdf.at[item[to_node_id_field], geometry_field]]), axis=1)
-        merge_link_index = list(to_be_merge_link_gdf.index)
-
-        if not ring:
-            # 不是环
-            if set(dir_list) == {0}:
-                new_dir = 0
-                # 任取一个首尾节点深度遍历
-                assume_from_node = head
-                assume_to_node = tail
-            else:
-                new_dir = 1
-                d_g = nx.DiGraph()
-
-                to_be_merge_link_gdf['_d_from_to_'] = \
-                    to_be_merge_link_gdf.apply(lambda x: [x[from_node_id_field], x[to_node_id_field]], axis=1)
-                d_edge_list = to_be_merge_link_gdf['_d_from_to_'].to_list()
-
-                d_g.add_edges_from(d_edge_list)
-                if nx.has_path(d_g, head, tail):
-                    assume_from_node = head
-                    assume_to_node = tail
-
-                else:
-                    assume_from_node = tail
-                    assume_to_node = head
-
-        else:
-            # 是环, 找到根结点
-            assume_from_node, assume_to_node = root, root
-            new_dir = dir_list[0]
-
-        # 获取待合并的路段的LineString
-        merge_line_list = to_be_merge_link_gdf[geometry_field].to_list()
-        merge_line = linemerge(merge_line_list)
-
-        # 获取此时假定的拓扑起点的坐标
-        assumed_from_point = node_gdf.at[assume_from_node, geometry_field]
-
-        # 获取实际的拓扑线段的起终点坐标
-        # 合并后有可能出现多段线
-        try:
-            merge_line_start_point = Point(merge_line.coords[0])
-            merge_line_end_point = Point(merge_line.coords[-1])
-
-        # 这个问题的出现是因为如果merge_line_list里面的线型不连续, 会组成一个MultiLineString
-        # 部分可以合并的链, 由于在其相接点上坐标有微小差异(小数点后8~9位不一样), 也会导致合并为MultiLineString
-        # 所以先修正
-        except NotImplementedError as e:
-            print(e)
-            # to_be_merge_link_gdf.to_csv(r'temp.csv', encoding='utf_8_sig', index=False)
-            # to_be_merge_link_gdf.drop(columns=['sorted_ft'], axis=1, inplace=True)
-            # to_be_merge_link_gdf.to_file(r'temp.shp')
-        else:
-            new_from_node, new_to_node = assume_from_node, assume_to_node
-
-            if assumed_from_point.distance(merge_line_start_point) >= assumed_from_point.distance(merge_line_end_point):
-                merge_line = LineString(list(merge_line.coords)[::-1])
-            else:
-                pass
-
-            # 记录删除结点的信息
-            if ring:
-                del_node_list = list(set(chain(*link_seq_list)) - {root})
-                sum_del_node_list.append(del_node_list)
-            else:
-                del_node_list = list(set(chain(*link_seq_list)) - {head, tail})
-                sum_del_node_list.append(del_node_list)
-
-            # 新增一条合并后的link
-            new_link_id = link_gdf.at[list(merge_link_index)[0], link_id_field]
-
-            # link表原有的属性
-            link_columns_list = list(link_gdf.columns)
-
-            # 未指定的属性置空
-            non_specified_field_list = list(set(link_columns_list) - set(required_field_list))
-            first_link_index = list(to_be_merge_link_gdf.index)[0]
-            non_specified_data_dict = {field: to_be_merge_link_gdf.loc[first_link_index, field] for field in non_specified_field_list}
-
-            length = get_length_from_linestring(linestring_obj=merge_line, crs=origin_crs)
-
-            data_dict = {link_id_field: new_link_id, direction_field: new_dir, length_field: length,
-                         from_node_id_field: new_from_node, to_node_id_field: new_to_node, geometry_field: merge_line}
-
-            data_dict.update(non_specified_data_dict)
-
-            sum_link_data_list.append(data_dict)
-            sum_merge_link_list.append(merge_link_index)
-
-        merge_info_dict[rf'Merge-{link_seq_list[0]}'] = list(merge_line.coords)[0]
-
-    node_gdf.reset_index(inplace=True, drop=False)
-    # 删除节点信息
-    sum_del_node_list = list(chain(*sum_del_node_list))
-    node_gdf.drop(index=node_gdf[node_gdf[node_id_field].isin(sum_del_node_list)].index, inplace=True)
-
-    # 删除被合并的Links
-    sum_merge_link_list = list(chain(*sum_merge_link_list))
-    link_gdf.drop(index=sum_merge_link_list, inplace=True)
-
-    # 添加合并后的link信息
-    new_link_dict = {field: [] for field in sum_link_data_list[0].keys()}
-
-    for data_dict in sum_link_data_list:
-        for key in data_dict.keys():
-            new_link_dict[key].append(data_dict[key])
-    new_link_df = pd.DataFrame(new_link_dict)
-    new_link_gdf = gpd.GeoDataFrame(new_link_df, geometry=geometry_field, crs=origin_crs)
-    link_gdf = pd.concat([link_gdf, new_link_gdf])
-    link_gdf.drop(columns=['sorted_ft'], axis=1, inplace=True)
-    link_gdf.reset_index(inplace=True, drop=True)
-    link_gdf.drop_duplicates(subset=[from_node_id_field, to_node_id_field], keep='first', inplace=True)
-    link_gdf.reset_index(inplace=True, drop=True)
-
-    node_gdf.reset_index(inplace=True, drop=True)
-    return link_gdf, node_gdf, merge_info_dict
-
-
-def get_length_from_linestring(linestring_obj=None, crs='EPSG:4326'):
-    """
-    在epsg:4326下计算LineString的长度, km
-    :param linestring_obj: LineString, 多段线对象
-    :param crs:
+
+def remapping_id(link_gdf: gpd.GeoDataFrame or pd.DataFrame = None,
+                 node_gdf: gpd.GeoDataFrame or pd.DataFrame = None) -> None:
+    """
+    change link and node inplace
+    :param link_gdf:
+    :param node_gdf:
     :return:
     """
-    if crs == 'EPSG:4326':
-        coord_list = list(linestring_obj.coords)
-        try:
-            length_list = [distance(tuple(coord_list[i][::-1]), tuple(coord_list[i + 1][::-1])).m for i in range(0, len(coord_list) - 1)]
-            return sum(length_list)
-        except ValueError as e:
-            # print(r'是平面坐标')
-            return linestring_obj.length
+    origin_node = set(node_gdf[node_id_field])
+    node_map = {origin_node: new_node for origin_node, new_node in
+                zip(origin_node, [i for i in range(1, len(origin_node) + 1)])}
+
+    node_gdf[node_id_field] = node_gdf[node_id_field].map(node_map)
+    link_gdf[link_id_field] = [i for i in range(1, len(link_gdf) + 1)]
+    link_gdf[[from_node_field, to_node_field]] = link_gdf.apply(lambda row: (node_map[row[from_node_field]],
+                                                                             node_map[row[to_node_field]]), axis=1,
+                                                                result_type='expand')
+
+
+def divide_line_by_l(line_geo: LineString = None, divide_l: float = 50.0, l_min: float = 0.5) -> tuple[
+    list[LineString], list[Point], int]:
+    """
+
+    :param line_geo:
+    :param divide_l:
+    :param l_min:
+    :return:
+    """
+    line_l = line_geo.length
+    n = int(line_l / divide_l)
+    remain_l = line_l % divide_l
+    is_remain = False
+    if remain_l > l_min:
+        is_remain = True
+    p_list = [line_geo.interpolate(i * divide_l) for i in range(1, n + 1)]
+    used_l = line_geo
+    divide_line_list = []
+    divide_point_list = []
+
+    for i, p in enumerate(p_list):
+        if i + 1 == len(p_list):
+            if not is_remain:
+                divide_line_list.append(used_l)
+                break
+        prj_p, _, dis, _, split_line_list, _ = prj_inf(p, used_l)
+        used_l = split_line_list[-1]
+        if i + 1 == len(p_list):
+            if is_remain:
+                divide_line_list.extend(split_line_list)
+                divide_point_list.append(p)
+                break
+        divide_line_list.append(split_line_list[0])
+        divide_point_list.append(p)
+
+    return divide_line_list, divide_point_list, len(divide_line_list)
+
+
+def vector_angle(v1: np.ndarray = None, v2: np.ndarray = None) -> float:
+    # 计算点积
+    dot_product = np.dot(v1, v2)
+    # 计算两个向量的模
+    norm_v1 = np.linalg.norm(v1)
+    norm_v2 = np.linalg.norm(v2)
+
+    # 避免除以零
+    if norm_v1 == 0 or norm_v2 == 0:
+        return 0
+    # 计算夹角
+    cos_angle = dot_product / (norm_v1 * norm_v2)
+
+    # 防止因浮点数计算问题导致cos_angle超出范围
+    cos_angle = min(max(cos_angle, -1), 1)
+
+    # 计算弧度表示
+    angle = np.arccos(cos_angle)
+    return min(180 * angle / np.pi, 179.9)
+
+
+def hmm_vector_angle(gps_diff_vec: np.ndarray = None, link_dir_vec: np.ndarray = None, omitted_l: float = 6.0) -> float:
+    """
+    计算GPS差分航向向量和候选路段切点方向向量的夹角
+    :param gps_diff_vec:
+    :param link_dir_vec:
+    :param omitted_l
+    :return:
+    """
+    # 在GPS点密集处, gps_diff_vec不准确, 往往gps_diff_vec的模会很小, 为了不干扰匹配, 返回0
+    if np.sqrt(gps_diff_vec[0] ** 2 + gps_diff_vec[1] ** 2) <= omitted_l:
+        return 0.0
+    else:
+        return vector_angle(v1=gps_diff_vec, v2=link_dir_vec)
+
+
+def angle_base_north(v: np.ndarray = None):
+    angle = vector_angle(v, np.array([0, 1]))
+    if v[0] <= 0:
+        return angle
     else:
-        return linestring_obj.length
+        return 360 - angle
+
+def judge_plain_crs(lng: float = None) -> str:
+    six_df = pd.DataFrame([(i * 6, 32631 + i) for i in range(0, 60)],
+                          columns=['start_lng', 'plain_crs'])
+    res = six_df[lng - six_df['start_lng'] >= 0]['plain_crs'].max()
+    return rf'EPSG:{res}'
+
+def judge_plain_crs_based_on_node(node_gdf: gpd.GeoDataFrame = None) -> str:
+    mean_x = np.array([geo.x for geo in node_gdf['geometry']]).mean()
+    return judge_plain_crs(lng=mean_x)
+
+
+if __name__ == '__main__':
+    pass
+    # import geopandas as gpd
+    # import matplotlib.pyplot as plt
+    #
+    # l = LineString([(0,0), (12, 90)])
+    # p = gpd.GeoDataFrame({'geometry': [Point(item) for item in l.coords]}, geometry='geometry')
+    # p.plot()
+    # plt.show()
+    #
+    # l_1 = segmentize(line=l, n=12)
+    # print(len(list(l_1.coords)))
+    # p1 = gpd.GeoDataFrame({'geometry': [Point(item) for item in l_1.coords]}, geometry='geometry')
+    # p1.plot()
+    # plt.show()
+
+
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Split/SplitPath.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/Tools/process.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/Tools/process.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     same crs as input
     输入的link的dir只能为0 or 1
     将那些连接在同一from_node和to_node上的合并为dir为0的
     :param link_gdf:
     :return:
     """
-    origin_crs = link_gdf.crs
+    origin_crs = link_gdf.crs.srs
 
     # 消除from_node = to_node的记录
     link_gdf.drop(index=link_gdf[link_gdf[from_node_id_field] == link_gdf[to_node_id_field]].index, inplace=True, axis=0)
 
     # 按照from_node, to_node去重
     link_gdf.drop_duplicates(subset=[from_node_id_field, to_node_id_field], keep='first', inplace=True)
     link_gdf.reset_index(inplace=True, drop=True)
@@ -85,15 +85,15 @@
     """
     # 找出dir为-1的记录
     link_neg = link_gdf[link_gdf[direction_field] == -1].copy()
 
     if link_neg.empty:
         return link_gdf
     else:
-        origin_crs = link_gdf.crs
+        origin_crs = link_gdf.crs.srs
 
         # 从原路网中删除dir为-1的记录
         link_gdf.drop(index=link_gdf[link_gdf[direction_field] == -1].index, axis=0, inplace=True)
 
         # 改变几何列的拓扑方向, 同时反转from_node和to_node字段
         if geometry_field in list(link_gdf.columns):
             link_neg[geometry_field] = link_neg[geometry_field].apply(lambda x: LineString(list(x.coords)[::-1]))
@@ -116,14 +116,32 @@
         link_gdf.reset_index(inplace=True, drop=True)
 
         link_gdf = gpd.GeoDataFrame(link_gdf, geometry=geometry_field, crs=origin_crs)
 
         return link_gdf
 
 
+def create_single_link(link_gdf: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
+    """
+    基于原来路网创建单向路网
+    :return:
+    """
+    link_gdf[net_field.DIRECTION_FIELD] = link_gdf[net_field.DIRECTION_FIELD].astype(int)
+    neg_link = link_gdf[link_gdf[net_field.DIRECTION_FIELD] == 0].copy()
+    if neg_link.empty:
+        return link_gdf
+    else:
+        neg_link[net_field.GEOMETRY_FIELD] = neg_link[net_field.GEOMETRY_FIELD].apply(
+            lambda line_geo: LineString(list(line_geo.coords)[::-1]))
+
+        single_link_gdf = pd.concat([link_gdf, neg_link])
+        single_link_gdf.reset_index(inplace=True, drop=True)
+        return single_link_gdf
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/conn.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/conn.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/increment.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/increment.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/net_reverse.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/net_reverse.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 
 def generate_net(path_gdf: gpd.GeoDataFrame = None, out_fldr: str = None,
                  save_split_link: bool = False, plain_prj: str = 'EPSG:4326', save_tpr_link: bool = False,
                  save_streets_before_modify_minimum: bool = True, restrict_angle: bool = True,
                  limit_col_name: str = 'road_name',
                  restrict_length: bool = True, accu_l_threshold: float = 150.0, angle_threshold: float = 15,
+                 multi_core_merge: bool = False, core_num: int = 3,
                  modify_minimum_buffer: float = 0.8, flag_name: str = None,
                  save_streets_after_modify_minimum: bool = True, save_preliminary: bool = False, save_done_topo:bool=False,
                  is_process_dup_link: bool = True, process_dup_link_buffer: float = 0.8, min_length: float = 50.0,
                  dup_link_buffer_ratio: float = 60.0, net_file_type: str = 'shp', modify_conn: bool = True,
                  conn_buffer: float = 0.8, conn_period: str = 'final'):
     """
     路网逆向主程序, 输入拆分好且去重的path_gdf(EPSG:4326), output: EPSG:4326
@@ -48,14 +49,16 @@
     :param save_split_link: 是否保存路段拆分后的link
     :param save_streets_before_modify_minimum: 是否保存做完拓扑关联但是还没做极小间隔点优化的路网
     :param save_streets_after_modify_minimum: 是否保存做完拓扑关联和极小间隔点优化的路网
     :param save_tpr_link: 是否保存拓扑关联、极小间隔点优化、双向路段合并后的link
     :param save_preliminary: 是否保存合并2度节点后的link
     :param accu_l_threshold: 合并后的link的长度的最大值(m)
     :param angle_threshold: 允许的最大转角(如果两个相邻的可合并link的转角超过这个角度则不允许合并)
+    :param multi_core_merge:
+    :param core_num:
     :param min_length: 允许的最小link长度
     :param limit_col_name: 属性限制字段
     :param restrict_length: 是否启用合并后的长度限制
     :param restrict_angle:  是否启用转角限制
     :param save_preliminary: 是否保存2度节点合并后的路网
     :param save_done_topo: 是否保存拓扑优化之后的路网
     :param is_process_dup_link: 是否处理重叠link
@@ -128,15 +131,16 @@
                                                                   accu_l_threshold=accu_l_threshold,
                                                                   angle_threshold=angle_threshold,
                                                                   process_dup_link_buffer=process_dup_link_buffer,
                                                                   is_process_dup_link=is_process_dup_link,
                                                                   allow_ring=False,
                                                                   modify_minimum_buffer=modify_minimum_buffer,
                                                                   min_length=min_length,
-                                                                  dup_link_buffer_ratio=dup_link_buffer_ratio)
+                                                                  dup_link_buffer_ratio=dup_link_buffer_ratio,
+                                                                  multi_core=multi_core_merge, core_num=core_num)
 
     if save_done_topo:
         save_file(data_item=final_link, out_fldr=out_fldr, file_name='DoneTopoLink', file_type=net_file_type)
         save_file(data_item=final_node, out_fldr=out_fldr, file_name='DoneTopoNode', file_type=net_file_type)
 
     if modify_conn:
         if conn_period == 'final':
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/optimize_net.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/optimize_net.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 """拓扑优化, 先合并2度节点, 再处理重复link"""
 
 import os
 import geopandas as gpd
 from ..book_mark import generate_book_mark
 from .DupProcess.DupLinks import process_dup_link
 from .Merge.merge_links import merge_two_degrees_node
+from .MultiCoreMerge.merge_links_multi import merge_links_multi
 
 
 def optimize(link_gdf: gpd.GeoDataFrame = None, node_gdf: gpd.GeoDataFrame = None, ignore_dir: bool = False,
              allow_ring: bool = False, limit_col_name: str = 'road_name', plain_prj: str = 'EPSG:32650',
              accu_l_threshold: float = 500.0, angle_threshold: float = 15.0, restrict_length: bool = True,
              restrict_angle: bool = True, save_preliminary: bool = True, out_fldr: str = None,
              is_process_dup_link: bool = True, process_dup_link_buffer: float = 0.75, min_length: float = 50.0,
-             dup_link_buffer_ratio: float = 60.0, modify_minimum_buffer: float = 0.8) -> \
+             dup_link_buffer_ratio: float = 60.0, modify_minimum_buffer: float = 0.8, multi_core: bool = False,
+             core_num: int = 3) -> \
         tuple[gpd.GeoDataFrame, gpd.GeoDataFrame, dict]:
     """crs input: EPSG:4326
     拓扑优化, 先合并2度节点, 再处理重复link
     :param link_gdf: 路网线层
     :param node_gdf: 路网点层
     :param ignore_dir: 是否忽略行车方向进行合并
     :param limit_col_name: 限制字段名称
@@ -34,46 +36,61 @@
     :param save_preliminary: 是否保存2度节点合并后的路网
     :param out_fldr: 输出文件目录
     :param is_process_dup_link: 是否处理重复link
     :param process_dup_link_buffer: 处理重复link时的buffer(m)
     :param min_length: 路段最小长度
     :param dup_link_buffer_ratio: LinkBuffer重叠率阈值, 推荐60
     :param modify_minimum_buffer
+    :param multi_core:
+    :param core_num
     :return:
     """
-
+    link_gdf.reset_index(inplace=True, drop=True)
+    node_gdf.reset_index(inplace=True, drop=True)
     # 1.按照规则合并2度节点
-    new_link, new_node, merge_info_dict = merge_two_degrees_node(link_gdf=link_gdf, limit_col_name=limit_col_name,
-                                                                 ignore_dir=ignore_dir,
-                                                                 allow_ring=allow_ring,
-                                                                 node_gdf=node_gdf,
-                                                                 plain_prj=plain_prj, accu_l_threshold=accu_l_threshold,
-                                                                 angle_threshold=angle_threshold,
-                                                                 restrict_length=restrict_length,
-                                                                 restrict_angle=restrict_angle,
-                                                                 min_length=min_length)
+    if multi_core:
+        new_link, new_node, merge_info_dict = merge_links_multi(link_gdf=link_gdf, limit_col_name=limit_col_name,
+                                                                ignore_dir=ignore_dir,
+                                                                allow_ring=allow_ring,
+                                                                node_gdf=node_gdf,
+                                                                plain_prj=plain_prj, accu_l_threshold=accu_l_threshold,
+                                                                angle_threshold=angle_threshold,
+                                                                restrict_length=restrict_length,
+                                                                restrict_angle=restrict_angle,
+                                                                min_length=min_length, core_num=core_num)
+    else:
+        new_link, new_node, merge_info_dict = merge_two_degrees_node(link_gdf=link_gdf, limit_col_name=limit_col_name,
+                                                                     ignore_dir=ignore_dir,
+                                                                     allow_ring=allow_ring,
+                                                                     node_gdf=node_gdf,
+                                                                     plain_prj=plain_prj,
+                                                                     accu_l_threshold=accu_l_threshold,
+                                                                     angle_threshold=angle_threshold,
+                                                                     restrict_length=restrict_length,
+                                                                     restrict_angle=restrict_angle,
+                                                                     min_length=min_length)
     if save_preliminary:
         generate_book_mark(input_fldr=out_fldr, name_loc_dict=merge_info_dict, prj_name=out_fldr.split('/')[-1])
         new_link.to_file(os.path.join(out_fldr, 'AfterTPMergeLink.shp'), encoding='gbk')
         new_node.to_file(os.path.join(out_fldr, 'AfterTPMergeNode.shp'), encoding='gbk')
 
     # 是否处理重复link
     if is_process_dup_link:
-        origin_crs = new_link.crs
-        if new_link.crs == plain_prj:
+        origin_crs = new_link.crs.srs
+        if new_link.crs.srs == plain_prj:
             pass
         else:
             new_link = new_link.to_crs(plain_prj)
             new_node = new_node.to_crs(plain_prj)
         print(r'##########   Remove Overlapping Road Segments')
         final_link, final_node, dup_info_dict = process_dup_link(link_gdf=new_link, node_gdf=new_node,
                                                                  buffer=process_dup_link_buffer,
                                                                  dup_link_buffer_ratio=dup_link_buffer_ratio,
                                                                  modify_minimum_buffer=modify_minimum_buffer)
-        if final_link.crs == origin_crs:
+        if final_link.crs.srs == origin_crs:
             pass
         else:
             final_link = final_link.to_crs(origin_crs)
             final_node = final_node.to_crs(origin_crs)
         return final_link, final_node, dup_info_dict
     else:
         return new_link, new_node, dict()
```

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/RoadNet/save_file.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/RoadNet/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/book_mark.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/book_mark.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/netreverse/format_od.py` & `gotrackit-0.2.0/src/gotrackit/netreverse/format_od.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/solver/Viterbi.py` & `gotrackit-0.2.0/src/gotrackit/solver/Viterbi.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/tools/coord_trans.py` & `gotrackit-0.2.0/src/gotrackit/tools/coord_trans.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/tools/save_file.py` & `gotrackit-0.2.0/src/gotrackit/tools/save_file.py`

 * *Files identical despite different names*

### Comparing `gotrackit-0.1.9/src/gotrackit/visualization.py` & `gotrackit-0.2.0/src/gotrackit/visualization.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,22 +31,25 @@
         else:
             self.__hmm_obj_list = [hmm_obj]
         self.use_gps_source = use_gps_source
 
     def collect_hmm(self, hmm_obj: HiddenMarkov = None):
         self.__hmm_obj_list.append(hmm_obj)
 
-    def visualization(self, zoom: int = 15, out_fldr: str = None, file_name: str = None) -> None:
+    def visualization(self, zoom: int = 15, out_fldr: str = None, file_name: str = None,
+                      link_width: float = 1.5, node_radius: float = 1.5,
+                      match_link_width: float = 5.0, gps_radius: float = 3.0) -> None:
         out_fldr = r'./' if out_fldr is None else out_fldr
         base_link_gdf = gpd.GeoDataFrame()
         base_node_gdf = gpd.GeoDataFrame()
         gps_link_gdf = gpd.GeoDataFrame()
         for hmm in self.__hmm_obj_list:
             _gps_link_gdf, _base_link_gdf, _base_node_gdf = hmm.acquire_visualization_res(
-                use_gps_source=self.use_gps_source)
+                use_gps_source=self.use_gps_source, link_width=link_width, gps_radius=gps_radius,
+                match_link_width=match_link_width, node_radius=node_radius)
             base_link_gdf = pd.concat([base_link_gdf, _base_link_gdf])
             base_node_gdf = pd.concat([base_node_gdf, _base_node_gdf])
             gps_link_gdf = pd.concat([gps_link_gdf, _gps_link_gdf])
 
         gps_link_gdf.reset_index(inplace=True, drop=True)
         base_link_gdf.drop_duplicates(subset=[net_field.LINK_ID_FIELD], keep='first', inplace=True)
         base_node_gdf.drop_duplicates(subset=[net_field.NODE_ID_FIELD], keep='first', inplace=True)
@@ -73,15 +76,16 @@
     :param node_gdf:
     :param zoom:
     :return:
     """
     # 生成KeplerGl对象
     if gps_field.HEADING_FIELD in mix_gdf.columns:
         mix_gdf.drop(columns=gps_field.HEADING_FIELD, axis=1, inplace=True)
-    data_item = {kepler_config.MIX_NAME: mix_gdf}
+    mix_gdf.sort_values(by='type', ascending=True, inplace=True)
+    data_item = dict()
 
     # 起点经纬度
     cen_geo = mix_gdf.at[0, net_field.GEOMETRY_FIELD].centroid
     cen_x, cen_y = cen_geo.x, cen_geo.y
     s_time, e_time = mix_gdf[gps_field.TIME_FIELD].min().timestamp(), mix_gdf[gps_field.TIME_FIELD].max().timestamp()
     mix_gdf[gps_field.TIME_FIELD] = mix_gdf[gps_field.TIME_FIELD].astype(str)
 
@@ -96,14 +100,15 @@
         user_config["config"]["visState"]["layers"].append(node_item)
         data_item[kepler_config.BASE_NODE_NAME] = node_gdf
 
     if link_gdf is not None:
         link_item = generate_polygon_layer(color=[65, 72, 88], layer_id=kepler_config.BASE_LINK_NAME)
         user_config["config"]["visState"]["layers"].append(link_item)
         data_item[kepler_config.BASE_LINK_NAME] = link_gdf
+    data_item[kepler_config.MIX_NAME] = mix_gdf
 
     user_map = KeplerGl(height=600, data=data_item)  # data以图层名为键，对应的矢量数据为值
     user_map.config = user_config
     user_map.save_to_html(file_name=os.path.join(out_fldr, file_name + '.html'))  # 导出到本地可编辑html文件
     # print(data_item)
     # print(user_map.config)
```

### Comparing `gotrackit-0.1.9/src/gotrackit.egg-info/PKG-INFO` & `gotrackit-0.2.0/src/gotrackit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotrackit
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python Package for Map Matching Algorithm Based on Hidden Markov Model
 Author-email: Kai Tang <794568794@qq.com>
 License: LICENCE
 Project-URL: Homepage, https://github.com/zdsjjtTLG/TrackIt
 Keywords: HMM,MapMatching,Net,Link,Node,Hidden Markov Model,Algorithm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,48 +16,74 @@
 Requires-Dist: shapely
 Requires-Dist: networkx
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: keplergl
 Requires-Dist: geopy
 
-# GoTrackIt
+
+![car_gps.png](docs/_static/images/gotrackit.png)
+
+
 [![Documentation Status](https://readthedocs.org/projects/gotrackit/badge/?version=latest)](https://gotrackit.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Version](https://img.shields.io/pypi/v/gotrackit)
 ![GitHub License](https://img.shields.io/github/license/zdsjjtTLG/Trackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/gotrackit)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/gotrackit)
 
 
-
 作者: 唐铠, 794568794@qq.com, tangkai@zhechengdata.com
 
 
-**2024.03.29即将更新: v0.1.9**
+**04.12已更新: v0.2.0**
 
-- 增加GPS增密功能
+更新命令：pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 
-- 引入GPS点差分方向向量来修正发射概率
+- 匹配过程增加多进程参数，拓扑优化过程增加多进程参数
 
-- 地图匹配接口升级，使用更加简单，暴露了更多的[可调参数](https://gotrackit.readthedocs.io/en/latest/%E5%A6%82%E4%BD%95%E4%BD%BF%E7%94%A8.html#id36)
+- GPS候选路段的选择：除开buffer选择外引入了top_k参数，用于指定buffer内最近的top_k个路段作为候选路段
 
-- 构建Net对象限制为：输入的link和node的数据必须为WGS-84 EPSG:4326地理坐标，平面投影坐标系不再需要手动指定，可自动进行6度带的确定
+- 增加GPS点停留点识别功能
 
-- 增加了路网处理函数：路段划分功能
+- 修正匹配结果中坐标不一致的BUG，现统一为EPSG:4326
 
-- 增加了路网处理函数：路段-link_id字段、from_node字段、to_node字段，节点-node_id字段重映射函数
+- 增加依据GPS数据提取带途径点OD的功能
 
-- 修复GPS生成接口中速度为负数的BUG
+- 增加了路网处理函数：路段、节点重塑
 
-- 修复Net初始化过程中由于节点ID过大导致内存溢出的问题
+- 修复了部分BUG
 
-- 新增路径缓存开关、ID缓存开关参数
 
 遇到BUG无法解决请进群交流，别忘了给项目一颗star哦~
 
+<div align="center">
+    <img src="docs/_static/images/l_f.gif" />
+</div>
+
+<div align="center">
+    <img src="docs/_static/images/m_h_f.gif" />
+</div>
+
+稀疏轨迹增密匹配：
+
+<div align="center">
+    <img src="docs/_static/images/dense_gps.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/taxi_xishu.gif" />
+</div>
+
+
+<div align="center">
+    <img src="docs/_static/images/xa_sample.gif" />
+</div>
+
+
 ![car_gps.png](docs/_static/images/wxq.jpg)
 
 
 
 ## 1. 简介
 本地图匹配包基于隐马尔可夫模型(HMM)实现了连续GPS点位的概率建模，利用这个包可以轻松对GPS数据进行地图匹配，本开源包的特点如下:
 
@@ -76,22 +102,23 @@
 
 
 
 ### 1.1. 如何安装gotrackit
 
 #### __所需前置依赖__
 
-- geopandas(0.14.1)
 - geopy(2.4.1)
 - gdal(3.4.3)
+- shapely(2.0.3)
+- fiona(1.9.5)
+- pyproj(3.6.1)
+- geopandas(0.14.3)
 - networkx(3.2.1)
-- shapely(2.0.2)
 - pandas(2.0.3)
 - numpy(1.26.2)
-- pyproj(3.6.1)
 - keplergl(0.3.2)
 
 括号中为作者使用版本(基于python3.11), 仅供参考
 
 geopandas为最新版本, 如果不是最新版本可能会报错(有个函数旧版本没有)
 
 #### __使用pip安装__
@@ -103,45 +130,37 @@
 ```
 
 更新：
 ``` shell
 pip install --upgrade  -i https://pypi.org/simple/ gotrackit
 ```
 
-### 1.2 用户手册
+### 1.2 用户手册与视频教程
+
+[用户手册](https://gotrackit.readthedocs.io/en/latest/)
+
+[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC)
+
+[一个python包搞定路网获取+地图匹配！](https://www.bilibili.com/video/BV1nC411z7Vg)
+
+[gotrackit地图匹配包参数详解与问题排查](https://www.bilibili.com/video/BV1qK421Y7hV)
 
-[用户手册](https://gotrackit.readthedocs.io/en/latest/)、
-[视频教程1](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)、
-[视频教程2](https://www.bilibili.com/video/BV1nC411z7Vg/?share_source=copy_web&vd_source=9b4518c7de4757ad3b99e18456efbaa6)
+[QGIS路网拓扑显示、底图加载、样式复用、map保存](https://www.bilibili.com/video/BV1Sq421F7QX)
 
 
 ## 2. 地图匹配问题
 
 ![car_gps.png](docs/_static/images/car_gps.png)
 
 ![where_car.png](docs/_static/images/whereIsCar.png)
 
 __如何依据GPS数据推算车辆的实际路径？__
 
-## 3. 地图匹配算法动画演示
-
-想了解算法过程的可以参考B站视频:
-[基于隐马尔可夫模型(HMM)的地图匹配算法动画版！学不会你来打我！](https://www.bilibili.com/video/BV1gQ4y1w7dC/?vd_source=7389960e7356c27a5d1849f7ee9ae6f2)
-
 ![main.png](docs/_static/images/single_p.png)
 
 ![main.png](docs/_static/images/transition.png)
 
 ![main.png](docs/_static/images/viterbi.png)
 
 ![main.png](docs/_static/images/trace.png)
 
 
-## 4. 匹配结果可视化
-
-中高频GPS匹配效果:
-
-![main.png](docs/_static/images/m_h_f.gif)
-
-低频GPS匹配效果:
-
-![main.png](docs/_static/images/l_f.gif)
```

### Comparing `gotrackit-0.1.9/src/gotrackit.egg-info/SOURCES.txt` & `gotrackit-0.2.0/src/gotrackit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -58,27 +58,28 @@
 src/gotrackit/netreverse/RoadNet/Merge/merge_short.py
 src/gotrackit/netreverse/RoadNet/Merge/limit/__init__.py
 src/gotrackit/netreverse/RoadNet/Merge/limit/attr_limit.py
 src/gotrackit/netreverse/RoadNet/Merge/limit/direction_limit.py
 src/gotrackit/netreverse/RoadNet/Merge/limit/same_head_tail_limit.py
 src/gotrackit/netreverse/RoadNet/Merge/limit/two_degrees_group.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/__init__.py
-src/gotrackit/netreverse/RoadNet/MultiCoreMerge/get_merged_link_seq.py
-src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links.py
-src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_short.py
+src/gotrackit/netreverse/RoadNet/MultiCoreMerge/merge_links_multi.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/__init__.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/attr_limit.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/direction_limit.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/same_head_tail_limit.py
 src/gotrackit/netreverse/RoadNet/MultiCoreMerge/limit/two_degrees_group.py
 src/gotrackit/netreverse/RoadNet/SaveStreets/__init__.py
 src/gotrackit/netreverse/RoadNet/SaveStreets/streets.py
 src/gotrackit/netreverse/RoadNet/Split/SplitPath.py
 src/gotrackit/netreverse/RoadNet/Split/__init__.py
 src/gotrackit/netreverse/RoadNet/Tools/__init__.py
 src/gotrackit/netreverse/RoadNet/Tools/process.py
+src/gotrackit/netxfer/SumoConvert.py
+src/gotrackit/netxfer/__init__.py
 src/gotrackit/solver/Viterbi.py
 src/gotrackit/solver/__init__.py
 src/gotrackit/tools/__init__.py
 src/gotrackit/tools/coord_trans.py
 src/gotrackit/tools/geo_process.py
+src/gotrackit/tools/group.py
 src/gotrackit/tools/save_file.py
```

