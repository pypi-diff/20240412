# Comparing `tmp/omuplugin_translator-0.2.3.tar.gz` & `tmp/omuplugin_translator-0.2.4.tar.gz`

## Comparing `omuplugin_translator-0.2.3.tar` & `omuplugin_translator-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/src/omuplugin_translator/__init__.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/src/omuplugin_translator/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/src/omuplugin_translator/__init__.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/src/omuplugin_translator/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 omuplugin_translator-0.2.4/PKG-INFO
```

### Comparing `omuplugin_translator-0.2.3/src/omuplugin_translator/plugin.py` & `omuplugin_translator-0.2.4/src/omuplugin_translator/plugin.py`

 * *Files identical despite different names*

### Comparing `omuplugin_translator-0.2.3/pyproject.toml` & `omuplugin_translator-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuplugin_translator"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["edgetrans>=0.2.3", "omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

