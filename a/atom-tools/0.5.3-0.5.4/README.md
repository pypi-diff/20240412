# Comparing `tmp/atom-tools-0.5.3.tar.gz` & `tmp/atom-tools-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom-tools-0.5.3.tar", last modified: Mon Apr  8 16:50:58 2024, max compression
+gzip compressed data, was "atom-tools-0.5.4.tar", last modified: Fri Apr 12 05:38:35 2024, max compression
```

## Comparing `atom-tools-0.5.3.tar` & `atom-tools-0.5.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 16:50:36.000000 atom-tools-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-08 16:50:36.000000 atom-tools-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-08 16:50:58.544552 atom-tools-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-08 16:50:36.000000 atom-tools-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/command_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.540552 atom-tools-0.5.3/atom_tools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/query_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/commands/validate_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/cli/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/atom_tools/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/regex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-04-08 16:50:36.000000 atom-tools-0.5.3/atom_tools/lib/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/atom_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 16:50:58.000000 atom-tools-0.5.3/atom_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 16:50:36.000000 atom-tools-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:50:58.544552 atom-tools-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:50:58.544552 atom-tools-0.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-08 16:50:36.000000 atom-tools-0.5.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.727645 atom-tools-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 05:38:30.000000 atom-tools-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 05:38:30.000000 atom-tools-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-12 05:38:35.727645 atom-tools-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12133 2024-04-12 05:38:30.000000 atom-tools-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.719645 atom-tools-0.5.4/atom_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.723645 atom-tools-0.5.4/atom_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.723645 atom-tools-0.5.4/atom_tools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/commands/validate_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/cli/logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.723645 atom-tools-0.5.4/atom_tools/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/regex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-04-12 05:38:30.000000 atom-tools-0.5.4/atom_tools/lib/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.727645 atom-tools-0.5.4/atom_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13401 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 05:38:35.000000 atom-tools-0.5.4/atom_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-12 05:38:30.000000 atom-tools-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:38:35.727645 atom-tools-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:35.727645 atom-tools-0.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-12 05:38:30.000000 atom-tools-0.5.4/test/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-12 05:38:30.000000 atom-tools-0.5.4/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-12 05:38:30.000000 atom-tools-0.5.4/test/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-12 05:38:30.000000 atom-tools-0.5.4/test/test_utils.py
```

### Comparing `atom-tools-0.5.3/LICENSE` & `atom-tools-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/PKG-INFO` & `atom-tools-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.3
+Version: 0.5.4
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -146,14 +146,17 @@
 
 Regex word boundaries can be used if you only want to be exact about the filename.
 
 `filter --criteria filename=\bserver.ts$ -i usages.json`
 
 This will filter files named server.ts - without the \b, files like ftpserver.ts would also be matched.
 
+>Note: You can search for a file name without including the path if needed and fuzzing ratios will be computed based 
+> only on the file name.
+
 ##### Chaining filter commands
 
 The filter command can act on itself by specifying an additional filter command as an argument.
 This may desirable for certain use cases where one wishes some criteria to be required.
 
 **Example**
```

### Comparing `atom-tools-0.5.3/README.md` & `atom-tools-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
 
 Regex word boundaries can be used if you only want to be exact about the filename.
 
 `filter --criteria filename=\bserver.ts$ -i usages.json`
 
 This will filter files named server.ts - without the \b, files like ftpserver.ts would also be matched.
 
+>Note: You can search for a file name without including the path if needed and fuzzing ratios will be computed based 
+> only on the file name.
+
 ##### Chaining filter commands
 
 The filter command can act on itself by specifying an additional filter command as an argument.
 This may desirable for certain use cases where one wishes some criteria to be required.
 
 **Example**
```

### Comparing `atom-tools-0.5.3/atom_tools/cli/application.py` & `atom-tools-0.5.4/atom_tools/cli/application.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/cli/command_loader.py` & `atom-tools-0.5.4/atom_tools/cli/command_loader.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/cli/commands/convert.py` & `atom-tools-0.5.4/atom_tools/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/cli/commands/filter.py` & `atom-tools-0.5.4/atom_tools/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/cli/commands/query_endpoints.py` & `atom-tools-0.5.4/atom_tools/cli/commands/query_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,17 @@
         if self.option('type') not in supported_types:
             raise ValueError(f'Unknown origin type: {self.option("type")}')
         converter = OpenAPI(
             'openapi3.1.0',
             self.option('type'),
             self.option('input-slice'),
         )
-        if not (result := converter.endpoints_to_openapi('')):
-            logging.warning('No results produced!')
+        result = converter.endpoints_to_openapi('')
+        if not result.get('paths'):
+            logger.warning('No results produced!')
             print('')
         else:
             line_filter = ()
             if self.option('filter-lines'):
                 line_filter = get_ln_range(self.option('filter-lines'))
             output = output_endpoints(result, self.option('sparse'), line_filter)
             print(output)
```

### Comparing `atom-tools-0.5.3/atom_tools/cli/commands/validate_lines.py` & `atom-tools-0.5.4/atom_tools/cli/commands/validate_lines.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/cli/logging_config.py` & `atom-tools-0.5.4/atom_tools/cli/logging_config.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/lib/converter.py` & `atom-tools-0.5.4/atom_tools/lib/converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/lib/filtering.py` & `atom-tools-0.5.4/atom_tools/lib/filtering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Classes and functions for filtering slices"""
 import logging
+import pathlib
 import re
 from copy import deepcopy
 from dataclasses import dataclass
 from typing import Dict, Generator, List, Set, Tuple
 
 from thefuzz import fuzz, process  # type: ignore
 
@@ -16,15 +17,15 @@
 
 
 @dataclass
 class AttributeFilter:
     """Attribute filter class"""
     def __init__(self, key: str, value: str, condition: str, fuzz_pct: int | None) -> None:
         self.attribute = key.lower()
-        self.value, self.line_numbers = create_attribute_filter(value, fuzz_pct)
+        self.value, self.line_numbers, self.fn_only = create_attribute_filter(key, value, fuzz_pct)
         self.condition = condition
 
 
 class Filter:
     """Class for filtering a slice"""
     def __init__(self, slice_file: str, outfile: str, fuzz_pct: str | None) -> None:
         self.slc = FlatSlice(slice_file)
@@ -93,22 +94,23 @@
             filtered_slice[i.group('type')][int(i.group('index'))] = None
         for key, value in self.slc.content.items():
             for k, v in value.items():
                 if v is None:
                     filtered_slice[key].pop(k)
         return filtered_slice
 
-    def _process_fuzzy_results(self, f: AttributeFilter, result: List[Tuple[str, int]]) -> None:
+    def _process_fuzzy_results(
+            self, f: AttributeFilter, result: List[Tuple[str, int, str]]) -> None:
         include = []
         exclude = []
         for i in result:
             if f.condition == '==':
-                include.extend(self.slc.attrib_dicts.get(f.attribute, {}).get(i[0], []))
+                include.extend(self.slc.attrib_dicts.get(f.attribute, {}).get(i[2], []))
             else:
-                exclude.extend(self.slc.attrib_dicts.get(f.attribute, {}).get(i[0], []))
+                exclude.extend(self.slc.attrib_dicts.get(f.attribute, {}).get(i[2], []))
         self.results.extend(list(set(include)))
         self.negative_results.extend(list(set(exclude)))
 
     def _process_slice_indexes(self) -> Dict:
         include_indexes = set()
         exclude_indexes = set()
         for k in self.results:
@@ -122,40 +124,54 @@
     def _search_values(self, f: AttributeFilter) -> None:
         include = []
         exclude = []
         for k, v in self.slc.attrib_dicts.get(f.attribute, {}).items():
             if f.value.search(k):
                 if f.condition == '==':
                     include.extend(v)
-                    # self.found_keys.append(k)
                 else:
                     exclude.extend(v)
         self.results.extend(list(set(include)))
         self.negative_results.extend(list(set(exclude)))
 
     def _search_values_fuzzy(self, f: AttributeFilter) -> None:
         search_values = self.slc.attrib_dicts.get(f.attribute, {}).keys()
+        if f.fn_only:
+            search_values = {
+                i: f'{pathlib.Path(i).stem}{pathlib.Path(i).suffix}'
+                for i in search_values
+            }
+        else:
+            search_values = {i: i for i in search_values}
         if result := process.extractBests(
             f.value,
             search_values,
             limit=len(search_values),
             score_cutoff=self.fuzz,
             scorer=fuzz.ratio,
         ):
             self._process_fuzzy_results(f, result)
 
 
-def create_attribute_filter(value: str, fuzz_pct: int | None) -> Tuple:
+def create_attribute_filter(key: str, value: str, fuzz_pct: int | None) -> Tuple:
     """Create an attribute filter"""
     lns = ()
+    fn_only = False
+    if key.lower() == 'filename' and '/' not in value and '\\' not in value:
+        fn_only = True
     if ':' in value and (match := filtering.attribute_and_line.search(value)):
         value = match.group('attrib')
         lns = get_ln_range(match.group('line_nums'))
-    new_value = value if fuzz_pct else re.compile(value, re.IGNORECASE)
-    return new_value, lns
+    if fuzz_pct:
+        new_value = value
+    else:
+        if '.' in value:
+            value += '$'
+        new_value = re.compile(value, re.IGNORECASE)  # type: ignore
+    return new_value, lns, fn_only
 
 
 def get_ln_range(value: str) -> Tuple[int, int] | Tuple:
     """
     Extracts line numbers from arguments and returns a tuple of (start, end)
     """
     try:
```

### Comparing `atom-tools-0.5.3/atom_tools/lib/regex_utils.py` & `atom-tools-0.5.4/atom_tools/lib/regex_utils.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/lib/slices.py` & `atom-tools-0.5.4/atom_tools/lib/slices.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/lib/utils.py` & `atom-tools-0.5.4/atom_tools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools/lib/validator.py` & `atom-tools-0.5.4/atom_tools/lib/validator.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/atom_tools.egg-info/PKG-INFO` & `atom-tools-0.5.4/atom_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.3
+Version: 0.5.4
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -146,14 +146,17 @@
 
 Regex word boundaries can be used if you only want to be exact about the filename.
 
 `filter --criteria filename=\bserver.ts$ -i usages.json`
 
 This will filter files named server.ts - without the \b, files like ftpserver.ts would also be matched.
 
+>Note: You can search for a file name without including the path if needed and fuzzing ratios will be computed based 
+> only on the file name.
+
 ##### Chaining filter commands
 
 The filter command can act on itself by specifying an additional filter command as an argument.
 This may desirable for certain use cases where one wishes some criteria to be required.
 
 **Example**
```

### Comparing `atom-tools-0.5.3/atom_tools.egg-info/SOURCES.txt` & `atom-tools-0.5.4/atom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/pyproject.toml` & `atom-tools-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atom-tools"
-version = "0.5.3"
+version = "0.5.4"
 description = "Collection of tools for use with AppThreat/atom."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
 dependencies = ["cleo>=1.0.0", "jmespath>=1.0.0", "thefuzz>=0.22.1", "json-flatten>=0.3"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
```

### Comparing `atom-tools-0.5.3/test/test_converter.py` & `atom-tools-0.5.4/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/test/test_filtering.py` & `atom-tools-0.5.4/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/test/test_slices.py` & `atom-tools-0.5.4/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.3/test/test_utils.py` & `atom-tools-0.5.4/test/test_utils.py`

 * *Files identical despite different names*

