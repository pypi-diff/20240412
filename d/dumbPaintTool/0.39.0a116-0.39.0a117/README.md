# Comparing `tmp/dumbPaintTool-0.39.0a116.tar.gz` & `tmp/dumbpainttool-0.39a117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbPaintTool-0.39.0a116.tar", last modified: Fri Apr 12 16:31:11 2024, max compression
+gzip compressed data, was "dumbpainttool-0.39a117.tar", last modified: Fri Apr 12 16:38:42 2024, max compression
```

## Comparing `dumbPaintTool-0.39.0a116.tar` & `dumbpainttool-0.39a117.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:31:06.000000 dumbPaintTool-0.39.0a116/LICENSE
--rw-r--r--   0 one       (1000) one       (1000)     2553 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1204 2024-04-12 16:31:06.000000 dumbPaintTool-0.39.0a116/README.md
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/dumbPaintTool/
--rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/dumbPaintTool/app/
--rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/brush.py
--rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/canvaslayer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:31:06.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/const.py
--rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/exportarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/glbls.py
--rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/importimage.py
--rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/layers.py
--rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/maintemplate.py
--rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/paintarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/painttoolkit.py
--rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/palette.py
--rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/textarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/app/toolspanel.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/dumbPaintTool/tui/
--rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/tui/paintToolKit.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/tui/quickImport.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbPaintTool-0.39.0a116/dumbPaintTool/tui/tools.tui.json
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/
--rw-r--r--   0 one       (1000) one       (1000)     2553 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      919 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       35 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:31:11.000000 dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/top_level.txt
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:31:11.347793 dumbPaintTool-0.39.0a116/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     2686 2024-04-12 16:31:06.000000 dumbPaintTool-0.39.0a116/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:38:42.027198 dumbpainttool-0.39a117/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:38:37.000000 dumbpainttool-0.39a117/LICENSE
+-rw-r--r--   0 one       (1000) one       (1000)     2556 2024-04-12 16:38:42.023198 dumbpainttool-0.39a117/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1204 2024-04-12 16:38:37.000000 dumbpainttool-0.39a117/README.md
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:38:42.023198 dumbpainttool-0.39a117/dumbPaintTool/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbpainttool-0.39a117/dumbPaintTool/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbpainttool-0.39a117/dumbPaintTool/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:38:42.023198 dumbpainttool-0.39a117/dumbPaintTool/app/
+-rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbpainttool-0.39a117/dumbPaintTool/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/brush.py
+-rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/canvaslayer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:38:37.000000 dumbpainttool-0.39a117/dumbPaintTool/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbpainttool-0.39a117/dumbPaintTool/app/const.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/exportarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbpainttool-0.39a117/dumbPaintTool/app/glbls.py
+-rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbpainttool-0.39a117/dumbPaintTool/app/importimage.py
+-rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/layers.py
+-rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbpainttool-0.39a117/dumbPaintTool/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbpainttool-0.39a117/dumbPaintTool/app/maintemplate.py
+-rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/paintarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbpainttool-0.39a117/dumbPaintTool/app/painttoolkit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/palette.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbpainttool-0.39a117/dumbPaintTool/app/textarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbpainttool-0.39a117/dumbPaintTool/app/toolspanel.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:38:42.023198 dumbpainttool-0.39a117/dumbPaintTool/tui/
+-rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbpainttool-0.39a117/dumbPaintTool/tui/paintToolKit.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbpainttool-0.39a117/dumbPaintTool/tui/quickImport.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbpainttool-0.39a117/dumbPaintTool/tui/tools.tui.json
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:38:42.023198 dumbpainttool-0.39a117/dumbPaintTool.egg-info/
+-rw-r--r--   0 one       (1000) one       (1000)     2556 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)      919 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:38:42.000000 dumbpainttool-0.39a117/dumbPaintTool.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:38:42.027198 dumbpainttool-0.39a117/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     2689 2024-04-12 16:38:37.000000 dumbpainttool-0.39a117/setup.py
```

### Comparing `dumbPaintTool-0.39.0a116/LICENSE` & `dumbpainttool-0.39a117/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/PKG-INFO` & `dumbpainttool-0.39a117/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a116
+Version: 0.39.0a117
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,28 +22,28 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyTermTk>=0.39.0a
+Requires-Dist: pyTermTk>=0.39.0a116
 Requires-Dist: pyperclip
 Requires-Dist: Pillow
 
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/b5d7b870-1217-45a0-9fec-17358b563aa9)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbPaintTool-0.39.0a116/README.md` & `dumbpainttool-0.39a117/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/b5d7b870-1217-45a0-9fec-17358b563aa9)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/__init__.py` & `dumbpainttool-0.39a117/dumbPaintTool/__init__.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/__main__.py` & `dumbpainttool-0.39a117/dumbPaintTool/__main__.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/about.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/about.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/brush.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/brush.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/canvaslayer.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/canvaslayer.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/cfg.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 
 class DPTCfg:
-    version="0.39.0-a116"
+    version="0.39.0-a117"
     name="dumbPaintTool"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/const.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/const.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/exportarea.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/exportarea.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/glbls.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/glbls.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/importimage.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/importimage.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/layers.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/layers.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/main.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/main.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/maintemplate.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/maintemplate.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/paintarea.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/paintarea.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/painttoolkit.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/painttoolkit.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/palette.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/palette.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/textarea.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/textarea.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/app/toolspanel.py` & `dumbpainttool-0.39a117/dumbPaintTool/app/toolspanel.py`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/tui/paintToolKit.tui.json` & `dumbpainttool-0.39a117/dumbPaintTool/tui/paintToolKit.tui.json`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/tui/quickImport.tui.json` & `dumbpainttool-0.39a117/dumbPaintTool/tui/quickImport.tui.json`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool/tui/tools.tui.json` & `dumbpainttool-0.39a117/dumbPaintTool/tui/tools.tui.json`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/PKG-INFO` & `dumbpainttool-0.39a117/dumbPaintTool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a116
+Version: 0.39.0a117
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,28 +22,28 @@
 Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyTermTk>=0.39.0a
+Requires-Dist: pyTermTk>=0.39.0a116
 Requires-Dist: pyperclip
 Requires-Dist: Pillow
 
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
 ![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/dumbPaintTool)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 
-[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/b5d7b870-1217-45a0-9fec-17358b563aa9)](https://pypi.org/project/tools/dumbPaintTool)
+[![dpt hero](https://github.com/ceccopierangiolieugenio/pyTermTk/assets/8876552/54d29d95-717d-404d-9112-efed866d4048)](https://pypi.org/project/tools/dumbPaintTool)
 
 
 ## [the Dumb Paint Tool](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/dumbPaintTool)
 
 A Terminal ASCII Photoshop
 
 Try it live on [itch.io](https://ceccopierangiolieugenio.itch.io/dumb-paint-tool)
```

### Comparing `dumbPaintTool-0.39.0a116/dumbPaintTool.egg-info/SOURCES.txt` & `dumbpainttool-0.39a117/dumbPaintTool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dumbPaintTool-0.39.0a116/setup.py` & `dumbpainttool-0.39a117/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.39.0-a116"
+version = "0.39.0-a117"
 name = "dumbPaintTool"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -38,15 +38,15 @@
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks"],
     include_package_data=False,
     packages=['dumbPaintTool','dumbPaintTool.app'],
     package_data={'dumbPaintTool': ['tui/*']},
     python_requires=">=3.9",
     install_requires=[
-        'pyTermTk>=0.39.0a',
+        'pyTermTk>=0.39.0a116',
         'pyperclip',
         'Pillow'],
     entry_points={
         'console_scripts': [
             'dumbPaintTool = dumbPaintTool:main',
         ],
     },
```

