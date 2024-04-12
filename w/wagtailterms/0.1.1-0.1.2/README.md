# Comparing `tmp/wagtailterms-0.1.1.tar.gz` & `tmp/wagtailterms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailterms-0.1.1.tar", last modified: Wed Apr  3 01:11:12 2024, max compression
+gzip compressed data, was "wagtailterms-0.1.2.tar", last modified: Fri Apr 12 17:14:02 2024, max compression
```

## Comparing `wagtailterms-0.1.1.tar` & `wagtailterms-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/default_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.502266 wagtailterms-0.1.1/wagtailterms/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.506265 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/
--rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popperjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popup-js-1.4.2.js
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/term.js
--rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/static/wagtailterms/tippyjs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-03 01:11:06.000000 wagtailterms-0.1.1/wagtailterms/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:11:12.510265 wagtailterms-0.1.1/wagtailterms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 01:11:12.000000 wagtailterms-0.1.1/wagtailterms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.865871 wagtailterms-0.1.2/wagtailterms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/default_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/wagtailterms/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.865871 wagtailterms-0.1.2/wagtailterms/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/wagtailterms/static/wagtailterms/
+-rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/static/wagtailterms/popperjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/static/wagtailterms/popup-js-1.4.2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7951 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/static/wagtailterms/term.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25716 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/static/wagtailterms/tippyjs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-12 17:13:59.000000 wagtailterms-0.1.2/wagtailterms/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:14:02.869871 wagtailterms-0.1.2/wagtailterms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-12 17:14:02.000000 wagtailterms-0.1.2/wagtailterms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-12 17:14:02.000000 wagtailterms-0.1.2/wagtailterms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:14:02.000000 wagtailterms-0.1.2/wagtailterms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 17:14:02.000000 wagtailterms-0.1.2/wagtailterms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 17:14:02.000000 wagtailterms-0.1.2/wagtailterms.egg-info/top_level.txt
```

### Comparing `wagtailterms-0.1.1/LICENSE` & `wagtailterms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/PKG-INFO` & `wagtailterms-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailterms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Wagtail plugin to add support for glossary terms entity to Draftail
 Home-page: https://github.com/smark-1/wagtailterms/
 Download-URL: https://pypi.python.org/pypi/wagtailterms
 License: MIT
 Keywords: wagtail,draftjs,Draftail,picker,term,definition,glossary
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -226,12 +226,14 @@
         "id": 1
     }
 
 ## Changelog
 ### 0.1.1
 - added settings to change the icon and menu order.
 
+### 0.1.2
+- fixed term search form wider than modal
+- Add dark mode support
+
 ## To Do
 - Allow frontend styles to be changed
 - Include a default javascript implementation for frontend
-- Support dark mode
-- Fix choose term search form wider than modal
```

### Comparing `wagtailterms-0.1.1/README.md` & `wagtailterms-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -201,12 +201,14 @@
         "id": 1
     }
 
 ## Changelog
 ### 0.1.1
 - added settings to change the icon and menu order.
 
+### 0.1.2
+- fixed term search form wider than modal
+- Add dark mode support
+
 ## To Do
 - Allow frontend styles to be changed
-- Include a default javascript implementation for frontend
-- Support dark mode
-- Fix choose term search form wider than modal
+- Include a default javascript implementation for frontend
```

### Comparing `wagtailterms-0.1.1/setup.py` & `wagtailterms-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/migrations/0001_initial.py` & `wagtailterms-0.1.2/wagtailterms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/models.py` & `wagtailterms-0.1.2/wagtailterms/models.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popperjs.js` & `wagtailterms-0.1.2/wagtailterms/static/wagtailterms/popperjs.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/popup-js-1.4.2.js` & `wagtailterms-0.1.2/wagtailterms/static/wagtailterms/popup-js-1.4.2.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/term.js` & `wagtailterms-0.1.2/wagtailterms/static/wagtailterms/term.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,20 @@
 // create popup to choose the term. The entire page uses the same popup. This makes it easier to select by id
 const termPopup = new Popup({
     id: "term-selector-popup",
     title: "Choose term",
     allowClose: false,
-    content: `<div style="position: relative">
-    <button style="position: absolute;top:-100px;right:0;background-color: white" id="term-selector-popup-close">X</button>
+    backgroundColor: 'var(--w-color-surface-field)',
+    textColor: 'var(--w-text-context)',
+    titleColor: 'var(--w-text-label)',
+    borderColor: 'var(--w-color-border-furniture)',
+    content: `<div style="position: relative;">
+    <button style="position: absolute;top:-80px;right:0;background-color: var(--w-color-surface-field)" id="term-selector-popup-close">X</button>
     <label for="term-selector-popup-search-box">Find Term</label><br>
-    <input type="search" name="fname" id="term-selector-popup-search-box">
+    <input type="search" name="fname" id="term-selector-popup-search-box" style="width: 100%; width: -moz-available; width: -webkit-fill-available; width: fill-available;">
     <div id="term-selector-popup-search-buttons-frame"></div>
     </div>
     `,
 });
 
 
 
@@ -118,15 +122,17 @@
                 .then(response => response.json())
                 .then(data => {
                     this.setState({
                         terms: data
                     })
                     frame.innerHTML = "";
                     for (const item of data) {
-                        frame.innerHTML += `<button data-term-id="${item.id}">${item.term}</button>`
+                        const button_style = 'background-color: var(--w-color-surface-button-default); color:var(--w-color-text-button); margin: 5px;'
+                        const update_hover_colors = "onMouseOver=\"this.style.backgroundColor='var(--w-color-surface-button-hover)'\" onMouseOut=\"this.style.backgroundColor='var(--w-color-surface-button-default)'"
+                        frame.innerHTML += `<button data-term-id="${item.id}" style="${button_style}" ${update_hover_colors}">${item.term}</button>`
                     }
                     for (const button of frame.children) {
                         button.onclick = this.handleSetTerm
                     }
                 })
         };
```

### Comparing `wagtailterms-0.1.1/wagtailterms/static/wagtailterms/tippyjs.js` & `wagtailterms-0.1.2/wagtailterms/static/wagtailterms/tippyjs.js`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/tests.py` & `wagtailterms-0.1.2/wagtailterms/tests.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/views.py` & `wagtailterms-0.1.2/wagtailterms/views.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms/wagtail_hooks.py` & `wagtailterms-0.1.2/wagtailterms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtailterms-0.1.1/wagtailterms.egg-info/PKG-INFO` & `wagtailterms-0.1.2/wagtailterms.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailterms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Wagtail plugin to add support for glossary terms entity to Draftail
 Home-page: https://github.com/smark-1/wagtailterms/
 Download-URL: https://pypi.python.org/pypi/wagtailterms
 License: MIT
 Keywords: wagtail,draftjs,Draftail,picker,term,definition,glossary
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -226,12 +226,14 @@
         "id": 1
     }
 
 ## Changelog
 ### 0.1.1
 - added settings to change the icon and menu order.
 
+### 0.1.2
+- fixed term search form wider than modal
+- Add dark mode support
+
 ## To Do
 - Allow frontend styles to be changed
 - Include a default javascript implementation for frontend
-- Support dark mode
-- Fix choose term search form wider than modal
```

### Comparing `wagtailterms-0.1.1/wagtailterms.egg-info/SOURCES.txt` & `wagtailterms-0.1.2/wagtailterms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

