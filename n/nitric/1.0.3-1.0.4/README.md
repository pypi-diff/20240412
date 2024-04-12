# Comparing `tmp/nitric-1.0.3.tar.gz` & `tmp/nitric-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-1.0.3.tar", last modified: Wed Apr 10 07:09:14 2024, max compression
+gzip compressed data, was "nitric-1.0.4.tar", last modified: Fri Apr 12 03:52:40 2024, max compression
```

## Comparing `nitric-1.0.3.tar` & `nitric-1.0.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 07:09:14.691824 nitric-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-10 07:08:34.000000 nitric-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/bidi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15159 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/KeyValue/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/KeyValue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/KeyValue/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/KeyValue/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/apis/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/apis/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/deployments/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/deployments/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/http/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/http/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/http/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/kvstore/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/kvstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/kvstore/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/kvstore/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/queues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/queues/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/queues/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/resources/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/schedules/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/schedules/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/secrets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/secrets/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric/proto/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/topics/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/topics/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/websockets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/proto/websockets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/proto/websockets/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 07:08:34.000000 nitric-1.0.3/nitric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.691824 nitric-1.0.3/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/resources/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-10 07:09:09.000000 nitric-1.0.3/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 07:09:14.687824 nitric-1.0.3/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 07:09:14.000000 nitric-1.0.3/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-10 07:08:34.000000 nitric-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 07:09:14.691824 nitric-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-10 07:08:34.000000 nitric-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:40.776903 nitric-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 03:52:02.000000 nitric-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/bidi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/KeyValue/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/KeyValue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/KeyValue/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/KeyValue/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/apis/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/apis/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/deployments/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/deployments/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/http/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/http/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/kvstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/kvstore/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/kvstore/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/queues/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/queues/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/queues/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/resources/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/schedules/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/schedules/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/secrets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/secrets/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/topics/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/websockets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/websockets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/websockets/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:02.000000 nitric-1.0.4/nitric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 03:52:02.000000 nitric-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:52:40.776903 nitric-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-12 03:52:02.000000 nitric-1.0.4/setup.py
```

### Comparing `nitric-1.0.3/PKG-INFO` & `nitric-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.3 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.4 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.3/README.md` & `nitric-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/__init__.py` & `nitric-1.0.4/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/application.py` & `nitric-1.0.4/nitric/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,12 +71,13 @@
             try:
                 loop = asyncio.get_running_loop()
             except RuntimeError:
                 loop = asyncio.get_event_loop()
 
             loop.run_until_complete(asyncio.gather(*[wkr.start() for wkr in cls._workers]))
         except KeyboardInterrupt:
+
             print("\nexiting")
         except ConnectionRefusedError:
             raise NitricUnavailableException(
                 'Unable to connect to a nitric server! If you\'re running locally make sure to run "nitric start"'
             ) from None
```

### Comparing `nitric-1.0.3/nitric/bidi.py` & `nitric-1.0.4/nitric/bidi.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/config/__init__.py` & `nitric-1.0.4/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/context.py` & `nitric-1.0.4/nitric/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,22 +24,18 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Any, Dict, Generic, List, Optional, Protocol, TypeVar, Union
 
 from opentelemetry import propagate
 
 from nitric.proto.schedules.v1 import ServerMessage as ScheduleServerMessage
-from nitric.proto.storage.v1 import BlobEventRequest, BlobEventType
 from nitric.proto.topics.v1 import ClientMessage as TopicClientMessage
 from nitric.proto.topics.v1 import MessageResponse as TopicResponse
 from nitric.proto.topics.v1 import ServerMessage as TopicServerMessage
 
-# from nitric.proto.websockets.v1 import ServerMessage as WebsocketServerMessage
-# from nitric.proto.websockets.v1 import WebsocketEventResponse
-
 Record = Dict[str, Union[str, List[str]]]
 PROPAGATOR = propagate.get_global_textmap()
 
 
 class HttpMethod(Enum):
     """Valid query expression operators."""
 
@@ -251,81 +247,14 @@
             self.res = response
         elif isinstance(request, WebsocketConnectionRequest):
             self.res = WebsocketConnectionResponse()
         else:
             self.res = WebsocketResponse()
 
 
-class BucketNotifyRequest:
-    """Represents a translated Event, from a subscribed bucket notification, forwarded from the Nitric Membrane."""
-
-    bucket_name: str
-    key: str
-    notification_type: BlobEventType
-
-    def __init__(self, bucket_name: str, key: str, notification_type: BlobEventType):
-        """Construct a new EventRequest."""
-        self.bucket_name = bucket_name
-        self.key = key
-        self.notification_type = notification_type
-
-
-class BucketNotifyResponse:
-    """Represents the response to a trigger from a Bucket."""
-
-    def __init__(self, success: bool = True):
-        """Construct a new BucketNotificationResponse."""
-        self.success = success
-
-
-class BucketNotificationContext:
-    """Represents the full request/response context for a bucket notification trigger."""
-
-    def __init__(self, request: BucketNotifyRequest, response: Optional[BucketNotifyResponse] = None):
-        """Construct a new BucketNotificationContext."""
-        self.req = request
-        self.res = response if response else BucketNotifyResponse()
-
-
-class FileNotifyRequest(BucketNotifyRequest):
-    """Represents a translated Event, from a subscribed bucket notification, forwarded from the Nitric Membrane."""
-
-    def __init__(
-        self,
-        bucket_name: str,
-        bucket_ref: Any,  # can't import BucketRef due to circular dependency problems
-        key: str,
-        notification_type: BlobEventType,
-    ):
-        """Construct a new FileNotificationRequest."""
-        super().__init__(bucket_name=bucket_name, key=key, notification_type=notification_type)
-        self.file = bucket_ref.file(key)
-
-
-class FileNotificationContext(BucketNotificationContext):
-    """Represents the full request/response context for a bucket notification trigger."""
-
-    def __init__(self, request: FileNotifyRequest, response: Optional[BucketNotifyResponse] = None):
-        """Construct a new FileNotificationContext."""
-        super().__init__(request=request, response=response)
-        self.req = request
-
-    @staticmethod
-    def _from_client_message_with_bucket(msg: BlobEventRequest, bucket_ref) -> FileNotificationContext:
-        """Construct a new FileNotificationTrigger from a Bucket Notification trigger from the Nitric Membrane."""
-        return FileNotificationContext(
-            request=FileNotifyRequest(
-                bucket_name=msg.bucket_name,
-                key=msg.blob_event.key,
-                bucket_ref=bucket_ref,
-                notification_type=msg.blob_event.type,
-            )
-        )
-
-
 # == Schedules ==
 
 
 class IntervalRequest:
     """Represents a translated Event, from a Schedule, forwarded from the Nitric Membrane."""
 
     def __init__(self, schedule_name: str):
@@ -348,24 +277,15 @@
 
     def __init__(self, msg: ScheduleServerMessage):
         """Construct a new EventContext."""
         self.req = IntervalRequest(schedule_name=msg.interval_request.schedule_name)
         self.res = IntervalResponse(msg.id)
 
 
-C = TypeVar(
-    "C",
-    TriggerContext,
-    HttpContext,
-    MessageContext,
-    FileNotificationContext,
-    BucketNotificationContext,
-    WebsocketContext,
-    IntervalContext,
-)
+C = TypeVar("C")
 
 
 class Middleware(Protocol, Generic[C]):
     """A middleware function."""
 
     async def __call__(self, ctx: C, nxt: Optional[Middleware[C]] = None) -> C:
         """Process trigger context."""
@@ -379,23 +299,19 @@
         """Process trigger context."""
         ...
 
 
 HttpMiddleware = Middleware[HttpContext]
 EventMiddleware = Middleware[MessageContext]
 IntervalMiddleware = Middleware[IntervalContext]
-BucketNotificationMiddleware = Middleware[BucketNotificationContext]
-FileNotificationMiddleware = Middleware[FileNotificationContext]
 WebsocketMiddleware = Middleware[WebsocketContext]
 
 HttpHandler = Handler[HttpContext]
 EventHandler = Handler[MessageContext]
 IntervalHandler = Handler[IntervalContext]
-BucketNotificationHandler = Handler[BucketNotificationContext]
-FileNotificationHandler = Handler[FileNotificationContext]
 WebsocketHandler = Handler[WebsocketContext]
 
 
 def _convert_to_middleware(handler: Handler[C] | Middleware[C]) -> Middleware[C]:
     """Convert a handler to a middleware, if it's already a middleware it's returned unchanged."""
     if not _is_handler(handler):
         # it's not a middleware, don't convert it.
```

### Comparing `nitric-1.0.3/nitric/exception.py` & `nitric-1.0.4/nitric/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/KeyValue/__init__.py` & `nitric-1.0.4/nitric/proto/KeyValue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/KeyValue/v1/__init__.py` & `nitric-1.0.4/nitric/proto/KeyValue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/__init__.py` & `nitric-1.0.4/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/apis/__init__.py` & `nitric-1.0.4/nitric/proto/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/apis/v1/__init__.py` & `nitric-1.0.4/nitric/proto/apis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/deployments/__init__.py` & `nitric-1.0.4/nitric/proto/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/deployments/v1/__init__.py` & `nitric-1.0.4/nitric/proto/deployments/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/http/__init__.py` & `nitric-1.0.4/nitric/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/http/v1/__init__.py` & `nitric-1.0.4/nitric/proto/http/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/kvstore/__init__.py` & `nitric-1.0.4/nitric/proto/kvstore/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/kvstore/v1/__init__.py` & `nitric-1.0.4/nitric/proto/kvstore/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/queues/__init__.py` & `nitric-1.0.4/nitric/proto/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/queues/v1/__init__.py` & `nitric-1.0.4/nitric/proto/queues/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/resources/__init__.py` & `nitric-1.0.4/nitric/proto/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/resources/v1/__init__.py` & `nitric-1.0.4/nitric/proto/resources/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/schedules/__init__.py` & `nitric-1.0.4/nitric/proto/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/schedules/v1/__init__.py` & `nitric-1.0.4/nitric/proto/schedules/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/secrets/__init__.py` & `nitric-1.0.4/nitric/proto/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/secrets/v1/__init__.py` & `nitric-1.0.4/nitric/proto/secrets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/storage/__init__.py` & `nitric-1.0.4/nitric/proto/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/storage/v1/__init__.py` & `nitric-1.0.4/nitric/proto/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/topics/__init__.py` & `nitric-1.0.4/nitric/proto/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/topics/v1/__init__.py` & `nitric-1.0.4/nitric/proto/topics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/websockets/__init__.py` & `nitric-1.0.4/nitric/proto/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/proto/websockets/v1/__init__.py` & `nitric-1.0.4/nitric/proto/websockets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/resources/__init__.py` & `nitric-1.0.4/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/resources/apis.py` & `nitric-1.0.4/nitric/resources/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         middleware: Optional[Union[HttpMiddleware, List[HttpMiddleware]]] = None,
         security: Optional[List[ScopedOidcOptions]] = None,
     ):
         """Construct a new API options object."""
         if middleware is None:
             middleware = []
         if security is None:
-            security = {}
+            security = []
         self.middleware = middleware
         self.security = security
         self.path = path
 
 
 class RouteOptions:
     """Represents options when creating a route, such as middleware to be applied to all HTTP Methods for the route."""
@@ -198,15 +198,15 @@
 
     def _route(self, match: str, opts: Optional[RouteOptions] = None) -> Route:
         """Define an HTTP route to be handled by this API."""
         if opts is None:
             opts = RouteOptions()
 
         if self.middleware is not None:
-            opts.middleware = self.middleware + opts.middleware
+            opts.middleware = (self.middleware + opts.middleware) if opts.middleware is not None else self.middleware
 
         r = Route(self, match, opts)
         self.routes.append(r)
         return r
 
     def all(self, match: str, opts: Optional[MethodOptions] = None) -> Callable[[HttpHandler], None]:
         """Define an HTTP route which will respond to HTTP GET requests."""
```

### Comparing `nitric-1.0.3/nitric/resources/buckets.py` & `nitric-1.0.4/nitric/resources/buckets.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,18 +28,19 @@
 import betterproto
 import grpclib
 from grpclib import GRPCError
 from grpclib.client import Channel
 
 from nitric.application import Nitric
 from nitric.bidi import AsyncNotifierList
-from nitric.context import BucketNotificationContext, BucketNotificationHandler, BucketNotifyRequest, FunctionServer
+from nitric.context import FunctionServer, Handler, Middleware
 from nitric.exception import InvalidArgumentException, exception_from_grpc_error
 from nitric.proto.resources.v1 import Action, ResourceDeclareRequest, ResourceIdentifier, ResourceType
 from nitric.proto.storage.v1 import (
+    BlobEventRequest,
     BlobEventResponse,
     BlobEventType,
     ClientMessage,
     RegistrationRequest,
     StorageDeleteRequest,
     StorageExistsRequest,
     StorageListBlobsRequest,
@@ -50,14 +51,92 @@
     StorageStub,
     StorageWriteRequest,
 )
 from nitric.resources.resource import SecureResource
 from nitric.utils import new_default_channel
 
 
+class BucketNotifyRequest:
+    """Represents a translated Event, from a subscribed bucket notification, forwarded from the Nitric Membrane."""
+
+    bucket_name: str
+    key: str
+    notification_type: BlobEventType
+    bucket: BucketRef
+    file: FileRef
+
+    def __init__(self, bucket_name: str, key: str, notification_type: BlobEventType):
+        """Construct a new BucketNotifyRequest."""
+        self.bucket_name = bucket_name
+        self.key = key
+        self.notification_type = notification_type
+        self.bucket = BucketRef(bucket_name)
+        self.file = self.bucket.file(key)
+
+
+class BucketNotifyResponse:
+    """Represents the response to a trigger from a Bucket."""
+
+    def __init__(self, success: bool = True):
+        """Construct a new BucketNotificationResponse."""
+        self.success = success
+
+
+class BucketNotificationContext:
+    """Represents the full request/response context for a bucket notification trigger."""
+
+    def __init__(self, request: BucketNotifyRequest, response: Optional[BucketNotifyResponse] = None):
+        """Construct a new BucketNotificationContext."""
+        self.req = request
+        self.res = response if response else BucketNotifyResponse()
+
+
+class FileNotifyRequest(BucketNotifyRequest):
+    """Represents a translated Event, from a subscribed bucket notification, forwarded from the Nitric Membrane."""
+
+    def __init__(
+        self,
+        bucket_name: str,
+        bucket_ref: BucketRef,
+        key: str,
+        notification_type: BlobEventType,
+    ):
+        """Construct a new FileNotificationRequest."""
+        super().__init__(bucket_name=bucket_name, key=key, notification_type=notification_type)
+        self.file = bucket_ref.file(key)
+
+
+class FileNotificationContext(BucketNotificationContext):
+    """Represents the full request/response context for a bucket notification trigger."""
+
+    def __init__(self, request: FileNotifyRequest, response: Optional[BucketNotifyResponse] = None):
+        """Construct a new FileNotificationContext."""
+        super().__init__(request=request, response=response)
+        self.req = request
+
+    @staticmethod
+    def _from_client_message_with_bucket(msg: BlobEventRequest, bucket_ref) -> FileNotificationContext:
+        """Construct a new FileNotificationTrigger from a Bucket Notification trigger from the Nitric Membrane."""
+        return FileNotificationContext(
+            request=FileNotifyRequest(
+                bucket_name=msg.bucket_name,
+                key=msg.blob_event.key,
+                bucket_ref=bucket_ref,
+                notification_type=msg.blob_event.type,
+            )
+        )
+
+
+BucketNotificationMiddleware = Middleware[BucketNotificationContext]
+BucketNotificationHandler = Handler[BucketNotificationContext]
+
+FileNotificationMiddleware = Middleware[FileNotificationContext]
+FileNotificationHandler = Handler[FileNotificationContext]
+
+
 class BucketRef(object):
     """A reference to a deployed storage bucket, used to interact with the bucket at runtime."""
 
     _channel: Channel
     _storage_stub: StorageStub
     name: str
 
@@ -86,14 +165,29 @@
     async def exists(self, key: str) -> bool:
         """Return true if a file in the bucket exists."""
         resp = await self._storage_stub.exists(
             storage_exists_request=StorageExistsRequest(bucket_name=self.name, key=key)
         )
         return resp.exists
 
+    def on(
+        self, notification_type: str, notification_prefix_filter: str
+    ) -> Callable[[BucketNotificationHandler], None]:
+        """Create and return a bucket notification decorator for this bucket."""
+
+        def decorator(func: BucketNotificationHandler) -> None:
+            Listener(
+                bucket_name=self.name,
+                notification_type=notification_type,
+                notification_prefix_filter=notification_prefix_filter,
+                handler=func,
+            )
+
+        return decorator
+
 
 class FileMode(Enum):
     """Definition of available operation modes for file signed URLs."""
 
     READ = 0
     WRITE = 1
 
@@ -117,76 +211,82 @@
     async def write(self, body: bytes):
         """
         Write the bytes as the content of this file.
 
         Will create the file if it doesn't already exist.
         """
         try:
-            await self._bucket._storage_stub.write(  # type: ignore pylint: disable=protected-access
+            await self._bucket._storage_stub.write(
                 storage_write_request=StorageWriteRequest(bucket_name=self._bucket.name, key=self.key, body=body)
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     async def read(self) -> bytes:
         """Read this files contents from the bucket."""
         try:
-            response = await self._bucket._storage_stub.read(  # type: ignore pylint: disable=protected-access
+            response = await self._bucket._storage_stub.read(
                 storage_read_request=StorageReadRequest(bucket_name=self._bucket.name, key=self.key)
             )
             return response.body
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     async def delete(self):
         """Delete this file from the bucket."""
         try:
-            await self._bucket._storage_stub.delete(  # type: ignore pylint: disable=protected-access
+            await self._bucket._storage_stub.delete(
                 storage_delete_request=StorageDeleteRequest(bucket_name=self._bucket.name, key=self.key)
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     async def upload_url(self, expiry: Optional[Union[timedelta, int]] = None):
         """
         Get a temporary writable URL to this file.
 
-        Parameters:
-
-        expiry (timedelta or int, optional): The expiry time for the signed URL.
-        If an integer is provided, it is treated as seconds. Default is 600 seconds.
+        Parameters
+        ----------
+        expiry : int, timedelta, optional
+            The expiry time for the signed URL.
+            If an integer is provided, it is treated as seconds. Default is 600 seconds.
 
-        Returns:
+        Returns
+        -------
         str: The signed URL.
+
         """
         return await self._sign_url(mode=FileMode.WRITE, expiry=expiry)
 
     async def download_url(self, expiry: Optional[Union[timedelta, int]] = None):
         """
         Get a temporary readable URL to this file.
 
-        Parameters:
+        Parameters
+        ----------
+        expiry : int, timedelta, optional
+            The expiry time for the signed URL.
+            If an integer is provided, it is treated as seconds. Default is 600 seconds.
 
-        expiry (timedelta or int, optional): The expiry time for the signed URL.
-        If an integer is provided, it is treated as seconds. Default is 600 seconds.
-
-        Returns:
+        Returns
+        -------
         str: The signed URL.
+
         """
         return await self._sign_url(mode=FileMode.READ, expiry=expiry)
 
     async def _sign_url(self, mode: FileMode = FileMode.READ, expiry: Optional[Union[timedelta, int]] = None):
         """Generate a signed URL for reading or writing to a file."""
         if expiry is None:
             expiry = timedelta(seconds=600)
         if not isinstance(expiry, timedelta):
             expiry = timedelta(seconds=expiry)
 
         try:
-            response = await self._bucket._storage_stub.pre_sign_url(  # type: ignore pylint: disable=protected-access
+            response = await self._bucket._storage_stub.pre_sign_url(
                 storage_pre_sign_url_request=StoragePreSignUrlRequest(
                     bucket_name=self._bucket.name, key=self.key, operation=mode.to_request_operation(), expiry=expiry
                 )
             )
             return response.url
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
@@ -253,15 +353,15 @@
             "write": [Action.BucketFilePut],
             "delete": [Action.BucketFileDelete],
         }
 
         return [action for perm in args for action in permission_actions_map[perm]]
 
     def _to_resource_id(self) -> ResourceIdentifier:
-        return ResourceIdentifier(name=self.name, type=ResourceType.Bucket)  # type:ignore
+        return ResourceIdentifier(name=self.name, type=ResourceType.Bucket)
 
     def allow(
         self,
         perm: Union[LegacyBucketPermission, BucketPermission],
         *args: Union[LegacyBucketPermission, BucketPermission],
     ) -> BucketRef:
         """Request the required permissions for this resource."""
@@ -312,14 +412,15 @@
 
         self._registration_request = RegistrationRequest(
             bucket_name=bucket_name,
             blob_event_type=event_type,
             key_prefix_filter=notification_prefix_filter,
         )
 
+        # noinspection PyProtectedMember
         Nitric._register_worker(self)
 
     async def _listener_request_iterator(self):
         # Register with the server
         yield ClientMessage(registration_request=self._registration_request)
         # wait for any responses for the server and send them
         async for response in self._responses:
@@ -355,19 +456,22 @@
                         be = BlobEventResponse(success=False)
                         response = ClientMessage(id=server_msg.id, blob_event_response=be)
                     await self._responses.add_item(response)
         except grpclib.exceptions.GRPCError as e:
             print(f"Stream terminated: {e.message}")
         except grpclib.exceptions.StreamTerminatedError:
             print("Stream from membrane closed.")
+        except KeyboardInterrupt:
+            print("Keyboard interrupt")
         finally:
             print("Closing client stream")
             channel.close()
+        print("Listener stopped")
 
 
 def bucket(name: str) -> Bucket:
     """
     Create and register a bucket.
 
     If a bucket has already been registered with the same name, the original reference will be reused.
     """
-    return Nitric._create_resource(Bucket, name)  # type: ignore pylint: disable=protected-access
+    return Nitric._create_resource(Bucket, name)
```

### Comparing `nitric-1.0.3/nitric/resources/kv.py` & `nitric-1.0.4/nitric/resources/kv.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/resources/queues.py` & `nitric-1.0.4/nitric/resources/queues.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     actions: List[Action]
 
     def __init__(self, name: str):
         """Construct a new queue resource."""
         super().__init__(name)
 
     def _to_resource_id(self) -> ResourceIdentifier:
-        return ResourceIdentifier(name=self.name, type=ResourceType.Queue)  # type:ignore
+        return ResourceIdentifier(name=self.name, type=ResourceType.Queue)
 
     def _perms_to_actions(self, *args: QueuePermission) -> List[Action]:
         permission_actions_map: dict[QueuePermission, List[Action]] = {
             "enqueue": [Action.QueueEnqueue],
             "dequeue": [Action.QueueDequeue],
         }
```

### Comparing `nitric-1.0.3/nitric/resources/resource.py` & `nitric-1.0.4/nitric/resources/resource.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/resources/schedules.py` & `nitric-1.0.4/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/resources/secrets.py` & `nitric-1.0.4/nitric/resources/secrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     actions: List[Action]
 
     def __init__(self, name: str):
         """Construct a new secret resource reference."""
         super().__init__(name)
 
     def _to_resource_id(self) -> ResourceIdentifier:
-        return ResourceIdentifier(name=self.name, type=ResourceType.Secret)  # type:ignore
+        return ResourceIdentifier(name=self.name, type=ResourceType.Secret)
 
     async def _register(self):
         try:
             await self._resources_stub.declare(
                 resource_declare_request=ResourceDeclareRequest(id=self._to_resource_id())
             )
         except GRPCError as grpc_err:
```

### Comparing `nitric-1.0.3/nitric/resources/topics.py` & `nitric-1.0.4/nitric/resources/topics.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             await self._resources_stub.declare(
                 resource_declare_request=ResourceDeclareRequest(id=self._to_resource_id())
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err) from grpc_err
 
     def _to_resource_id(self) -> ResourceIdentifier:
-        return ResourceIdentifier(name=self.name, type=ResourceType.Topic)  # type:ignore
+        return ResourceIdentifier(name=self.name, type=ResourceType.Topic)
 
     def _perms_to_actions(self, *args: TopicPermission) -> List[Action]:
         _permMap: dict[TopicPermission, List[Action]] = {"publish": [Action.TopicPublish]}
 
         return [action for perm in args for action in _permMap[perm]]
 
     def allow(self, perm: TopicPermission, *args: TopicPermission) -> TopicRef:
```

### Comparing `nitric-1.0.3/nitric/resources/websockets.py` & `nitric-1.0.4/nitric/resources/websockets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric/utils.py` & `nitric-1.0.4/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/nitric.egg-info/PKG-INFO` & `nitric-1.0.4/nitric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.3 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.4 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.3/nitric.egg-info/SOURCES.txt` & `nitric-1.0.4/nitric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitric-1.0.3/setup.py` & `nitric-1.0.4/setup.py`

 * *Files identical despite different names*

