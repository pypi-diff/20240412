# Comparing `tmp/click-app-template-demo-auto-0.2.0.tar.gz` & `tmp/click-app-template-demo-auto-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click-app-template-demo-auto-0.2.0.tar", last modified: Fri Apr 12 14:53:00 2024, max compression
+gzip compressed data, was "click-app-template-demo-auto-0.3.0.tar", last modified: Fri Apr 12 15:09:48 2024, max compression
```

## Comparing `click-app-template-demo-auto-0.2.0.tar` & `click-app-template-demo-auto-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.496433 click-app-template-demo-auto-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.488433 click-app-template-demo-auto-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.492433 click-app-template-demo-auto-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 14:53:00.496433 click-app-template-demo-auto-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.492433 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.492433 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 14:53:00.000000 click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:53:00.496433 click-app-template-demo-auto-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:53:00.492433 click-app-template-demo-auto-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 14:52:54.000000 click-app-template-demo-auto-0.2.0/tests/test_click_app_template_demo_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.551762 click-app-template-demo-auto-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-12 15:09:48.000000 click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:09:48.555762 click-app-template-demo-auto-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 15:09:42.000000 click-app-template-demo-auto-0.3.0/tests/test_click_app_template_demo_auto.py
```

### Comparing `click-app-template-demo-auto-0.2.0/.github/workflows/publish.yml` & `click-app-template-demo-auto-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/.github/workflows/test.yml` & `click-app-template-demo-auto-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/CHANGELOG.md` & `click-app-template-demo-auto-0.3.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.3.0 (2024-04-12)
+
+### Unknown
+
+* Demo of click-app 3bdd6a643cb88c943ab76cbae772feea8f3ec890 ([`0fe0b9b`](https://github.com/AH-Merii/click-app-template-demo-auto/commit/0fe0b9b431ce183c3ac158a6add732fb81bdf703))
+
+
 ## v0.2.0 (2024-04-12)
 
 ### Unknown
 
 * Demo of click-app c75ffe2b82ad4e550ccfb81ecbdc7b4f62a827ff ([`bcc9cd4`](https://github.com/AH-Merii/click-app-template-demo-auto/commit/bcc9cd48e91608e5e9480cb012dffeda189fd079))
```

### Comparing `click-app-template-demo-auto-0.2.0/LICENSE` & `click-app-template-demo-auto-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/Makefile` & `click-app-template-demo-auto-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/PKG-INFO` & `click-app-template-demo-auto-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-app-template-demo-auto
-Version: 0.2.0
+Version: 0.3.0
 Summary: Demonstrating https://github.com/AH-Merii/click-app
 Author: AbdulHamid Merii
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/AH-Merii/click-app-template-demo-auto
 Project-URL: Changelog, https://github.com/AH-Merii/click-app-template-demo-auto/releases
 Project-URL: Issues, https://github.com/AH-Merii/click-app-template-demo-auto/issues
 Project-URL: CI, https://github.com/AH-Merii/click-app-template-demo-auto/actions
```

### Comparing `click-app-template-demo-auto-0.2.0/README.md` & `click-app-template-demo-auto-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/click_app_template_demo_auto/cli.py` & `click-app-template-demo-auto-0.3.0/click_app_template_demo_auto/cli.py`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/PKG-INFO` & `click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-app-template-demo-auto
-Version: 0.2.0
+Version: 0.3.0
 Summary: Demonstrating https://github.com/AH-Merii/click-app
 Author: AbdulHamid Merii
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/AH-Merii/click-app-template-demo-auto
 Project-URL: Changelog, https://github.com/AH-Merii/click-app-template-demo-auto/releases
 Project-URL: Issues, https://github.com/AH-Merii/click-app-template-demo-auto/issues
 Project-URL: CI, https://github.com/AH-Merii/click-app-template-demo-auto/actions
```

### Comparing `click-app-template-demo-auto-0.2.0/click_app_template_demo_auto.egg-info/SOURCES.txt` & `click-app-template-demo-auto-0.3.0/click_app_template_demo_auto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `click-app-template-demo-auto-0.2.0/pyproject.toml` & `click-app-template-demo-auto-0.3.0/pyproject.toml`

 * *Files identical despite different names*

