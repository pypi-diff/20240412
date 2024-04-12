# Comparing `tmp/marcgrep-0.3.0.tar.gz` & `tmp/marcgrep-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marcgrep-0.3.0.tar", max compression
+gzip compressed data, was "marcgrep-0.4.0.tar", max compression
```

## Comparing `marcgrep-0.3.0.tar` & `marcgrep-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1596 2024-04-04 19:20:55.544537 marcgrep-0.3.0/marcgrep/cli.py
--rw-r--r--   0        0        0     3840 2024-04-04 19:20:55.544537 marcgrep-0.3.0/marcgrep/filter.py
--rw-r--r--   0        0        0     1036 2024-04-04 19:20:55.544537 marcgrep-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3270 2024-04-04 19:20:55.544537 marcgrep-0.3.0/readme.md
--rw-r--r--   0        0        0     4270 1970-01-01 00:00:00.000000 marcgrep-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1842 2024-04-12 03:39:47.247563 marcgrep-0.4.0/marcgrep/cli.py
+-rw-r--r--   0        0        0     3840 2024-04-12 03:39:47.247563 marcgrep-0.4.0/marcgrep/filter.py
+-rw-r--r--   0        0        0     1036 2024-04-12 03:39:47.247563 marcgrep-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3783 2024-04-12 03:39:47.247563 marcgrep-0.4.0/readme.md
+-rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 marcgrep-0.4.0/PKG-INFO
```

### Comparing `marcgrep-0.3.0/marcgrep/cli.py` & `marcgrep-0.4.0/marcgrep/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import math
-from typing import BinaryIO, Literal
+from typing import BinaryIO
 
 import click
 from pymarc import MARCReader
 
 from .filter import Filter
 
 
@@ -13,21 +12,23 @@
 @click.option("--count", "-c", help="Count matching records", is_flag=True)
 @click.option(
     "--include", "-i", help="Include matching records (repeatable)", multiple=True
 )
 @click.option(
     "--exclude", "-e", help="Exclude matching records (repeatable)", multiple=True
 )
+@click.option("--fields", "-f", help="Comma-separated list of fields to print")
 @click.option("--limit", "-l", help="Limit number of records to process", type=int)
 @click.version_option(package_name="marcgrep", message="%(prog)s %(version)s")
 def main(
     file: BinaryIO,
     count: bool,
     include: list[str],
     exclude: list[str],
+    fields: str,
     limit: int,
 ):
     counter = 0
     matched_records = 0
     reader = MARCReader(file)
 
     # build a list of filters, start with exclusive because they rule out records quicker
@@ -36,15 +37,19 @@
 
     for record in reader:
         if record:
             counter += 1
             if all(f.match(record) for f in filters):
                 matched_records += 1
                 if not count:
-                    print(record)
+                    if fields:
+                        for f in record.get_fields(*fields.split(",")):
+                            print(f)
+                    else:
+                        print(record)
             if limit and counter >= limit:
                 break
 
     if count:
         print(matched_records)
 
     # non-zero exit if no records match
```

### Comparing `marcgrep-0.3.0/marcgrep/filter.py` & `marcgrep-0.4.0/marcgrep/filter.py`

 * *Files identical despite different names*

### Comparing `marcgrep-0.3.0/pyproject.toml` & `marcgrep-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marcgrep"
-version = "0.3.0"
+version = "0.4.0"
 description = "search MARC files for regex matches"
 authors = ["phette23 <phette23@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/phette23/marcgreppy"
 repository = "https://github.com/phette23/marcgreppy"
 keywords = ["marc", "grep", "regex", "libraries", "cli", "metadata", "bibliographic", "cataloging"]
```

### Comparing `marcgrep-0.3.0/readme.md` & `marcgrep-0.4.0/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A CLI for searching MARC files like [MARCgrep.pl](https://pusc.it/bib/MARCgrep) but in Python and a bit different syntax.
 
 [marcli](https://github.com/hectorcorrea/marcli) is also a similar project that's faster but a little less flexible.
 
 ## Installation
 
-Python 3.9 or later. [Poetry](https://python-poetry.org/) is used for development.
+Python 3.9 or later.
 
 ```sh
 pipx install marcgrep # install globally with pipx
 pip install marcgrep # or use pip/pip3
 ```
 
 ## Usage
@@ -26,14 +26,15 @@
   Find MARC records matching patterns in a file.
 
 Options:
   -h, --help           Show this message and exit.
   -c, --count          Count matching records
   -i, --include TEXT   Include matching records (repeatable)
   -e, --exclude TEXT   Exclude matching records (repeatable)
+  -f, --fields TEXT    Comma-separated list of fields to print
   -l, --limit INTEGER  Limit number of records to process
   --version            Show the version and exit.
 ```
 
 The `--include` and `--exclude` flags can be used multiple times to specify multiple criteria. They accept a pattern which is a sort of comma-separated filter expression for matching MARC fields. Examples:
 
 ```sh
@@ -57,25 +58,30 @@
 
 The intention of this syntax is to facilitate searching subfields and field values more easily than MARCgrep.pl since we care about them more often than indicators. To ignore a component but use one of lesser priority, leave the component empty. For instance, `856,s,` refers to records with an `856` field with a `$s` subfield but the trailing comma means we don't care about the subfield's value. The pattern `245,,4,,` refers to records with a `245` field with a second indicator of `4` regardless its subfields or value.
 
 Multiple criteria are combined with logical AND. Multiple `--include` flags is narrower than one, as is an `--include` and an `--exclude`.
 
 ## Development
 
+[Poetry](https://python-poetry.org/) is used for development.
+
 - [x] -c count
 - [x] -v version
 - [x] -l limit (number of records to process)
 - [x] -i include criteria (multiple)
 - [x] -e exclude criteria (multiple)
-- [ ] -f fields to print
+- [x] -f fields to print
 - [ ] work with MARC leader
 - [ ] regex for all components? e.g. `24.,text in any 240-249 field`
 - [ ] relatedly, specify _not_ to treat value as a regex?
+- [ ] colorize output?
 
 ```sh
 poetry install # install dependencies
 poetry run pytest # run tests
 ```
 
+Any tag triggers a release to [Test PyPI](https://test.pypi.org/project/marcgrep/). Any tag beginning with the letter `v` requires manual approval to be released to [PyPI](https://pypi.org/project/marcgrep/) and [GitHub](https://github.com/phette23/marcgreppy/releases). There are protection rules on the `pypi` and `testpypi` [environments](https://github.com/phette23/marcgreppy/settings/environments) to this effect, too.
+
 ## License
 
 [MIT](https://opensource.org/license/mit) © Eric Phetteplace 2024.
```

### Comparing `marcgrep-0.3.0/PKG-INFO` & `marcgrep-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marcgrep
-Version: 0.3.0
+Version: 0.4.0
 Summary: search MARC files for regex matches
 Home-page: https://github.com/phette23/marcgreppy
 License: MIT
 Keywords: marc,grep,regex,libraries,cli,metadata,bibliographic,cataloging
 Author: phette23
 Author-email: phette23@gmail.com
 Requires-Python: >3.8
@@ -28,15 +28,15 @@
 
 A CLI for searching MARC files like [MARCgrep.pl](https://pusc.it/bib/MARCgrep) but in Python and a bit different syntax.
 
 [marcli](https://github.com/hectorcorrea/marcli) is also a similar project that's faster but a little less flexible.
 
 ## Installation
 
-Python 3.9 or later. [Poetry](https://python-poetry.org/) is used for development.
+Python 3.9 or later.
 
 ```sh
 pipx install marcgrep # install globally with pipx
 pip install marcgrep # or use pip/pip3
 ```
 
 ## Usage
@@ -52,14 +52,15 @@
   Find MARC records matching patterns in a file.
 
 Options:
   -h, --help           Show this message and exit.
   -c, --count          Count matching records
   -i, --include TEXT   Include matching records (repeatable)
   -e, --exclude TEXT   Exclude matching records (repeatable)
+  -f, --fields TEXT    Comma-separated list of fields to print
   -l, --limit INTEGER  Limit number of records to process
   --version            Show the version and exit.
 ```
 
 The `--include` and `--exclude` flags can be used multiple times to specify multiple criteria. They accept a pattern which is a sort of comma-separated filter expression for matching MARC fields. Examples:
 
 ```sh
@@ -83,26 +84,31 @@
 
 The intention of this syntax is to facilitate searching subfields and field values more easily than MARCgrep.pl since we care about them more often than indicators. To ignore a component but use one of lesser priority, leave the component empty. For instance, `856,s,` refers to records with an `856` field with a `$s` subfield but the trailing comma means we don't care about the subfield's value. The pattern `245,,4,,` refers to records with a `245` field with a second indicator of `4` regardless its subfields or value.
 
 Multiple criteria are combined with logical AND. Multiple `--include` flags is narrower than one, as is an `--include` and an `--exclude`.
 
 ## Development
 
+[Poetry](https://python-poetry.org/) is used for development.
+
 - [x] -c count
 - [x] -v version
 - [x] -l limit (number of records to process)
 - [x] -i include criteria (multiple)
 - [x] -e exclude criteria (multiple)
-- [ ] -f fields to print
+- [x] -f fields to print
 - [ ] work with MARC leader
 - [ ] regex for all components? e.g. `24.,text in any 240-249 field`
 - [ ] relatedly, specify _not_ to treat value as a regex?
+- [ ] colorize output?
 
 ```sh
 poetry install # install dependencies
 poetry run pytest # run tests
 ```
 
+Any tag triggers a release to [Test PyPI](https://test.pypi.org/project/marcgrep/). Any tag beginning with the letter `v` requires manual approval to be released to [PyPI](https://pypi.org/project/marcgrep/) and [GitHub](https://github.com/phette23/marcgreppy/releases). There are protection rules on the `pypi` and `testpypi` [environments](https://github.com/phette23/marcgreppy/settings/environments) to this effect, too.
+
 ## License
 
 [MIT](https://opensource.org/license/mit) © Eric Phetteplace 2024.
```

