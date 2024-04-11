# Comparing `tmp/pillory-1.0.1.tar.gz` & `tmp/pillory-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pillory-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pillory-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pillory-1.0.1.tar` & `pillory-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      880 2024-04-07 02:49:31.399297 pillory-1.0.1/.circleci/config.yml
--rw-r--r--   0        0        0       18 2024-04-07 02:49:31.399297 pillory-1.0.1/.gitignore
--rw-r--r--   0        0        0      359 2024-04-07 02:49:31.399297 pillory-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     9161 2024-04-07 02:49:31.399297 pillory-1.0.1/LICENSE
--rw-r--r--   0        0        0     3465 2024-04-07 02:49:31.399297 pillory-1.0.1/README.md
--rw-r--r--   0        0        0     1321 2024-04-07 02:49:31.399297 pillory-1.0.1/dev-requirements.txt
--rwxr-xr-x   0        0        0     2932 2024-04-07 02:49:31.399297 pillory-1.0.1/pillory.py
--rw-r--r--   0        0        0      587 2024-04-07 02:49:31.399297 pillory-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 pillory-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-04-11 23:14:04.031983 pillory-1.0.2/.circleci/config.yml
+-rw-r--r--   0        0        0       18 2024-04-11 23:14:04.031983 pillory-1.0.2/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-11 23:14:04.031983 pillory-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     9161 2024-04-11 23:14:04.031983 pillory-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4361 2024-04-11 23:14:04.031983 pillory-1.0.2/README.md
+-rw-r--r--   0        0        0     1321 2024-04-11 23:14:04.031983 pillory-1.0.2/dev-requirements.txt
+-rwxr-xr-x   0        0        0     3188 2024-04-11 23:14:04.031983 pillory-1.0.2/pillory.py
+-rw-r--r--   0        0        0      587 2024-04-11 23:14:04.031983 pillory-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3082 2024-04-11 23:14:04.031983 pillory-1.0.2/test_example.py
+-rw-r--r--   0        0        0      513 2024-04-11 23:14:04.031983 pillory-1.0.2/test_pillory.py
+-rw-r--r--   0        0        0     4898 1970-01-01 00:00:00.000000 pillory-1.0.2/PKG-INFO
```

### Comparing `pillory-1.0.1/.circleci/config.yml` & `pillory-1.0.2/.circleci/config.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 version: 2.1
 
 orbs:
   python: circleci/python@2.1.1
 
 jobs:
-  lint:
+  test:
     executor:
         name: python/default
         tag: "3.10"
     steps:
       - checkout
-      - python/install-packages:
-          pip-dependency-file: dev-requirements.txt
-          pkg-manager: pip
       - run:
-          name: ruff
-          command: ruff check
+          name: unit tests
+          command: python test_pillory.py -v
       - run:
-          name: ruff format
-          command: ruff format --check
+          name: example tests
+          command: python test_example.py -v
 
   publish:
     executor:
         name: python/default
         tag: "3.10"
     steps:
       - checkout
@@ -30,16 +27,16 @@
           pip-dependency-file: dev-requirements.txt
           pkg-manager: pip
       - run:
           name: flit publish
           command: flit publish
 
 workflows:
-  lint-and-publish:
+  test-and-publish:
     jobs:
-      - lint
+      - test
       - publish:
           requires:
-            - lint
+            - test
           filters:
             branches:
               only: main
```

### Comparing `pillory-1.0.1/LICENSE` & `pillory-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pillory-1.0.1/README.md` & `pillory-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -24,33 +24,33 @@
 
 ```
 python -m pillory 'tests/**/test_*.py'
 ```
 
 ### Rules
 
-*PM101 patched implementation*
+**PM101 patched implementation**
 : You patched the implementation of a class or function instead of where it is
 imported to in the module under test. e.g. "parsers.Parser" where Parser is
 defined instead of "__main__.Parser" where it is used. This means you may not
 have affected the module under test at all, or you have replaced the target in a
 way which will affect other code that uses it, which is bad for test isolation
 (making sure tests don't affect other tests, and that each test tests what is
 intended and don't change how other parts of the code work). There is a warning
 about not affecting the right module in the [Python Standard Library
 docs][stdlibdocs], but there is an [even better article by Ned
 Batchelder][nedbat] explaining how it works and the additional problems with
 test isolation.
 
-*PM102 patched is not a top level module attribute*
+**PM102 patched is not a top level module attribute**
 : You patched something like a method on a class. Because class methods can't be
 imported by themselves, this means all uses of the class will be affected, not
 just the module under test.
 
-*PM103 patched builtins*
+**PM103 patched builtins**
 : You patched the builtins module instead of the built-in function in the module
 under test. Built-ins are actually added to every module and that's where they
 should be patched, to avoid similar issues to patching the implementation. There
 is a CPython detail that means the builtins module may be added to the lookup of
 each module, so patching the builtins module _can_ work, but it's not guaranteed
 and it still has problems with test isolation.
 
@@ -58,15 +58,17 @@
 [nedbat]: https://nedbatchelder.com/blog/201908/why_your_mock_doesnt_work.html
 
 ## Known issues
 
 * No --help text.
 * No console script entry point (pillory command), have to use with python -m.
 * Only takes one path or glob.
+* Only tested with Python 3.10.
 * No config file support.
+* No comments to ignore rules.
 * Not fast.
 * Must import modules. Doesn't work well with frameworks like Django that
   require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
@@ -86,7 +88,39 @@
 Thank you for your interest in making a contribution.
 
 Please talk to the maintainer before making a pull request to make sure what you
 are adding is wanted.
 
 This project uses the Apache License 2.0. You will be credited in the git
 history, but for ease of maintenance copyright stays with the maintainer.
+
+There are linters, formatters, and tests as part of the CI. You can check them
+yourself locally too. To set up the linters as a pre-commit hook:
+
+```
+# Install the dev dependencies if not done already
+pip install -r dev-requirements.txt
+# Install the pre-commit hooks
+pre-commit install
+```
+
+You can run the linters on command with:
+
+```
+pre-commit run -a
+```
+
+The unit tests are supposed to be fast tests for testing logic in a test driven
+developement style. They shouldn't have mocking or accounting for side effects.
+You can run them with:
+
+```
+python test_pillory.py
+```
+
+The example tests have a more complicated setup to include the file system and
+command line args. Try to limit the number of example tests. The tests use
+doctest to easily check the outputs. You can run them with:
+
+```
+python test_example.py -v
+```
```

### Comparing `pillory-1.0.1/dev-requirements.txt` & `pillory-1.0.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `pillory-1.0.1/pyproject.toml` & `pillory-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pillory-1.0.1/PKG-INFO` & `pillory-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pillory
-Version: 1.0.1
+Version: 1.0.2
 Summary: A linter to scrutinize how you are using mocks in Python.
 Author-email: Fergal Armstrong <patio.algebra0i@icloud.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: flit~=3.9 ; extra == "dev"
 Requires-Dist: pip-tools~=7.4 ; extra == "dev"
 Requires-Dist: pre-commit~=3.7 ; extra == "dev"
@@ -38,33 +38,33 @@
 
 ```
 python -m pillory 'tests/**/test_*.py'
 ```
 
 ### Rules
 
-*PM101 patched implementation*
+**PM101 patched implementation**
 : You patched the implementation of a class or function instead of where it is
 imported to in the module under test. e.g. "parsers.Parser" where Parser is
 defined instead of "__main__.Parser" where it is used. This means you may not
 have affected the module under test at all, or you have replaced the target in a
 way which will affect other code that uses it, which is bad for test isolation
 (making sure tests don't affect other tests, and that each test tests what is
 intended and don't change how other parts of the code work). There is a warning
 about not affecting the right module in the [Python Standard Library
 docs][stdlibdocs], but there is an [even better article by Ned
 Batchelder][nedbat] explaining how it works and the additional problems with
 test isolation.
 
-*PM102 patched is not a top level module attribute*
+**PM102 patched is not a top level module attribute**
 : You patched something like a method on a class. Because class methods can't be
 imported by themselves, this means all uses of the class will be affected, not
 just the module under test.
 
-*PM103 patched builtins*
+**PM103 patched builtins**
 : You patched the builtins module instead of the built-in function in the module
 under test. Built-ins are actually added to every module and that's where they
 should be patched, to avoid similar issues to patching the implementation. There
 is a CPython detail that means the builtins module may be added to the lookup of
 each module, so patching the builtins module _can_ work, but it's not guaranteed
 and it still has problems with test isolation.
 
@@ -72,15 +72,17 @@
 [nedbat]: https://nedbatchelder.com/blog/201908/why_your_mock_doesnt_work.html
 
 ## Known issues
 
 * No --help text.
 * No console script entry point (pillory command), have to use with python -m.
 * Only takes one path or glob.
+* Only tested with Python 3.10.
 * No config file support.
+* No comments to ignore rules.
 * Not fast.
 * Must import modules. Doesn't work well with frameworks like Django that
   require special setup for things like settings before importing.
 * Globs have to be relative to the current directory.
 * No further explanations for the errors.
 * No pretty error handling, just tracebacks.
 * Will error when mocking something in the module under test, which is arguably
@@ -101,7 +103,39 @@
 
 Please talk to the maintainer before making a pull request to make sure what you
 are adding is wanted.
 
 This project uses the Apache License 2.0. You will be credited in the git
 history, but for ease of maintenance copyright stays with the maintainer.
 
+There are linters, formatters, and tests as part of the CI. You can check them
+yourself locally too. To set up the linters as a pre-commit hook:
+
+```
+# Install the dev dependencies if not done already
+pip install -r dev-requirements.txt
+# Install the pre-commit hooks
+pre-commit install
+```
+
+You can run the linters on command with:
+
+```
+pre-commit run -a
+```
+
+The unit tests are supposed to be fast tests for testing logic in a test driven
+developement style. They shouldn't have mocking or accounting for side effects.
+You can run them with:
+
+```
+python test_pillory.py
+```
+
+The example tests have a more complicated setup to include the file system and
+command line args. Try to limit the number of example tests. The tests use
+doctest to easily check the outputs. You can run them with:
+
+```
+python test_example.py -v
+```
+
```

