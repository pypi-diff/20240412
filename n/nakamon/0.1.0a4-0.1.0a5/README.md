# Comparing `tmp/nakamon-0.1.0a4.tar.gz` & `tmp/nakamon-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakamon-0.1.0a4.tar", max compression
+gzip compressed data, was "nakamon-0.1.0a5.tar", max compression
```

## Comparing `nakamon-0.1.0a4.tar` & `nakamon-0.1.0a5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a4/LICENSE
--rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a4/README.md
--rw-r--r--   0        0        0   445554 2024-04-08 04:27:44.869120 nakamon-0.1.0a4/data/nakamon_status.csv
--rw-r--r--   0        0        0    13822 2024-04-09 04:15:52.083469 nakamon-0.1.0a4/data/orange_skill.csv
--rw-r--r--   0        0        0     8449 2024-04-05 00:15:11.226076 nakamon-0.1.0a4/data/red_skill.csv
--rw-r--r--   0        0        0     4474 2024-04-09 04:11:06.526795 nakamon-0.1.0a4/data/resistance_skill.csv
--rw-r--r--   0        0        0     5578 2024-04-08 04:44:28.569145 nakamon-0.1.0a4/data/resistance_status.csv
--rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a4/nakamon/__init__.py
--rw-r--r--   0        0        0     7648 2024-04-10 05:58:17.894293 nakamon-0.1.0a4/nakamon/damage.py
--rw-r--r--   0        0        0     5372 2024-04-10 05:57:19.617626 nakamon-0.1.0a4/nakamon/nakamon.py
--rw-r--r--   0        0        0      404 2024-04-10 05:59:06.654293 nakamon-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a5/LICENSE
+-rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a5/README.md
+-rw-r--r--   0        0        0   445554 2024-04-08 04:27:44.869120 nakamon-0.1.0a5/data/nakamon_status.csv
+-rw-r--r--   0        0        0    13822 2024-04-09 04:15:52.083469 nakamon-0.1.0a5/data/orange_skill.csv
+-rw-r--r--   0        0        0     8449 2024-04-05 00:15:11.226076 nakamon-0.1.0a5/data/red_skill.csv
+-rw-r--r--   0        0        0     4474 2024-04-09 04:11:06.526795 nakamon-0.1.0a5/data/resistance_skill.csv
+-rw-r--r--   0        0        0     5578 2024-04-08 04:44:28.569145 nakamon-0.1.0a5/data/resistance_status.csv
+-rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a5/nakamon/__init__.py
+-rw-r--r--   0        0        0     7648 2024-04-10 05:58:17.894293 nakamon-0.1.0a5/nakamon/damage.py
+-rw-r--r--   0        0        0     5371 2024-04-11 03:24:50.237880 nakamon-0.1.0a5/nakamon/nakamon.py
+-rw-r--r--   0        0        0      404 2024-04-12 06:04:48.131713 nakamon-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a5/PKG-INFO
```

### Comparing `nakamon-0.1.0a4/LICENSE` & `nakamon-0.1.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/README.md` & `nakamon-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/data/nakamon_status.csv` & `nakamon-0.1.0a5/data/nakamon_status.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/data/orange_skill.csv` & `nakamon-0.1.0a5/data/orange_skill.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/data/red_skill.csv` & `nakamon-0.1.0a5/data/red_skill.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/data/resistance_skill.csv` & `nakamon-0.1.0a5/data/resistance_skill.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/data/resistance_status.csv` & `nakamon-0.1.0a5/data/resistance_status.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/nakamon/damage.py` & `nakamon-0.1.0a5/nakamon/damage.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a4/nakamon/nakamon.py` & `nakamon-0.1.0a5/nakamon/nakamon.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def add_red_skill(self, skill_name: str):
         status_change_map = {
             "さいだいHP": "HP",
             "さいだいMP": "MP",
             "こうげき力": "攻",
             "しゅび力": "守",
-            "こうげき魔力": "攻魔 ",
+            "こうげき魔力": "攻魔",
             "きようさ": "器用",
             "すばやさ": "素早",
         }
         skill_category = skill_name.split(":")[0]
         status_change = status_change_map.get(skill_category)
         if status_change:
             diff = red_skill.set_index("スキル").loc[skill_name, :].iloc[0]
```

### Comparing `nakamon-0.1.0a4/PKG-INFO` & `nakamon-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakamon
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: 
 Author: driller
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
```

