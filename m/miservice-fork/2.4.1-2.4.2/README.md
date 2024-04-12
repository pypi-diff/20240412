# Comparing `tmp/miservice_fork-2.4.1.tar.gz` & `tmp/miservice_fork-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.4.1.tar", last modified: Tue Apr  2 14:00:29 2024, max compression
+gzip compressed data, was "miservice_fork-2.4.2.tar", last modified: Fri Apr 12 15:29:28 2024, max compression
```

## Comparing `miservice_fork-2.4.1.tar` & `miservice_fork-2.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.302715 miservice_fork-2.4.1/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.1/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-02 14:00:29.302225 miservice_fork-2.4.1/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     4541 2024-04-02 13:57:51.000000 miservice_fork-2.4.1/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.1/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.290848 miservice_fork-2.4.1/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.1/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.1/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     7930 2024-04-02 14:00:08.000000 miservice_fork-2.4.1/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.1/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.1/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.1/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     4251 2024-01-24 14:39:17.000000 miservice_fork-2.4.1/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.301142 miservice_fork-2.4.1/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       21 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-02 14:00:29.302763 miservice_fork-2.4.1/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-04-02 14:00:19.000000 miservice_fork-2.4.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.152382 miservice_fork-2.4.2/
+-rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.2/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-12 15:29:28.151923 miservice_fork-2.4.2/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     4541 2024-04-03 05:25:43.000000 miservice_fork-2.4.2/README.md
+-rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.2/micli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.146475 miservice_fork-2.4.2/miservice/
+-rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.2/miservice/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.2/miservice/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7927 2024-04-03 05:25:43.000000 miservice_fork-2.4.2/miservice/cli.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.2/miservice/miaccount.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.2/miservice/miiocommand.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.2/miservice/miioservice.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4251 2024-04-12 15:28:29.000000 miservice_fork-2.4.2/miservice/minaservice.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-12 15:29:28.150599 miservice_fork-2.4.2/miservice_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      424 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       46 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       21 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       10 2024-04-12 15:29:28.000000 miservice_fork-2.4.2/miservice_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-12 15:29:28.152442 miservice_fork-2.4.2/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-04-12 15:28:11.000000 miservice_fork-2.4.2/setup.py
```

### Comparing `miservice_fork-2.4.1/LICENSE` & `miservice_fork-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.1/PKG-INFO` & `miservice_fork-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.1
+Version: 2.4.2
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.1/README.md` & `miservice_fork-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.1/miservice/cli.py` & `miservice_fork-2.4.2/miservice/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,16 @@
             # TODO refactor this shit
             elif args.split(" ")[0].strip() in [
                 "play",
                 "pause",
                 "loop",
                 "play_list",
                 "suno",
-                "suno_random"
-                ]:
+                "suno_random",
+            ]:
                 arg = args.split(" ")[0].strip()
                 result = await mina_service.device_list()
                 if not env.get("MI_DID"):
                     raise Exception("Please export MI_DID in your env")
                 device_id = find_device_id(result, env.get("MI_DID", ""))
                 # tricky add it to global
                 device_id_list.append(device_id)
```

### Comparing `miservice_fork-2.4.1/miservice/miaccount.py` & `miservice_fork-2.4.2/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.1/miservice/miiocommand.py` & `miservice_fork-2.4.2/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.1/miservice/miioservice.py` & `miservice_fork-2.4.2/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.1/miservice/minaservice.py` & `miservice_fork-2.4.2/miservice/minaservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         )
 
     async def play_by_url(self, deviceId, url):
         return await self.ubus_request(
             deviceId,
             "player_play_url",
             "mediaplayer",
-            {"url": url, "type": 0, "media": "app_ios"},
+            {"url": url, "type": 1, "media": "app_ios"},
         )
 
     async def send_message(self, devices, devno, message, volume=None):  # -1/0/1...
         result = False
         for i in range(0, len(devices)):
             if (
                 devno == -1
```

### Comparing `miservice_fork-2.4.1/miservice_fork.egg-info/PKG-INFO` & `miservice_fork-2.4.2/miservice_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.1
+Version: 2.4.2
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.1/setup.py` & `miservice_fork-2.4.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.4.1",
+    version="2.4.2",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

