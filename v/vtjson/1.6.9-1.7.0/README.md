# Comparing `tmp/vtjson-1.6.9.tar.gz` & `tmp/vtjson-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.6.9.tar", last modified: Thu Apr 11 00:18:49 2024, max compression
+gzip compressed data, was "vtjson-1.7.0.tar", last modified: Fri Apr 12 01:05:52 2024, max compression
```

## Comparing `vtjson-1.6.9.tar` & `vtjson-1.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:18:49.634645 vtjson-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-11 00:18:37.000000 vtjson-1.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-04-11 00:18:49.634645 vtjson-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-11 00:18:37.000000 vtjson-1.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-11 00:18:37.000000 vtjson-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:18:49.634645 vtjson-1.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:18:49.634645 vtjson-1.6.9/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17961 2024-04-11 00:18:49.000000 vtjson-1.6.9/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 00:18:49.000000 vtjson-1.6.9/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:18:49.000000 vtjson-1.6.9/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 00:18:49.000000 vtjson-1.6.9/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 00:18:49.000000 vtjson-1.6.9/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25142 2024-04-11 00:18:37.000000 vtjson-1.6.9/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:05:52.900255 vtjson-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-12 01:05:46.000000 vtjson-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-12 01:05:52.900255 vtjson-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17660 2024-04-12 01:05:46.000000 vtjson-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 01:05:46.000000 vtjson-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:05:52.900255 vtjson-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:05:52.900255 vtjson-1.7.0/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 01:05:52.000000 vtjson-1.7.0/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27113 2024-04-12 01:05:46.000000 vtjson-1.7.0/vtjson.py
```

### Comparing `vtjson-1.6.9/LICENSE` & `vtjson-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.9/PKG-INFO` & `vtjson-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.9
+Version: 1.7.0
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -220,15 +220,14 @@
 A wrapper takes one or more schemas as arguments and produces a new schema.
 - An object matches the schema `union(schema1, ..., schemaN)` if it matches one of the schemas `schema1, ..., schemaN`. This is almost the same as `{schema1, ..., schemaN}`, or equivalently `set((schema1, ..., schemaN))` if `schema1, ..., schemaN` are hashable.
 - An object matches the schema `intersect(schema1, ..., schemaN)` if it matches all the schemas `schema1, ..., schemaN`.
 - An object matches the schema `complement(schema)` if it does not match `schema`.
 - An object matches the schema `lax(schema)` if it matches `schema` when validated with `strict=False`.
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
@@ -249,14 +248,16 @@
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
+## Pre-compiling a schema
+- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -317,15 +318,28 @@
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
 Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
 
-A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
+Q: Does vtjson support recursive schemas?
+
+A: Yes. Here is an example
+```python
+person={}
+person["mother"]=union(person, None)
+person["father"]=union(person, None)
+```
+which matches e.g.
+```python
+{"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
+```
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.6.9/README.md` & `vtjson-1.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,14 @@
 A wrapper takes one or more schemas as arguments and produces a new schema.
 - An object matches the schema `union(schema1, ..., schemaN)` if it matches one of the schemas `schema1, ..., schemaN`. This is almost the same as `{schema1, ..., schemaN}`, or equivalently `set((schema1, ..., schemaN))` if `schema1, ..., schemaN` are hashable.
 - An object matches the schema `intersect(schema1, ..., schemaN)` if it matches all the schemas `schema1, ..., schemaN`.
 - An object matches the schema `complement(schema)` if it does not match `schema`.
 - An object matches the schema `lax(schema)` if it matches `schema` when validated with `strict=False`.
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
@@ -232,14 +231,16 @@
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
+## Pre-compiling a schema
+- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -300,15 +301,28 @@
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
 Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
 
-A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
+Q: Does vtjson support recursive schemas?
+
+A: Yes. Here is an example
+```python
+person={}
+person["mother"]=union(person, None)
+person["father"]=union(person, None)
+```
+which matches e.g.
+```python
+{"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
+```
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.6.9/pyproject.toml` & `vtjson-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.6.9/vtjson.egg-info/PKG-INFO` & `vtjson-1.7.0/vtjson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.6.9
+Version: 1.7.0
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -220,15 +220,14 @@
 A wrapper takes one or more schemas as arguments and produces a new schema.
 - An object matches the schema `union(schema1, ..., schemaN)` if it matches one of the schemas `schema1, ..., schemaN`. This is almost the same as `{schema1, ..., schemaN}`, or equivalently `set((schema1, ..., schemaN))` if `schema1, ..., schemaN` are hashable.
 - An object matches the schema `intersect(schema1, ..., schemaN)` if it matches all the schemas `schema1, ..., schemaN`.
 - An object matches the schema `complement(schema)` if it does not match `schema`.
 - An object matches the schema `lax(schema)` if it matches `schema` when validated with `strict=False`.
 - An object matches the schema `strict(schema)` if it matches `schema` when validated with `strict=True`.
 - An object matches the schema `set_name(schema, name)` if it matches `schema`. But the `name` argument will be used in non-validation messages.
-- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 - An object matches the schema `quote(schema)` if it is equal to `schema`. For example the schema `{"cats", "dogs"}` matches the strings `"cats"` and `"dogs"` but the schema `quote({"cats", "dogs"})` matches the set `{"cats", "dogs"}`. 
 ## Built-ins
 Some built-ins take arguments. If no arguments are given then the parentheses can be omitted. So `email` is equivalent to `email()`.
 - `regex(pattern, name=None, fullmatch=True, flags=0)`. This matches the strings which match the given pattern. The optional `name` argument may be used to give the regular expression a descriptive name. By default the entire string is matched, but this can be overruled via the `fullmatch` argument. The `flags` argument has the usual meaning.
 - `glob(pattern, name=None)`. Unix style filename matching. This is implemented using `pathlib.PurePath().match()`.
 - `div(divisor, remainder=0, name=None)`. This matches the integers `x` such that `(x - remainder) % divisor` == 0.
 - `number`. Matches `int` and `float`.
@@ -249,14 +248,16 @@
 corresponding inequality is not checked.
 - `size(lowerbound, upperbound)`. Matches the objects (which support `len()` such as strings or lists) whose length is in the interval `[upperbound, lowerbound]`. The value of `upperbound` can be `...` (ellipsis).
 ## Conditional schemas
 - `ifthen(if_schema, then_schema, else_schema=None)`. It the object matches the `if_schema` then it should also match the `then_schema`. If the object does not match the `if_schema` then it should match
 the `else_schema`, if present.
 - `cond((if_schema1, then_schema1), ... , (if_schemaN, then_schemaN))`. An object is successively validated against `if_schema1`, `if_schema2`, ... until a validation succeeds. When this happens the object should
 match the corresponding `then_schema`. If no `if_schema` succeeds then the object is considered to have been validated. If one sets `if_schemaN` equal to `anything` then this serves as a catch all.
+## Pre-compiling a schema
+- An object matches the schema `compile(schema)` if it matches `schema`. `vtjson` compiles the schema before performing a validation so pre-compiling is not necessary but, in some cases, it may gain a bit of performance. 
 ## Format
 A schema can be, in order of precedence:
 - A class with the following properties:
   - it has a no-argument constructor;
   - the instances have a `__validate__` method with signature
   ```python
   __validate__(self, object, name, strict)
@@ -317,15 +318,28 @@
 
 Q: How is this different from https://pypi.org/project/json-checker/ \?
 
 A: Good question! I discovered `json-checker` after I had written `vtjson`. Although the details are different `json-checker` and `vtjson` share many of the same principles.
 
 Q: Why are there no variables in vtjson (see https://opis.io/json-schema/2.x/variables.html)?
 
-A: They did not seem to essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+A: They did not seem to be essential yet. In our use cases conditional schemas were sufficient to achieve the required functionality. See for example the `action_schema` in <a href=https://raw.githubusercontent.com/official-stockfish/fishtest/master/server/fishtest/schemas.py>`schemas.py`</a>. More importantly `vtjson` has a strict separation between the definition of a schema and its subsequent use for validation. By allowing a schema to refer directly to the object being validated this separation would become blurred. This being said, I am still thinking about a good way to introduce variables.
+
+Q: Does vtjson support recursive schemas?
+
+A: Yes. Here is an example
+```python
+person={}
+person["mother"]=union(person, None)
+person["father"]=union(person, None)
+```
+which matches e.g.
+```python
+{"father": {"father": None, "mother": None}, "mother": {"father": None, "mother": None}}
+```
 
 Q: How to combine validations?
 
 A: Use `intersect`. For example the following schema validates positive integers but reject positive floats.
 ```python
 schema = intersect(int, interval(0, ...))
 ```
```

### Comparing `vtjson-1.6.9/vtjson.py` & `vtjson-1.7.0/vtjson.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.6.9"
+__version__ = "1.7.0"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -111,91 +111,144 @@
     def __eq__(self, key):
         return self.key == key.key
 
     def __hash__(self):
         return hash(self.key)
 
 
-class union:
-    def __init__(self, *schemas):
-        self.schemas = [compile(s) for s in schemas]
+class _union:
+    def __init__(self, schemas, _deferred_compiles={}):
+        self.schemas = [
+            compile(s, _deferred_compiles=_deferred_compiles) for s in schemas
+        ]
 
     def __validate__(self, object, name, strict):
         messages = []
         for schema in self.schemas:
             message = schema.__validate__(object, name=name, strict=strict)
             if message == "":
                 return ""
             else:
                 messages.append(message)
         return " and ".join(messages)
 
 
-class intersect:
+class union:
     def __init__(self, *schemas):
-        self.schemas = [compile(s) for s in schemas]
+        self.schemas = schemas
+
+    def __compile__(self, _deferred_compiles={}):
+        return _union(self.schemas, _deferred_compiles=_deferred_compiles)
+
+
+class _intersect:
+    def __init__(self, schemas, _deferred_compiles={}):
+        self.schemas = [
+            compile(s, _deferred_compiles=_deferred_compiles) for s in schemas
+        ]
 
     def __validate__(self, object, name, strict):
         for schema in self.schemas:
             message = schema.__validate__(object, name=name, strict=strict)
             if message != "":
                 return message
         return ""
 
 
-class complement:
-    def __init__(self, schema):
-        self.schema = compile(schema)
+class intersect:
+    def __init__(self, *schemas):
+        self.schemas = schemas
+
+    def __compile__(self, _deferred_compiles={}):
+        return _intersect(self.schemas, _deferred_compiles=_deferred_compiles)
+
+
+class _complement:
+    def __init__(self, schema, _deferred_compiles={}):
+        self.schema = compile(schema, _deferred_compiles=_deferred_compiles)
 
     def __validate__(self, object, name, strict):
         message = self.schema.__validate__(object, name=name, strict=strict)
         if message != "":
             return ""
         else:
             return f"{name} does not match the complemented schema"
 
 
-class lax:
+class complement:
     def __init__(self, schema):
-        self.schema = compile(schema)
+        self.schema = schema
+
+    def __compile__(self, _deferred_compiles={}):
+        return _complement(self.schema, _deferred_compiles=_deferred_compiles)
+
+
+class _lax:
+    def __init__(self, schema, _deferred_compiles={}):
+        self.schema = compile(schema, _deferred_compiles=_deferred_compiles)
 
     def __validate__(self, object, name, strict):
         return self.schema.__validate__(object, name=name, strict=False)
 
 
-class strict:
+class lax:
     def __init__(self, schema):
-        self.schema = compile(schema)
+        self.schema = schema
+
+    def __compile__(self, _deferred_compiles={}):
+        return _lax(self.schema, _deferred_compiles=_deferred_compiles)
+
+
+class _strict:
+    def __init__(self, schema, _deferred_compiles={}):
+        self.schema = compile(schema, _deferred_compiles=_deferred_compiles)
 
     def __validate__(self, object, name, strict):
         return self.schema.__validate__(object, name=name, strict=True)
 
 
+class strict:
+    def __init__(self, schema):
+        self.schema = schema
+
+    def __compile__(self, _deferred_compiles={}):
+        return _strict(self.schema, _deferred_compiles=_deferred_compiles)
+
+
 class quote:
     def __init__(self, schema):
         self.schema = _object(schema)
 
     def __validate__(self, object, name, strict):
         return self.schema.__validate__(object, name, strict)
 
 
-class set_name:
-    def __init__(self, schema, name):
-        if not isinstance(name, str):
-            raise SchemaError(f"The name {_c(name)} is not a string")
-        self.schema = compile(schema)
+class _set_name:
+    def __init__(self, schema, name, _deferred_compiles={}):
+        self.schema = compile(schema, _deferred_compiles=_deferred_compiles)
         self.__name__ = name
 
     def __validate__(self, object, name, strict):
         message = self.schema.__validate__(object, name=name, strict=strict)
         if message != "":
             return _wrong_type_message(object, name, self.__name__)
         return ""
 
 
+class set_name:
+    def __init__(self, schema, name):
+        if not isinstance(name, str):
+            raise SchemaError(f"The name {_c(name)} is not a string")
+        self.schema = schema
+        self.name = name
+
+    def __compile__(self, _deferred_compiles={}):
+        return _set_name(self.schema, self.name, _deferred_compiles=_deferred_compiles)
+
+
 class regex:
     def __init__(self, regex, name=None, fullmatch=True, flags=0):
         self.regex = regex
         self.fullmatch = fullmatch
         if name is not None:
             if not isinstance(name, str):
                 raise SchemaError(f"The regex name {_c(name)} is not a string")
@@ -373,53 +426,59 @@
         return self.interval.__validate__(L, f"len({name})", strict)
 
 
 class _deferred:
     def __init__(self, collection, key):
         if not isinstance(collection, dict):
             raise SchemaError(f"{repr(collection)} is not a dictionary")
+        try:
+            hash(key)
+        except Exception as e:
+            raise SchemaError(f"{str(e)}") from None
         self.collection = collection
         self.key = key
 
     def __validate__(self, object, name, strict):
         if self.key not in self.collection:
             raise ValidationError(f"{name}: key {self.key} is unknown")
         return self.collection[self.key].__validate__(object, name, strict)
 
 
-def compile(schema, _compiled_schemas={}):
+def compile(schema, _deferred_compiles={}):
     id_ = id(schema)
     # avoid infinite loop in case of a recursive schema
-    if id_ in _compiled_schemas:
-        compiled_schema = _compiled_schemas[id_]
+    if id_ in _deferred_compiles:
+        compiled_schema = _deferred_compiles[id_]
         if isinstance(compiled_schema, _deferred):
             return compiled_schema
-    _compiled_schemas[id_] = _deferred(_compiled_schemas, id_)
+    _deferred_compiles[id_] = _deferred(_deferred_compiles, id_)
     if isinstance(schema, type) and hasattr(schema, "__validate__"):
         try:
             ret = schema()
         except Exception:
             raise SchemaError(
                 f"{repr(schema.__name__)} does " f"not have a no-argument constructor"
             ) from None
     elif hasattr(schema, "__validate__"):
         ret = schema
+    elif hasattr(schema, "__compile__"):
+        ret = schema.__compile__(_deferred_compiles=_deferred_compiles)
     elif isinstance(schema, type) or isinstance(schema, _GenericAlias):
         ret = _type(schema)
     elif callable(schema):
         ret = _callable(schema)
     elif isinstance(schema, tuple) or isinstance(schema, list):
-        ret = _sequence(schema, _compiled_schemas=_compiled_schemas)
+        ret = _sequence(schema, _deferred_compiles=_deferred_compiles)
     elif isinstance(schema, dict):
-        ret = _dict(schema, _compiled_schemas=_compiled_schemas)
+        ret = _dict(schema, _deferred_compiles=_deferred_compiles)
     elif isinstance(schema, set):
-        ret = union(*schema)
+        ret = _union(schema, _deferred_compiles=_deferred_compiles)
     else:
         ret = _object(schema)
-    _compiled_schemas[id_] = ret
+    _deferred_compiles[id_] = ret
     return ret
 
 
 def _validate(schema, object, name="object", strict=True):
     schema = compile(schema)
     return schema.__validate__(object, name=name, strict=strict)
 
@@ -648,24 +707,24 @@
         for c in self.conditions:
             if c[0].__validate__(object, name, strict) == "":
                 return c[1].__validate__(object, name, strict)
         return ""
 
 
 class _dict:
-    def __init__(self, schema, _compiled_schemas={}):
+    def __init__(self, schema, _deferred_compiles={}):
         self.schema = collections.OrderedDict()
         for k, v in schema.items():
-            self.schema[k] = compile(v, _compiled_schemas=_compiled_schemas)
+            self.schema[k] = compile(v, _deferred_compiles=_deferred_compiles)
         self.keys = _keys(self.schema)
         self.keys2 = _keys2(self.schema)
 
     def __validate__(self, object, name, strict):
-        if type(object) is not dict:
-            return _wrong_type_message(object, name, type(self.schema).__name__)
+        if not isinstance(object, dict):
+            return _wrong_type_message(object, name, "dict")
         for k_, k, o in self.keys2:
             # (k_,k,o)=(normalized key, key, optional)
             name_ = f"{name}['{k_}']"
             if k_ not in object:
                 if o:
                     continue
                 else:
@@ -700,18 +759,18 @@
             return f"{self.schema} is not a valid type: {str(e)}"
 
     def __str__(self):
         return self.schema.__name__
 
 
 class _sequence:
-    def __init__(self, schema, _compiled_schemas={}):
+    def __init__(self, schema, _deferred_compiles={}):
         self.type_schema = type(schema)
         self.schema = [
-            compile(o, _compiled_schemas=_compiled_schemas) if o is not ... else ...
+            compile(o, _deferred_compiles=_deferred_compiles) if o is not ... else ...
             for o in schema
         ]
         if len(schema) > 0 and schema[-1] is ...:
             if len(schema) >= 2:
                 self.fill = self.schema[-2]
                 self.schema = self.schema[:-2]
             else:
```

