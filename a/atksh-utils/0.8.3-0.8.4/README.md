# Comparing `tmp/atksh-utils-0.8.3.tar.gz` & `tmp/atksh-utils-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.8.3.tar", last modified: Thu Mar 28 12:53:57 2024, max compression
+gzip compressed data, was "atksh-utils-0.8.4.tar", last modified: Fri Apr 12 03:34:23 2024, max compression
```

## Comparing `atksh-utils-0.8.3.tar` & `atksh-utils-0.8.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.958907 atksh-utils-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.958907 atksh-utils-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 12:53:57.966907 atksh-utils-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.958907 atksh-utils-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.958907 atksh-utils-0.8.3/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/src/atksh_utils/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/basic/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/src/atksh_utils/nlp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/nlp/str_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6316 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/askgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/src/atksh_utils/openai/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 12:53:57.000000 atksh-utils-0.8.3/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:57.962907 atksh-utils-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:53:50.000000 atksh-utils-0.8.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.403105 atksh-utils-0.8.4/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/basic/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/nlp/str_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.407105 atksh-utils-0.8.4/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6309 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/askgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/src/atksh_utils/openai/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 03:34:23.000000 atksh-utils-0.8.4/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:23.411105 atksh-utils-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:34:18.000000 atksh-utils-0.8.4/tests/__init__.py
```

### Comparing `atksh-utils-0.8.3/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.8.4/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/.gitignore` & `atksh-utils-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/LICENSE` & `atksh-utils-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/PKG-INFO` & `atksh-utils-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.3
+Version: 0.8.4
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.8.3/README.md` & `atksh-utils-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/pyproject.toml` & `atksh-utils-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/basic/functools.py` & `atksh-utils-0.8.4/src/atksh_utils/basic/functools.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/nlp/str_kernel.py` & `atksh-utils-0.8.4/src/atksh_utils/nlp/str_kernel.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/api.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/askgpt.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/askgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         tokens.append(token)
         if token.endswith("\n"):
             print_tokens()
 
 
 def setup_ai() -> OpenAI:
     key = os.getenv("OPENAI_API_KEY")
-    ai = OpenAI(key, "gpt-4-0125-preview")
+    ai = OpenAI(key, "gpt-4-turbo")
     ai.set_browser_functions()
     ai.set_python_functions()
     ai.set_bash_function()
     ai.set_utility_functions()
     return ai
```

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/functional.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/prompt.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/prompt.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/token.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/token.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils/openai/tool.py` & `atksh-utils-0.8.4/src/atksh_utils/openai/tool.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.8.3/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.8.4/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.8.3
+Version: 0.8.4
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.8.3/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.8.4/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

