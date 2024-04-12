# Comparing `tmp/tinyra-0.3.2rc1.tar.gz` & `tmp/tinyra-0.3.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyra-0.3.2rc1.tar", last modified: Wed Mar 27 03:55:59 2024, max compression
+gzip compressed data, was "tinyra-0.3.3rc1.tar", last modified: Fri Apr 12 08:43:18 2024, max compression
```

## Comparing `tinyra-0.3.2rc1.tar` & `tinyra-0.3.3rc1.tar`

### file list

```diff
@@ -1,17 +1,51 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-27 03:55:59.120327 tinyra-0.3.2rc1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-03-27 03:55:59.120327 tinyra-0.3.2rc1/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:36:57.000000 tinyra-0.3.2rc1/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-03-27 03:55:59.120327 tinyra-0.3.2rc1/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      657 2024-03-26 06:20:30.000000 tinyra-0.3.2rc1/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-27 03:55:59.116327 tinyra-0.3.2rc1/tinyra/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-03-26 06:36:06.000000 tinyra-0.3.2rc1/tinyra/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6159 2024-03-27 03:53:31.000000 tinyra-0.3.2rc1/tinyra/tui.css
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    44583 2024-03-27 03:53:31.000000 tinyra-0.3.2rc1/tinyra/tui.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-03-27 03:55:44.000000 tinyra-0.3.2rc1/tinyra/version.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-03-27 03:55:59.120327 tinyra-0.3.2rc1/tinyra.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      266 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-03-27 03:55:58.000000 tinyra-0.3.2rc1/tinyra.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.641446 tinyra-0.3.3rc1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:35:52.000000 tinyra-0.3.3rc1/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-12 08:43:18.641446 tinyra-0.3.3rc1/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      723 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.601446 tinyra-0.3.3rc1/tinyra/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-02 06:05:20.000000 tinyra-0.3.3rc1/tinyra/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.617446 tinyra-0.3.3rc1/tinyra/agents/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1046 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12401 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/autogen_agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1521 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/app_config.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.617446 tinyra-0.3.3rc1/tinyra/database/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1632 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/database.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15395 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/database_sqllite.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1909 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/files.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/llm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      759 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/messages.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.621446 tinyra-0.3.3rc1/tinyra/profiler/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/profiler/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6190 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/profiler/profiler.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.633446 tinyra-0.3.3rc1/tinyra/screens/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4043 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/chat_display.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.633446 tinyra-0.3.3rc1/tinyra/screens/learning/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1231 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3724 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/preference_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4507 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/tool_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1722 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/monitoring.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1825 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/notifications.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3201 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/profiler_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      893 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/quit_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11063 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/settings.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2967 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/sidebar.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1585 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tools.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2966 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tui.css
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9659 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tui.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-12 08:42:51.000000 tinyra-0.3.3rc1/tinyra/version.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/tinyra/widgets/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/widgets/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1638 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/widgets/custom_widgets.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/tinyra.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1059 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/top_level.txt
```

### Comparing `tinyra-0.3.2rc1/README.md` & `tinyra-0.3.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.2rc1/setup.py` & `tinyra-0.3.3rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # setup.py
 import os
-from setuptools import setup
+from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 requirements = ["textual[syntax]", "tiktoken", "pyautogen", "aiosqlite"]
 
 version = {}
 with open(os.path.join(here, "tinyra/version.py")) as fp:
     exec(fp.read(), version)
 __version__ = version["__version__"]
 
 setup(
     name="tinyra",
     version=__version__,
     description="A minimalistic, terminal-based research assistant built with AutoGen.",
-    packages=["tinyra"],
+    packages=find_packages(),  # This will find all packages and subpackages
     package_data={"tinyra": ["*"]},
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "tinyra = tinyra:run_app",
         ],
     },
-)
+)
```

