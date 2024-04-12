# Comparing `tmp/tinyra-0.3.3rc2.tar.gz` & `tmp/tinyra-0.3.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyra-0.3.3rc2.tar", last modified: Fri Apr 12 08:52:30 2024, max compression
+gzip compressed data, was "tinyra-0.3.3rc3.tar", last modified: Fri Apr 12 08:58:48 2024, max compression
```

## Comparing `tinyra-0.3.3rc2.tar` & `tinyra-0.3.3rc3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:35:52.000000 tinyra-0.3.3rc2/README.md
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/setup.cfg
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      723 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/setup.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.453458 tinyra-0.3.3rc2/tinyra/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-02 06:05:20.000000 tinyra-0.3.3rc2/tinyra/__init__.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.457459 tinyra-0.3.3rc2/tinyra/agents/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1046 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/agents.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12401 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/agents/autogen_agents.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1521 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/app_config.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.457459 tinyra-0.3.3rc2/tinyra/database/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1632 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/database.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15395 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/database/database_sqllite.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/exceptions.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1909 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/files.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/llm.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      759 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/messages.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/profiler/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/profiler/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6190 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/profiler/profiler.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/screens/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4043 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/chat_display.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.461459 tinyra-0.3.3rc2/tinyra/screens/learning/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1231 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3724 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/preference_learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4507 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/learning/tool_learning.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1722 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/monitoring.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1825 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/notifications.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3201 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/profiler_screen.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)      893 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/quit_screen.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11063 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/screens/settings.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2024-04-12 08:50:26.000000 tinyra-0.3.3rc2/tinyra/screens/sidebar.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1585 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/tools.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2885 2024-04-12 08:50:42.000000 tinyra-0.3.3rc2/tinyra/tui.css
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9626 2024-04-12 08:46:55.000000 tinyra-0.3.3rc2/tinyra/tui.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-12 08:52:07.000000 tinyra-0.3.3rc2/tinyra/version.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/tinyra/widgets/
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/widgets/__init__.py
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1638 2024-04-12 08:41:36.000000 tinyra-0.3.3rc2/tinyra/widgets/custom_widgets.py
-drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:52:30.465458 tinyra-0.3.3rc2/tinyra.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/PKG-INFO
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1059 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/SOURCES.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/dependency_links.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/entry_points.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/requires.txt
--rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-04-12 08:52:30.000000 tinyra-0.3.3rc2/tinyra.egg-info/top_level.txt
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1607 2024-03-26 05:35:52.000000 tinyra-0.3.3rc3/README.md
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       38 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/setup.cfg
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      723 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/setup.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.785467 tinyra-0.3.3rc3/tinyra/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-02 06:05:20.000000 tinyra-0.3.3rc3/tinyra/__init__.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.785467 tinyra-0.3.3rc3/tinyra/agents/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/agents/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1046 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/agents/agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    12401 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/agents/autogen_agents.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1521 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/app_config.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.789467 tinyra-0.3.3rc3/tinyra/database/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/database/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1632 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/database/database.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    15395 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/database/database_sqllite.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      277 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/exceptions.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1909 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/files.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1284 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/llm.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)      759 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/messages.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.789467 tinyra-0.3.3rc3/tinyra/profiler/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/profiler/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     6190 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/profiler/profiler.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.789467 tinyra-0.3.3rc3/tinyra/screens/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4043 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/chat_display.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/tinyra/screens/learning/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/learning/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1231 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/learning/learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3724 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/learning/preference_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     4507 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/learning/tool_learning.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1722 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/monitoring.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1825 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/notifications.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3201 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/profiler_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1350 2024-04-12 08:57:10.000000 tinyra-0.3.3rc3/tinyra/screens/quit_screen.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)    11063 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/screens/settings.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     3706 2024-04-12 08:50:26.000000 tinyra-0.3.3rc3/tinyra/screens/sidebar.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1585 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/tools.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     2700 2024-04-12 08:57:58.000000 tinyra-0.3.3rc3/tinyra/tui.css
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     9626 2024-04-12 08:46:55.000000 tinyra-0.3.3rc3/tinyra/tui.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       25 2024-04-12 08:58:31.000000 tinyra-0.3.3rc3/tinyra/version.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/tinyra/widgets/
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/widgets/__init__.py
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1638 2024-04-12 08:41:36.000000 tinyra-0.3.3rc3/tinyra/widgets/custom_widgets.py
+drwxrwxrwx   0 vscode    (1000) vscode    (1000)        0 2024-04-12 08:58:48.793467 tinyra-0.3.3rc3/tinyra.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      237 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/PKG-INFO
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)     1059 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/SOURCES.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        1 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/dependency_links.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       42 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/entry_points.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)       45 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/requires.txt
+-rw-rw-rw-   0 vscode    (1000) vscode    (1000)        7 2024-04-12 08:58:48.000000 tinyra-0.3.3rc3/tinyra.egg-info/top_level.txt
```

### Comparing `tinyra-0.3.3rc2/README.md` & `tinyra-0.3.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/setup.py` & `tinyra-0.3.3rc3/setup.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/agents/agents.py` & `tinyra-0.3.3rc3/tinyra/agents/agents.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/agents/autogen_agents.py` & `tinyra-0.3.3rc3/tinyra/agents/autogen_agents.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/app_config.py` & `tinyra-0.3.3rc3/tinyra/app_config.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/database/database.py` & `tinyra-0.3.3rc3/tinyra/database/database.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/database/database_sqllite.py` & `tinyra-0.3.3rc3/tinyra/database/database_sqllite.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/files.py` & `tinyra-0.3.3rc3/tinyra/files.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/llm.py` & `tinyra-0.3.3rc3/tinyra/llm.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/messages.py` & `tinyra-0.3.3rc3/tinyra/messages.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/profiler/profiler.py` & `tinyra-0.3.3rc3/tinyra/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/chat_display.py` & `tinyra-0.3.3rc3/tinyra/screens/chat_display.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/learning/learning.py` & `tinyra-0.3.3rc3/tinyra/screens/learning/learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/learning/preference_learning.py` & `tinyra-0.3.3rc3/tinyra/screens/learning/preference_learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/learning/tool_learning.py` & `tinyra-0.3.3rc3/tinyra/screens/learning/tool_learning.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/monitoring.py` & `tinyra-0.3.3rc3/tinyra/screens/monitoring.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/notifications.py` & `tinyra-0.3.3rc3/tinyra/screens/notifications.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/profiler_screen.py` & `tinyra-0.3.3rc3/tinyra/screens/profiler_screen.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/settings.py` & `tinyra-0.3.3rc3/tinyra/screens/settings.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/screens/sidebar.py` & `tinyra-0.3.3rc3/tinyra/screens/sidebar.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/tools.py` & `tinyra-0.3.3rc3/tinyra/tools.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/tui.css` & `tinyra-0.3.3rc3/tinyra/tui.css`

 * *Files 3% similar despite different names*

```diff
@@ -66,26 +66,14 @@
 
 .assistant-message {
     border: $primary;
     margin-left: 10;
     content-align: left middle;
 }
 
-
-#quit-screen-grid {
-    height: 40%;
-    width: 40%;
-    background: $surface;
-    border: thick $primary-background 80%;
-    padding: 1;
-
-    grid-size: 2 3;
-    grid-gutter: 1 2;
-}
-
 #chat-screen-contents {
     border: solid $background 40%;
 }
 
 #chat-screen-footer {
     column-span: 2;
     height: 5;
```

### Comparing `tinyra-0.3.3rc2/tinyra/tui.py` & `tinyra-0.3.3rc3/tinyra/tui.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra/widgets/custom_widgets.py` & `tinyra-0.3.3rc3/tinyra/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `tinyra-0.3.3rc2/tinyra.egg-info/SOURCES.txt` & `tinyra-0.3.3rc3/tinyra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

