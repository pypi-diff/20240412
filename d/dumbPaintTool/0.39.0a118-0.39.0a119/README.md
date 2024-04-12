# Comparing `tmp/dumbpainttool-0.39a118.tar.gz` & `tmp/dumbpainttool-0.39a119.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbpainttool-0.39a118.tar", last modified: Fri Apr 12 16:45:42 2024, max compression
+gzip compressed data, was "dumbpainttool-0.39a119.tar", last modified: Fri Apr 12 16:47:12 2024, max compression
```

## Comparing `dumbpainttool-0.39a118.tar` & `dumbpainttool-0.39a119.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:45:38.000000 dumbpainttool-0.39a118/LICENSE
--rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1204 2024-04-12 16:45:38.000000 dumbpainttool-0.39a118/README.md
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/dumbPaintTool/
--rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbpainttool-0.39a118/dumbPaintTool/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbpainttool-0.39a118/dumbPaintTool/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/dumbPaintTool/app/
--rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbpainttool-0.39a118/dumbPaintTool/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/brush.py
--rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/canvaslayer.py
--rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:45:38.000000 dumbpainttool-0.39a118/dumbPaintTool/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbpainttool-0.39a118/dumbPaintTool/app/const.py
--rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/exportarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbpainttool-0.39a118/dumbPaintTool/app/glbls.py
--rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbpainttool-0.39a118/dumbPaintTool/app/importimage.py
--rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/layers.py
--rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbpainttool-0.39a118/dumbPaintTool/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbpainttool-0.39a118/dumbPaintTool/app/maintemplate.py
--rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/paintarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbpainttool-0.39a118/dumbPaintTool/app/painttoolkit.py
--rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/palette.py
--rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbpainttool-0.39a118/dumbPaintTool/app/textarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbpainttool-0.39a118/dumbPaintTool/app/toolspanel.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/dumbPaintTool/tui/
--rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbpainttool-0.39a118/dumbPaintTool/tui/paintToolKit.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbpainttool-0.39a118/dumbPaintTool/tui/quickImport.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbpainttool-0.39a118/dumbPaintTool/tui/tools.tui.json
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/dumbPaintTool.egg-info/
--rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)      919 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:45:42.000000 dumbpainttool-0.39a118/dumbPaintTool.egg-info/top_level.txt
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:45:42.770907 dumbpainttool-0.39a118/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     2140 2024-04-12 16:45:38.000000 dumbpainttool-0.39a118/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/LICENSE
+-rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1204 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/README.md
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1218 2024-04-12 07:54:44.000000 dumbpainttool-0.39a119/dumbPaintTool/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-04-12 07:46:57.000000 dumbpainttool-0.39a119/dumbPaintTool/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/app/
+-rw-rw-r--   0 one       (1000) one       (1000)      448 2024-04-12 07:58:02.000000 dumbpainttool-0.39a119/dumbPaintTool/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4078 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4181 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/brush.py
+-rw-rw-r--   0 one       (1000) one       (1000)    17850 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/canvaslayer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1309 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/dumbPaintTool/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1452 2024-04-12 07:58:02.000000 dumbpainttool-0.39a119/dumbPaintTool/app/const.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7397 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/exportarea.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/app/filters/
+-rw-rw-r--   0 one       (1000) one       (1000)       72 2024-03-29 18:33:39.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5552 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/brightness_contrast.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8696 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/filters/hue_chroma_lightness.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1368 2024-04-12 16:16:08.000000 dumbpainttool-0.39a119/dumbPaintTool/app/glbls.py
+-rw-rw-r--   0 one       (1000) one       (1000)    20869 2024-04-12 16:17:09.000000 dumbpainttool-0.39a119/dumbPaintTool/app/importimage.py
+-rw-rw-r--   0 one       (1000) one       (1000)    13367 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/layers.py
+-rwxrwxr-x   0 one       (1000) one       (1000)     2054 2024-04-12 16:17:22.000000 dumbpainttool-0.39a119/dumbPaintTool/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    12705 2024-04-12 16:14:37.000000 dumbpainttool-0.39a119/dumbPaintTool/app/maintemplate.py
+-rw-rw-r--   0 one       (1000) one       (1000)    21343 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/paintarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4641 2024-04-12 16:14:10.000000 dumbpainttool-0.39a119/dumbPaintTool/app/painttoolkit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     7990 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/palette.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9507 2024-04-12 16:13:19.000000 dumbpainttool-0.39a119/dumbPaintTool/app/textarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8468 2024-04-12 16:14:55.000000 dumbpainttool-0.39a119/dumbPaintTool/app/toolspanel.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool/tui/
+-rw-rw-r--   0 one       (1000) one       (1000)    15264 2024-03-22 15:39:11.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/paintToolKit.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-03-22 15:39:11.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/quickImport.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     6803 2024-04-05 11:36:24.000000 dumbpainttool-0.39a119/dumbPaintTool/tui/tools.tui.json
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/dumbPaintTool.egg-info/
+-rw-r--r--   0 one       (1000) one       (1000)     2793 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1056 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       53 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       14 2024-04-12 16:47:12.000000 dumbpainttool-0.39a119/dumbPaintTool.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:47:12.125995 dumbpainttool-0.39a119/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     2168 2024-04-12 16:47:07.000000 dumbpainttool-0.39a119/setup.py
```

### Comparing `dumbpainttool-0.39a118/LICENSE` & `dumbpainttool-0.39a119/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/PKG-INFO` & `dumbpainttool-0.39a119/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a118
+Version: 0.39.0a119
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dumbpainttool-0.39a118/README.md` & `dumbpainttool-0.39a119/README.md`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/__init__.py` & `dumbpainttool-0.39a119/dumbPaintTool/__init__.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/__main__.py` & `dumbpainttool-0.39a119/dumbPaintTool/__main__.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/about.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/about.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/brush.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/brush.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/canvaslayer.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/canvaslayer.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/cfg.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 
 class DPTCfg:
-    version="0.39.0-a118"
+    version="0.39.0-a119"
     name="dumbPaintTool"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/const.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/const.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/exportarea.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/exportarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/glbls.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/glbls.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/importimage.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/importimage.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/layers.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/layers.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/main.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/main.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/maintemplate.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/maintemplate.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/paintarea.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/paintarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/painttoolkit.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/painttoolkit.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/palette.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/palette.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/textarea.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/textarea.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/app/toolspanel.py` & `dumbpainttool-0.39a119/dumbPaintTool/app/toolspanel.py`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/tui/paintToolKit.tui.json` & `dumbpainttool-0.39a119/dumbPaintTool/tui/paintToolKit.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/tui/quickImport.tui.json` & `dumbpainttool-0.39a119/dumbPaintTool/tui/quickImport.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool/tui/tools.tui.json` & `dumbpainttool-0.39a119/dumbPaintTool/tui/tools.tui.json`

 * *Files identical despite different names*

### Comparing `dumbpainttool-0.39a118/dumbPaintTool.egg-info/PKG-INFO` & `dumbpainttool-0.39a119/dumbPaintTool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbPaintTool
-Version: 0.39.0a118
+Version: 0.39.0a119
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dumbpainttool-0.39a118/dumbPaintTool.egg-info/SOURCES.txt` & `dumbpainttool-0.39a119/dumbPaintTool.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,10 +22,13 @@
 dumbPaintTool/app/main.py
 dumbPaintTool/app/maintemplate.py
 dumbPaintTool/app/paintarea.py
 dumbPaintTool/app/painttoolkit.py
 dumbPaintTool/app/palette.py
 dumbPaintTool/app/textarea.py
 dumbPaintTool/app/toolspanel.py
+dumbPaintTool/app/filters/__init__.py
+dumbPaintTool/app/filters/brightness_contrast.py
+dumbPaintTool/app/filters/hue_chroma_lightness.py
 dumbPaintTool/tui/paintToolKit.tui.json
 dumbPaintTool/tui/quickImport.tui.json
 dumbPaintTool/tui/tools.tui.json
```

### Comparing `dumbpainttool-0.39a118/setup.py` & `dumbpainttool-0.39a119/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-version = "0.39.0-a118"
+version = "0.39.0-a119"
 name = "dumbPaintTool"
 
 print(f"Version: {version}")
 print(f"Name: {name}")
 
 setup(
     name=name,
@@ -39,15 +39,15 @@
         "Topic :: Multimedia :: Graphics :: Editors :: Raster-Based",
         "Topic :: Multimedia :: Graphics :: Graphics Conversion",
         "Topic :: Software Development :: User Interfaces",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks"],
     include_package_data=False,
-    packages=['dumbPaintTool','dumbPaintTool.app'],
+    packages=['dumbPaintTool','dumbPaintTool.app','dumbPaintTool.app.filters'],
     package_data={'dumbPaintTool': ['tui/*']},
     python_requires=">=3.9",
     install_requires=[
         'pyTermTk>=0.39.0a116',
         'pyperclip',
         'Pillow'],
     entry_points={
```

