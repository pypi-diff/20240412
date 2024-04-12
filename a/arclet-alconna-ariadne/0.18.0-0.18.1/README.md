# Comparing `tmp/arclet_alconna_ariadne-0.18.0.tar.gz` & `tmp/arclet_alconna_ariadne-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna_ariadne-0.18.0.tar", last modified: Thu Feb 29 14:15:34 2024, max compression
+gzip compressed data, was "arclet_alconna_ariadne-0.18.1.tar", last modified: Fri Apr 12 13:02:35 2024, max compression
```

## Comparing `arclet_alconna_ariadne-0.18.0.tar` & `arclet_alconna_ariadne-0.18.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      953 2024-02-29 12:52:01.562442 arclet_alconna_ariadne-0.18.0/.mina/ariadne.toml
--rw-r--r--   0        0        0    35184 2024-02-29 12:41:23.690545 arclet_alconna_ariadne-0.18.0/LICENSE
--rw-r--r--   0        0        0     7388 2024-02-29 12:41:23.691520 arclet_alconna_ariadne-0.18.0/README.md
--rw-r--r--   0        0        0     1546 2024-02-29 14:15:34.076577 arclet_alconna_ariadne-0.18.0/pyproject.toml
--rw-r--r--   0        0        0      147 2024-02-29 12:41:23.692494 arclet_alconna_ariadne-0.18.0/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     6092 2024-02-29 12:41:23.692494 arclet_alconna_ariadne-0.18.0/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1299 2024-02-29 13:23:49.808889 arclet_alconna_ariadne-0.18.0/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7974 1970-01-01 00:00:00.000000 arclet_alconna_ariadne-0.18.0/PKG-INFO
+-rw-r--r--   0        0        0      953 2024-04-12 13:00:38.675105 arclet_alconna_ariadne-0.18.1/.mina/ariadne.toml
+-rw-r--r--   0        0        0    35184 2024-02-29 12:41:23.690545 arclet_alconna_ariadne-0.18.1/LICENSE
+-rw-r--r--   0        0        0     7388 2024-02-29 12:41:23.691520 arclet_alconna_ariadne-0.18.1/README.md
+-rw-r--r--   0        0        0     1516 2024-04-12 13:02:35.124098 arclet_alconna_ariadne-0.18.1/pyproject.toml
+-rw-r--r--   0        0        0      147 2024-02-29 12:41:23.692494 arclet_alconna_ariadne-0.18.1/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     6092 2024-02-29 12:41:23.692494 arclet_alconna_ariadne-0.18.1/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1299 2024-02-29 13:23:49.808889 arclet_alconna_ariadne-0.18.1/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7974 1970-01-01 00:00:00.000000 arclet_alconna_ariadne-0.18.1/PKG-INFO
```

### Comparing `arclet_alconna_ariadne-0.18.0/.mina/ariadne.toml` & `arclet_alconna_ariadne-0.18.1/.mina/ariadne.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 includes = ["src/arclet/alconna/ariadne"]
 raw-dependencies = [
-    "arclet-alconna-graia<0.18.0, >= 0.18.0",
+    "arclet-alconna-graia<0.19.0, >= 0.18.1",
     "graia-ariadne<1.0.0, >=0.11.0",
 ]
 
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.18.0"
+version = "0.18.1"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"}
 ]
 dependencies = [
 
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
```

### Comparing `arclet_alconna_ariadne-0.18.0/LICENSE` & `arclet_alconna_ariadne-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.18.0/README.md` & `arclet_alconna_ariadne-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.18.0/pyproject.toml` & `arclet_alconna_ariadne-0.18.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.18.0"
+version = "0.18.1"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "arclet-alconna-graia<0.18.0, >= 0.18.0",
+    "arclet-alconna-graia<0.19.0, >= 0.18.1",
     "graia-ariadne<1.0.0, >=0.11.0",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
     "alconna",
@@ -56,16 +56,16 @@
     "editables>=0.3.0",
     "fix-future-annotations>=0.5.0",
     "avilla-console>=0.2.0",
     "avilla-qqapi>=1.0.0a20",
 ]
 
 [tool.pdm.scripts]
-buildall = "pdm mina build --all --no-isolation"
-pub = "pdm publish --no-build --no-isolation"
+buildall = "pdm mina build --all"
+pub = "pdm publish --no-build"
 
 [tool.pdm.scripts.puball]
 composite = [
     "buildall",
     "pub",
 ]
```

### Comparing `arclet_alconna_ariadne-0.18.0/src/arclet/alconna/ariadne/adapter.py` & `arclet_alconna_ariadne-0.18.1/src/arclet/alconna/ariadne/adapter.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.18.0/src/arclet/alconna/ariadne/typings.py` & `arclet_alconna_ariadne-0.18.1/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.18.0/PKG-INFO` & `arclet_alconna_ariadne-0.18.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.18.0
+Version: 0.18.1
 Summary: Support Alconna to GraiaProject/Ariadne
 Keywords: alconna graia arclet
 Home-page: https://github.com/ArcletProject/Alconna-Graia
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Project-URL: Homepage, https://github.com/ArcletProject/Alconna-Graia
 Project-URL: Repository, https://github.com/ArcletProject/Alconna-Graia
 Requires-Python: >=3.8
-Requires-Dist: arclet-alconna-graia<0.18.0,>=0.18.0
+Requires-Dist: arclet-alconna-graia<0.19.0,>=0.18.1
 Requires-Dist: graia-ariadne<1.0.0,>=0.11.0
 Description-Content-Type: text/markdown
 
 # Alconna Graia
 
 该项目为 [`Alconna`](https://github.com/ArcletProject/Alconna) 为 [`GraiaProject`](https://github.com/GraiaProject) 下项目的内建支持
```

