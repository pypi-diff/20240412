# Comparing `tmp/walkmate-1.3.1.tar.gz` & `tmp/walkmate-1.4.0.tar.gz`

## Comparing `walkmate-1.3.1.tar` & `walkmate-1.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 walkmate-1.3.1/src/__init__.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 walkmate-1.3.1/src/files.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 walkmate-1.3.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 walkmate-1.3.1/LICENSE.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 walkmate-1.3.1/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 walkmate-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 walkmate-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 walkmate-1.4.0/src/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 walkmate-1.4.0/src/files.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 walkmate-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 walkmate-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 walkmate-1.4.0/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 walkmate-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 walkmate-1.4.0/PKG-INFO
```

### Comparing `walkmate-1.3.1/src/files.py` & `walkmate-1.4.0/src/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import re
-from typing import Generator, List, Optional, Tuple, Iterator
+from typing import Generator, List, Optional, Tuple
 
 
 def step(
     root: str, depth: Optional[int] = None
 ) -> Generator[Tuple[str, List[str]], None, None]:
     """
     Step into the file tree
@@ -32,26 +32,26 @@
         if "__pycache__" in subdirs:
             subdirs.remove("__pycache__")
 
         yield (folder, files)
 
 
 def tree(
-    root: str, depth: Optional[int] = None, regex: Optional[str] = None
-) -> Iterator[str]:
+    root: str, regex: Optional[str] = None, depth: Optional[int] = None
+) -> List[str]:
     """
     Traverse the file tree
 
     Args:
         root (str): The root directory.
-        depth (Optional[int], optional): The maximum depth. Defaults to None.
         regex (Optional[str], optional): The regex to match. Defaults to None.
+        depth (Optional[int], optional): The maximum depth. Defaults to None.
 
     Returns:
         Iterator[str]: An iterator containing the file paths
     """
-    return (
+    return [
         os.path.join(folder, file)
         for folder, files in step(root, depth)
         for file in files
         if regex is None or re.search(regex, file)
-    )
+    ]
```

### Comparing `walkmate-1.3.1/LICENSE.md` & `walkmate-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `walkmate-1.3.1/pyproject.toml` & `walkmate-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "walkmate"
-version = "1.3.1"
+version = "1.4.0"
 description = "Traverse the file tree."
 
 dependencies = []
 requires-python = ">=3.6"
 
 license = { file = "LICENSE.md" }
 readme = "README.md"
```

### Comparing `walkmate-1.3.1/PKG-INFO` & `walkmate-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: walkmate
-Version: 1.3.1
+Version: 1.4.0
 Summary: Traverse the file tree.
 Project-URL: Homepage, https://github.com/JoelLefkowitz/walkmate
 Author-email: Joel Lefkowitz <joellefkowitz@hotmail.com>
 License: # MIT License
         
         Copyright (c) 2024 Joel Lefkowitz
```

