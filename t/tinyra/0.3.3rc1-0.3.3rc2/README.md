# Comparing `tmp/tinyra-0.3.3rc1.tar.gz` & `tmp/tinyra-0.3.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyra-0.3.3rc1.tar", last modified: Fri Apr 12 08:43:18 2024, max compression
+gzip compressed data, was "tinyra-0.3.3rc2.tar", last modified: Fri Apr 12 08:52:30 2024, max compression
```

## Comparing `tinyra-0.3.3rc1.tar` & `tinyra-0.3.3rc2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.641446 tinyra-0.3.3rc1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:35:52.000000 tinyra-0.3.3rc1/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-12 08:43:18.641446 tinyra-0.3.3rc1/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      723 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.601446 tinyra-0.3.3rc1/tinyra/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-02 06:05:20.000000 tinyra-0.3.3rc1/tinyra/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.617446 tinyra-0.3.3rc1/tinyra/agents/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1046 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/agents.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12401 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/agents/autogen_agents.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1521 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/app_config.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.617446 tinyra-0.3.3rc1/tinyra/database/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1632 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/database.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15395 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/database/database_sqllite.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/exceptions.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1909 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/files.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/llm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      759 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/messages.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.621446 tinyra-0.3.3rc1/tinyra/profiler/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/profiler/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6190 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/profiler/profiler.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.633446 tinyra-0.3.3rc1/tinyra/screens/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4043 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/chat_display.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.633446 tinyra-0.3.3rc1/tinyra/screens/learning/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1231 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3724 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/preference_learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4507 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/learning/tool_learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1722 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/monitoring.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1825 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/notifications.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3201 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/profiler_screen.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      893 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/quit_screen.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11063 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/settings.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2967 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/screens/sidebar.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1585 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tools.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2966 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tui.css
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9659 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/tui.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-12 08:42:51.000000 tinyra-0.3.3rc1/tinyra/version.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/tinyra/widgets/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/widgets/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1638 2024-04-12 08:41:36.000000 tinyra-0.3.3rc1/tinyra/widgets/custom_widgets.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:43:18.637446 tinyra-0.3.3rc1/tinyra.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1059 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-04-12 08:43:18.000000 tinyra-0.3.3rc1/tinyra.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:35:52.000000 tinyra-0.3.3rc2/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      723 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.453458 tinyra-0.3.3rc2/tinyra/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-02 06:05:20.000000 tinyra-0.3.3rc2/tinyra/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.457459 tinyra-0.3.3rc2/tinyra/agents/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1046 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12401 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/autogen_agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1521 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/app_config.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.457459 tinyra-0.3.3rc2/tinyra/database/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1632 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/database.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15395 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/database_sqllite.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1909 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/files.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/llm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      759 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/messages.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/profiler/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/profiler/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6190 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/profiler/profiler.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/screens/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4043 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/chat_display.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/screens/learning/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1231 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3724 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/preference_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4507 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/tool_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1722 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/monitoring.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1825 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/notifications.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3201 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/profiler_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      893 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/quit_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11063 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/settings.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2024-04-12 08:50:26.000000 tinyra-0.3.3rc2/tinyra/screens/sidebar.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1585 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/tools.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2885 2024-04-12 08:50:42.000000 tinyra-0.3.3rc2/tinyra/tui.css
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9626 2024-04-12 08:46:55.000000 tinyra-0.3.3rc2/tinyra/tui.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-12 08:52:07.000000 tinyra-0.3.3rc2/tinyra/version.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/tinyra/widgets/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/widgets/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1638 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/widgets/custom_widgets.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/tinyra.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1059 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/top_level.txt
```

### Comparing `tinyra-0.3.3rc1/README.md` & `tinyra-0.3.3rc2/README.md`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/setup.py` & `tinyra-0.3.3rc2/setup.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/agents/agents.py` & `tinyra-0.3.3rc2/tinyra/agents/agents.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/agents/autogen_agents.py` & `tinyra-0.3.3rc2/tinyra/agents/autogen_agents.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/app_config.py` & `tinyra-0.3.3rc2/tinyra/app_config.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/database/database.py` & `tinyra-0.3.3rc2/tinyra/database/database.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/database/database_sqllite.py` & `tinyra-0.3.3rc2/tinyra/database/database_sqllite.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/files.py` & `tinyra-0.3.3rc2/tinyra/files.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/llm.py` & `tinyra-0.3.3rc2/tinyra/llm.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/messages.py` & `tinyra-0.3.3rc2/tinyra/messages.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/profiler/profiler.py` & `tinyra-0.3.3rc2/tinyra/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/chat_display.py` & `tinyra-0.3.3rc2/tinyra/screens/chat_display.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/learning/learning.py` & `tinyra-0.3.3rc2/tinyra/screens/learning/learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/learning/preference_learning.py` & `tinyra-0.3.3rc2/tinyra/screens/learning/preference_learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/learning/tool_learning.py` & `tinyra-0.3.3rc2/tinyra/screens/learning/tool_learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/monitoring.py` & `tinyra-0.3.3rc2/tinyra/screens/monitoring.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/notifications.py` & `tinyra-0.3.3rc2/tinyra/screens/notifications.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/profiler_screen.py` & `tinyra-0.3.3rc2/tinyra/screens/profiler_screen.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/quit_screen.py` & `tinyra-0.3.3rc2/tinyra/screens/quit_screen.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/settings.py` & `tinyra-0.3.3rc2/tinyra/screens/settings.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/screens/sidebar.py` & `tinyra-0.3.3rc2/tinyra/screens/sidebar.py`

 * *Files 24% similar despite different names*

```diff
@@ -44,14 +44,53 @@
             await fm.open_file(event.path)
         except Exception as e:
             raise FileManagerError(f"Error opening file {event.path}", e)
 
 
 class Sidebar(Grid):
 
+    DEFAULT_CSS = """
+    Sidebar {
+        width: 40%;
+        background: $panel;
+        border: thick $primary-background 90%;
+        transition: offset 500ms in_out_cubic;
+        layer: overlay;
+        margin: 1;
+        padding: 1;
+
+        grid-size: 1 2;
+        grid-rows: 1fr 5;
+        grid-gutter: 1 2;
+    }
+
+    Sidebar:focus-within {
+        offset: 0 0 !important;
+    }
+
+    Sidebar.-hidden {
+        offset-x: -100%;
+    }
+
+    Sidebar Static {
+        background: $boost;
+        color: $secondary;
+        border-right: vkey $background;
+        dock: top;
+        text-align: center;
+        text-style: bold;
+    }
+
+    #directory-tree-footer{
+        grid-size: 2 1;
+        align: center middle;
+    }
+
+    """
+
     def compose(self) -> ComposeResult:
         logger = logging.getLogger(__name__)
         logger.info("Composing the sidebar")
 
         yield Static("Work Directory")
 
         yield DirectoryTreeContainer(id="directory-tree")
```

### Comparing `tinyra-0.3.3rc1/tinyra/tools.py` & `tinyra-0.3.3rc2/tinyra/tools.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra/tui.css` & `tinyra-0.3.3rc2/tinyra/tui.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-* {
-    transition: background 500ms in_out_cubic, color 500ms in_out_cubic;
-}
-
 Screen {
     layers: base overlay top;
     overflow: hidden;
 }
 
 Header {
     layer: top;
 }
 
 Footer {
     layer: top;
 }
 
 
-
 #chat-grid{
     margin: 2;
 
     layout: grid;
     grid-size: 1 2;
     grid-gutter: 2 1;
```

### Comparing `tinyra-0.3.3rc1/tinyra/tui.py` & `tinyra-0.3.3rc2/tinyra/tui.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     BINDINGS = [
         ("ctrl+b", "toggle_sidebar", "Work Directory"),
         ("ctrl+c", "request_quit", "Quit"),
         ("ctrl+s", "request_settings", "Settings"),
     ]
 
-    CSS_PATH = ["tui.css", Path("screens") / "sidebar.css"]
+    CSS_PATH = ["tui.css"]
 
     TITLE = "TinyRA"
     SUB_TITLE = "A minimalistic, long-lived research assistant"
 
     def __init__(self, *args, app_config: AppConfiguration, **kwargs):
         super().__init__(*args, **kwargs)
         self.config = app_config
```

### Comparing `tinyra-0.3.3rc1/tinyra/widgets/custom_widgets.py` & `tinyra-0.3.3rc2/tinyra/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc1/tinyra.egg-info/SOURCES.txt` & `tinyra-0.3.3rc2/tinyra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

