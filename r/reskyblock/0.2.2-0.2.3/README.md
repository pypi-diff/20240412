# Comparing `tmp/reskyblock-0.2.2.tar.gz` & `tmp/reskyblock-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reskyblock-0.2.2.tar", last modified: Sat Feb 24 05:17:54 2024, max compression
+gzip compressed data, was "reskyblock-0.2.3.tar", last modified: Fri Apr 12 01:58:45 2024, max compression
```

## Comparing `reskyblock-0.2.2.tar` & `reskyblock-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       13 2024-02-24 05:17:31.879412 reskyblock-0.2.2/README.md
--rw-r--r--   0        0        0     2689 2024-02-24 05:17:54.015764 reskyblock-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      282 2024-02-24 05:17:31.879412 reskyblock-0.2.2/src/reskyblock/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 05:17:31.879412 reskyblock-0.2.2/src/reskyblock/__main__.py
--rw-r--r--   0        0        0     4458 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/client.py
--rw-r--r--   0        0        0      212 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/http/__init__.py
--rw-r--r--   0        0        0     2129 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/http/http_adapter.py
--rw-r--r--   0        0        0      331 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/models/__init__.py
--rw-r--r--   0        0        0     1259 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/models/auctions.py
--rw-r--r--   0        0        0      625 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/models/auctions_ended.py
--rw-r--r--   0        0        0      716 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/models/bazaar.py
--rw-r--r--   0        0        0       73 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/nbt/__init__.py
--rw-r--r--   0        0        0     2520 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/nbt/decoder.py
--rw-r--r--   0        0        0        0 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/py.typed
--rw-r--r--   0        0        0      131 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/serialization/__init__.py
--rw-r--r--   0        0        0      992 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/serialization/json.py
--rw-r--r--   0        0        0      574 2024-02-24 05:17:31.883412 reskyblock-0.2.2/src/reskyblock/urls.py
--rw-r--r--   0        0        0        0 2024-02-24 05:17:31.883412 reskyblock-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0  2018239 2024-02-24 05:17:31.891412 reskyblock-0.2.2/tests/data/auctions.json
--rw-r--r--   0        0        0  2039142 2024-02-24 05:17:31.903412 reskyblock-0.2.2/tests/data/auctions2.json
--rw-r--r--   0        0        0   315276 2024-02-24 05:17:31.907412 reskyblock-0.2.2/tests/data/auctions_ended.json
--rw-r--r--   0        0        0  2264250 2024-02-24 05:17:31.911412 reskyblock-0.2.2/tests/data/bazaar.json
--rw-r--r--   0        0        0    89195 2024-02-24 05:17:31.915412 reskyblock-0.2.2/tests/data/item_bytes.txt
--rw-r--r--   0        0        0     3204 2024-02-24 05:17:31.915412 reskyblock-0.2.2/tests/test_client.py
--rw-r--r--   0        0        0      692 2024-02-24 05:17:31.915412 reskyblock-0.2.2/tests/test_httpx_client.py
--rw-r--r--   0        0        0     6279 2024-02-24 05:17:31.915412 reskyblock-0.2.2/tests/test_nbt.py
--rw-r--r--   0        0        0      819 2024-02-24 05:17:31.915412 reskyblock-0.2.2/tests/test_urls.py
--rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-12 01:58:24.860889 reskyblock-0.2.3/README.md
+-rw-r--r--   0        0        0     2689 2024-04-12 01:58:45.760933 reskyblock-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      282 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/__main__.py
+-rw-r--r--   0        0        0     4458 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/client.py
+-rw-r--r--   0        0        0      212 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/http/__init__.py
+-rw-r--r--   0        0        0     2129 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/http/http_adapter.py
+-rw-r--r--   0        0        0      331 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/__init__.py
+-rw-r--r--   0        0        0     1259 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/auctions.py
+-rw-r--r--   0        0        0      625 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/auctions_ended.py
+-rw-r--r--   0        0        0      716 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/models/bazaar.py
+-rw-r--r--   0        0        0       73 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/nbt/__init__.py
+-rw-r--r--   0        0        0     2541 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/nbt/decoder.py
+-rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/py.typed
+-rw-r--r--   0        0        0      131 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/serialization/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/serialization/json.py
+-rw-r--r--   0        0        0      574 2024-04-12 01:58:24.860889 reskyblock-0.2.3/src/reskyblock/urls.py
+-rw-r--r--   0        0        0        0 2024-04-12 01:58:24.860889 reskyblock-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0  2018239 2024-04-12 01:58:24.872889 reskyblock-0.2.3/tests/data/auctions.json
+-rw-r--r--   0        0        0  2039142 2024-04-12 01:58:24.884889 reskyblock-0.2.3/tests/data/auctions2.json
+-rw-r--r--   0        0        0   315276 2024-04-12 01:58:24.884889 reskyblock-0.2.3/tests/data/auctions_ended.json
+-rw-r--r--   0        0        0  2264250 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/data/bazaar.json
+-rw-r--r--   0        0        0    89195 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/data/item_bytes.txt
+-rw-r--r--   0        0        0     3204 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_client.py
+-rw-r--r--   0        0        0      692 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_httpx_client.py
+-rw-r--r--   0        0        0     6279 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_nbt.py
+-rw-r--r--   0        0        0      819 2024-04-12 01:58:24.892889 reskyblock-0.2.3/tests/test_urls.py
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 reskyblock-0.2.3/PKG-INFO
```

### Comparing `reskyblock-0.2.2/pyproject.toml` & `reskyblock-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "reskyblock"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python API wrapper for Hypixel SkyBlock"
 authors = [
     { name = "ch-iv", email = "alicesummer38@gmail.com" },
 ]
 dependencies = [
     "pyright>=1.1.350",
     "httpx>=0.26.0",
```

### Comparing `reskyblock-0.2.2/src/reskyblock/client.py` & `reskyblock-0.2.3/src/reskyblock/client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/http/http_adapter.py` & `reskyblock-0.2.3/src/reskyblock/http/http_adapter.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/models/auctions.py` & `reskyblock-0.2.3/src/reskyblock/models/auctions.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/models/auctions_ended.py` & `reskyblock-0.2.3/src/reskyblock/models/auctions_ended.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/models/bazaar.py` & `reskyblock-0.2.3/src/reskyblock/models/bazaar.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/nbt/decoder.py` & `reskyblock-0.2.3/src/reskyblock/nbt/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     raw_data: str
     is_pet: bool = False
     skyblock_id: str = ""
     reforge: str | None = None
     dungeon_stars: int = 0
     hot_potato_count: int = 0
     rarity_upgrades: int = 0
-    enchantments: list[str] = []
     art_of_war_count: int = 0
-    gems: list[str] = []
-    scrolls: list[str] = []
+    gems: list[str] | None = []
+    scrolls: list[str] | None = []
+    enchantments: list[str] | None = []
 
     def __post_init__(self) -> None:
         nbt_data = _decode_nbt(self.raw_data)
         ea = nbt_data["tag"]["ExtraAttributes"]
 
         self.skyblock_id = str(ea["id"]).replace("STARRED_", "")
```

### Comparing `reskyblock-0.2.2/src/reskyblock/serialization/json.py` & `reskyblock-0.2.3/src/reskyblock/serialization/json.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/src/reskyblock/urls.py` & `reskyblock-0.2.3/src/reskyblock/urls.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/data/auctions.json` & `reskyblock-0.2.3/tests/data/auctions.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/data/auctions2.json` & `reskyblock-0.2.3/tests/data/auctions2.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/data/auctions_ended.json` & `reskyblock-0.2.3/tests/data/auctions_ended.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/data/bazaar.json` & `reskyblock-0.2.3/tests/data/bazaar.json`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/data/item_bytes.txt` & `reskyblock-0.2.3/tests/data/item_bytes.txt`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/test_client.py` & `reskyblock-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/test_httpx_client.py` & `reskyblock-0.2.3/tests/test_httpx_client.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/test_nbt.py` & `reskyblock-0.2.3/tests/test_nbt.py`

 * *Files identical despite different names*

### Comparing `reskyblock-0.2.2/tests/test_urls.py` & `reskyblock-0.2.3/tests/test_urls.py`

 * *Files identical despite different names*

