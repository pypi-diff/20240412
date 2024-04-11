# Comparing `tmp/edq-canvas-0.0.3.tar.gz` & `tmp/edq-canvas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edq-canvas-0.0.3.tar", last modified: Mon Mar 25 20:09:43 2024, max compression
+gzip compressed data, was "edq-canvas-0.0.4.tar", last modified: Thu Apr 11 22:18:16 2024, max compression
```

## Comparing `edq-canvas-0.0.3.tar` & `edq-canvas-0.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.406026 edq-canvas-0.0.3/
--rw-rw----   0 eriq      (1000) eriq      (1000)     1071 2024-02-03 22:26:13.000000 edq-canvas-0.0.3/LICENSE
--rw-r--r--   0 eriq      (1000) eriq      (1000)    10904 2024-03-25 20:09:43.406026 edq-canvas-0.0.3/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)     8991 2024-03-25 20:07:38.000000 edq-canvas-0.0.3/README.md
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.399359 edq-canvas-0.0.3/canvas/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-03 22:28:32.000000 edq-canvas-0.0.3/canvas/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      201 2024-03-07 16:13:16.000000 edq-canvas-0.0.3/canvas/__main__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.399359 edq-canvas-0.0.3/canvas/api/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:59:27.000000 edq-canvas-0.0.3/canvas/api/__init__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.399359 edq-canvas-0.0.3/canvas/api/assignment/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.3/canvas/api/assignment/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      633 2024-03-07 19:12:01.000000 edq-canvas-0.0.3/canvas/api/assignment/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1312 2024-03-07 19:35:20.000000 edq-canvas-0.0.3/canvas/api/assignment/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2418 2024-03-07 21:36:19.000000 edq-canvas-0.0.3/canvas/api/assignment/fetchscores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      819 2024-03-07 19:12:56.000000 edq-canvas-0.0.3/canvas/api/assignment/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2845 2024-03-07 19:33:43.000000 edq-canvas-0.0.3/canvas/api/assignment/resolve.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2741 2024-03-10 23:58:43.000000 edq-canvas-0.0.3/canvas/api/assignment/uploadscores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3435 2024-03-09 13:59:12.000000 edq-canvas-0.0.3/canvas/api/common.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/api/gradebook/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.3/canvas/api/gradebook/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3166 2024-02-17 15:14:24.000000 edq-canvas-0.0.3/canvas/api/gradebook/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3194 2024-03-10 23:57:17.000000 edq-canvas-0.0.3/canvas/api/gradebook/upload.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/api/user/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 05:13:50.000000 edq-canvas-0.0.3/canvas/api/user/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      815 2024-03-07 21:55:23.000000 edq-canvas-0.0.3/canvas/api/user/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1319 2024-02-17 15:02:45.000000 edq-canvas-0.0.3/canvas/api/user/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      877 2024-02-17 14:57:23.000000 edq-canvas-0.0.3/canvas/api/user/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3029 2024-03-07 19:24:09.000000 edq-canvas-0.0.3/canvas/api/user/resolve.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/cli/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:48:49.000000 edq-canvas-0.0.3/canvas/cli/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      409 2024-03-07 15:45:52.000000 edq-canvas-0.0.3/canvas/cli/__main__.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/cli/assignment/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.3/canvas/cli/assignment/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      318 2024-03-07 16:09:16.000000 edq-canvas-0.0.3/canvas/cli/assignment/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      324 2024-02-15 17:43:24.000000 edq-canvas-0.0.3/canvas/cli/assignment/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1483 2024-03-10 22:45:10.000000 edq-canvas-0.0.3/canvas/cli/assignment/fetch-scores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1961 2024-03-07 19:15:25.000000 edq-canvas-0.0.3/canvas/cli/assignment/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-02-15 17:43:24.000000 edq-canvas-0.0.3/canvas/cli/assignment/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1361 2024-03-11 15:58:40.000000 edq-canvas-0.0.3/canvas/cli/assignment/upload-score.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2659 2024-03-11 15:49:58.000000 edq-canvas-0.0.3/canvas/cli/assignment/upload-scores.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1159 2024-03-18 22:04:11.000000 edq-canvas-0.0.3/canvas/cli/common.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/cli/gradebook/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.3/canvas/cli/gradebook/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      316 2024-03-07 16:10:20.000000 edq-canvas-0.0.3/canvas/cli/gradebook/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2912 2024-03-08 16:20:14.000000 edq-canvas-0.0.3/canvas/cli/gradebook/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     3706 2024-03-11 00:08:28.000000 edq-canvas-0.0.3/canvas/cli/gradebook/upload.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.402692 edq-canvas-0.0.3/canvas/cli/user/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 04:32:06.000000 edq-canvas-0.0.3/canvas/cli/user/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      306 2024-03-07 16:10:42.000000 edq-canvas-0.0.3/canvas/cli/user/__main__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      267 2024-02-17 05:36:04.000000 edq-canvas-0.0.3/canvas/cli/user/common.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1891 2024-03-07 19:15:25.000000 edq-canvas-0.0.3/canvas/cli/user/fetch.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-03-10 21:53:47.000000 edq-canvas-0.0.3/canvas/cli/user/list.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     4696 2024-03-10 22:45:58.000000 edq-canvas-0.0.3/canvas/config.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      803 2024-02-13 16:16:03.000000 edq-canvas-0.0.3/canvas/log.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.406026 edq-canvas-0.0.3/canvas/util/
--rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:49:12.000000 edq-canvas-0.0.3/canvas/util/__init__.py
--rw-rw----   0 eriq      (1000) eriq      (1000)     2872 2024-03-07 16:35:41.000000 edq-canvas-0.0.3/canvas/util/cli.py
--rw-rw----   0 eriq      (1000) eriq      (1000)      341 2024-02-04 23:50:26.000000 edq-canvas-0.0.3/canvas/util/code.py
-drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-03-25 20:09:43.406026 edq-canvas-0.0.3/edq_canvas.egg-info/
--rw-r--r--   0 eriq      (1000) eriq      (1000)    10904 2024-03-25 20:09:43.000000 edq-canvas-0.0.3/edq_canvas.egg-info/PKG-INFO
--rw-rw----   0 eriq      (1000) eriq      (1000)     1437 2024-03-25 20:09:43.000000 edq-canvas-0.0.3/edq_canvas.egg-info/SOURCES.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-03-25 20:09:43.000000 edq-canvas-0.0.3/edq_canvas.egg-info/dependency_links.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)       52 2024-03-25 20:09:43.000000 edq-canvas-0.0.3/edq_canvas.egg-info/requires.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)        7 2024-03-25 20:09:43.000000 edq-canvas-0.0.3/edq_canvas.egg-info/top_level.txt
--rw-rw----   0 eriq      (1000) eriq      (1000)      918 2024-03-25 20:09:20.000000 edq-canvas-0.0.3/pyproject.toml
--rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-03-25 20:09:43.406026 edq-canvas-0.0.3/setup.cfg
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1071 2024-02-03 22:26:13.000000 edq-canvas-0.0.4/LICENSE
+-rw-r--r--   0 eriq      (1000) eriq      (1000)    11022 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)     9109 2024-04-11 22:00:49.000000 edq-canvas-0.0.4/README.md
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-03 22:28:32.000000 edq-canvas-0.0.4/canvas/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      201 2024-03-07 16:13:16.000000 edq-canvas-0.0.4/canvas/__main__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/api/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:59:27.000000 edq-canvas-0.0.4/canvas/api/__init__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/api/assignment/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.4/canvas/api/assignment/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      633 2024-03-07 19:12:01.000000 edq-canvas-0.0.4/canvas/api/assignment/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1312 2024-03-07 19:35:20.000000 edq-canvas-0.0.4/canvas/api/assignment/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2418 2024-03-07 21:36:19.000000 edq-canvas-0.0.4/canvas/api/assignment/fetchscores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      819 2024-03-07 19:12:56.000000 edq-canvas-0.0.4/canvas/api/assignment/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2845 2024-03-07 19:33:43.000000 edq-canvas-0.0.4/canvas/api/assignment/resolve.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2741 2024-03-10 23:58:43.000000 edq-canvas-0.0.4/canvas/api/assignment/uploadscores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3435 2024-03-09 13:59:12.000000 edq-canvas-0.0.4/canvas/api/common.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/api/gradebook/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.4/canvas/api/gradebook/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3166 2024-02-17 15:14:24.000000 edq-canvas-0.0.4/canvas/api/gradebook/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3194 2024-03-10 23:57:17.000000 edq-canvas-0.0.4/canvas/api/gradebook/upload.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/api/user/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 05:13:50.000000 edq-canvas-0.0.4/canvas/api/user/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      815 2024-03-07 21:55:23.000000 edq-canvas-0.0.4/canvas/api/user/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1319 2024-02-17 15:02:45.000000 edq-canvas-0.0.4/canvas/api/user/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      877 2024-02-17 14:57:23.000000 edq-canvas-0.0.4/canvas/api/user/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3029 2024-03-07 19:24:09.000000 edq-canvas-0.0.4/canvas/api/user/resolve.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.970612 edq-canvas-0.0.4/canvas/cli/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:48:49.000000 edq-canvas-0.0.4/canvas/cli/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      409 2024-03-07 15:45:52.000000 edq-canvas-0.0.4/canvas/cli/__main__.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/canvas/cli/assignment/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:28:53.000000 edq-canvas-0.0.4/canvas/cli/assignment/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      318 2024-03-07 16:09:16.000000 edq-canvas-0.0.4/canvas/cli/assignment/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      324 2024-02-15 17:43:24.000000 edq-canvas-0.0.4/canvas/cli/assignment/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1483 2024-03-10 22:45:10.000000 edq-canvas-0.0.4/canvas/cli/assignment/fetch-scores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1961 2024-03-07 19:15:25.000000 edq-canvas-0.0.4/canvas/cli/assignment/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-02-15 17:43:24.000000 edq-canvas-0.0.4/canvas/cli/assignment/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1361 2024-03-11 15:58:40.000000 edq-canvas-0.0.4/canvas/cli/assignment/upload-score.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2659 2024-03-11 15:49:58.000000 edq-canvas-0.0.4/canvas/cli/assignment/upload-scores.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1159 2024-03-18 22:04:11.000000 edq-canvas-0.0.4/canvas/cli/common.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/canvas/cli/gradebook/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-11 22:26:51.000000 edq-canvas-0.0.4/canvas/cli/gradebook/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      316 2024-03-07 16:10:20.000000 edq-canvas-0.0.4/canvas/cli/gradebook/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2912 2024-03-08 16:20:14.000000 edq-canvas-0.0.4/canvas/cli/gradebook/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     3706 2024-03-11 00:08:28.000000 edq-canvas-0.0.4/canvas/cli/gradebook/upload.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/canvas/cli/user/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 04:32:06.000000 edq-canvas-0.0.4/canvas/cli/user/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      306 2024-03-07 16:10:42.000000 edq-canvas-0.0.4/canvas/cli/user/__main__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      267 2024-02-17 05:36:04.000000 edq-canvas-0.0.4/canvas/cli/user/common.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1891 2024-03-07 19:15:25.000000 edq-canvas-0.0.4/canvas/cli/user/fetch.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1649 2024-03-10 21:53:47.000000 edq-canvas-0.0.4/canvas/cli/user/list.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     4706 2024-04-11 21:58:26.000000 edq-canvas-0.0.4/canvas/config.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      803 2024-02-13 16:16:03.000000 edq-canvas-0.0.4/canvas/log.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/canvas/util/
+-rw-rw----   0 eriq      (1000) eriq      (1000)        0 2024-02-04 23:49:12.000000 edq-canvas-0.0.4/canvas/util/__init__.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)     2872 2024-03-07 16:35:41.000000 edq-canvas-0.0.4/canvas/util/cli.py
+-rw-rw----   0 eriq      (1000) eriq      (1000)      341 2024-02-04 23:50:26.000000 edq-canvas-0.0.4/canvas/util/code.py
+drwxrwx---   0 eriq      (1000) eriq      (1000)        0 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/edq_canvas.egg-info/
+-rw-r--r--   0 eriq      (1000) eriq      (1000)    11022 2024-04-11 22:18:16.000000 edq-canvas-0.0.4/edq_canvas.egg-info/PKG-INFO
+-rw-rw----   0 eriq      (1000) eriq      (1000)     1437 2024-04-11 22:18:16.000000 edq-canvas-0.0.4/edq_canvas.egg-info/SOURCES.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        1 2024-04-11 22:18:16.000000 edq-canvas-0.0.4/edq_canvas.egg-info/dependency_links.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)       52 2024-04-11 22:18:16.000000 edq-canvas-0.0.4/edq_canvas.egg-info/requires.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)        7 2024-04-11 22:18:16.000000 edq-canvas-0.0.4/edq_canvas.egg-info/top_level.txt
+-rw-rw----   0 eriq      (1000) eriq      (1000)      918 2024-04-11 22:03:39.000000 edq-canvas-0.0.4/pyproject.toml
+-rw-rw----   0 eriq      (1000) eriq      (1000)       38 2024-04-11 22:18:16.973945 edq-canvas-0.0.4/setup.cfg
```

### Comparing `edq-canvas-0.0.3/LICENSE` & `edq-canvas-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/PKG-INFO` & `edq-canvas-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edq-canvas
-Version: 0.0.3
+Version: 0.0.4
 Summary: A suite of tools and Python interface for Instructure's Canvas LMS.
 Author-email: Eriq Augustine <eaugusti@ucsc.edu>
 License: MIT License
         
         Copyright (c) 2023 Eriq Augustine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -90,31 +90,33 @@
 python3 -m canvas.cli.user.list --server canvas.test.com --course 12345 --token abc123
 ```
 However, it will generally be more convenient to hold these common options in a more reusable location.
 
 There are several other places that config options can be specified,
 with each later location overriding any earlier options.
 Here are the places options can be specified in the order that they are checked:
- 1. `./config.json` -- If a `config.json` exists in the current directory, it is loaded.
+ 1. `./edq-canvas.json` -- If a `edq-canvas.json` exists in the current directory, it is loaded.
  2. `<platform-specific user config location>/edq-canvas.json` -- A directory which is considered the "proper" place to store user-related config for the platform you are using (according to [platformdirs](https://github.com/platformdirs/platformdirs)). Use `--help` to see the exact place in your specific case. This is a great place to store login credentials.
  3. Files specified by `--config` -- These files are loaded in the order they appear on the command-line.
  4. Bare Options -- Options specified directly like `--course` or `--token`. These will override all previous options.
 
-Using the default config file (`config.json`):
+Using the default config file (`edq-canvas.json`):
 ```sh
-# `./config.json` will be looked for and loaded if it exists.
+# `./edq-canvas.json` will be looked for and loaded if it exists.
 python3 -m canvas.cli.user.list
 ```
 
 Using a custom config file (`my_config.json`):
 ```sh
 # `./my_config.json` will be used.
 python3 -m canvas.cli.user.list --config my_config.json
 ```
 
+A sample config file is provided in this repo at [sample-edq-canvas.json](./sample-edq-canvas.json).
+
 For brevity, all future commands in this document will assume that all standard config options are in the default
 config files (and thus will not need to be specified).
 
 ## Usage Notes
 
 ### User Queries
```

### Comparing `edq-canvas-0.0.3/README.md` & `edq-canvas-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,31 +50,33 @@
 python3 -m canvas.cli.user.list --server canvas.test.com --course 12345 --token abc123
 ```
 However, it will generally be more convenient to hold these common options in a more reusable location.
 
 There are several other places that config options can be specified,
 with each later location overriding any earlier options.
 Here are the places options can be specified in the order that they are checked:
- 1. `./config.json` -- If a `config.json` exists in the current directory, it is loaded.
+ 1. `./edq-canvas.json` -- If a `edq-canvas.json` exists in the current directory, it is loaded.
  2. `<platform-specific user config location>/edq-canvas.json` -- A directory which is considered the "proper" place to store user-related config for the platform you are using (according to [platformdirs](https://github.com/platformdirs/platformdirs)). Use `--help` to see the exact place in your specific case. This is a great place to store login credentials.
  3. Files specified by `--config` -- These files are loaded in the order they appear on the command-line.
  4. Bare Options -- Options specified directly like `--course` or `--token`. These will override all previous options.
 
-Using the default config file (`config.json`):
+Using the default config file (`edq-canvas.json`):
 ```sh
-# `./config.json` will be looked for and loaded if it exists.
+# `./edq-canvas.json` will be looked for and loaded if it exists.
 python3 -m canvas.cli.user.list
 ```
 
 Using a custom config file (`my_config.json`):
 ```sh
 # `./my_config.json` will be used.
 python3 -m canvas.cli.user.list --config my_config.json
 ```
 
+A sample config file is provided in this repo at [sample-edq-canvas.json](./sample-edq-canvas.json).
+
 For brevity, all future commands in this document will assume that all standard config options are in the default
 config files (and thus will not need to be specified).
 
 ## Usage Notes
 
 ### User Queries
```

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/common.py` & `edq-canvas-0.0.4/canvas/api/assignment/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/fetch.py` & `edq-canvas-0.0.4/canvas/api/assignment/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/fetchscores.py` & `edq-canvas-0.0.4/canvas/api/assignment/fetchscores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/list.py` & `edq-canvas-0.0.4/canvas/api/assignment/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/resolve.py` & `edq-canvas-0.0.4/canvas/api/assignment/resolve.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/assignment/uploadscores.py` & `edq-canvas-0.0.4/canvas/api/assignment/uploadscores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/common.py` & `edq-canvas-0.0.4/canvas/api/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/gradebook/fetch.py` & `edq-canvas-0.0.4/canvas/api/gradebook/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/gradebook/upload.py` & `edq-canvas-0.0.4/canvas/api/gradebook/upload.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/user/common.py` & `edq-canvas-0.0.4/canvas/api/user/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/user/fetch.py` & `edq-canvas-0.0.4/canvas/api/user/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/user/list.py` & `edq-canvas-0.0.4/canvas/api/user/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/api/user/resolve.py` & `edq-canvas-0.0.4/canvas/api/user/resolve.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/assignment/fetch-scores.py` & `edq-canvas-0.0.4/canvas/cli/assignment/fetch-scores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/assignment/fetch.py` & `edq-canvas-0.0.4/canvas/cli/assignment/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/assignment/list.py` & `edq-canvas-0.0.4/canvas/cli/assignment/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/assignment/upload-score.py` & `edq-canvas-0.0.4/canvas/cli/assignment/upload-score.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/assignment/upload-scores.py` & `edq-canvas-0.0.4/canvas/cli/assignment/upload-scores.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/common.py` & `edq-canvas-0.0.4/canvas/cli/common.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/gradebook/fetch.py` & `edq-canvas-0.0.4/canvas/cli/gradebook/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/gradebook/upload.py` & `edq-canvas-0.0.4/canvas/cli/gradebook/upload.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/user/fetch.py` & `edq-canvas-0.0.4/canvas/cli/user/fetch.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/cli/user/list.py` & `edq-canvas-0.0.4/canvas/cli/user/list.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/config.py` & `edq-canvas-0.0.4/canvas/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import urllib.parse
 
 import json5
 import platformdirs
 
 import canvas.log
 
-DEFAULT_CONFIG_FILENAME = 'config.json'
-DEFAULT_USER_CONFIG_PATH = platformdirs.user_config_dir('edq-canvas.json')
+DEFAULT_CONFIG_FILENAME = 'edq-canvas.json'
+DEFAULT_USER_CONFIG_PATH = platformdirs.user_config_dir(DEFAULT_CONFIG_FILENAME)
 
 CONFIG_PATHS_KEY = 'config_paths'
 
 REQUIRED_KEYS = ['server', 'token']
 
 def get_config(exit_on_error = False, modify_parser = None, **parser_options):
     """
```

### Comparing `edq-canvas-0.0.3/canvas/log.py` & `edq-canvas-0.0.4/canvas/log.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/canvas/util/cli.py` & `edq-canvas-0.0.4/canvas/util/cli.py`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/edq_canvas.egg-info/PKG-INFO` & `edq-canvas-0.0.4/edq_canvas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edq-canvas
-Version: 0.0.3
+Version: 0.0.4
 Summary: A suite of tools and Python interface for Instructure's Canvas LMS.
 Author-email: Eriq Augustine <eaugusti@ucsc.edu>
 License: MIT License
         
         Copyright (c) 2023 Eriq Augustine
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -90,31 +90,33 @@
 python3 -m canvas.cli.user.list --server canvas.test.com --course 12345 --token abc123
 ```
 However, it will generally be more convenient to hold these common options in a more reusable location.
 
 There are several other places that config options can be specified,
 with each later location overriding any earlier options.
 Here are the places options can be specified in the order that they are checked:
- 1. `./config.json` -- If a `config.json` exists in the current directory, it is loaded.
+ 1. `./edq-canvas.json` -- If a `edq-canvas.json` exists in the current directory, it is loaded.
  2. `<platform-specific user config location>/edq-canvas.json` -- A directory which is considered the "proper" place to store user-related config for the platform you are using (according to [platformdirs](https://github.com/platformdirs/platformdirs)). Use `--help` to see the exact place in your specific case. This is a great place to store login credentials.
  3. Files specified by `--config` -- These files are loaded in the order they appear on the command-line.
  4. Bare Options -- Options specified directly like `--course` or `--token`. These will override all previous options.
 
-Using the default config file (`config.json`):
+Using the default config file (`edq-canvas.json`):
 ```sh
-# `./config.json` will be looked for and loaded if it exists.
+# `./edq-canvas.json` will be looked for and loaded if it exists.
 python3 -m canvas.cli.user.list
 ```
 
 Using a custom config file (`my_config.json`):
 ```sh
 # `./my_config.json` will be used.
 python3 -m canvas.cli.user.list --config my_config.json
 ```
 
+A sample config file is provided in this repo at [sample-edq-canvas.json](./sample-edq-canvas.json).
+
 For brevity, all future commands in this document will assume that all standard config options are in the default
 config files (and thus will not need to be specified).
 
 ## Usage Notes
 
 ### User Queries
```

### Comparing `edq-canvas-0.0.3/edq_canvas.egg-info/SOURCES.txt` & `edq-canvas-0.0.4/edq_canvas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edq-canvas-0.0.3/pyproject.toml` & `edq-canvas-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "packaging>=21.3",
     "twine",
     "vermin",
 ]
 
 [project]
 name = "edq-canvas"
-version = "0.0.3"
+version = "0.0.4"
 description = "A suite of tools and Python interface for Instructure's Canvas LMS."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "Eriq Augustine", email = "eaugusti@ucsc.edu"},
```

