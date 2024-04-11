# Comparing `tmp/pytest_nlcov-0.2.0.tar.gz` & `tmp/pytest_nlcov-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_nlcov-0.2.0.tar", max compression
+gzip compressed data, was "pytest_nlcov-0.3.0.tar", max compression
```

## Comparing `pytest_nlcov-0.2.0.tar` & `pytest_nlcov-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1119 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/README.md
--rw-r--r--   0        0        0     1285 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4909 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pytest_nlcov/__init__.py
--rw-r--r--   0        0        0     2525 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pytest_nlcov/cov.py
--rw-r--r--   0        0        0      571 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pytest_nlcov/data.py
--rw-r--r--   0        0        0     1282 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pytest_nlcov/format.py
--rw-r--r--   0        0        0     1079 2021-07-07 17:51:56.815132 pytest_nlcov-0.2.0/pytest_nlcov/git.py
--rw-r--r--   0        0        0     2094 2021-07-07 17:52:06.570848 pytest_nlcov-0.2.0/setup.py
--rw-r--r--   0        0        0     1929 2021-07-07 17:52:06.571208 pytest_nlcov-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1358 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/README.md
+-rw-r--r--   0        0        0     1177 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4834 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pytest_nlcov/__init__.py
+-rw-r--r--   0        0        0     2527 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pytest_nlcov/cov.py
+-rw-r--r--   0        0        0      571 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pytest_nlcov/data.py
+-rw-r--r--   0        0        0     1244 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pytest_nlcov/format.py
+-rw-r--r--   0        0        0     1103 2024-04-11 22:40:37.212545 pytest_nlcov-0.3.0/pytest_nlcov/git.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 pytest_nlcov-0.3.0/PKG-INFO
```

### Comparing `pytest_nlcov-0.2.0/README.md` & `pytest_nlcov-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,25 +28,30 @@
 - fail threshold
 
 ### Revision
 
 Default, the new lines are based on the git diff with master. You can specify other revisions.
 
 ```sh
-pytest --nlcov-revision main
+pytest --cov=myproj --nlcov-revision main
 ```
 
 ### Fail Threshold
 
 Optionally you can add a threshold to fail the tests when the coverage is below the threshold.
 
 ```sh
-pytest --nlcov-fail-under 0.6
+pytest --cov=myproj --nlcov-fail-under 0.6
 ```
 
+### Note
+It's important to include `--cov` to load the **pytest_cov** plugin; otherwise an error message will appear saying:
+> nlcov is installed, but pytest-cov is not installed, so nlcov will not be executed.
+
+
 ## Usage without pytest
 
 `pytest_nlcov` can be run without pytest. Therefor you have to run `coverage` first, because `pytest_nlcov`
 needs its coverage data.
 
 ```sh
 coverage
```

### Comparing `pytest_nlcov-0.2.0/pytest_nlcov/__init__.py` & `pytest_nlcov-0.3.0/pytest_nlcov/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 
 import pytest
 import typer
 
-from .cov import mark_coveraged_lines_per_file
-from .cov import mark_executable_lines_per_file
-from .format import format_lines
-from .git import get_new_lines_per_file
+from pytest_nlcov.cov import mark_coveraged_lines_per_file
+from pytest_nlcov.cov import mark_executable_lines_per_file
+from pytest_nlcov.format import format_lines
+from pytest_nlcov.git import get_new_lines_per_file
 
 
 def make_relative(path: pathlib.Path) -> str:
     return str(path.relative_to(str(pathlib.Path(".").resolve())))
 
 
 def nl_cov(revision: str = "master") -> float:
@@ -24,16 +24,14 @@
 
     mark_executable_lines_per_file(new_lines_per_file)
     mark_coveraged_lines_per_file(new_lines_per_file)
 
     # Prepare the formatting strings, header, and column sorting.
     max_name = max([len(make_relative(p)) for p in new_lines_per_file] + [5])
     fmt_name = "%%- %ds  " % max_name
-    fmt_skip_covered = "\n%s file%s skipped due to complete coverage."
-    fmt_skip_empty = "\n%s empty file%s skipped."
 
     header = (fmt_name % "Name") + " Lines   Miss"
     fmt_coverage = fmt_name + "%6d %6d"
 
     header += "%*s" % (9, "Cover")
     fmt_coverage += " %%%ds" % (8,)
 
@@ -44,15 +42,15 @@
 
     # Write the header
     typer.echo(header)
     typer.echo(rule)
 
     total_num_newlines = 0
     total_num_covered = 0
-    for (p, new_lines) in new_lines_per_file.items():
+    for p, new_lines in new_lines_per_file.items():
         num_newlines = len(
             [lineno for lineno, line in new_lines.items() if line.is_empty is False and line.is_executable is True]
         )
 
         if num_newlines == 0:
             continue
```

### Comparing `pytest_nlcov-0.2.0/pytest_nlcov/cov.py` & `pytest_nlcov-0.3.0/pytest_nlcov/cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 
 from coverage import CoverageData
 from coverage import parser
 
-from .data import LinesPerFile
+from pytest_nlcov.data import LinesPerFile
 
 
 def get_coverage_data():
     coverage_data = CoverageData()
     coverage_data.read()
 
     return {
@@ -26,30 +26,30 @@
     not_covered_newline_files = newline_files - covered_files
     for file in not_covered_newline_files:
         del lines_per_file[file]
 
     for measured_file, coveraged_linenos in coverage_data.items():
         if measured_file not in lines_per_file:
             continue
-        for coveraged_lineno in coveraged_linenos:
+        for coveraged_lineno in coveraged_linenos or []:
             if coveraged_lineno not in lines_per_file[measured_file]:
                 continue
             lines_per_file[measured_file][coveraged_lineno].is_executed = True
             for subline in lines_per_file[measured_file][coveraged_lineno].multilines or []:
                 lines_per_file[measured_file][subline].is_executed = True
 
 
 def get_python_parser(file_path) -> parser.PythonParser:
     parsed_file = parser.PythonParser(filename=file_path)
     parsed_file.parse_source()
 
     return parsed_file
 
 
-def mark_executable_lines_per_file(lines_per_file: LinesPerFile) -> LinesPerFile:
+def mark_executable_lines_per_file(lines_per_file: LinesPerFile):
     """
     Mark the executable lines based on a Python parser.
     When a line is marked as new and it belongs to a multiline statement,
     the first line of that statement is added and marked as new too.
     """
     for file_path, lines in lines_per_file.items():
         parsed_file = get_python_parser(file_path)
```

### Comparing `pytest_nlcov-0.2.0/pytest_nlcov/data.py` & `pytest_nlcov-0.3.0/pytest_nlcov/data.py`

 * *Files identical despite different names*

### Comparing `pytest_nlcov-0.2.0/pytest_nlcov/format.py` & `pytest_nlcov-0.3.0/pytest_nlcov/format.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from typing import Iterator
-from typing import List
-from typing import Tuple
+from typing import Iterator, List, Tuple
 
 
 def list_to_ranges(lines: List[int]) -> List[Tuple[int, int]]:
     """Produce a list of ranges for `format_lines`.
 
     >>> list_to_ranges([1,2,3,4])
     [(1, 4)]
@@ -18,40 +16,40 @@
     []
 
 
     """
     lines = sorted(lines)
 
     pairs = []
-    start = None
-    prev_line = None
+    start = -1
+    prev_line = -1
     for line in lines:
-        if start is None:
+        if start == -1:
             start = prev_line = line
             continue
 
         if line == prev_line + 1:
             prev_line = line
             continue
 
         pairs.append((start, prev_line))
         start = prev_line = line
 
-    if start and prev_line:
+    if start != -1 and prev_line:
         pairs.append((start, prev_line))
 
     return pairs
 
 
 def format_ranges(pairs: List[Tuple[int, int]]) -> Iterator[str]:
     """
     >>> list(format_ranges([(1,2), (3,3), (4,20)]))
     ['1-2', '3', '4-20']
     """
-    for (start, end) in pairs:
+    for start, end in pairs:
         if start == end:
             yield f"{start}"
         else:
             yield f"{start}-{end}"
 
 
 def format_lines(lines: List[int]):
```

### Comparing `pytest_nlcov-0.2.0/pytest_nlcov/git.py` & `pytest_nlcov-0.3.0/pytest_nlcov/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pathlib
 from io import StringIO
 from typing import Optional
 
 import git
 from unidiff import PatchSet
 
-from .data import LinesPerFile
-from .data import lines_per_file_factory
+from pytest_nlcov.data import LinesPerFile
+from pytest_nlcov.data import lines_per_file_factory
 
 
 def get_diff(revision: str):
     return git.Repo(".").git.diff(revision, ignore_blank_lines=True, ignore_space_at_eol=True)
 
 
 def get_new_lines_per_file(revision: str, glob: Optional[str] = None) -> LinesPerFile:
```

### Comparing `pytest_nlcov-0.2.0/PKG-INFO` & `pytest_nlcov-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
-Name: pytest-nlcov
-Version: 0.2.0
+Name: pytest_nlcov
+Version: 0.3.0
 Summary: Pytest plugin to get the coverage of the new lines (based on git diff) only
 Home-page: https://github.com/mrijken/pytest_nlcov
 License: MIT
 Author: Marc Rijken
 Author-email: marc@rijken.org
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: GitPython (>=3.1.17)
 Requires-Dist: coverage (>=5.5)
 Requires-Dist: pytest-cov (>=2.10.1)
 Requires-Dist: typer (>=0.3.2)
 Requires-Dist: unidiff (>=0.6.0)
 Project-URL: Repository, https://github.com/mrijken/pytest_nlcov
 Description-Content-Type: text/markdown
@@ -50,25 +52,30 @@
 - fail threshold
 
 ### Revision
 
 Default, the new lines are based on the git diff with master. You can specify other revisions.
 
 ```sh
-pytest --nlcov-revision main
+pytest --cov=myproj --nlcov-revision main
 ```
 
 ### Fail Threshold
 
 Optionally you can add a threshold to fail the tests when the coverage is below the threshold.
 
 ```sh
-pytest --nlcov-fail-under 0.6
+pytest --cov=myproj --nlcov-fail-under 0.6
 ```
 
+### Note
+It's important to include `--cov` to load the **pytest_cov** plugin; otherwise an error message will appear saying:
+> nlcov is installed, but pytest-cov is not installed, so nlcov will not be executed.
+
+
 ## Usage without pytest
 
 `pytest_nlcov` can be run without pytest. Therefor you have to run `coverage` first, because `pytest_nlcov`
 needs its coverage data.
 
 ```sh
 coverage
```

