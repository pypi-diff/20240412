# Comparing `tmp/tues-3.1.1.tar.gz` & `tmp/tues-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tues-3.1.1.tar", last modified: Thu Mar 21 12:26:35 2024, max compression
+gzip compressed data, was "tues-3.1.2.tar", last modified: Fri Apr 12 07:00:15 2024, max compression
```

## Comparing `tues-3.1.1.tar` & `tues-3.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.364827 tues-3.1.1/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1109 2023-07-20 11:22:00.000000 tues-3.1.1/LICENSE.txt
--rw-r--r--   0 marc      (1000) marc      (1000)     6425 2024-03-21 12:26:35.364827 tues-3.1.1/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     4219 2023-07-20 11:22:00.000000 tues-3.1.1/README.md
--rw-rw-r--   0 marc      (1000) marc      (1000)     1234 2024-03-21 12:25:35.000000 tues-3.1.1/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2024-03-21 12:26:35.364827 tues-3.1.1/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.360827 tues-3.1.1/src/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.360827 tues-3.1.1/src/tues/
--rw-rw-r--   0 marc      (1000) marc      (1000)    38074 2024-03-21 12:13:25.000000 tues-3.1.1/src/tues/__init__.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.360827 tues-3.1.1/src/tues/cli/
--rwxrwxr-x   0 marc      (1000) marc      (1000)     8598 2024-03-12 13:36:35.000000 tues-3.1.1/src/tues/cli/tues.py
--rwxrwxr-x   0 marc      (1000) marc      (1000)      249 2023-07-20 11:22:00.000000 tues-3.1.1/src/tues/cli/tues_provider_cl.py
--rwxrwxr-x   0 marc      (1000) marc      (1000)      451 2023-07-20 11:22:00.000000 tues-3.1.1/src/tues/cli/tues_provider_file.py
--rwxrwxr-x   0 marc      (1000) marc      (1000)     1123 2024-03-14 14:26:13.000000 tues-3.1.1/src/tues/cli/tues_provider_fm.py
--rwxrwxr-x   0 marc      (1000) marc      (1000)     1028 2023-07-20 11:22:00.000000 tues-3.1.1/src/tues/cli/tues_provider_icinga2.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.360827 tues-3.1.1/src/tues.egg-info/
--rw-r--r--   0 marc      (1000) marc      (1000)     6425 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)      429 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      267 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/entry_points.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)      127 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/requires.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        5 2024-03-21 12:26:35.000000 tues-3.1.1/src/tues.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-03-21 12:26:35.360827 tues-3.1.1/test/
--rw-rw-r--   0 marc      (1000) marc      (1000)    15363 2024-03-21 12:11:50.000000 tues-3.1.1/test/test_tues.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.544903 tues-3.1.2/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1109 2023-07-20 11:22:00.000000 tues-3.1.2/LICENSE.txt
+-rw-r--r--   0 marc      (1000) marc      (1000)     6425 2024-04-12 07:00:15.544903 tues-3.1.2/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4219 2023-07-20 11:22:00.000000 tues-3.1.2/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1234 2024-04-12 06:58:52.000000 tues-3.1.2/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2024-04-12 07:00:15.544903 tues-3.1.2/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.540903 tues-3.1.2/src/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.540903 tues-3.1.2/src/tues/
+-rw-rw-r--   0 marc      (1000) marc      (1000)    38204 2024-04-12 06:53:02.000000 tues-3.1.2/src/tues/__init__.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.544903 tues-3.1.2/src/tues/cli/
+-rwxrwxr-x   0 marc      (1000) marc      (1000)     8598 2024-03-12 13:36:35.000000 tues-3.1.2/src/tues/cli/tues.py
+-rwxrwxr-x   0 marc      (1000) marc      (1000)      249 2023-07-20 11:22:00.000000 tues-3.1.2/src/tues/cli/tues_provider_cl.py
+-rwxrwxr-x   0 marc      (1000) marc      (1000)      451 2023-07-20 11:22:00.000000 tues-3.1.2/src/tues/cli/tues_provider_file.py
+-rwxrwxr-x   0 marc      (1000) marc      (1000)     1123 2024-03-14 14:26:13.000000 tues-3.1.2/src/tues/cli/tues_provider_fm.py
+-rwxrwxr-x   0 marc      (1000) marc      (1000)     1028 2023-07-20 11:22:00.000000 tues-3.1.2/src/tues/cli/tues_provider_icinga2.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.544903 tues-3.1.2/src/tues.egg-info/
+-rw-r--r--   0 marc      (1000) marc      (1000)     6425 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)      429 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      267 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/entry_points.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)      127 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/requires.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        5 2024-04-12 07:00:15.000000 tues-3.1.2/src/tues.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2024-04-12 07:00:15.544903 tues-3.1.2/test/
+-rw-rw-r--   0 marc      (1000) marc      (1000)    15363 2024-03-21 12:11:50.000000 tues-3.1.2/test/test_tues.py
```

### Comparing `tues-3.1.1/LICENSE.txt` & `tues-3.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tues-3.1.1/PKG-INFO` & `tues-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tues
-Version: 3.1.1
+Version: 3.1.2
 Summary: Easy remote command execution
 Author-email: Michael van Bracht <michael@wontfix.org>, Marc Schmitzer <marc@solute.de>, Roland Sommer <rol@ndsommer.de>
 License: The MIT License (MIT)
         
         Copyright (c) 2014-2023, Michael van Bracht and contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tues-3.1.1/README.md` & `tues-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tues-3.1.1/pyproject.toml` & `tues-3.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tues"
-version = "3.1.1"
+version = "3.1.2"
 description = "Easy remote command execution"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Michael van Bracht", email = "michael@wontfix.org"},
     {name = "Marc Schmitzer", email = "marc@solute.de"},
```

### Comparing `tues-3.1.1/src/tues/__init__.py` & `tues-3.1.2/src/tues/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,17 @@
         self.returncode = None
         self._stdout = None
         self._stderr = None
         self.preexec_fn = preexec_fn
         self.postexec_fn = postexec_fn
         self.authorization_failed = False
 
+    def __repr__(self):
+        return f"<{type(self).__name__} cmd={self.cmd!r} host={self.host!r} at 0x{id(self):x}>"
+
     @property
     def sudo(self):
         """Whether the task requires use of `sudo`"""
         return self.user is not None and self.user != self.login_user
 
     @property
     def stdout(self):
@@ -858,15 +861,15 @@
             result, exc = None, err
         else:
             result, exc = _collect(atask)
 
         if task.authorization_failed:
             raise TuesUserAbort("Sudo authorization failed")
         if exc or (check and result.returncode > 0):
-            raise TuesTaskError(task)
+            raise TuesTaskError(task) from exc
         results.append(result)
 
     return results
 
 
 def _collect(atask):
     if atask.cancelled():
```

### Comparing `tues-3.1.1/src/tues/cli/tues.py` & `tues-3.1.2/src/tues/cli/tues.py`

 * *Files identical despite different names*

### Comparing `tues-3.1.1/src/tues/cli/tues_provider_fm.py` & `tues-3.1.2/src/tues/cli/tues_provider_fm.py`

 * *Files identical despite different names*

### Comparing `tues-3.1.1/src/tues/cli/tues_provider_icinga2.py` & `tues-3.1.2/src/tues/cli/tues_provider_icinga2.py`

 * *Files identical despite different names*

### Comparing `tues-3.1.1/src/tues.egg-info/PKG-INFO` & `tues-3.1.2/src/tues.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tues
-Version: 3.1.1
+Version: 3.1.2
 Summary: Easy remote command execution
 Author-email: Michael van Bracht <michael@wontfix.org>, Marc Schmitzer <marc@solute.de>, Roland Sommer <rol@ndsommer.de>
 License: The MIT License (MIT)
         
         Copyright (c) 2014-2023, Michael van Bracht and contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tues-3.1.1/test/test_tues.py` & `tues-3.1.2/test/test_tues.py`

 * *Files identical despite different names*

