# Comparing `tmp/dumbpainttool-0.39a119.tar.gz` & `tmp/dumbpainttool-0.39a121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbpainttool-0.39a119.tar", last modified: Fri Apr 12 16:47:12 2024, max compression
+gzip compressed data, was "dumbpainttool-0.39a121.tar", last modified: Fri Apr 12 16:55:29 2024, max compression
```

## Comparing `dumbpainttool-0.39a119.tar` & `dumbpainttool-0.39a121.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/LICENSE
--rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1204 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/README.md
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/
--rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbpainttool-0.39a119/dumbPaintTool/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbpainttool-0.39a119/dumbPaintTool/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/app/
--rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbpainttool-0.39a119/dumbPaintTool/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/brush.py
--rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/canvaslayer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/dumbPaintTool/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbpainttool-0.39a119/dumbPaintTool/app/const.py
--rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/exportarea.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/app/filters/
--rw-rw-r--   0 one       (1000) one       (1000)       72 2024-03-29 18:33:39.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     5552 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/brightness_contrast.py
--rw-rw-r--   0 one       (1000) one       (1000)     8696 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/hue_chroma_lightness.py
--rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbpainttool-0.39a119/dumbPaintTool/app/glbls.py
--rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbpainttool-0.39a119/dumbPaintTool/app/importimage.py
--rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/layers.py
--rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbpainttool-0.39a119/dumbPaintTool/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbpainttool-0.39a119/dumbPaintTool/app/maintemplate.py
--rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/paintarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbpainttool-0.39a119/dumbPaintTool/app/painttoolkit.py
--rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/palette.py
--rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/textarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbpainttool-0.39a119/dumbPaintTool/app/toolspanel.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/tui/
--rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/paintToolKit.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/quickImport.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/tools.tui.json
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool.egg-info/
--rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1056 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/top_level.txt
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     2168 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:55:25.000000 dumbpainttool-0.39a121/LICENSE
+-rw-r--r--   0 one       (1000) one       (1000)     2791 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1198 2024-04-12 16:55:25.000000 dumbpainttool-0.39a121/README.md
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.332981 dumbpainttool-0.39a121/dumbPaintTool/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbpainttool-0.39a121/dumbPaintTool/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbpainttool-0.39a121/dumbPaintTool/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/dumbPaintTool/app/
+-rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbpainttool-0.39a121/dumbPaintTool/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/brush.py
+-rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/canvaslayer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:55:25.000000 dumbpainttool-0.39a121/dumbPaintTool/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbpainttool-0.39a121/dumbPaintTool/app/const.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/exportarea.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/dumbPaintTool/app/filters/
+-rw-rw-r--   0 one       (1000) one       (1000)       72 2024-03-29 18:33:39.000000 dumbpainttool-0.39a121/dumbPaintTool/app/filters/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5552 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/filters/brightness_contrast.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8696 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/filters/hue_chroma_lightness.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbpainttool-0.39a121/dumbPaintTool/app/glbls.py
+-rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbpainttool-0.39a121/dumbPaintTool/app/importimage.py
+-rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/layers.py
+-rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbpainttool-0.39a121/dumbPaintTool/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbpainttool-0.39a121/dumbPaintTool/app/maintemplate.py
+-rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/paintarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbpainttool-0.39a121/dumbPaintTool/app/painttoolkit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/palette.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbpainttool-0.39a121/dumbPaintTool/app/textarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbpainttool-0.39a121/dumbPaintTool/app/toolspanel.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/dumbPaintTool/tui/
+-rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbpainttool-0.39a121/dumbPaintTool/tui/paintToolKit.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbpainttool-0.39a121/dumbPaintTool/tui/quickImport.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbpainttool-0.39a121/dumbPaintTool/tui/tools.tui.json
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/dumbPaintTool.egg-info/
+-rw-r--r--   0 one       (1000) one       (1000)     2791 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1056 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:55:29.000000 dumbpainttool-0.39a121/dumbPaintTool.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:55:29.336981 dumbpainttool-0.39a121/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     2172 2024-04-12 16:55:25.000000 dumbpainttool-0.39a121/setup.py
```

### Comparing `dumbpainttool-0.39a119/LICENSE` & `dumbpainttool-0.39a121/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/PKG-INFO` & `dumbpainttool-0.39a121/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a119
-Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
-Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
+Version: 0.39.0a121
+Summary: the Dumb Paint Tool is a Terminal ASCII Photoshop
+Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -39,15 +39,15 @@
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbpainttool-0.39a119/README.md` & `dumbpainttool-0.39a121/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/__init__.py` & `dumbpainttool-0.39a121/dumbPaintTool/__init__.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/__main__.py` & `dumbpainttool-0.39a121/dumbPaintTool/__main__.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/about.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/about.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/brush.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/brush.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/canvaslayer.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/canvaslayer.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/cfg.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 
 class DPTCfg:
-    version="0.39.0-a119"
+    version="0.39.0-a121"
     name="dumbPaintTool"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/const.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/const.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/exportarea.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/exportarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/filters/brightness_contrast.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/filters/brightness_contrast.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/filters/hue_chroma_lightness.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/filters/hue_chroma_lightness.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/glbls.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/glbls.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/importimage.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/importimage.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/layers.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/layers.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/main.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/main.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/maintemplate.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/maintemplate.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/paintarea.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/paintarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/painttoolkit.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/painttoolkit.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/palette.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/palette.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/textarea.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/textarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/app/toolspanel.py` & `dumbpainttool-0.39a121/dumbPaintTool/app/toolspanel.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/tui/paintToolKit.tui.json` & `dumbpainttool-0.39a121/dumbPaintTool/tui/paintToolKit.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/tui/quickImport.tui.json` & `dumbpainttool-0.39a121/dumbPaintTool/tui/quickImport.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool/tui/tools.tui.json` & `dumbpainttool-0.39a121/dumbPaintTool/tui/tools.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/dumbPaintTool.egg-info/PKG-INFO` & `dumbpainttool-0.39a121/dumbPaintTool.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a119
-Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
-Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
+Version: 0.39.0a121
+Summary: the Dumb Paint Tool is a Terminal ASCII Photoshop
+Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -39,15 +39,15 @@
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbpainttool-0.39a119/dumbPaintTool.egg-info/SOURCES.txt` & `dumbpainttool-0.39a121/dumbPaintTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a119/setup.py` & `dumbpainttool-0.39a121/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.39.0-a119"
+version = "0.39.0-a121"
 name = "dumbPaintTool"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
     version=version,
     author='Eugenio Parodi',
     author_email='ceccopierangiolieugenio@googlemail.com',
-    description='ttkDesigner is a terminal user interface designer for pyTermTk applications',
+    description='the Dumb Paint Tool is a Terminal ASCII Photoshop',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/ceccopierangiolieugenio/pyTermTk",
+    url="https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool",
     classifiers=[
         # https://pypi.org/classifiers/
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
```

