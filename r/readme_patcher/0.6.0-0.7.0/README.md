# Comparing `tmp/readme_patcher-0.6.0.tar.gz` & `tmp/readme_patcher-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_patcher-0.6.0.tar", max compression
+gzip compressed data, was "readme_patcher-0.7.0.tar", max compression
```

## Comparing `readme_patcher-0.6.0.tar` & `readme_patcher-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1096 2022-07-17 07:04:29.513389 readme_patcher-0.6.0/LICENSE
--rw-r--r--   0        0        0     2654 2022-07-20 20:45:01.141849 readme_patcher-0.6.0/README.rst
--rw-r--r--   0        0        0      766 2022-07-20 21:00:04.791714 readme_patcher-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      924 2022-07-20 20:50:24.967366 readme_patcher-0.6.0/readme_patcher/__init__.py
--rw-r--r--   0        0        0     2074 2022-07-20 11:09:50.838659 readme_patcher-0.6.0/readme_patcher/badge.py
--rw-r--r--   0        0        0      373 2022-07-20 11:09:50.838659 readme_patcher-0.6.0/readme_patcher/config.py
--rw-r--r--   0        0        0     2410 2022-07-20 20:50:56.959904 readme_patcher-0.6.0/readme_patcher/file.py
--rw-r--r--   0        0        0     1598 2022-07-20 20:55:34.833802 readme_patcher-0.6.0/readme_patcher/filters.py
--rw-r--r--   0        0        0     1061 2022-07-20 19:49:13.612614 readme_patcher-0.6.0/readme_patcher/functions.py
--rw-r--r--   0        0        0      712 2022-07-20 11:09:50.842659 readme_patcher-0.6.0/readme_patcher/github.py
--rw-r--r--   0        0        0     2452 2022-07-20 19:49:13.612614 readme_patcher-0.6.0/readme_patcher/project.py
--rw-r--r--   0        0        0      944 2022-07-20 19:49:13.612614 readme_patcher-0.6.0/readme_patcher/py_project.py
--rw-r--r--   0        0        0     1240 2022-07-20 19:49:13.612614 readme_patcher-0.6.0/readme_patcher/template.py
--rw-r--r--   0        0        0     3792 1970-01-01 00:00:00.000000 readme_patcher-0.6.0/setup.py
--rw-r--r--   0        0        0     3503 1970-01-01 00:00:00.000000 readme_patcher-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2806 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/README.rst
+-rw-r--r--   0        0        0      744 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      924 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/readme_patcher/__init__.py
+-rw-r--r--   0        0        0     2096 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/readme_patcher/badge.py
+-rw-r--r--   0        0        0      373 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/readme_patcher/config.py
+-rw-r--r--   0        0        0     2410 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/readme_patcher/file.py
+-rw-r--r--   0        0        0     1598 2024-04-12 16:50:32.337362 readme_patcher-0.7.0/readme_patcher/filters.py
+-rw-r--r--   0        0        0     1060 2024-04-12 16:50:32.341362 readme_patcher-0.7.0/readme_patcher/functions.py
+-rw-r--r--   0        0        0      584 2024-04-12 16:50:32.341362 readme_patcher-0.7.0/readme_patcher/github.py
+-rw-r--r--   0        0        0     2504 2024-04-12 16:50:32.341362 readme_patcher-0.7.0/readme_patcher/project.py
+-rw-r--r--   0        0        0      944 2024-04-12 16:50:32.341362 readme_patcher-0.7.0/readme_patcher/py_project.py
+-rw-r--r--   0        0        0     1190 2024-04-12 16:50:32.341362 readme_patcher-0.7.0/readme_patcher/template.py
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 readme_patcher-0.7.0/PKG-INFO
```

### Comparing `readme_patcher-0.6.0/LICENSE` & `readme_patcher-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_patcher-0.6.0/README.rst` & `readme_patcher-0.7.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -29,19 +29,24 @@
 .. code-block:: jinja
 
     {{ py_project.repository }}
 
 github
 ^^^^^^
 
+https://docs.github.com/en/rest/repos/repos#get-a-repository
+
+https://api.github.com/repos/Josef-Friedrich/readme_patcher
+
 .. code-block:: jinja
 
     {{ github.name }}
     {{ github.full_name }}
     {{ github.description }}
+    {{ github.owner.login }}
 
 badge
 ^^^^^
 
 .. code-block:: jinja
 
     {{ badge.pypi }}
```

### Comparing `readme_patcher-0.6.0/pyproject.toml` & `readme_patcher-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "readme_patcher"
-version = "0.6.0"
+version = "0.7.0"
 description = "Generate README files from templates. Allow input from functions calls and cli output."
 authors = ["Josef Friedrich <josef@friedrich.rocks>"]
 readme = "README.rst"
 repository = "https://github.com/Josef-Friedrich/readme_patcher"
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Jinja2 = "^3.1.2"
-pyproject-parser = "^0.7.0"
+Jinja2 = "^3.1.3"
+pyproject-parser = "^0.11.0"
 requests = "^2"
-types-requests = "^2.28.2"
+types-requests = "^2"
 
 [tool.poetry.group.dev.dependencies]
-black = "22.6.0"
-isort = "^5.10.1"
+ruff = "^0"
+responses = "^0.25.0"
+pytest = "^8"
 
 [build-system]
-requires = ["poetry>=1.2.0b2", "setuptools", "setuptools-scm"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 "readme-patcher" = "readme_patcher:main"
```

### Comparing `readme_patcher-0.6.0/readme_patcher/__init__.py` & `readme_patcher-0.7.0/readme_patcher/__init__.py`

 * *Files identical despite different names*

### Comparing `readme_patcher-0.6.0/readme_patcher/badge.py` & `readme_patcher-0.7.0/readme_patcher/badge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 import typing
 from functools import cached_property
 from typing import Optional
 
 if typing.TYPE_CHECKING:
-    from .github import Github
+    from .github import GithubRepository
     from .project import Project
     from .py_project import SimplePyProject
 
 
 class Badge:
-
     project: "Project"
 
     def __init__(self, project: "Project"):
         self.project = project
 
     @cached_property
-    def _github(self) -> "Github":
+    def _github(self) -> "GithubRepository":
         if not self.project.github:
             raise Exception("No github repo found")
         return self.project.github
 
     @cached_property
     def _py_project(self) -> "SimplePyProject":
         if not self.project.py_project:
@@ -45,15 +44,15 @@
             "This package on the Python Package Index",
         )
 
     def github_workflow(
         self, workflow: str = "tests", alt: Optional[str] = "Tests"
     ) -> str:
         url = "https://github.com/{}/actions/workflows/{}.yml".format(
-            self._github.full_name, workflow
+            self._github["full_name"], workflow
         )
         return self._linked_image(url + "/badge.svg", url, alt)
 
     @cached_property
     def readthedocs(self) -> str:
         return self._linked_image(
             "https://readthedocs.org/projects/{}/badge/?version=latest".format(
```

### Comparing `readme_patcher-0.6.0/readme_patcher/file.py` & `readme_patcher-0.7.0/readme_patcher/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import typing
 from typing import Dict, Optional, TypedDict
 
 from jinja2 import Template
 
-from . import functions, config
+from . import config, functions
 
 if typing.TYPE_CHECKING:
     from .project import Project
 
 
 class Replacement:
     """A variable and its replacement text."""
```

### Comparing `readme_patcher-0.6.0/readme_patcher/filters.py` & `readme_patcher-0.7.0/readme_patcher/filters.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from __future__ import annotations
-
 """Custom jinja filters
 
 https://jinja.palletsprojects.com/en/3.1.x/api/#custom-filters
 """
 
+from __future__ import annotations
+
 from jinja2.filters import do_indent
 
 
 def _indent_block(content: str, strip_whitespace: bool = True) -> str:
     if strip_whitespace:
         content = content.strip()
     return "\n\n" + do_indent(content, width=4, first=True) + "\n\n"
```

### Comparing `readme_patcher-0.6.0/readme_patcher/functions.py` & `readme_patcher-0.7.0/readme_patcher/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from __future__ import annotations
-import os
-
 """https://jinja.palletsprojects.com/en/3.1.x/api/#custom-filters"""
 
+from __future__ import annotations
 
 import importlib
+import os
 import re
 import subprocess
 
 from jinja2 import pass_context
 from jinja2.runtime import Context
```

### Comparing `readme_patcher-0.6.0/readme_patcher/project.py` & `readme_patcher-0.7.0/readme_patcher/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Dict, List, Optional
-from jinja2 import Environment
 
+from jinja2 import Environment
 from pyproject_parser import PyProject
 
 from readme_patcher.template import setup_environment
 
 from .file import File, Variables
-from .github import Github
+from .github import GithubRepository, request_github_api
 from .py_project import SimplePyProject
 
 
 class Project:
     """A project corresponds to a code repository. In its root there is a
     README file."""
 
@@ -43,17 +43,17 @@
     @cached_property
     def py_project_config(self) -> Dict[str, Any] | None:
         if self._py_project and "readme_patcher" in self._py_project.tool:
             return self._py_project.tool["readme_patcher"]
         return None
 
     @cached_property
-    def github(self) -> Github | None:
+    def github(self) -> GithubRepository | None:
         if self.py_project and self.py_project.repository:
-            return Github(self.py_project.repository)
+            return request_github_api(self.py_project.repository)
         return None
 
     def patch_file(
         self, src: str, dest: str, variables: Optional[Variables] = None
     ) -> str:
         return File(project=self, src=src, dest=dest, variables=variables).patch()
```

### Comparing `readme_patcher-0.6.0/readme_patcher/py_project.py` & `readme_patcher-0.7.0/readme_patcher/py_project.py`

 * *Files identical despite different names*

### Comparing `readme_patcher-0.6.0/readme_patcher/template.py` & `readme_patcher-0.7.0/readme_patcher/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import os
 import typing
 
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 
 from . import filters, functions
 from .badge import Badge
-from .github import Github
 
 if typing.TYPE_CHECKING:
     from .project import Project
 
 
-def setup_environment(project: 'Project') -> Environment:
+def setup_environment(project: "Project") -> Environment:
     """
     Setup the search paths for the template engine Jinja2. ``os.path.sep`` is
 
     required to be able to include absolute paths, quotes around
     ``os.PathLike[str]`` to get py38 compatibility."""
     environment = Environment(
         loader=FileSystemLoader([project.base_dir, os.path.sep]),
@@ -27,15 +26,15 @@
 
     environment.globals.update(functions.collection)
     environment.globals.update(project=project)
     if project.py_project:
         environment.globals.update(py_project=project.py_project)
         if project.py_project.repository:
             try:
-                github = Github(project.py_project.repository)
+                github = project.github
                 environment.globals.update(github=github)
             except Exception:
                 pass
 
     environment.globals.update(badge=Badge(project))
 
     return environment
```

### Comparing `readme_patcher-0.6.0/PKG-INFO` & `readme_patcher-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
-Name: readme-patcher
-Version: 0.6.0
+Name: readme_patcher
+Version: 0.7.0
 Summary: Generate README files from templates. Allow input from functions calls and cli output.
 Home-page: https://github.com/Josef-Friedrich/readme_patcher
 License: MIT
 Author: Josef Friedrich
 Author-email: josef@friedrich.rocks
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pyproject-parser (>=0.7.0,<0.8.0)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: pyproject-parser (>=0.11.0,<0.12.0)
 Requires-Dist: requests (>=2,<3)
-Requires-Dist: types-requests (>=2.28.2,<3.0.0)
+Requires-Dist: types-requests (>=2,<3)
 Project-URL: Repository, https://github.com/Josef-Friedrich/readme_patcher
 Description-Content-Type: text/x-rst
 
 .. image:: http://img.shields.io/pypi/v/readme-patcher.svg
     :target: https://pypi.org/project/readme-patcher
     :alt: This package on the Python Package Index
 
@@ -50,19 +52,24 @@
 .. code-block:: jinja
 
     {{ py_project.repository }}
 
 github
 ^^^^^^
 
+https://docs.github.com/en/rest/repos/repos#get-a-repository
+
+https://api.github.com/repos/Josef-Friedrich/readme_patcher
+
 .. code-block:: jinja
 
     {{ github.name }}
     {{ github.full_name }}
     {{ github.description }}
+    {{ github.owner.login }}
 
 badge
 ^^^^^
 
 .. code-block:: jinja
 
     {{ badge.pypi }}
```

