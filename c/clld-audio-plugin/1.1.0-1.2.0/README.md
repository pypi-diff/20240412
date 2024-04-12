# Comparing `tmp/clld-audio-plugin-1.1.0.tar.gz` & `tmp/clld-audio-plugin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clld-audio-plugin-1.1.0.tar", last modified: Thu Mar 21 11:31:07 2024, max compression
+gzip compressed data, was "clld-audio-plugin-1.2.0.tar", last modified: Fri Apr 12 08:48:51 2024, max compression
```

## Comparing `clld-audio-plugin-1.1.0.tar` & `clld-audio-plugin-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       34 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)     2103 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1203 2024-03-21 10:08:42.000000 clld-audio-plugin-1.1.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)       91 2024-03-21 11:22:37.000000 clld-audio-plugin-1.1.0/pyproject.toml
--rw-rw-r--   0 robert    (1000) robert    (1000)     1688 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)       38 2024-03-21 11:21:03.000000 clld-audio-plugin-1.1.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.281737 clld-audio-plugin-1.1.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.281737 clld-audio-plugin-1.1.0/src/clld_audio_plugin/
--rw-rw-r--   0 robert    (1000) robert    (1000)      260 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      432 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/datatables.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      375 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/maps.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      421 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/models.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.281737 clld-audio-plugin-1.1.0/src/clld_audio_plugin/static/
--rw-rw-r--   0 robert    (1000) robert    (1000)      194 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/static/clld_audio_plugin.css
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/src/clld_audio_plugin/templates/
--rw-rw-r--   0 robert    (1000) robert    (1000)      133 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/templates/clld_audio_plugin_util.mako
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/src/clld_audio_plugin/templates/language/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1077 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/templates/language/snippet_html.mako
--rw-rw-r--   0 robert    (1000) robert    (1000)      404 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin/util.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.281737 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     2103 2024-03-21 11:31:07.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      682 2024-03-21 11:31:07.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-03-21 11:31:07.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      116 2024-03-21 11:31:07.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       18 2024-03-21 11:31:07.000000 clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-03-21 11:31:07.285737 clld-audio-plugin-1.1.0/tests/
--rw-rw-r--   0 robert    (1000) robert    (1000)      821 2022-12-23 09:31:00.000000 clld-audio-plugin-1.1.0/tests/test_misc.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       34 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2103 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1203 2024-03-21 10:08:42.000000 clld-audio-plugin-1.2.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       91 2024-03-21 11:22:37.000000 clld-audio-plugin-1.2.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1688 2024-04-12 08:48:51.755264 clld-audio-plugin-1.2.0/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)       38 2024-03-21 11:21:03.000000 clld-audio-plugin-1.2.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/clld_audio_plugin/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      260 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      432 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/datatables.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      374 2024-04-12 06:46:34.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/maps.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      421 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/models.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/clld_audio_plugin/static/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      194 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/static/clld_audio_plugin.css
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/clld_audio_plugin/templates/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      133 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/templates/clld_audio_plugin_util.mako
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/clld_audio_plugin/templates/language/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1077 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/templates/language/snippet_html.mako
+-rw-rw-r--   0 robert    (1000) robert    (1000)      616 2024-04-12 06:52:07.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin/util.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2103 2024-04-12 08:48:51.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      682 2024-04-12 08:48:51.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2024-04-12 08:48:51.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 09:31:00.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      116 2024-04-12 08:48:51.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       18 2024-04-12 08:48:51.000000 clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 08:48:51.751264 clld-audio-plugin-1.2.0/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      827 2024-04-12 06:50:06.000000 clld-audio-plugin-1.2.0/tests/test_misc.py
```

### Comparing `clld-audio-plugin-1.1.0/LICENSE` & `clld-audio-plugin-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clld-audio-plugin-1.1.0/PKG-INFO` & `clld-audio-plugin-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld-audio-plugin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Render linked audio files in clld apps.
 Home-page: https://github.com/clld/clld-audio-plugin
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 Project-URL: Bug Tracker, https://github.com/clld/clld-audio-plugin/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `clld-audio-plugin-1.1.0/README.md` & `clld-audio-plugin-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `clld-audio-plugin-1.1.0/setup.cfg` & `clld-audio-plugin-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clld-audio-plugin
-version = 1.1.0
+version = 1.2.0
 license_file = LICENSE
 author = Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
```

### Comparing `clld-audio-plugin-1.1.0/src/clld_audio_plugin/templates/language/snippet_html.mako` & `clld-audio-plugin-1.2.0/src/clld_audio_plugin/templates/language/snippet_html.mako`

 * *Files identical despite different names*

### Comparing `clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/PKG-INFO` & `clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clld-audio-plugin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Render linked audio files in clld apps.
 Home-page: https://github.com/clld/clld-audio-plugin
 Author: Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 Project-URL: Bug Tracker, https://github.com/clld/clld-audio-plugin/issues
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `clld-audio-plugin-1.1.0/src/clld_audio_plugin.egg-info/SOURCES.txt` & `clld-audio-plugin-1.2.0/src/clld_audio_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clld-audio-plugin-1.1.0/tests/test_misc.py` & `clld-audio-plugin-1.2.0/tests/test_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def test_AudioCol(mocker):
     assert AudioCol(mocker.MagicMock(), '').format(mocker.Mock(audio='x'))
     assert not AudioCol(mocker.MagicMock(), '').format(mocker.Mock(audio=None))
 
 
 def test_form2audio(mocker):
-    res =form2audio(mocker.Mock(
+    res = form2audio(mocker.MagicMock(
         iter_rows=lambda *args: [dict(mimetype='audio/mpeg', formReference='x')],
         get_row_url=lambda *args: 'http://example.org'))
     assert res['x'] == 'http://example.org'
 
 
 def test_ParamMap(mocker):
     assert ParamMap(mocker.Mock(), mocker.Mock()).options['with_audioplayer']
```

