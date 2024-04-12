# Comparing `tmp/nonebot_plugin_dicky_pk-0.5.0.tar.gz` & `tmp/nonebot_plugin_dicky_pk-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_dicky_pk-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_dicky_pk-0.5.1.tar", max compression
```

## Comparing `nonebot_plugin_dicky_pk-0.5.0.tar` & `nonebot_plugin_dicky_pk-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1066 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/LICENSE
--rw-r--r--   0        0        0     3504 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/README.md
--rw-r--r--   0        0        0     6319 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/__init__.py
--rw-r--r--   0        0        0     7307 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/badge.py
--rw-r--r--   0        0        0     1190 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/badge_parser.py
--rw-r--r--   0        0        0     2226 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/cd.py
--rw-r--r--   0        0        0    10484 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config.json
--rw-r--r--   0        0        0     5502 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config.py
--rw-r--r--   0        0        0     1899 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config_parser.py
--rw-r--r--   0        0        0     1358 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/constants.py
--rw-r--r--   0        0        0    37395 2024-02-22 03:53:55.416486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/db.py
--rw-r--r--   0        0        0     6644 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/farm.py
--rw-r--r--   0        0        0    14281 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/friends.py
--rw-r--r--   0        0        0      423 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/impl.py
--rw-r--r--   0        0        0    38512 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/main.py
--rw-r--r--   0        0        0     2837 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/rebirth.py
--rw-r--r--   0        0        0     1368 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/rebirth_view.py
--rw-r--r--   0        0        0     4983 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/utils.py
--rw-r--r--   0        0        0      806 2024-02-22 03:53:55.420486 nonebot_plugin_dicky_pk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4406 1970-01-01 00:00:00.000000 nonebot_plugin_dicky_pk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3504 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/README.md
+-rw-r--r--   0        0        0     6384 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/__init__.py
+-rw-r--r--   0        0        0     7307 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/badge.py
+-rw-r--r--   0        0        0     1190 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/badge_parser.py
+-rw-r--r--   0        0        0     2226 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/cd.py
+-rw-r--r--   0        0        0    10484 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config.json
+-rw-r--r--   0        0        0     5502 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config.py
+-rw-r--r--   0        0        0     1899 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config_parser.py
+-rw-r--r--   0        0        0     1358 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/constants.py
+-rw-r--r--   0        0        0    37395 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/db.py
+-rw-r--r--   0        0        0     6644 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/farm.py
+-rw-r--r--   0        0        0    14281 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/friends.py
+-rw-r--r--   0        0        0      423 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/impl.py
+-rw-r--r--   0        0        0    38512 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/main.py
+-rw-r--r--   0        0        0     2837 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/rebirth.py
+-rw-r--r--   0        0        0     1368 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/rebirth_view.py
+-rw-r--r--   0        0        0     4983 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/utils.py
+-rw-r--r--   0        0        0      806 2024-04-12 10:01:56.904605 nonebot_plugin_dicky_pk-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4406 1970-01-01 00:00:00.000000 nonebot_plugin_dicky_pk-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_dicky_pk-0.5.0/LICENSE` & `nonebot_plugin_dicky_pk-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/README.md` & `nonebot_plugin_dicky_pk-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/__init__.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 """.strip()
 
 
 __plugin_meta__ = PluginMetadata(
     name="牛子PK",
     description="🥵",
     usage=usage,
-    type="application"
+    type="application",
+    homepage="https://github.com/tkgs0/nonebot-plugin-dicky-pk"
 )
 
 
 confpath = Path() / 'data' / 'chinchin_pk' / 'chinchin.json'
 confpath.parent.mkdir(parents=True, exist_ok=True)
 
 enablelist = (
```

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/badge.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/badge.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/badge_parser.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/badge_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/cd.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/cd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config.json` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/config_parser.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/config_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/constants.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/db.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/farm.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/farm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/friends.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/friends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/main.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/rebirth.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/rebirth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/rebirth_view.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/rebirth_view.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/nonebot_plugin_dicky_pk/src/utils.py` & `nonebot_plugin_dicky_pk-0.5.1/nonebot_plugin_dicky_pk/src/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_dicky_pk-0.5.0/pyproject.toml` & `nonebot_plugin_dicky_pk-0.5.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-dicky-pk"
-version = "0.5.0"
+version = "0.5.1"
 description = "Dicky-PK in NoneBot2"
 authors = ["月ヶ瀬"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "nonebot_plugin_dicky_pk" },
 ]
```

### Comparing `nonebot_plugin_dicky_pk-0.5.0/PKG-INFO` & `nonebot_plugin_dicky_pk-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-dicky-pk
-Version: 0.5.0
+Version: 0.5.1
 Summary: Dicky-PK in NoneBot2
 Home-page: https://github.com/tkgs0/nonebot-plugin-dicky-pk
 License: MIT
 Keywords: NoneBot,Dicky-PK
 Author: 月ヶ瀬
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-dicky-pk Version: 0.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-dicky-pk Version: 0.5.1 Summary:
 Dicky-PK in NoneBot2 Home-page: https://github.com/tkgs0/nonebot-plugin-dicky-
 pk License: MIT Keywords: NoneBot,Dicky-PK Author: æã¶ç¬ Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
```

