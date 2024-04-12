# Comparing `tmp/cs.py.doc-20220311.tar.gz` & `tmp/cs.py.doc-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.py.doc-20220311.tar", last modified: Fri Mar 11 00:39:56 2022, max compression
+gzip compressed data, was "cs.py.doc-20240412.tar", last modified: Fri Apr 12 04:57:47 2024, max compression
```

## Comparing `cs.py.doc-20220311.tar` & `cs.py.doc-20240412.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.049699 cs.py.doc-20220311/
--rw-rw-r--   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:55.000000 cs.py.doc-20220311/MANIFEST.in
--rw-rw-r--   0 cameron    (501) staff       (20)     2413 2022-03-11 00:39:56.048810 cs.py.doc-20220311/PKG-INFO
--rw-rw-r--   0 cameron    (501) staff       (20)     1643 2022-03-11 00:39:55.000000 cs.py.doc-20220311/README.md
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.045670 cs.py.doc-20220311/lib/
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.045916 cs.py.doc-20220311/lib/python/
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.046017 cs.py.doc-20220311/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.048432 cs.py.doc-20220311/lib/python/cs/py/
--rw-r--r--   0 cameron    (501) staff       (20)     5753 2022-03-11 00:39:45.000000 cs.py.doc-20220311/lib/python/cs/py/doc.py
-drwxrwxr-x   0 cameron    (501) staff       (20)        0 2022-03-11 00:39:56.048061 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/
--rw-rw-r--   0 cameron    (501) staff       (20)     2413 2022-03-11 00:39:55.000000 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) staff       (20)      273 2022-03-11 00:39:55.000000 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) staff       (20)        1 2022-03-11 00:39:55.000000 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) staff       (20)       40 2022-03-11 00:39:55.000000 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) staff       (20)        3 2022-03-11 00:39:55.000000 cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) staff       (20)       38 2022-03-11 00:39:56.049799 cs.py.doc-20220311/setup.cfg
--rw-rw-r--   0 cameron    (501) staff       (20)     3104 2022-03-11 00:39:55.000000 cs.py.doc-20220311/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.638689 cs.py.doc-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 04:57:40.000000 cs.py.doc-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2683 2024-04-12 04:57:47.638310 cs.py.doc-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1912 2024-04-12 04:57:42.000000 cs.py.doc-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.633975 cs.py.doc-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.634311 cs.py.doc-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.634428 cs.py.doc-20240412/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.637807 cs.py.doc-20240412/lib/python/cs/py/
+-rw-r--r--   0 cameron    (501) cameron    (502)     6136 2024-04-12 04:57:25.000000 cs.py.doc-20240412/lib/python/cs/py/doc.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 04:57:47.637440 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2683 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       80 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 04:57:47.000000 cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3105 2024-04-12 04:57:46.000000 cs.py.doc-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 04:57:47.638809 cs.py.doc-20240412/setup.cfg
```

### Comparing `cs.py.doc-20220311/PKG-INFO` & `cs.py.doc-20240412/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 Metadata-Version: 2.1
 Name: cs.py.doc
-Version: 20220311
+Version: 20240412
 Summary: Create documentation from python modules and other objects.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: cs@cskk.id.au
+Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Create documentation from python modules and other objects.
 
-*Latest release 20220311*:
-module_doc: class members no longer rendered as headings, too verbose.
+*Latest release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x10bca9040>, filter_key=<function <lambda> at 0x10bca90d0>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
 * filter_key`: optional test for a key used to select or reject keys
   to appear in the documentation
+* `method_names`: optional list of method names to document;
+  the default is to document `__init__`, then CONSTANTS, the
+  dunders, then other public names
 
 ## Function `obj_docstring(obj)`
 
 Return a docstring for `obj` which has been passed through `stripped_dedent`.
 
 This function uses `obj.__doc__` if it is not `None`,
 otherwise `getcomments(obj)` if that is not `None`,
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
 Drop noise leaked into output.
 
 *Release 20210123*:
```

### Comparing `cs.py.doc-20220311/README.md` & `cs.py.doc-20240412/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Create documentation from python modules and other objects.
 
-*Latest release 20220311*:
-module_doc: class members no longer rendered as headings, too verbose.
+*Latest release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x10bca9040>, filter_key=<function <lambda> at 0x10bca90d0>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
 * filter_key`: optional test for a key used to select or reject keys
   to appear in the documentation
+* `method_names`: optional list of method names to document;
+  the default is to document `__init__`, then CONSTANTS, the
+  dunders, then other public names
 
 ## Function `obj_docstring(obj)`
 
 Return a docstring for `obj` which has been passed through `stripped_dedent`.
 
 This function uses `obj.__doc__` if it is not `None`,
 otherwise `getcomments(obj)` if that is not `None`,
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
 Drop noise leaked into output.
 
 *Release 20210123*:
```

### Comparing `cs.py.doc-20220311/lib/python/cs/py/doc.py` & `cs.py.doc-20240412/lib/python/cs/py/doc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from itertools import chain
 from cs.lex import cutprefix, stripped_dedent
 from cs.logutils import warning
 from cs.pfx import Pfx
 from cs.py.modules import module_attributes
 
-__version__ = '20220311'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -42,14 +42,17 @@
 
       Parameters:
       * `module`: the module or module name to inspect
       * `sort_key`: optional key for sorting names in the documentation;
         default: `name`
       * filter_key`: optional test for a key used to select or reject keys
         to appear in the documentation
+      * `method_names`: optional list of method names to document;
+        the default is to document `__init__`, then CONSTANTS, the
+        dunders, then other public names
   '''
   if isinstance(module, str):
     module_name = module
     with Pfx("import_module(%r)", module_name):
       module = importlib.import_module(module_name)
   full_doc = obj_docstring(module)
   for Mname, obj in sorted(module_attributes(module), key=sort_key):
@@ -69,22 +72,26 @@
         continue
       if isfunction(obj):
         sig = signature(obj)
         full_doc += f'\n\n## Function `{Mname}{sig}`\n\n{obj_doc}'
       elif isclass(obj):
         classname_etc = Mname
         mro_names = []
+        mro_set = set(obj.__mro__)
         for superclass in obj.__mro__:
+          if superclass not in mro_set:
+            continue
           if (superclass is not object and superclass is not obj
               and superclass is not abc.ABC):
             supername = superclass.__name__
             supermod = getmodule(superclass)
             if supermod is not module:
               supername = supermod.__name__ + '.' + supername
             mro_names.append(supername)
+            mro_set.difference_update(superclass.__mro__)
         if mro_names:
           classname_etc += '(' + ', '.join(mro_names) + ')'
           ##obj_doc = 'MRO: ' + ', '.join(mro_names) + '  \n' + obj_doc
         seen_names = set()
         direct_attrs = dict(obj.__dict__)
         # iterate over specified names or default names in order
         for attr_name in method_names or chain(
@@ -110,32 +117,34 @@
             if attr_name in ('__abstractmethods__', '__doc__',
                              '__getnewargs__', '__module__', '__new__',
                              '__repr__', '__weakref__'):
               continue
             # prune private names which are not dunder names
             if attr_name.startswith('_') and not is_dunder(attr_name):
               continue
-          if attr_name in direct_attrs:
-            attr = getattr(obj, attr_name)
-            attr_doc = obj_docstring(attr)
-            if not attr_doc:
-              continue
-            # Class.name is a function, not a method
-            if ismethod(attr) or isfunction(attr):
-              method_sig = signature(attr)
-              obj_doc += f'\n\n*Method `{Mname}.{attr_name}{method_sig}`*:\n{attr_doc}'
-            elif isdatadescriptor(attr):
-              obj_doc += f'\n\n*Property `{Mname}.{attr_name}`*:\n{attr_doc}'
-            elif not callable(attr):
-              ##obj_doc += f'\n\n*`{Mname}.{attr_name} = {repr(attr)}`*:\n{attr_doc}'
-              pass
-            elif isinstance(attr, property):
-              obj_doc += f'\n\n*`{Mname}.{attr_name}`*:\n{attr_doc}'
-            else:
-              obj_doc += f'\n\n*`{Mname}.{attr_name}`*'
+          if attr_name not in direct_attrs:
+            print("  skip, not in direct_attrs", direct_attrs)
+            continue
+          attr = getattr(obj, attr_name)
+          attr_doc = obj_docstring(attr)
+          if not attr_doc:
+            continue
+          # Class.name is a function, not a method
+          if ismethod(attr) or isfunction(attr):
+            method_sig = signature(attr)
+            obj_doc += f'\n\n*Method `{Mname}.{attr_name}{method_sig}`*:\n{attr_doc}'
+          elif isdatadescriptor(attr):
+            obj_doc += f'\n\n*Property `{Mname}.{attr_name}`*:\n{attr_doc}'
+          elif not callable(attr):
+            ##obj_doc += f'\n\n*`{Mname}.{attr_name} = {repr(attr)}`*:\n{attr_doc}'
+            pass
+          elif isinstance(attr, property):
+            obj_doc += f'\n\n*`{Mname}.{attr_name}`*:\n{attr_doc}'
+          else:
+            obj_doc += f'\n\n*`{Mname}.{attr_name}`*'
         full_doc += f'\n\n## Class `{classname_etc}`\n\n{obj_doc}'
       else:
         warning("UNHANDLED %r, neither function nor class", Mname)
   return full_doc
 
 def obj_docstring(obj):
   ''' Return a docstring for `obj` which has been passed through `stripped_dedent`.
```

### Comparing `cs.py.doc-20220311/lib/python/cs.py.doc.egg-info/PKG-INFO` & `cs.py.doc-20240412/lib/python/cs.py.doc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,64 @@
 Metadata-Version: 2.1
 Name: cs.py.doc
-Version: 20220311
+Version: 20240412
 Summary: Create documentation from python modules and other objects.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: cs@cskk.id.au
+Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Create documentation from python modules and other objects.
 
-*Latest release 20220311*:
-module_doc: class members no longer rendered as headings, too verbose.
+*Latest release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
 
 ## Function `is_dunder(name)`
 
 Test whether a name is a dunder name (`__`*foo*`__`).
 
-## Function `module_doc(module, *, sort_key=<function <lambda> at 0x10bca9040>, filter_key=<function <lambda> at 0x10bca90d0>, method_names=None)`
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
 
 Fetch the docstrings from a module and assemble a MarkDown document.
 
 Parameters:
 * `module`: the module or module name to inspect
 * `sort_key`: optional key for sorting names in the documentation;
   default: `name`
 * filter_key`: optional test for a key used to select or reject keys
   to appear in the documentation
+* `method_names`: optional list of method names to document;
+  the default is to document `__init__`, then CONSTANTS, the
+  dunders, then other public names
 
 ## Function `obj_docstring(obj)`
 
 Return a docstring for `obj` which has been passed through `stripped_dedent`.
 
 This function uses `obj.__doc__` if it is not `None`,
 otherwise `getcomments(obj)` if that is not `None`,
 otherwise `''`.
 The chosen string is passed through `stripped_dedent` before return.
 
 # Release Log
 
 
 
+*Release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+
 *Release 20220311*:
 module_doc: class members no longer rendered as headings, too verbose.
 
 *Release 20210306*:
 Drop noise leaked into output.
 
 *Release 20210123*:
```

### Comparing `cs.py.doc-20220311/setup.py` & `cs.py.doc-20240412/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,108 @@
-#!/usr/bin/env python
-from setuptools import setup
-setup(
-  name = 'cs.py.doc',
-  author = 'Cameron Simpson',
-  author_email = 'cs@cskk.id.au',
-  version = '20220311',
-  url = 'https://bitbucket.org/cameron_simpson/css/commits/all',
-  description =
-    'Create documentation from python modules and other objects.',
-  long_description =
-    ('Create documentation from python modules and other objects.\n'    
- '\n'    
- '*Latest release 20220311*:\n'    
- 'module_doc: class members no longer rendered as headings, too verbose.\n'    
- '\n'    
- '## Function `is_dunder(name)`\n'    
- '\n'    
- 'Test whether a name is a dunder name (`__`*foo*`__`).\n'    
- '\n'    
- '## Function `module_doc(module, *, sort_key=<function <lambda> at '    
- '0x10bca9040>, filter_key=<function <lambda> at 0x10bca90d0>, '    
- 'method_names=None)`\n'    
- '\n'    
- 'Fetch the docstrings from a module and assemble a MarkDown document.\n'    
- '\n'    
- 'Parameters:\n'    
- '* `module`: the module or module name to inspect\n'    
- '* `sort_key`: optional key for sorting names in the documentation;\n'    
- '  default: `name`\n'    
- '* filter_key`: optional test for a key used to select or reject keys\n'    
- '  to appear in the documentation\n'    
- '\n'    
- '## Function `obj_docstring(obj)`\n'    
- '\n'    
- 'Return a docstring for `obj` which has been passed through '    
- '`stripped_dedent`.\n'    
- '\n'    
- 'This function uses `obj.__doc__` if it is not `None`,\n'    
- 'otherwise `getcomments(obj)` if that is not `None`,\n'    
- "otherwise `''`.\n"    
- 'The chosen string is passed through `stripped_dedent` before return.\n'    
- '\n'    
- '# Release Log\n'    
- '\n'    
- '\n'    
- '\n'    
- '*Release 20220311*:\n'    
- 'module_doc: class members no longer rendered as headings, too verbose.\n'    
- '\n'    
- '*Release 20210306*:\n'    
- 'Drop noise leaked into output.\n'    
- '\n'    
- '*Release 20210123*:\n'    
- '* module_doc: include properties/descriptors.\n'    
- '* DISTINFO: this is not Python 2 compatible, drop tag.\n'    
- '\n'    
- '*Release 20200718*:\n'    
- '* New is_dunder(name) function to test whether name is a dunder name.\n'    
- '* module_doc: new method_names parameter to report only specific attributes '    
- 'from a class - default is all public names and most dunder methods - things '    
- 'without docs are not reported.\n'    
- '* Assorted small changes.\n'    
- '\n'    
- '*Release 20200521*:\n'    
- 'Initial PyPI release.'),
-  install_requires = ['cs.lex', 'cs.logutils', 'cs.pfx', 'cs.py.modules'],
-  classifiers = ['Programming Language :: Python', 'Programming Language :: Python :: 3', 'Development Status :: 4 - Beta', 'Intended Audience :: Developers', 'Operating System :: OS Independent', 'Topic :: Software Development :: Libraries :: Python Modules', 'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)'],
-  keywords = ['python2', 'python3'],
-  license = 'GNU General Public License v3 or later (GPLv3+)',
-  long_description_content_type = 'text/markdown',
-  package_dir = {'': 'lib/python'},
-  py_modules = ['cs.py.doc'],
-)
+[project]
+name = "cs.py.doc"
+description = "Create documentation from python modules and other objects."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.lex>=20240316",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20240412",
+    "cs.py.modules>=20220606",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240412"
+
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
+Create documentation from python modules and other objects.
+
+*Latest release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+
+## Function `is_dunder(name)`
+
+Test whether a name is a dunder name (`__`*foo*`__`).
+
+## Function `module_doc(module, *, sort_key=<function <lambda> at 0x11128cf70>, filter_key=<function <lambda> at 0x11128d000>, method_names=None)`
+
+Fetch the docstrings from a module and assemble a MarkDown document.
+
+Parameters:
+* `module`: the module or module name to inspect
+* `sort_key`: optional key for sorting names in the documentation;
+  default: `name`
+* filter_key`: optional test for a key used to select or reject keys
+  to appear in the documentation
+* `method_names`: optional list of method names to document;
+  the default is to document `__init__`, then CONSTANTS, the
+  dunders, then other public names
+
+## Function `obj_docstring(obj)`
+
+Return a docstring for `obj` which has been passed through `stripped_dedent`.
+
+This function uses `obj.__doc__` if it is not `None`,
+otherwise `getcomments(obj)` if that is not `None`,
+otherwise `''`.
+The chosen string is passed through `stripped_dedent` before return.
+
+# Release Log
+
+
+
+*Release 20240412*:
+module_doc: classes: MRO: suppress classes which are not immediate superclasses.
+
+*Release 20220311*:
+module_doc: class members no longer rendered as headings, too verbose.
+
+*Release 20210306*:
+Drop noise leaked into output.
+
+*Release 20210123*:
+* module_doc: include properties/descriptors.
+* DISTINFO: this is not Python 2 compatible, drop tag.
+
+*Release 20200718*:
+* New is_dunder(name) function to test whether name is a dunder name.
+* module_doc: new method_names parameter to report only specific attributes from a class - default is all public names and most dunder methods - things without docs are not reported.
+* Assorted small changes.
+
+*Release 20200521*:
+Initial PyPI release."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.py.doc",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

