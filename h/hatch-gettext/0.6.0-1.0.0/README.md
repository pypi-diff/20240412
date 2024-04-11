# Comparing `tmp/hatch_gettext-0.6.0.tar.gz` & `tmp/hatch_gettext-1.0.0.tar.gz`

## Comparing `hatch_gettext-0.6.0.tar` & `hatch_gettext-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/CHANGES.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/hatch_gettext/__about__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/hatch_gettext/__init__.py
--rwxr-xr-x   0        0        0      282 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/hatch_gettext/hooks.py
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/hatch_gettext/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/hatch_gettext/py.typed
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/README.md
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    11261 2020-02-02 00:00:00.000000 hatch_gettext-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/CHANGES.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/__about__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/__init__.py
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/hooks.py
+-rw-r--r--   0        0        0    13707 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/hatch_gettext/py.typed
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/README.md
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13070 2020-02-02 00:00:00.000000 hatch_gettext-1.0.0/PKG-INFO
```

### Comparing `hatch_gettext-0.6.0/hatch_gettext/plugin.py` & `hatch_gettext-1.0.0/hatch_gettext/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: Copyright 2024 Damon Lynch <damonlynch@gmail.com>
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import functools
+import os
 import shlex
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 from typing import Any
 
@@ -153,19 +154,22 @@
 
     def load_gettextbuild_config(self) -> None:
         """
         Load the gettextbuild config from pyproject.toml using hatch's interface
         and assign the values to private class variables.
         """
 
-        self._i18n_name = self.config.get("i18n-name") or self.metadata.name
+        self._i18n_name: str = self.config.get("i18n-name") or self.metadata.name
+        self._identify_left_out: bool = self.config.get("identify-left-out", False)
+        self._regenerate_template: bool = self.config.get("regenerate-template", False)
+        self._show_report: bool = self.config.get("show-report", False)
 
         project_root = Path(self.root)
 
-        self._po_dir = project_root / (self.config.get("po-directory") or "po")
+        self._po_dir = project_root / (self.config.get("po-directory", "po"))
         if not self._po_dir.is_dir():
             raise ValueError(
                 f'Configure "po-directory" in "{self.config_name()}" in pyproject.toml '
                 'to the project\'s po directory [default: "po"], and ensure the '
                 "directory exists."
             )
         try:
@@ -196,27 +200,45 @@
     def po_mo_pairs(self) -> list[tuple[Path, str]]:
         """
         :return: a list of tuples containing po files, and their corresponding mo
          filenames that the build will create.
 
          Each po file will be a full Path, but the mo files' path will be a string
          whose path is relative to the project root.
+
+         If a LINGUAS file is found in the po directory or as an environment variable,
+         only specified po files will be included.
         """
 
+        filter_languages: list[str] = []
+        linguas_file = self._po_dir / "LINGUAS"
+        if linguas_file.is_file():
+            with open(linguas_file) as f:
+                filter_languages = f.read().split()
+        if "LINGUAS" in os.environ:
+            filter_languages = os.environ["LINGUAS"].split()
+
+        po_files = self._po_dir.glob("*.po")
+        if filter_languages:
+            po_files = (p for p in po_files if p.stem in filter_languages)
+
+        po_files = list(po_files)
+        po_files.sort()
+
         return [
             (
                 Path(po_file),
                 str(
                     Path(self.config["locale-directory"])
                     / po_file.stem
                     / "LC_MESSAGES"
                     / f"{self._i18n_name}.mo"
                 ),
             )
-            for po_file in self._po_dir.glob("*.po")
+            for po_file in po_files
         ]
 
     @functools.cache
     def translate_file_pairs(self) -> list[tuple[Path, str]]:
         """
         :return: a list of tuples containing .in files, and their corresponding
          files to be translated by intltool-merge that the build will create.
@@ -275,17 +297,50 @@
         project_root: Path = Path(self.root)
         for in_file, to_translate in self.translate_file_pairs():
             path_to_translate = project_root / to_translate
             path_to_translate.parent.mkdir(parents=True, exist_ok=True)
             self.console_output(f'Translating "{path_to_translate.stem}"', level=2)
             self._translate_file(self._po_dir, in_file, path_to_translate)
 
+    def identify_left_out(self) -> None:
+        cmd = self._assemble_command("intltool-update -m")
+        p = subprocess.run(
+            cmd,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            text=True,
+            cwd=self._po_dir,
+        )
+        if p.stdout:
+            self.console_output(p.stdout, level=0, style=self._style_level_error)
+            raise ValueError("Files missing from translation template")
+
+    def regenerate_template(self) -> None:
+        cmd = self._assemble_command(f"intltool-update -p -g {self._i18n_name}")
+        self.console_output(
+            "Regenerating .pot template", level=2, style=self._style_level_debug
+        )
+        subprocess.run(cmd, check=True, cwd=self._po_dir)
+
+    def show_report(self) -> None:
+        cmd = self._assemble_command(f"intltool-update -r -g {self._i18n_name}")
+        self.console_output("Generating report", level=2, style=self._style_level_debug)
+        subprocess.run(cmd, check=True, cwd=self._po_dir)
+
     def do_work(self, build_data: dict[str, Any]) -> None:
         self.load_gettextbuild_config()
 
+        if self.target_name == "sdist":
+            if self._identify_left_out:
+                self.identify_left_out()
+            if self._regenerate_template:
+                self.regenerate_template()
+            if self._show_report:
+                self.show_report()
+
         build_data["artifacts"].extend(self.mo_files_to_build)
         self.compile_mo_files()
 
         if self._gtb_files:
             build_data["artifacts"].extend(self.translate_files_to_build)
             self.translate_files()
```

### Comparing `hatch_gettext-0.6.0/.gitignore` & `hatch_gettext-1.0.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -156,8 +156,31 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+# User-specific stuff
+.idea/**/workspace.xml
+.idea/**/tasks.xml
+.idea/**/usage.statistics.xml
+.idea/**/dictionaries
+.idea/**/shelf
+
+# AWS User-specific
+.idea/**/aws.xml
+
+# Generated files
+.idea/**/contentModel.xml
+
+# Sensitive or high-churn files
+.idea/**/dataSources/
+.idea/**/dataSources.ids
+.idea/**/dataSources.local.xml
+.idea/**/sqlDataSources.xml
+.idea/**/dynamic.xml
+.idea/**/uiDesigner.xml
+.idea/**/dbnavigator.xml
+
+# Mypy
 mypy.ini
```

### Comparing `hatch_gettext-0.6.0/LICENSE.txt` & `hatch_gettext-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_gettext-0.6.0/README.md` & `hatch_gettext-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,25 +6,35 @@
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![GitButler](https://img.shields.io/badge/GitButler-%23B9F4F2?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCAzOSAyOCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTI1LjIxNDUgMTIuMTk5N0wyLjg3MTA3IDEuMzg5MTJDMS41NDI5NSAwLjc0NjUzMiAwIDEuNzE0MDYgMCAzLjE4OTQ3VjI0LjgxMDVDMCAyNi4yODU5IDEuNTQyOTUgMjcuMjUzNSAyLjg3MTA3IDI2LjYxMDlMMjUuMjE0NSAxNS44MDAzQzI2LjcxOTcgMTUuMDcyMSAyNi43MTk3IDEyLjkyNzkgMjUuMjE0NSAxMi4xOTk3WiIgZmlsbD0iYmxhY2siLz4KPHBhdGggZD0iTTEzLjc4NTUgMTIuMTk5N0wzNi4xMjg5IDEuMzg5MTJDMzcuNDU3MSAwLjc0NjUzMiAzOSAxLjcxNDA2IDM5IDMuMTg5NDdWMjQuODEwNUMzOSAyNi4yODU5IDM3LjQ1NzEgMjcuMjUzNSAzNi4xMjg5IDI2LjYxMDlMMTMuNzg1NSAxNS44MDAzQzEyLjI4MDMgMTUuMDcyMSAxMi4yODAzIDEyLjkyNzkgMTMuNzg1NSAxMi4xOTk3WiIgZmlsbD0idXJsKCNwYWludDBfcmFkaWFsXzMxMF8xMjkpIi8%2BCjxkZWZzPgo8cmFkaWFsR3JhZGllbnQgaWQ9InBhaW50MF9yYWRpYWxfMzEwXzEyOSIgY3g9IjAiIGN5PSIwIiByPSIxIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgZ3JhZGllbnRUcmFuc2Zvcm09InRyYW5zbGF0ZSgxNi41NzAxIDE0KSBzY2FsZSgxOS44NjQxIDE5LjgzODMpIj4KPHN0b3Agb2Zmc2V0PSIwLjMwMTA1NiIgc3RvcC1vcGFjaXR5PSIwIi8%2BCjxzdG9wIG9mZnNldD0iMSIvPgo8L3JhZGlhbEdyYWRpZW50Pgo8L2RlZnM%2BCjwvc3ZnPgo%3D)](https://gitbutler.com/) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![GitHub Sponsors](https://img.shields.io/github/sponsors/damonlynch?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/damonlynch)  |
 
 
 -----
 
 This provides a [build hook](https://hatch.pypa.io/latest/config/build/#build-hooks) plugin 
 for [Hatch](https://github.com/pypa/hatch) that compiles multi-lingual messages with GNU 
-gettext's tools `msgfmt` and (optionally) translates files using 
-gettext's `intltool-merge`.
+gettext's tools `msgfmt`. It can also (optionally) use `intltool` to: 
+- translate .xml and .desktop files
+- search for left out files
+- regenerate the .pot template 
+- display a status report for all translations
 
 **Table of Contents**
 
-- [Configuration](#configuration)
-  - [Calling the plugin](#calling-the-plugin)
-  - [Compiling messages with msgfmt](#compiling-messages-with-msgfmt)
-  - [Translating files using intltool-merge](#translating-files-using-intltool-merge)
-- [Cleaning output files](#cleaning-output-files)
-- [License](#license)
+<!-- TOC -->
+* [Hatch Gettext](#hatch-gettext)
+  * [Configuration](#configuration)
+    * [Calling the plugin](#calling-the-plugin)
+    * [Compiling messages with msgfmt](#compiling-messages-with-msgfmt)
+    * [Identifying left out files using intltool-update](#identifying-left-out-files-using-intltool-update)
+    * [Regenerating the .pot template using intltool-update](#regenerating-the-pot-template-using-intltool-update)
+    * [Displaying a status report using intltool-update](#displaying-a-status-report-using-intltool-update)
+    * [Translating files using intltool-merge](#translating-files-using-intltool-merge)
+  * [Cleaning output files](#cleaning-output-files)
+  * [Related Hatch plugin](#related-hatch-plugin)
+  * [License](#license)
+<!-- TOC -->
 
 ## Configuration
 
 The [build hook plugin](https://hatch.pypa.io/latest/plugins/build-hook/) 
 name is `gettext`.
 
 ### Calling the plugin
@@ -38,15 +48,16 @@
 ```
 
 ### Compiling messages with msgfmt
  
 This plugin requires `.mo` files be created; it also requires that the 
 directory storing them is within the project's base directory, and is not 
 equal to the project's base directory or the directory in which `po` files
-are sourced.  
+are sourced. The mo file directory is set using `locale-directory`, which is 
+required. 
 
 For example, for a project named `myproject`, and a src layout 
 `src/myproject`, an acceptable directory in which to store the 
 `LC_MESSAGES/myproject.mo` files would be `src/myproject/locale`
 
 ```toml
 [tool.hatch.build.hooks.gettext]
@@ -63,14 +74,48 @@
 po-directory = "po-files"
 ```
 
 If `i18n-name` is not specified, the `name` in `[project]` in the 
 `pyproject.toml` is used. If `po-directory` is not specified, the 
 directory `po` is used.
 
+### Identifying left out files using intltool-update
+
+With every source distribution (sdist) build, to search for left out files, 
+which should have been listed in `POTFILES.in` or `POTFILES.skip`, set 
+`identify-left-out` to true (the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+identify-left-out = true
+```
+
+### Regenerating the .pot template using intltool-update
+
+To regenerate the .pot template with every sdist build, set 
+`regenerate-template` to true (the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+regenerate-template = true
+```
+
+### Displaying a status report using intltool-update
+
+To display a status report for all translations, set `show-report` to true 
+(the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+show-report = true
+```
+
 ### Translating files using intltool-merge
 
 This plugin allows for but does not mandate translating `.xml` and 
 `.desktop` files using `intltool-merge`. Using 
 `[tool.hatch.build.hooks.gettext.files]`, specify the destination directories
 for the translated files on the left, and arrays of source files on the 
 right. For example:  
@@ -85,10 +130,15 @@
 ## Cleaning output files
 
 The plugin includes logic to remove the files it outputs using hatch's
 `clean` hook. As well as individual files, any output directories created 
 will also be removed, as long as these directories do not contain files 
 created by something other than this plugin.
 
+## Related Hatch plugin
+
+To automatically generate a manual page from an `ArgumentParser` object,
+see [hatch-argparse-manpage](https://github.com/damonlynch/hatch-argparse-manpage).
+
 ## License
 
 `hatch-gettext` is distributed under the terms of the [GPL-3.0-or-later](https://spdx.org/licenses/GPL-3.0-or-later.html) license.
```

### Comparing `hatch_gettext-0.6.0/pyproject.toml` & `hatch_gettext-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -17,28 +17,43 @@
   "plugin",
   "typing",
 ]
 authors = [
   { name = "Damon Lynch", email = "damonlynch@gmail.com" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 5 - Production/Stable",
   "Framework :: Hatch",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
+  "Typing :: Typed",
 ]
 dependencies = ["rich", ]
 
 [project.urls]
 Documentation = "https://github.com/damonlynch/hatch-gettext#readme"
 Issues = "https://github.com/damonlynch/hatch-gettext/issues"
 Homepage = "https://github.com/damonlynch/hatch-gettext"
 
 [project.entry-points.hatch]
 gettext = "hatch_gettext.hooks"
 
 [tool.hatch.version]
 path = "hatch_gettext/__about__.py"
+
+[tool.ruff.lint]
+select = [
+    # pycodestyle
+    "E",
+    # Pyflakes
+    "F",
+    # pyupgrade
+    "UP",
+    # flake8-simplify
+    "SIM",
+    # isort
+    "I",
+]
```

### Comparing `hatch_gettext-0.6.0/PKG-INFO` & `hatch_gettext-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.3
 Name: hatch-gettext
-Version: 0.6.0
+Version: 1.0.0
 Summary: Hatch build hook plugin for GNU gettext
 Project-URL: Documentation, https://github.com/damonlynch/hatch-gettext#readme
 Project-URL: Issues, https://github.com/damonlynch/hatch-gettext/issues
 Project-URL: Homepage, https://github.com/damonlynch/hatch-gettext
 Author-email: Damon Lynch <damonlynch@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
 Keywords: build,gettext,hatch,i18n,plugin,typing
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # Hatch Gettext
 
 | |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
@@ -29,25 +30,35 @@
 | Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![GitButler](https://img.shields.io/badge/GitButler-%23B9F4F2?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCAzOSAyOCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTI1LjIxNDUgMTIuMTk5N0wyLjg3MTA3IDEuMzg5MTJDMS41NDI5NSAwLjc0NjUzMiAwIDEuNzE0MDYgMCAzLjE4OTQ3VjI0LjgxMDVDMCAyNi4yODU5IDEuNTQyOTUgMjcuMjUzNSAyLjg3MTA3IDI2LjYxMDlMMjUuMjE0NSAxNS44MDAzQzI2LjcxOTcgMTUuMDcyMSAyNi43MTk3IDEyLjkyNzkgMjUuMjE0NSAxMi4xOTk3WiIgZmlsbD0iYmxhY2siLz4KPHBhdGggZD0iTTEzLjc4NTUgMTIuMTk5N0wzNi4xMjg5IDEuMzg5MTJDMzcuNDU3MSAwLjc0NjUzMiAzOSAxLjcxNDA2IDM5IDMuMTg5NDdWMjQuODEwNUMzOSAyNi4yODU5IDM3LjQ1NzEgMjcuMjUzNSAzNi4xMjg5IDI2LjYxMDlMMTMuNzg1NSAxNS44MDAzQzEyLjI4MDMgMTUuMDcyMSAxMi4yODAzIDEyLjkyNzkgMTMuNzg1NSAxMi4xOTk3WiIgZmlsbD0idXJsKCNwYWludDBfcmFkaWFsXzMxMF8xMjkpIi8%2BCjxkZWZzPgo8cmFkaWFsR3JhZGllbnQgaWQ9InBhaW50MF9yYWRpYWxfMzEwXzEyOSIgY3g9IjAiIGN5PSIwIiByPSIxIiBncmFkaWVudFVuaXRzPSJ1c2VyU3BhY2VPblVzZSIgZ3JhZGllbnRUcmFuc2Zvcm09InRyYW5zbGF0ZSgxNi41NzAxIDE0KSBzY2FsZSgxOS44NjQxIDE5LjgzODMpIj4KPHN0b3Agb2Zmc2V0PSIwLjMwMTA1NiIgc3RvcC1vcGFjaXR5PSIwIi8%2BCjxzdG9wIG9mZnNldD0iMSIvPgo8L3JhZGlhbEdyYWRpZW50Pgo8L2RlZnM%2BCjwvc3ZnPgo%3D)](https://gitbutler.com/) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) [![GitHub Sponsors](https://img.shields.io/github/sponsors/damonlynch?logo=GitHub%20Sponsors&style=social)](https://github.com/sponsors/damonlynch)  |
 
 
 -----
 
 This provides a [build hook](https://hatch.pypa.io/latest/config/build/#build-hooks) plugin 
 for [Hatch](https://github.com/pypa/hatch) that compiles multi-lingual messages with GNU 
-gettext's tools `msgfmt` and (optionally) translates files using 
-gettext's `intltool-merge`.
+gettext's tools `msgfmt`. It can also (optionally) use `intltool` to: 
+- translate .xml and .desktop files
+- search for left out files
+- regenerate the .pot template 
+- display a status report for all translations
 
 **Table of Contents**
 
-- [Configuration](#configuration)
-  - [Calling the plugin](#calling-the-plugin)
-  - [Compiling messages with msgfmt](#compiling-messages-with-msgfmt)
-  - [Translating files using intltool-merge](#translating-files-using-intltool-merge)
-- [Cleaning output files](#cleaning-output-files)
-- [License](#license)
+<!-- TOC -->
+* [Hatch Gettext](#hatch-gettext)
+  * [Configuration](#configuration)
+    * [Calling the plugin](#calling-the-plugin)
+    * [Compiling messages with msgfmt](#compiling-messages-with-msgfmt)
+    * [Identifying left out files using intltool-update](#identifying-left-out-files-using-intltool-update)
+    * [Regenerating the .pot template using intltool-update](#regenerating-the-pot-template-using-intltool-update)
+    * [Displaying a status report using intltool-update](#displaying-a-status-report-using-intltool-update)
+    * [Translating files using intltool-merge](#translating-files-using-intltool-merge)
+  * [Cleaning output files](#cleaning-output-files)
+  * [Related Hatch plugin](#related-hatch-plugin)
+  * [License](#license)
+<!-- TOC -->
 
 ## Configuration
 
 The [build hook plugin](https://hatch.pypa.io/latest/plugins/build-hook/) 
 name is `gettext`.
 
 ### Calling the plugin
@@ -61,15 +72,16 @@
 ```
 
 ### Compiling messages with msgfmt
  
 This plugin requires `.mo` files be created; it also requires that the 
 directory storing them is within the project's base directory, and is not 
 equal to the project's base directory or the directory in which `po` files
-are sourced.  
+are sourced. The mo file directory is set using `locale-directory`, which is 
+required. 
 
 For example, for a project named `myproject`, and a src layout 
 `src/myproject`, an acceptable directory in which to store the 
 `LC_MESSAGES/myproject.mo` files would be `src/myproject/locale`
 
 ```toml
 [tool.hatch.build.hooks.gettext]
@@ -86,14 +98,48 @@
 po-directory = "po-files"
 ```
 
 If `i18n-name` is not specified, the `name` in `[project]` in the 
 `pyproject.toml` is used. If `po-directory` is not specified, the 
 directory `po` is used.
 
+### Identifying left out files using intltool-update
+
+With every source distribution (sdist) build, to search for left out files, 
+which should have been listed in `POTFILES.in` or `POTFILES.skip`, set 
+`identify-left-out` to true (the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+identify-left-out = true
+```
+
+### Regenerating the .pot template using intltool-update
+
+To regenerate the .pot template with every sdist build, set 
+`regenerate-template` to true (the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+regenerate-template = true
+```
+
+### Displaying a status report using intltool-update
+
+To display a status report for all translations, set `show-report` to true 
+(the default value is false):
+
+```toml
+[tool.hatch.build.hooks.gettext]
+locale-directory = "src/myproject/locale"
+show-report = true
+```
+
 ### Translating files using intltool-merge
 
 This plugin allows for but does not mandate translating `.xml` and 
 `.desktop` files using `intltool-merge`. Using 
 `[tool.hatch.build.hooks.gettext.files]`, specify the destination directories
 for the translated files on the left, and arrays of source files on the 
 right. For example:  
@@ -108,10 +154,15 @@
 ## Cleaning output files
 
 The plugin includes logic to remove the files it outputs using hatch's
 `clean` hook. As well as individual files, any output directories created 
 will also be removed, as long as these directories do not contain files 
 created by something other than this plugin.
 
+## Related Hatch plugin
+
+To automatically generate a manual page from an `ArgumentParser` object,
+see [hatch-argparse-manpage](https://github.com/damonlynch/hatch-argparse-manpage).
+
 ## License
 
 `hatch-gettext` is distributed under the terms of the [GPL-3.0-or-later](https://spdx.org/licenses/GPL-3.0-or-later.html) license.
```

