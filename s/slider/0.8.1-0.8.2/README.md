# Comparing `tmp/slider-0.8.1.tar.gz` & `tmp/slider-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slider-0.8.1.tar", last modified: Thu Feb 15 16:13:24 2024, max compression
+gzip compressed data, was "slider-0.8.2.tar", last modified: Fri Apr 12 18:29:18 2024, max compression
```

## Comparing `slider-0.8.1.tar` & `slider-0.8.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.416378 slider-0.8.1/
--rw-r--r--   0 tybug      (501) staff       (20)     7651 2020-04-18 02:02:45.000000 slider-0.8.1/LICENSE
--rw-r--r--   0 tybug      (501) staff       (20)     1831 2024-02-15 16:13:24.416161 slider-0.8.1/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      936 2022-05-12 04:10:02.000000 slider-0.8.1/README.rst
--rw-r--r--   0 tybug      (501) staff       (20)       38 2024-02-15 16:13:24.416420 slider-0.8.1/setup.cfg
--rw-r--r--   0 tybug      (501) staff       (20)     1174 2024-02-15 16:11:36.000000 slider-0.8.1/setup.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.414003 slider-0.8.1/slider/
--rw-r--r--   0 tybug      (501) staff       (20)      570 2024-02-15 16:11:42.000000 slider-0.8.1/slider/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)     1009 2022-05-12 04:10:02.000000 slider-0.8.1/slider/__main__.py
--rw-r--r--   0 tybug      (501) staff       (20)      639 2020-04-18 02:02:45.000000 slider-0.8.1/slider/abc.py
--rw-r--r--   0 tybug      (501) staff       (20)   114116 2024-02-15 16:13:07.000000 slider-0.8.1/slider/beatmap.py
--rw-r--r--   0 tybug      (501) staff       (20)     1247 2022-05-12 04:10:02.000000 slider-0.8.1/slider/bit_enum.py
--rw-r--r--   0 tybug      (501) staff       (20)      974 2022-05-12 04:10:02.000000 slider-0.8.1/slider/cli.py
--rw-r--r--   0 tybug      (501) staff       (20)    24944 2022-05-12 04:10:02.000000 slider-0.8.1/slider/client.py
--rw-r--r--   0 tybug      (501) staff       (20)     2598 2020-04-18 02:02:45.000000 slider-0.8.1/slider/collection.py
--rw-r--r--   0 tybug      (501) staff       (20)    15974 2023-12-18 18:50:00.000000 slider-0.8.1/slider/curve.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.414744 slider-0.8.1/slider/example_data/
--rw-r--r--   0 tybug      (501) staff       (20)        0 2020-04-18 02:02:45.000000 slider-0.8.1/slider/example_data/__init__.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.414847 slider-0.8.1/slider/example_data/beatmaps/
--rw-r--r--   0 tybug      (501) staff       (20)     2003 2023-12-18 18:51:34.000000 slider-0.8.1/slider/example_data/beatmaps/__init__.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.414977 slider-0.8.1/slider/example_data/collections/
--rw-r--r--   0 tybug      (501) staff       (20)      492 2023-12-18 18:51:34.000000 slider-0.8.1/slider/example_data/collections/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)      172 2020-04-18 02:02:45.000000 slider-0.8.1/slider/game_mode.py
--rw-r--r--   0 tybug      (501) staff       (20)    13548 2022-07-24 00:25:48.000000 slider-0.8.1/slider/library.py
--rw-r--r--   0 tybug      (501) staff       (20)     5548 2020-04-18 02:02:45.000000 slider-0.8.1/slider/mod.py
--rw-r--r--   0 tybug      (501) staff       (20)     1165 2022-05-12 04:10:02.000000 slider-0.8.1/slider/position.py
--rw-r--r--   0 tybug      (501) staff       (20)    23945 2023-06-23 03:50:49.000000 slider-0.8.1/slider/replay.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.415451 slider-0.8.1/slider/tests/
--rw-r--r--   0 tybug      (501) staff       (20)        0 2020-07-24 20:29:28.000000 slider-0.8.1/slider/tests/__init__.py
--rw-r--r--   0 tybug      (501) staff       (20)    12556 2023-09-06 00:23:12.000000 slider-0.8.1/slider/tests/test_beatmap.py
--rw-r--r--   0 tybug      (501) staff       (20)      574 2020-07-24 20:29:28.000000 slider-0.8.1/slider/tests/test_collection.py
--rw-r--r--   0 tybug      (501) staff       (20)      348 2020-12-15 00:26:02.000000 slider-0.8.1/slider/tests/test_utils.py
--rw-r--r--   0 tybug      (501) staff       (20)     3797 2021-07-29 19:01:04.000000 slider-0.8.1/slider/utils.py
-drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-02-15 16:13:24.415626 slider-0.8.1/slider.egg-info/
--rw-r--r--   0 tybug      (501) staff       (20)     1831 2024-02-15 16:13:24.000000 slider-0.8.1/slider.egg-info/PKG-INFO
--rw-r--r--   0 tybug      (501) staff       (20)      667 2024-02-15 16:13:24.000000 slider-0.8.1/slider.egg-info/SOURCES.txt
--rw-r--r--   0 tybug      (501) staff       (20)        1 2024-02-15 16:13:24.000000 slider-0.8.1/slider.egg-info/dependency_links.txt
--rw-r--r--   0 tybug      (501) staff       (20)       99 2024-02-15 16:13:24.000000 slider-0.8.1/slider.egg-info/requires.txt
--rw-r--r--   0 tybug      (501) staff       (20)        7 2024-02-15 16:13:24.000000 slider-0.8.1/slider.egg-info/top_level.txt
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.468815 slider-0.8.2/
+-rw-r--r--   0 tybug      (501) staff       (20)     7651 2020-04-18 02:02:45.000000 slider-0.8.2/LICENSE
+-rw-r--r--   0 tybug      (501) staff       (20)     1831 2024-04-12 18:29:18.467986 slider-0.8.2/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      936 2022-05-12 04:10:02.000000 slider-0.8.2/README.rst
+-rw-r--r--   0 tybug      (501) staff       (20)       38 2024-04-12 18:29:18.468948 slider-0.8.2/setup.cfg
+-rw-r--r--   0 tybug      (501) staff       (20)     1174 2024-04-12 18:28:49.000000 slider-0.8.2/setup.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.457477 slider-0.8.2/slider/
+-rw-r--r--   0 tybug      (501) staff       (20)      570 2024-04-12 18:28:59.000000 slider-0.8.2/slider/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1009 2022-05-12 04:10:02.000000 slider-0.8.2/slider/__main__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      639 2020-04-18 02:02:45.000000 slider-0.8.2/slider/abc.py
+-rw-r--r--   0 tybug      (501) staff       (20)   114116 2024-02-15 16:13:07.000000 slider-0.8.2/slider/beatmap.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1247 2022-05-12 04:10:02.000000 slider-0.8.2/slider/bit_enum.py
+-rw-r--r--   0 tybug      (501) staff       (20)      974 2022-05-12 04:10:02.000000 slider-0.8.2/slider/cli.py
+-rw-r--r--   0 tybug      (501) staff       (20)    24944 2022-05-12 04:10:02.000000 slider-0.8.2/slider/client.py
+-rw-r--r--   0 tybug      (501) staff       (20)     2598 2020-04-18 02:02:45.000000 slider-0.8.2/slider/collection.py
+-rw-r--r--   0 tybug      (501) staff       (20)    15974 2023-12-18 18:50:00.000000 slider-0.8.2/slider/curve.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.461834 slider-0.8.2/slider/example_data/
+-rw-r--r--   0 tybug      (501) staff       (20)        0 2020-04-18 02:02:45.000000 slider-0.8.2/slider/example_data/__init__.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.461978 slider-0.8.2/slider/example_data/beatmaps/
+-rw-r--r--   0 tybug      (501) staff       (20)     2003 2023-12-18 18:51:34.000000 slider-0.8.2/slider/example_data/beatmaps/__init__.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.462427 slider-0.8.2/slider/example_data/collections/
+-rw-r--r--   0 tybug      (501) staff       (20)      492 2023-12-18 18:51:34.000000 slider-0.8.2/slider/example_data/collections/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)      172 2020-04-18 02:02:45.000000 slider-0.8.2/slider/game_mode.py
+-rw-r--r--   0 tybug      (501) staff       (20)    13548 2022-07-24 00:25:48.000000 slider-0.8.2/slider/library.py
+-rw-r--r--   0 tybug      (501) staff       (20)     5548 2020-04-18 02:02:45.000000 slider-0.8.2/slider/mod.py
+-rw-r--r--   0 tybug      (501) staff       (20)     1165 2022-05-12 04:10:02.000000 slider-0.8.2/slider/position.py
+-rw-r--r--   0 tybug      (501) staff       (20)    23947 2024-04-12 18:25:45.000000 slider-0.8.2/slider/replay.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.465114 slider-0.8.2/slider/tests/
+-rw-r--r--   0 tybug      (501) staff       (20)        0 2020-07-24 20:29:28.000000 slider-0.8.2/slider/tests/__init__.py
+-rw-r--r--   0 tybug      (501) staff       (20)    12556 2023-09-06 00:23:12.000000 slider-0.8.2/slider/tests/test_beatmap.py
+-rw-r--r--   0 tybug      (501) staff       (20)      574 2020-07-24 20:29:28.000000 slider-0.8.2/slider/tests/test_collection.py
+-rw-r--r--   0 tybug      (501) staff       (20)      348 2020-12-15 00:26:02.000000 slider-0.8.2/slider/tests/test_utils.py
+-rw-r--r--   0 tybug      (501) staff       (20)     3797 2021-07-29 19:01:04.000000 slider-0.8.2/slider/utils.py
+drwxr-xr-x   0 tybug      (501) staff       (20)        0 2024-04-12 18:29:18.465441 slider-0.8.2/slider.egg-info/
+-rw-r--r--   0 tybug      (501) staff       (20)     1831 2024-04-12 18:29:18.000000 slider-0.8.2/slider.egg-info/PKG-INFO
+-rw-r--r--   0 tybug      (501) staff       (20)      667 2024-04-12 18:29:18.000000 slider-0.8.2/slider.egg-info/SOURCES.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        1 2024-04-12 18:29:18.000000 slider-0.8.2/slider.egg-info/dependency_links.txt
+-rw-r--r--   0 tybug      (501) staff       (20)       99 2024-04-12 18:29:18.000000 slider-0.8.2/slider.egg-info/requires.txt
+-rw-r--r--   0 tybug      (501) staff       (20)        7 2024-04-12 18:29:18.000000 slider-0.8.2/slider.egg-info/top_level.txt
```

### Comparing `slider-0.8.1/LICENSE` & `slider-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/PKG-INFO` & `slider-0.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slider
-Version: 0.8.1
+Version: 0.8.2
 Summary: Utilities for working with osu! files and data
 Home-page: https://github.com/llllllllll/slider
 Author: Joe Jevnik
 Author-email: joejev@gmail.com
 License: LGPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `slider-0.8.1/README.rst` & `slider-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/setup.py` & `slider-0.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if 'sdist' in sys.argv:
     with open('README.rst') as f:
         long_description = f.read()
 
 
 setup(
     name='slider',
-    version='0.8.1',
+    version='0.8.2',
     description='Utilities for working with osu! files and data',
     author='Joe Jevnik',
     author_email='joejev@gmail.com',
     packages=find_packages(),
     long_description=long_description,
     license='LGPLv3+',
     classifiers=[
```

### Comparing `slider-0.8.1/slider/__init__.py` & `slider-0.8.2/slider/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .game_mode import GameMode
 from .mod import Mod
 from .position import Position
 from .replay import Replay
 from .library import Library
 from .collection import CollectionDB
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 
 __all__ = [
     'Beatmap',
     'Client',
     'GameMode',
     'Library',
```

### Comparing `slider-0.8.1/slider/__main__.py` & `slider-0.8.2/slider/__main__.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/abc.py` & `slider-0.8.2/slider/abc.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/beatmap.py` & `slider-0.8.2/slider/beatmap.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/bit_enum.py` & `slider-0.8.2/slider/bit_enum.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/cli.py` & `slider-0.8.2/slider/cli.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/client.py` & `slider-0.8.2/slider/client.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/collection.py` & `slider-0.8.2/slider/collection.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/curve.py` & `slider-0.8.2/slider/curve.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/example_data/beatmaps/__init__.py` & `slider-0.8.2/slider/example_data/beatmaps/__init__.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/library.py` & `slider-0.8.2/slider/library.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/mod.py` & `slider-0.8.2/slider/mod.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/position.py` & `slider-0.8.2/slider/position.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/replay.py` & `slider-0.8.2/slider/replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
     for datum in rdata:
         t = (datum.offset - obj.time) / duration
         if 0 <= t <= 1:
             nearest_pos = obj.curve(t)
             if (on and
                 not (_pressed(datum)
-                     and _within(nearest_pos, datum.position, rad * 3))):
+                     and _within(nearest_pos, datum.position, rad * 2.4))):
                 t_changes_append(t)
                 on = False
             elif (not on and
                   (_pressed(datum) and
                    _within(nearest_pos, datum.position, rad))):
                 t_changes_append(t)
                 on = True
```

### Comparing `slider-0.8.1/slider/tests/test_beatmap.py` & `slider-0.8.2/slider/tests/test_beatmap.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/tests/test_collection.py` & `slider-0.8.2/slider/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider/utils.py` & `slider-0.8.2/slider/utils.py`

 * *Files identical despite different names*

### Comparing `slider-0.8.1/slider.egg-info/PKG-INFO` & `slider-0.8.2/slider.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slider
-Version: 0.8.1
+Version: 0.8.2
 Summary: Utilities for working with osu! files and data
 Home-page: https://github.com/llllllllll/slider
 Author: Joe Jevnik
 Author-email: joejev@gmail.com
 License: LGPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `slider-0.8.1/slider.egg-info/SOURCES.txt` & `slider-0.8.2/slider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

