# Comparing `tmp/cloudflare-radar-0.2.tar.gz` & `tmp/cloudflare-radar-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-radar-0.2.tar", last modified: Sat Mar 23 06:55:52 2024, max compression
+gzip compressed data, was "cloudflare-radar-0.3.tar", last modified: Fri Apr 12 05:53:56 2024, max compression
```

## Comparing `cloudflare-radar-0.2.tar` & `cloudflare-radar-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/
--rw-r--r--   0 root         (0) root         (0)    18092 2024-03-19 03:04:54.000000 cloudflare-radar-0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      752 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-19 03:05:16.000000 cloudflare-radar-0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/cloudflare_radar/
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-19 04:23:55.000000 cloudflare-radar-0.2/cloudflare_radar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/cloudflare_radar/cmds/
--rw-r--r--   0 root         (0) root         (0)      766 2024-03-20 05:47:18.000000 cloudflare-radar-0.2/cloudflare_radar/cmds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1968 2024-03-22 09:55:10.000000 cloudflare-radar-0.2/cloudflare_radar/cmds/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/cloudflare_radar/utils/
--rw-r--r--   0 root         (0) root         (0)      446 2024-03-22 09:23:19.000000 cloudflare-radar-0.2/cloudflare_radar/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-03-23 06:46:21.000000 cloudflare-radar-0.2/cloudflare_radar/utils/attribute.py
--rw-r--r--   0 root         (0) root         (0)     2494 2024-03-22 09:26:45.000000 cloudflare-radar-0.2/cloudflare_radar/utils/domains.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-03-23 06:45:53.000000 cloudflare-radar-0.2/cloudflare_radar/utils/ranking.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-03-20 06:16:17.000000 cloudflare-radar-0.2/cloudflare_radar/utils/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/cloudflare_radar.egg-info/
--rw-r--r--   0 root         (0) root         (0)      752 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-23 06:55:52.000000 cloudflare-radar-0.2/cloudflare_radar.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)      513 2024-03-23 06:55:52.814119 cloudflare-radar-0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      889 2024-03-19 04:27:44.000000 cloudflare-radar-0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/
+-rw-r--r--   0 root         (0) root         (0)    18092 2024-03-19 03:04:54.000000 cloudflare-radar-0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       19 2024-03-19 03:05:16.000000 cloudflare-radar-0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:53:56.589274 cloudflare-radar-0.3/cloudflare_radar/
+-rw-r--r--   0 root         (0) root         (0)       15 2024-03-19 04:23:55.000000 cloudflare-radar-0.3/cloudflare_radar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/cloudflare_radar/cmds/
+-rw-r--r--   0 root         (0) root         (0)      766 2024-03-20 05:47:18.000000 cloudflare-radar-0.3/cloudflare_radar/cmds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2024-03-23 08:41:05.000000 cloudflare-radar-0.3/cloudflare_radar/cmds/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/cloudflare_radar/utils/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-03-23 08:15:15.000000 cloudflare-radar-0.3/cloudflare_radar/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-04-12 05:53:09.000000 cloudflare-radar-0.3/cloudflare_radar/utils/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     2689 2024-03-23 08:38:46.000000 cloudflare-radar-0.3/cloudflare_radar/utils/domains.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-09 12:36:21.000000 cloudflare-radar-0.3/cloudflare_radar/utils/ranking.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-03-20 06:16:17.000000 cloudflare-radar-0.3/cloudflare_radar/utils/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/cloudflare_radar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 05:53:56.000000 cloudflare-radar-0.3/cloudflare_radar.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-12 05:53:56.599274 cloudflare-radar-0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      889 2024-03-19 04:27:44.000000 cloudflare-radar-0.3/setup.py
```

### Comparing `cloudflare-radar-0.2/LICENSE` & `cloudflare-radar-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare-radar-0.2/PKG-INFO` & `cloudflare-radar-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-radar
-Version: 0.2
+Version: 0.3
 Summary: Get data from https://radar.cloudflare.com
 Home-page: https://github.com/DNSet/cloudflare-radar/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: GPLv2
 Project-URL: Source Code, https://github.com/DNSet/cloudflare-radar/
 Project-URL: Bug Tracker, https://github.com/DNSet/cloudflare-radar/issues
```

### Comparing `cloudflare-radar-0.2/cloudflare_radar/cmds/__init__.py` & `cloudflare-radar-0.3/cloudflare_radar/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudflare-radar-0.2/cloudflare_radar/cmds/ranking.py` & `cloudflare-radar-0.3/cloudflare_radar/cmds/ranking.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pycountry
 from xarg import add_command
 from xarg import argp
 from xarg import commands
 from xarg import run_command
 
-from ..utils import domain_database
+from ..utils import domain_dbstore
 from ..utils import domain_ranking
 
 DEF_RETRIES: int = 100
 MAX_RETRIES: int = 1000
 
 
 @add_command("update-rankings", help="Update the ranking of domain names")
@@ -30,27 +30,26 @@
 @run_command(add_cmd_update_rankings)
 def run_cmd_update_rankings(cmds: commands) -> int:
     dir: str = os.path.abspath(cmds.args.dir[0])
     latest_dir: str = os.path.join(dir, "latest")
     if not os.path.exists(latest_dir):
         os.makedirs(latest_dir)
     assert os.path.isdir(latest_dir), f"{latest_dir} not an existing directory"
-    database = domain_database(os.path.join(dir, "domains.csv"))
+    database = domain_dbstore(os.path.join(dir, "domains.csv"))
     cmds.logger.info(f"save rankings to directory: {dir}")
     retries: int = min(cmds.args.retries[0], MAX_RETRIES)
     queue: Queue[domain_ranking] = Queue()
-    queue.put(domain_ranking())
+    queue.put(domain_ranking(database=database))
     for country in pycountry.countries:
-        queue.put(domain_ranking(country))
+        queue.put(domain_ranking(location=country, database=database))
     entry: List[domain_ranking] = list()
     while not queue.empty():
         object = queue.get(block=False)
         if not object.download(latest_dir):
             if retries > 0:
                 queue.put(object)
                 retries -= 1
             continue
+        cmds.logger.debug({k: v for k, v in object.items()})
         entry.append(object)
     database.dump()
-    for item in entry:
-        cmds.logger.info({k: database.index(k) for k in item})
     return 0
```

### Comparing `cloudflare-radar-0.2/cloudflare_radar/utils/domains.py` & `cloudflare-radar-0.3/cloudflare_radar/utils/domains.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # coding:utf-8
 
 import csv
 import os
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Optional
 from typing import Union
 
-from xarg import commands
 from xarg import safile
 
 
 class domain_name(object):
     FIELDS: List[str] = ["number", "domain"]
 
     def __init__(self, number: Union[int, str], domain: str, **kwargs: Any):
@@ -31,56 +29,70 @@
     def dump(self) -> Dict[str, str]:
         values = [self.number, self.domain]
         return {k: v for k, v in zip(self.FIELDS, values)}
 
 
 class domain_database(dict[str, domain_name]):
 
-    def __init__(self, path: str):
+    def __init__(self):
         self.__updated: bool = False
-        self.__path: str = path
         self.__peak: int = 0
         super().__init__()
-        self.__load()
-
-    @property
-    def path(self) -> str:
-        return self.__path
 
     @property
     def peak(self) -> int:
         return self.__peak
 
-    def __add(self, object: domain_name):
+    @property
+    def updated(self) -> bool:
+        return self.__updated
+
+    @updated.setter
+    def updated(self, value: bool):
+        self.__updated = value
+
+    def add(self, object: domain_name):
         assert object.domain not in self, f"{object.domain} already exists"
         self.__peak = max(self.peak, object.number)
         self[object.domain] = object
 
+    def index(self, domain: str) -> int:
+        if domain not in self:
+            self.add(domain_name(number=self.peak + 1, domain=domain))
+            self.updated = True
+        assert domain in self, f"{domain} not exists"
+        return self[domain].number
+
+
+class domain_dbstore(domain_database):
+
+    def __init__(self, path: str):
+        self.__path: str = path
+        super().__init__()
+        self.__load()
+
     def __load(self):
         assert safile.restore(self.path), f"restore {self.path} failed"
         if not os.path.exists(self.path):
             return
         assert os.path.isfile(self.path), f"{self.path} not a regular file"
         with open(self.path) as rhdl:
             for line in csv.DictReader(rhdl):
-                self.__add(domain_name(**line))
+                self.add(domain_name(**line))
 
     def dump(self):
-        if not self.__updated:
+        if not self.updated:
             return
         assert safile.create_backup(self.path), \
             f"create {self.path} backup failed"
         with open(self.path, "w") as whdl:
             writer = csv.DictWriter(whdl, fieldnames=domain_name.FIELDS)
             writer.writeheader()
             for item in self.values():
                 writer.writerow(item.dump())
         assert safile.delete_backup(self.path), \
             f"delete {self.path} backup failed"
-        self.__updated = False
+        self.updated = False
 
-    def index(self, domain: str) -> int:
-        self.__updated = True
-        if domain not in self:
-            self.__add(domain_name(number=self.peak + 1, domain=domain))
-        assert domain in self, f"{domain} not exists"
-        return self[domain].number
+    @property
+    def path(self) -> str:
+        return self.__path
```

### Comparing `cloudflare-radar-0.2/cloudflare_radar/utils/ranking.py` & `cloudflare-radar-0.3/cloudflare_radar/utils/ranking.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,40 +3,53 @@
 import csv
 import os
 from typing import Optional
 
 from pycountry.db import Country
 from xarg import commands
 
+from .domains import domain_database
 from .request import download
 
 
-class domain_ranking(list):
+class domain_ranking(dict[str, int]):
     PREFIX = "http://radar.cloudflare.com/charts/TopDomainsTable"
 
-    def __init__(self, location: Optional[Country] = None):
+    def __init__(self, location: Optional[Country] = None,
+                 database: Optional[domain_database] = None):
+        if database is None:
+            database = domain_database()
         self.__location: Optional[Country] = location
+        self.__database: domain_database = database
         super().__init__()
 
     @property
     def location(self) -> str:
         return self.__location.name if self.__location else "Worldwide"
 
     @property
+    def database(self) -> domain_database:
+        return self.__database
+
+    @property
     def url(self) -> str:
         location: str = self.__location.alpha_2 if self.__location else ""
         return f"{self.PREFIX}/attachment?location={location.lower()}"
 
     def load(self, path: str) -> bool:
         if not os.path.isfile(path):
             return False
         self.clear()
         for line in sorted(csv.DictReader(open(path)),
                            key=lambda x: int(x["rank"])):
-            self.append(line["domain"])
+            domain: str = line["domain"]
+            assert domain not in self, f"{domain} already exists in {path}"
+            self[domain] = self.database.index(domain)
         return True
 
     def download(self, path: str) -> bool:
         filepath: Optional[str] = download(url=self.url, path=path)
-        status: str = "success" if isinstance(filepath, str) else "failed"
-        commands().logger.debug(f"download {self.url} {status}")
+        if isinstance(filepath, str):
+            commands().logger.info(f"download {self.url} success")
+        else:
+            commands().logger.warn(f"download {self.url} failed")
         return self.load(filepath) if isinstance(filepath, str) else False
```

### Comparing `cloudflare-radar-0.2/cloudflare_radar/utils/request.py` & `cloudflare-radar-0.3/cloudflare_radar/utils/request.py`

 * *Files identical despite different names*

### Comparing `cloudflare-radar-0.2/cloudflare_radar.egg-info/PKG-INFO` & `cloudflare-radar-0.3/cloudflare_radar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudflare-radar
-Version: 0.2
+Version: 0.3
 Summary: Get data from https://radar.cloudflare.com
 Home-page: https://github.com/DNSet/cloudflare-radar/
 Author: Mingzhe Zou
 Author-email: zoumingzhe@outlook.com
 License: GPLv2
 Project-URL: Source Code, https://github.com/DNSet/cloudflare-radar/
 Project-URL: Bug Tracker, https://github.com/DNSet/cloudflare-radar/issues
```

### Comparing `cloudflare-radar-0.2/cloudflare_radar.egg-info/SOURCES.txt` & `cloudflare-radar-0.3/cloudflare_radar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudflare-radar-0.2/setup.cfg` & `cloudflare-radar-0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudflare-radar-0.2/setup.py` & `cloudflare-radar-0.3/setup.py`

 * *Files identical despite different names*

