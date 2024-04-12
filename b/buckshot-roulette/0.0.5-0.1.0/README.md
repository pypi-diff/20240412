# Comparing `tmp/buckshot-roulette-0.0.5.tar.gz` & `tmp/buckshot-roulette-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckshot-roulette-0.0.5.tar", last modified: Tue Apr  9 21:20:27 2024, max compression
+gzip compressed data, was "buckshot-roulette-0.1.0.tar", last modified: Fri Apr 12 05:32:20 2024, max compression
```

## Comparing `buckshot-roulette-0.0.5.tar` & `buckshot-roulette-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.997105 buckshot-roulette-0.0.5/
--rw-rw-rw-   0        0        0     1064 2024-04-09 20:48:52.000000 buckshot-roulette-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1203 2024-04-09 21:20:27.997105 buckshot-roulette-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      616 2024-04-09 21:10:53.000000 buckshot-roulette-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.984104 buckshot-roulette-0.0.5/buckshot_roulette/
--rw-rw-rw-   0        0        0       58 2024-04-08 21:41:52.000000 buckshot-roulette-0.0.5/buckshot_roulette/__init__.py
--rw-rw-rw-   0        0        0     4946 2024-04-09 21:12:32.000000 buckshot-roulette-0.0.5/buckshot_roulette/ai.py
--rw-rw-rw-   0        0        0    10035 2024-04-09 21:10:19.000000 buckshot-roulette-0.0.5/buckshot_roulette/game.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:20:27.996105 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/
--rw-rw-rw-   0        0        0     1203 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 21:20:27.000000 buckshot-roulette-0.0.5/buckshot_roulette.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      709 2024-04-09 21:14:42.000000 buckshot-roulette-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 21:20:27.998105 buckshot-roulette-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/buckshot_roulette/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:32:20.240260 buckshot-roulette-0.1.0/setup.cfg
```

### Comparing `buckshot-roulette-0.0.5/LICENSE` & `buckshot-roulette-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2024 Bytestorm
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Copyright 2024 Bytestorm
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `buckshot-roulette-0.0.5/README.md` & `buckshot-roulette-0.1.0/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Buckshot Roulette
-> BETA- Things may be broken or not work as intended. If you find something wrong, make a PR or an Issue!
-
-A Buckshot Roulette library ([PyPI](https://pypi.org/project/buckshot-roulette/)) for python, with complete game features & reasonable efficiency.
-
-[What is Buckshot Roulette?](https://store.steampowered.com/app/2835570/Buckshot_Roulette/)
-
-Mainly intended for use in developing engines to play the game optimally.
-
-## Quickstart
-```
-pip install buckshot-roulette
-```
-```python
-from buckshot_roulette import BuckshotRoulette
-
-board = BuckshotRoulette(charge_count=4)
-```
+# Buckshot Roulette
+> BETA- Things may be broken or not work as intended. If you find something wrong, make a PR or an Issue!
+
+A Buckshot Roulette library ([PyPI](https://pypi.org/project/buckshot-roulette/)) for python, with complete game features & reasonable efficiency.
+
+[What is Buckshot Roulette?](https://store.steampowered.com/app/2835570/Buckshot_Roulette/)
+
+Mainly intended for use in developing engines to play the game optimally.
+
+## Quickstart
+```
+pip install buckshot-roulette
+```
+```python
+from buckshot_roulette import BuckshotRoulette
+
+board = BuckshotRoulette(charge_count=4)
+```
```

