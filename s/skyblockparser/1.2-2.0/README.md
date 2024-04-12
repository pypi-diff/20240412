# Comparing `tmp/skyblockparser-1.2.tar.gz` & `tmp/skyblockparser-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyblockparser-1.2.tar", last modified: Fri Mar  8 12:22:51 2024, max compression
+gzip compressed data, was "skyblockparser-2.0.tar", last modified: Fri Apr 12 16:06:38 2024, max compression
```

## Comparing `skyblockparser-1.2.tar` & `skyblockparser-2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 12:22:51.074131 skyblockparser-1.2/
--rw-rw-rw-   0        0        0      294 2024-02-03 14:56:30.000000 skyblockparser-1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4720 2024-03-08 12:22:51.071607 skyblockparser-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4058 2024-03-08 12:21:45.000000 skyblockparser-1.2/README.md
--rw-rw-rw-   0        0        0      755 2024-03-08 12:21:49.000000 skyblockparser-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-08 12:22:51.074131 skyblockparser-1.2/setup.cfg
--rw-rw-rw-   0        0        0      905 2024-03-08 12:21:40.000000 skyblockparser-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 12:22:50.986078 skyblockparser-1.2/skyblockparser/
--rw-rw-rw-   0        0        0      173 2024-02-04 16:07:59.000000 skyblockparser-1.2/skyblockparser/__init__.py
--rw-rw-rw-   0        0        0     6444 2024-02-04 17:00:35.000000 skyblockparser-1.2/skyblockparser/auctionhouse.py
--rw-rw-rw-   0        0        0    38945 2024-02-03 14:32:32.000000 skyblockparser-1.2/skyblockparser/constants.py
--rw-rw-rw-   0        0        0       51 2024-02-03 12:14:09.000000 skyblockparser-1.2/skyblockparser/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-08 12:22:51.055337 skyblockparser-1.2/skyblockparser/fonts/
--rw-rw-rw-   0        0        0    12100 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/Minecraft-Italic.otf
--rw-rw-rw-   0        0        0    11164 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/MinecraftBold.otf
--rw-rw-rw-   0        0        0    11772 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/MinecraftBoldItalic.otf
--rw-rw-rw-   0        0        0    12100 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/MinecraftItalic.otf
--rw-rw-rw-   0        0        0    11016 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/MinecraftRegular.otf
--rw-rw-rw-   0        0        0 12273956 2023-08-07 11:08:34.000000 skyblockparser-1.2/skyblockparser/fonts/unifont.ttf
--rw-rw-rw-   0        0        0     6306 2024-03-06 16:04:27.000000 skyblockparser-1.2/skyblockparser/levels.py
--rw-rw-rw-   0        0        0     3307 2024-02-03 14:39:47.000000 skyblockparser-1.2/skyblockparser/pets.py
--rw-rw-rw-   0        0        0    14668 2024-03-08 12:22:07.000000 skyblockparser-1.2/skyblockparser/profile.py
--rw-rw-rw-   0        0        0     9675 2024-02-03 14:14:10.000000 skyblockparser-1.2/skyblockparser/renderer.py
-drwxrwxrwx   0        0        0        0 2024-03-08 12:22:51.071607 skyblockparser-1.2/skyblockparser.egg-info/
--rw-rw-rw-   0        0        0     4720 2024-03-08 12:22:50.000000 skyblockparser-1.2/skyblockparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-03-08 12:22:50.000000 skyblockparser-1.2/skyblockparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 12:22:50.000000 skyblockparser-1.2/skyblockparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-08 12:22:50.000000 skyblockparser-1.2/skyblockparser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-08 12:22:50.000000 skyblockparser-1.2/skyblockparser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 16:06:38.596283 skyblockparser-2.0/
+-rw-rw-rw-   0        0        0      294 2024-02-03 14:56:30.000000 skyblockparser-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4720 2024-04-12 16:06:38.595287 skyblockparser-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4058 2024-04-12 16:06:12.000000 skyblockparser-2.0/README.md
+-rw-rw-rw-   0        0        0      755 2024-04-12 16:05:54.000000 skyblockparser-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 16:06:38.596283 skyblockparser-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      905 2024-04-12 16:05:47.000000 skyblockparser-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:06:38.530302 skyblockparser-2.0/skyblockparser/
+-rw-rw-rw-   0        0        0      173 2024-02-04 16:07:59.000000 skyblockparser-2.0/skyblockparser/__init__.py
+-rw-rw-rw-   0        0        0     6444 2024-03-22 15:02:54.000000 skyblockparser-2.0/skyblockparser/auctionhouse.py
+-rw-rw-rw-   0        0        0    38945 2024-03-22 15:02:54.000000 skyblockparser-2.0/skyblockparser/constants.py
+-rw-rw-rw-   0        0        0       51 2024-03-22 15:02:54.000000 skyblockparser-2.0/skyblockparser/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:06:38.582812 skyblockparser-2.0/skyblockparser/fonts/
+-rw-rw-rw-   0        0        0    12100 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/Minecraft-Italic.otf
+-rw-rw-rw-   0        0        0    11164 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/MinecraftBold.otf
+-rw-rw-rw-   0        0        0    11772 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/MinecraftBoldItalic.otf
+-rw-rw-rw-   0        0        0    12100 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/MinecraftItalic.otf
+-rw-rw-rw-   0        0        0    11016 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/MinecraftRegular.otf
+-rw-rw-rw-   0        0        0 12273956 2023-08-07 11:08:34.000000 skyblockparser-2.0/skyblockparser/fonts/unifont.ttf
+-rw-rw-rw-   0        0        0     6442 2024-04-12 16:01:39.000000 skyblockparser-2.0/skyblockparser/levels.py
+-rw-rw-rw-   0        0        0     3069 2024-04-06 00:05:48.000000 skyblockparser-2.0/skyblockparser/pets.py
+-rw-rw-rw-   0        0        0    18786 2024-04-12 12:18:17.000000 skyblockparser-2.0/skyblockparser/profile.py
+-rw-rw-rw-   0        0        0     9675 2024-03-22 15:02:54.000000 skyblockparser-2.0/skyblockparser/renderer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 16:06:38.594288 skyblockparser-2.0/skyblockparser.egg-info/
+-rw-rw-rw-   0        0        0     4720 2024-04-12 16:06:38.000000 skyblockparser-2.0/skyblockparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-04-12 16:06:38.000000 skyblockparser-2.0/skyblockparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 16:06:38.000000 skyblockparser-2.0/skyblockparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 16:06:38.000000 skyblockparser-2.0/skyblockparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 16:06:38.000000 skyblockparser-2.0/skyblockparser.egg-info/top_level.txt
```

### Comparing `skyblockparser-1.2/PKG-INFO` & `skyblockparser-2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: skyblockparser
-Version: 1.2
+Version: 2.0
 Summary: A package allowing you to parse skyblock profile information including networth.
 Author: nom
 Author-email: nom <noemtdev@gmail.com>
 Project-URL: Homepage, https://github.com/noemtdev/skyblockparser
 Project-URL: Bug Tracker, https://github.com/noemtdev/skyblockparser/issues
 Keywords: python,hypixel,skyblock,hypixel skyblock
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: pillow
 
-# skyblockparser v1.2
+# skyblockparser v2.0
 ## This requires a [Hypixel API Key](https://developer.hypixel.net)
 
 ## Installation
 Python 3.7 or higher is required.
 
 Run `pip install skyblockparser`.
```

### Comparing `skyblockparser-1.2/README.md` & `skyblockparser-2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# skyblockparser v1.2
+# skyblockparser v2.0
 ## This requires a [Hypixel API Key](https://developer.hypixel.net)
 
 ## Installation
 Python 3.7 or higher is required.
 
 Run `pip install skyblockparser`.
```

### Comparing `skyblockparser-1.2/pyproject.toml` & `skyblockparser-2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skyblockparser"
-version = "1.2"
+version = "2.0"
 authors = [
   { name="nom", email="noemtdev@gmail.com" },
 ]
 description = "A package allowing you to parse skyblock profile information including networth."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `skyblockparser-1.2/setup.py` & `skyblockparser-2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.2'
+VERSION = '2.0'
 DESCRIPTION = 'A package allowing you to parse skyblock profile information including networth.'
 
 # Setting up
 setup(
     name="skyblockparser",
     version=VERSION,
     author="nom",
```

### Comparing `skyblockparser-1.2/skyblockparser/auctionhouse.py` & `skyblockparser-2.0/skyblockparser/auctionhouse.py`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/constants.py` & `skyblockparser-2.0/skyblockparser/constants.py`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/Minecraft-Italic.otf` & `skyblockparser-2.0/skyblockparser/fonts/Minecraft-Italic.otf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/MinecraftBold.otf` & `skyblockparser-2.0/skyblockparser/fonts/MinecraftBold.otf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/MinecraftBoldItalic.otf` & `skyblockparser-2.0/skyblockparser/fonts/MinecraftBoldItalic.otf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/MinecraftItalic.otf` & `skyblockparser-2.0/skyblockparser/fonts/MinecraftItalic.otf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/MinecraftRegular.otf` & `skyblockparser-2.0/skyblockparser/fonts/MinecraftRegular.otf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/fonts/unifont.ttf` & `skyblockparser-2.0/skyblockparser/fonts/unifont.ttf`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser/levels.py` & `skyblockparser-2.0/skyblockparser/levels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,44 @@
-def get_cata_lvl(exp):
-    levels = {
+cata_levels = {
         '1': 50, '2': 125, '3': 235, '4': 395, '5': 625, '6': 955, '7': 1425, '8': 2095, '9': 3045,
         '10': 4385, '11': 6275, '12': 8940, '13': 12700, '14': 17960, '15': 25340, '16': 35640,
         '17': 50040, '18': 70040, '19': 97640, '20': 135640, '21': 188140, '22': 259640, '23': 356640,
         '24': 488640, '25': 668640, '26': 911640, '27': 1239640, '28': 1684640, '29': 2284640,
         '30': 3084640, '31': 4149640, '32': 5559640, '33': 7459640, '34': 9959640, '35': 13259640,
         '36': 17559640, '37': 23159640, '38': 30359640, '39': 39559640, '40': 51559640, '41': 66559640,
         '42': 85559640, '43': 109559640, '44': 139559640, '45': 177559640, '46': 225559640,
         '47': 285559640, '48': 360559640, '49': 453559640, '50': 569809640
-    }
-    for level in levels:
-        if exp >= levels["50"]:
-            return 50
-        if levels[level] > exp:
+}
+
+revenant = {"0": 0, "1": 5, "2": 15, "3": 200, "4": 1000,
+            "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
+spider = {"0": 0, "1": 5, "2": 15, "3": 200, "4": 1000,
+            "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
+sven = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500, "5": 5000,
+        "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
+enderman = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500,
+            "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
+blaze = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500,
+            "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
+vampire = {"0": 0, "1": 20, "2": 75, "3": 240, "4": 840, "5": 2400}
+
+def get_cata_lvl(exp):
+    
+    for level in cata_levels:
+        if exp >= cata_levels["50"]:
+            xp_above_50 = exp - cata_levels["50"]
+            levels = xp_above_50 / 200000000
+            return 50 + levels
+
+
+        if cata_levels[level] > exp:
             if int(level) == 1:
                 level = str(2)
-            lowexp = levels[str(int(level) - 1)]
-            highexp = levels[level]
+            lowexp = cata_levels[str(int(level) - 1)]
+            highexp = cata_levels[level]
             difference = highexp - lowexp
             extra = exp - lowexp
             percentage = (extra / difference)
             return (int(level) - 1) + percentage
 
 
 SKILL_MAX_LEVELS = {
@@ -68,38 +86,26 @@
         "maxLevel": 50,
     }
 }
 
 
 def get_hotm_level(exp):
     levels = {
-        "1": 0, "2": 3000, "3": 12000, "4": 37000, "5": 97000, "6": 197000, "7": 347000
+        "1": 0, "2": 3000, "3": 12000, "4": 37000, "5": 97000, "6": 197000, "7": 347000, "8": 557000, "9": 847000, "10": 1247000
     }
     for level in levels:
-        if exp >= levels["7"]:
-            return 7
+        if exp >= levels["10"]:
+            return 10
         
         if levels[level] > exp:
-            level = int(level) - 1
+            return int(level) - 1
         
-        return level
-
+    return 10
 
 def get_slayer_level(slayer_type, exp):
-    revenant = {"0": 0, "1": 5, "2": 15, "3": 200, "4": 1000,
-                "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
-    spider = {"0": 0, "1": 5, "2": 15, "3": 200, "4": 1000,
-              "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
-    sven = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500, "5": 5000,
-            "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
-    enderman = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500,
-                "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
-    blaze = {"0": 0, "1": 10, "2": 30, "3": 250, "4": 1500,
-             "5": 5000, "6": 20000, "7": 100000, "8": 400000, "9": 1000000}
-    vampire = {"0": 0, "1": 20, "2": 75, "3": 240, "4": 840, "5": 2400}
 
     if slayer_type == "zombie":
         levels = revenant
     elif slayer_type == "spider":
         levels = spider
     elif slayer_type == "wolf":
         levels = sven
```

### Comparing `skyblockparser-1.2/skyblockparser/pets.py` & `skyblockparser-2.0/skyblockparser/pets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from .constants import *
 from .exceptions import SkyblockParserException
 from .renderer import render
-import json
 
 def format_stat(stat):
     formatted_stat = "{:.2f}".format(stat).rstrip('0').rstrip('.')
     if stat > 0:
         return f"§a+{formatted_stat}"
     else:
         return f"§a{formatted_stat}"
@@ -23,46 +22,40 @@
     def __init__(self, data, menu:bool=True):
 
         self.lore = []
         self.uuid = None
         self.active = False
 
         if not menu:
-
-            extra_attributes = data.get("ExtraAttributes", {})
-            self.uuid = extra_attributes.get("uuid", "")
-            self.active = False
-
             
             item_name = data.get("display", {}).get("Name", "")
             item_lore = data.get("display", {}).get("Lore", [])
 
             lore = [item_name, *item_lore]
             for line in lore:
                 if "§r §e" in line:
                     line = line.split(" §r ")[1]
                 line = line.replace("§", "&")
                 self.lore.append(line)
 
-            data = json.loads(extra_attributes.get("petInfo", "{}"))
-            
 
         if self.uuid is None:
             self.uuid = data.get("uuid", "")
 
         self.type = data.get("type", "")
         self.exp = data.get("exp", 0)
 
         if self.active is None:
             self.active = data.get("active", False)
 
         self.tier = data.get("tier", 0)
         self.rarity_color = rarity_colors.get(self.tier, "")
+
         if self.rarity_color == "":
-            raise SkyblockParserException("Unknown rarity")
+            raise SkyblockParserException(f"Unknown rarity, '{self.tier}'")
 
 
         self.held_item = data.get("heldItem", "")
 
         if self.held_item in rarity_upgrading_pet_items:
             if self.type not in ignores_tierboost:
                 current_tier = pet_tiers.index(self.tier)
```

### Comparing `skyblockparser-1.2/skyblockparser/profile.py` & `skyblockparser-2.0/skyblockparser/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -171,45 +171,127 @@
         else:
             for profile in profile_data["profiles"]:
                 if profile["selected"] is True:
                     _profile = profile
                     self.cute_name = profile["cute_name"]
                     break
 
+        self._profile = _profile
+
+        self.coops:list[str] = [member for member in _profile["members"]]
+        self.coop_names:list[str] = []
+
+        self.selected = _profile["selected"]
 
         banking = _profile.get("banking", {})
         self.bank_balance = banking.get("balance", 0)
         self.profile_data_raw = _profile
         self.profile_id = _profile["profile_id"]
         self.profile_type = _profile.get("game_mode", "normal")
 
         if uuid in _profile["members"]:
             self.profile_data_user = _profile["members"][uuid]
 
         else:
             raise SkyblockParserException("User not in Profile")
+        
+        try:
+            self.created_at = _profile["created_at"]
+        except:
+            self.created_at = self.profile_data_user["profile"]["first_join"]
 
         leveling = self.profile_data_user.get("leveling", {})
         self.skyblock_level = leveling.get("experience", 0) / 100
 
         self.collections = self.profile_data_user.get("collection", {})
         self.bestiary = self.profile_data_user.get("bestiary", {})
         self.quests = self.profile_data_user.get("quests", {})
         self.nether = self.profile_data_user.get("nether_island_player_data", {})
 
+        self.rift:dict = self.profile_data_user.get("rift", {})
+        self.rift.pop("inventory", None)
 
-    def get_items(self):
+        self.currencies = self.profile_data_user.get("currencies", {})
+        self.player_data = self.profile_data_user.get("player_data", {})
+        self.get_pets()
+
+    async def get_json(self):
+        await self.get_coop_names()
+        await self.init()
+        await self.get_networth()
+
+        data = {
+            "profile_id": self.profile_id,
+            "uuid": self.uuid,
+            "cute_name": self.cute_name,
+            "profile_type": self.profile_type,
+            "bank_balance": self.bank_balance,
+            "created_at": self.created_at,
+            "skyblock_level": self.skyblock_level,
+            "collections": self.collections,
+            "bestiary": self.bestiary,
+            "nether": self.nether,
+            "currencies": self.currencies,
+            "networth": self.networth_data,
+            "dungeons": self.dungeon_data,
+            "slayers": self.slayer_data,
+            "skills": self.skill_data,
+            "mining": self.mining_data,
+            "general": self.general_stats,
+            "farming": self.farming_data,
+            "coop_names": self.coop_names,
+            "coop_count": len(self.coops),
+            "rift": self.rift,
+        }
+
+
+        return data
+
+    async def get_coop_names(self):
+        if self.coop_names != []:
+            return
+        
+        names = []
+        async with aiohttp.ClientSession() as session:
+            for member in self.coops:
+                user_data = self._profile["members"].get(member, {})
+                profile = user_data.get("profile", {})
+                deletion_notice = profile.get("deletion_notice", None)
+                wavy = ""
+                if deletion_notice:
+                    wavy = "~~"
+                    
+                async with session.get(f"https://sessionserver.mojang.com/session/minecraft/profile/{member}") as response:
+                    data = await response.json()
+                    username = data.get("name")
+                    if username:
+                        names.append(f"**{wavy}{username}{wavy}**")
+                    else:
+                        names.append("**-**")
+
+        self.coop_names = names
+
+
+    def get_pets(self):
         self.pets = []
-        pet_data = self.profile_data_user.get("pets_data", [])
+        pet_data = self.profile_data_user.get("pets_data", {})
         for pet in pet_data.get("pets", []):
-            self.pets.append(Pet(pet))
+            try:
+                self.pets.append(Pet(pet, False))
+            except SkyblockParserException:
+                continue
 
         if self.profile_data_user.get("rift", {}).get("dead_cats", {}).get("montezuma"):
-            self.pets.append(
-                Pet(self.profile_data_user["rift"]["dead_cats"]["montezuma"]))
+            try:
+                self.pets.append(
+                    Pet(self.profile_data_user["rift"]["dead_cats"]["montezuma"], False))
+            except SkyblockParserException:
+                pass
+
+    def get_items(self):
 
         inventory = self.profile_data_user.get("inventory", {})
         self.sacks = inventory.get("sacks_counts", {})
 
         to_decode = [
             "inv",
             "ender_chest",
@@ -237,25 +319,29 @@
 
         bags = inventory.get("bag_contents", {})
         for bag in bags:	
             data = bags[bag].get("data", "")
             self.decode_items(data, bag)
 
     async def init(self):
+        if self.museum_data != {}:
+            return
+        
         await self.get_museum()
         await self.get_stats()
 
     async def get_stats(self):
         await asyncio.gather(
             self.get_dungeon_stats(),
             self.get_slayer_stats(),
             self.get_skill_stats(),
             self.get_mining_stats(),
             self.get_general_stats(),
-            self.get_networth()
+            self.get_networth(),
+            self.get_farming()
         )
 
     def decode_items(self, nbt, _type):
         if nbt:
             items = decode_item(nbt)[""]["i"]
             for item in items:
                 if item.get("tag", {}).get("ExtraAttributes", {}).get("id", "") == "PET":
@@ -353,39 +439,44 @@
             }
 
         self.skill_data = skill_data
         return
     
     async def get_mining_stats(self):
         mining_data = self.profile_data_user.get("mining_core", {})
+        nodes = mining_data.get("nodes", {})
         hotm_experience = mining_data.get("experience", 0)
         hotm_level = get_hotm_level(hotm_experience)
 
         powder = {
             "gemstone": {
                 "available": mining_data.get("powder_gemstone", 0),
                 "total": mining_data.get("powder_gemstone", 0) + mining_data.get("powder_spent_gemstone", 0)
-
             },
             "mithril": {
                 "available": mining_data.get("powder_mithril", 0),
                 "total": mining_data.get("powder_mithril_total", 0) + mining_data.get("powder_spent_mithril", 0)
+            },
+            "glacite": {
+                "available": mining_data.get("powder_glacite", 0),
+                "total": mining_data.get("powder_glacite_total", 0) + mining_data.get("powder_spent_glacite", 0)
             }
         }
 
         self.mining_data = {
             "forge": self.profile_data_user.get("forge", {}),
             "hotm": {
                 "experience": hotm_experience,
                 "level": hotm_level,
                 "tokens": mining_data.get("tokens_spent", 0) + mining_data.get("tokens", 0),
                 "tokens_spent": mining_data.get("tokens_spent", 0),
                 "selected_ability": mining_data.get("selected_pickaxe_ability", ""),
                 "powder": powder,
-                "crystals": mining_data.get("crystals", {})
+                "crystals": mining_data.get("crystals", {}),
+                "nodes": nodes
             }
         }
 
         return
     
     async def get_general_stats(self):
         player_stats = self.profile_data_user.get("player_stats", {})
@@ -437,14 +528,36 @@
             "spooky_festival": spooky,
             "damages": damages,
             "fishing": fishing,
             "fairy_souls": faily_souls
         }
 
         return
+    
+    async def get_farming(self):
+        jacobs_contests = self.profile_data_user.get("jacobs_contest", {})
+        unique_brackets = jacobs_contests.get("unique_brackets", {})
+        perks = jacobs_contests.get("perks", {})
+        medals_inv = jacobs_contests.get("medals_inv", {})
+        contests = jacobs_contests.get("contests", {})
+
+        quests = self.profile_data_user.get("quests", {})
+        trapper = quests.get("trapper_quest", {})
+        pelt_count = trapper.get("pelt_count", 0)
+
+
+        farming_data = {
+            "perks": perks,
+            "unique_brackets": unique_brackets,
+            "medals": medals_inv,
+            "contests": contests,
+            "pelts": pelt_count
+        }
+
+        self.farming_data = farming_data
 
 class SkyblockParser:
     """
     Use raw Hypixel API Data
     """
 
     def __init__(self, data, uuid, api_key):
```

### Comparing `skyblockparser-1.2/skyblockparser/renderer.py` & `skyblockparser-2.0/skyblockparser/renderer.py`

 * *Files identical despite different names*

### Comparing `skyblockparser-1.2/skyblockparser.egg-info/PKG-INFO` & `skyblockparser-2.0/skyblockparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: skyblockparser
-Version: 1.2
+Version: 2.0
 Summary: A package allowing you to parse skyblock profile information including networth.
 Author: nom
 Author-email: nom <noemtdev@gmail.com>
 Project-URL: Homepage, https://github.com/noemtdev/skyblockparser
 Project-URL: Bug Tracker, https://github.com/noemtdev/skyblockparser/issues
 Keywords: python,hypixel,skyblock,hypixel skyblock
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: pillow
 
-# skyblockparser v1.2
+# skyblockparser v2.0
 ## This requires a [Hypixel API Key](https://developer.hypixel.net)
 
 ## Installation
 Python 3.7 or higher is required.
 
 Run `pip install skyblockparser`.
```

### Comparing `skyblockparser-1.2/skyblockparser.egg-info/SOURCES.txt` & `skyblockparser-2.0/skyblockparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

