# Comparing `tmp/unityparser-3.0.1.tar.gz` & `tmp/unityparser-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unityparser-3.0.1.tar", last modified: Wed Jul 26 14:13:05 2023, max compression
+gzip compressed data, was "unityparser-4.0.0.tar", last modified: Fri Apr 12 09:28:17 2024, max compression
```

## Comparing `unityparser-3.0.1.tar` & `unityparser-4.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.649252 unityparser-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 14:12:45.000000 unityparser-3.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 14:12:45.000000 unityparser-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 14:12:45.000000 unityparser-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-26 14:13:05.649252 unityparser-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 14:12:45.000000 unityparser-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.641251 unityparser-3.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/development.in
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/publish.in
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/publish.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 14:13:05.649252 unityparser-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-26 14:12:45.000000 unityparser-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.645251 unityparser-3.0.1/unityparser/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 14:13:02.000000 unityparser-3.0.1/unityparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/representer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.649252 unityparser-3.0.1/unityparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:28:17.842365 unityparser-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 09:28:01.000000 unityparser-4.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 09:28:01.000000 unityparser-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 09:28:01.000000 unityparser-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-12 09:28:17.842365 unityparser-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-12 09:28:01.000000 unityparser-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:28:17.838365 unityparser-4.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/development.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/publish.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-12 09:28:01.000000 unityparser-4.0.0/requirements/publish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 09:28:17.842365 unityparser-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-12 09:28:01.000000 unityparser-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:28:17.842365 unityparser-4.0.0/unityparser/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 09:28:14.000000 unityparser-4.0.0/unityparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/representer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-12 09:28:01.000000 unityparser-4.0.0/unityparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:28:17.842365 unityparser-4.0.0/unityparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-12 09:28:17.000000 unityparser-4.0.0/unityparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 09:28:17.000000 unityparser-4.0.0/unityparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:28:17.000000 unityparser-4.0.0/unityparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 09:28:17.000000 unityparser-4.0.0/unityparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 09:28:17.000000 unityparser-4.0.0/unityparser.egg-info/top_level.txt
```

### Comparing `unityparser-3.0.1/LICENSE` & `unityparser-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/PKG-INFO` & `unityparser-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 3.0.1
+Version: 4.0.0
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
```

### Comparing `unityparser-3.0.1/README.md` & `unityparser-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/requirements/ci.txt` & `unityparser-4.0.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/requirements/development.txt` & `unityparser-4.0.0/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/requirements/publish.txt` & `unityparser-4.0.0/requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/setup.py` & `unityparser-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/commands.py` & `unityparser-4.0.0/unityparser/commands.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/composer.py` & `unityparser-4.0.0/unityparser/composer.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/constants.py` & `unityparser-4.0.0/unityparser/constants.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/constructor.py` & `unityparser-4.0.0/unityparser/constructor.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/dumper.py` & `unityparser-4.0.0/unityparser/dumper.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 
     def __init__(self, stream,
                  default_style=None, default_flow_style=False,
                  canonical=None, indent=None, width=None,
                  allow_unicode=None, line_break=None,
                  encoding=None, explicit_start=None, explicit_end=None,
                  version=None, tags=None, sort_keys=True, register=None):
-        tags = tags or {}
-        tags.update(UNITY_TAG)
-        version = version or VERSION
         Emitter.__init__(self, stream, canonical=canonical,
                          indent=indent, width=width,
                          allow_unicode=allow_unicode, line_break=line_break)
         Serializer.__init__(self, encoding=encoding,
                             explicit_start=explicit_start, explicit_end=explicit_end,
                             version=version, tags=tags)
         Representer.__init__(self, default_style=default_style,
```

### Comparing `unityparser-3.0.1/unityparser/emitter.py` & `unityparser-4.0.0/unityparser/emitter.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/loader.py` & `unityparser-4.0.0/unityparser/loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from yaml.reader import Reader
 
 from .scanner import Scanner
 from .composer import Composer
 from .constants import UNITY_TAG_URI, OrderedFlowDict, UnityClassIdMap
 from .constructor import Constructor
 from .parser import Parser
-from .resolver import Resolver
+from .resolver import Resolver, SmartResolver
 
 
 class UpgradeVersionError(Exception):
     def __init__(self, *args, should_upgrade=False, **kwargs):
         super().__init__(*args, **kwargs)
         self.should_upgrade = should_upgrade
 
@@ -34,14 +34,25 @@
         Scanner.__init__(self)
         Parser.__init__(self)
         Composer.__init__(self)
         Constructor.__init__(self, register)
         Resolver.__init__(self)
 
 
+class SmartUnityLoader(Reader, Scanner, Parser, Composer, Constructor, SmartResolver):
+
+    def __init__(self, stream, register=None):
+        Reader.__init__(self, stream)
+        Scanner.__init__(self)
+        Parser.__init__(self)
+        Composer.__init__(self)
+        Constructor.__init__(self, register)
+        SmartResolver.__init__(self)
+
+
 def construct_unity_class(loader, tag_suffix, node):
     try:
         classid = tag_suffix
         classname = node.value[0][0].value
     except (ValueError, KeyError):
         raise LoaderVersionError('Unknown class id {}.'.format(tag_suffix))
     class_attributes_node = node.value[0][1]
@@ -62,7 +73,9 @@
     yield data
     value = loader.construct_mapping(node)
     data.update(value)
 
 
 UnityLoader.add_constructor('tag:yaml.org,2002:map', construct_yaml_map)
 UnityLoader.add_multi_constructor(UNITY_TAG_URI, construct_unity_class)
+SmartUnityLoader.add_constructor('tag:yaml.org,2002:map', construct_yaml_map)
+SmartUnityLoader.add_multi_constructor(UNITY_TAG_URI, construct_unity_class)
```

### Comparing `unityparser-3.0.1/unityparser/parser.py` & `unityparser-4.0.0/unityparser/parser.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 
 
 class Parser(YamlParser):
 
     def __init__(self):
         super(Parser, self).__init__()
         self.parsing_inverted_scalar = False
+        self.non_default_tags = None
 
     def parse_document_start(self):
 
         # Parse any extra document end indicators.
         while self.check_token(DocumentEndToken):
             self.get_token()
 
         # Parse an explicit document.
         if not self.check_token(StreamEndToken):
             token = self.peek_token()
             start_mark = token.start_mark
             # UNITY: only process directives(version and tags) on the first document
             if self.check_prev_token(StreamStartToken):
                 version, tags = self.process_directives()
+                # UNITY: keep track of tags explicitly defined in the document
+                if self.non_default_tags is None:
+                    self.non_default_tags = tags
             else:
                 version, tags = self.yaml_version, self.tag_handles.copy() if self.tag_handles else None
             if not self.check_token(DocumentStartToken):
                 raise ParserError(None, None,
                                   "expected '<document start>', but found %r"
                                   % self.peek_token().id,
                                   self.peek_token().start_mark)
```

### Comparing `unityparser-3.0.1/unityparser/resolver.py` & `unityparser-4.0.0/unityparser/resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,25 +14,14 @@
 # Resolver.add_implicit_resolver(
 #     'tag:yaml.org,2002:bool',
 #     re.compile(r'''^(?:yes|Yes|YES|no|No|NO
 #                     |true|True|TRUE|false|False|FALSE
 #                     |on|On|ON|off|Off|OFF)$''', re.X),
 #     list('yYnNtTfFoO'))
 
-Resolver.add_implicit_resolver(
-    'tag:yaml.org,2002:float',
-    re.compile(r'''^(?:[-+]?(?:0|[1-9][0-9]*)\.(?:[1-9]|[0-9][0-9]*[1-9])?)$''', re.X),
-    list('-+0123456789.'))
-
-Resolver.add_implicit_resolver(
-    'tag:yaml.org,2002:int',
-    # UNITY: Restrict to simple integer values
-    re.compile(r'''^(?:[-+]?(?:0|[1-9][0-9]*))$''', re.X),
-    list('-+0123456789'))
-
 # Resolver.add_implicit_resolver(
 #     'tag:yaml.org,2002:merge',
 #     re.compile(r'^(?:<<)$'),
 #     ['<'])
 
 Resolver.add_implicit_resolver(
     'tag:yaml.org,2002:null',
@@ -56,7 +45,28 @@
 
 # The following resolver is only for documentation purposes. It cannot work
 # because plain scalars cannot start with '!', '&', or '*'.
 Resolver.add_implicit_resolver(
     'tag:yaml.org,2002:yaml',
     re.compile(r'^(?:!|&|\*)$'),
     list('!&*'))
+
+
+class SmartResolver(Resolver):
+    """
+    A Resolver that tries to be smart about how Unity serializes int and float values, but it's known that does not
+    cover all cases.
+    """
+    pass
+
+
+SmartResolver.add_implicit_resolver(
+    'tag:yaml.org,2002:float',
+    re.compile(r'''^(?:[-+]?(?:0|[1-9][0-9]*)\.(?:[1-9]|[0-9][0-9]*[1-9])?)$''', re.X),
+    list('-+0123456789.'))
+
+SmartResolver.add_implicit_resolver(
+    'tag:yaml.org,2002:int',
+    # UNITY: Restrict to simple integer values
+    re.compile(r'''^(?:[-+]?(?:0|[1-9][0-9]*))$''', re.X),
+    list('-+0123456789'))
+
```

### Comparing `unityparser-3.0.1/unityparser/scanner.py` & `unityparser-4.0.0/unityparser/scanner.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/serializer.py` & `unityparser-4.0.0/unityparser/serializer.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.1/unityparser/utils.py` & `unityparser-4.0.0/unityparser/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import io
+from copy import copy
 
 from .dumper import UnityDumper
 from .errors import UnityDocumentError
-from .loader import UnityLoader
+from .loader import UnityLoader, SmartUnityLoader
 from .register import UnityScalarRegister
 
 UNIX_LINE_ENDINGS = '\n'
 
 
 class UnityDocument:
 
-    def __init__(self, data, newline=None, file_path=None, register=None):
+    def __init__(self, data, newline=None, file_path=None, register=None, version=None, tags=None):
         self.newline = newline
         self.data = data
         self.file_path = file_path
         self.register = register or UnityScalarRegister()
+        self.version = version
+        self.tags = tags
 
     @property
     def entry(self):
         # as many documents contain a single document entry, this might be handy
         return self.data[0]
 
     @property
@@ -30,25 +33,43 @@
         :param file_path: If self.file_path is None, it must be passed
         :type file_path:
         :return:
         :rtype:
         """
         file_path = file_path or self.file_path
         assert_or_raise(file_path is not None, UnityDocumentError("file_path parameter must be passed"))
+        kwargs_copy = copy(kwargs)
+        if 'version' not in kwargs:
+            kwargs_copy['version'] = self.version
+        if 'tags' not in kwargs:
+            kwargs_copy['tags'] = self.tags
         with open(file_path, 'w', newline=self.newline) as fp:
-            dump_all(self.data, stream=fp, register=self.register, **kwargs)
+            dump_all(self.data, stream=fp, register=self.register, **kwargs_copy)
 
     @classmethod
-    def load_yaml(cls, file_path):
+    def load_yaml(cls, file_path, try_preserve_types=False):
+        """
+        :param file_path: Path to the file to load
+        :param try_preserve_types: If true, will deserialize what seems to be int and float types to the same Python
+            data types instead of deserializing them all as the string type. When/if this value is later serialized
+            back it might be represented differently in some corner cases.
+        """
+        loader_cls = SmartUnityLoader if try_preserve_types else UnityLoader
         register = UnityScalarRegister()
         with open(file_path, newline='') as fp:
-            data = [d for d in load_all(fp, register)]
+            loader = loader_cls(fp)
+            loader.check_data()
+            fp.seek(0)
+            version = loader.yaml_version
+            tags = loader.non_default_tags
+            data = [d for d in load_all(fp, register, loader_cls)]
             # use document line endings if no mixed lien endings found, else default to linux
             line_endings = UNIX_LINE_ENDINGS if isinstance(fp.newlines, tuple) else fp.newlines
-        doc = UnityDocument(data, newline=line_endings, file_path=file_path, register=register)
+        doc = UnityDocument(data, newline=line_endings, file_path=file_path, register=register, version=version,
+                            tags=tags)
         return doc
 
     # region Filtering
 
     def filter(self, class_names=None, attributes=None):
         """
         Filter a group of entries
@@ -91,20 +112,20 @@
 
 
 def assert_or_raise(condition, exception):
     if not condition:
         raise exception
 
 
-def load_all(stream, register=None):
+def load_all(stream, register=None, loader_cls=UnityLoader):
     """
     Parse all YAML documents in a stream
     and produce corresponding Python objects.
     """
-    loader = UnityLoader(stream, register)
+    loader = loader_cls(stream, register)
     try:
         while loader.check_data():
             yield loader.get_data()
     finally:
         loader.dispose()
```

### Comparing `unityparser-3.0.1/unityparser.egg-info/PKG-INFO` & `unityparser-4.0.0/unityparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 3.0.1
+Version: 4.0.0
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
```

### Comparing `unityparser-3.0.1/unityparser.egg-info/SOURCES.txt` & `unityparser-4.0.0/unityparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

