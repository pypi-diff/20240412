# Comparing `tmp/pysu-0.2.0.tar.gz` & `tmp/pysu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysu-0.2.0.tar", last modified: Fri May  6 18:35:24 2016, max compression
+gzip compressed data, was "pysu-1.0.0.tar", last modified: Thu Apr 11 23:38:31 2024, max compression
```

## Comparing `pysu-0.2.0.tar` & `pysu-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2062 2016-04-21 10:14:55.000000 pysu-0.2.0/README.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1100 2016-04-21 10:39:01.000000 pysu-0.2.0/tox.ini
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       27 2016-04-19 20:07:49.000000 pysu-0.2.0/.dockerignore
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      587 2016-05-06 18:35:24.000000 pysu-0.2.0/setup.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2016-04-19 19:04:57.000000 pysu-0.2.0/AUTHORS.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      134 2016-05-06 18:33:07.000000 pysu-0.2.0/.bumpversion.cfg
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      684 2016-04-21 10:31:38.000000 pysu-0.2.0/.travis.yml
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/ci/
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/ci/py35/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     3160 2016-05-06 18:31:10.000000 pysu-0.2.0/ci/py35/Dockerfile
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/ci/py27/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     3160 2016-05-06 18:31:10.000000 pysu-0.2.0/ci/py27/Dockerfile
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/ci/templates/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     3170 2016-05-06 18:31:10.000000 pysu-0.2.0/ci/templates/Dockerfile
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      705 2016-04-21 10:31:13.000000 pysu-0.2.0/ci/templates/.travis.yml
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/ci/py34/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     3160 2016-05-06 18:31:10.000000 pysu-0.2.0/ci/py34/Dockerfile
--rwxrwxr-x   0 ionel     (1000) ionel     (1000)     2372 2016-04-21 10:31:36.000000 pysu-0.2.0/ci/bootstrap.py
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/src/
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      578 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/SOURCES.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       40 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/entry_points.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        5 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/top_level.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/dependency_links.txt
--rw-rw-r--   0 ionel     (1000) ionel     (1000)        1 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/not-zip-safe
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2168 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu.egg-info/PKG-INFO
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/src/pysu/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1888 2016-05-06 18:31:10.000000 pysu-0.2.0/src/pysu/cli.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      377 2016-04-19 19:04:57.000000 pysu-0.2.0/src/pysu/__main__.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       22 2016-05-06 18:33:07.000000 pysu-0.2.0/src/pysu/__init__.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      406 2016-04-19 21:22:35.000000 pysu-0.2.0/MANIFEST.in
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      215 2016-04-19 19:04:57.000000 pysu-0.2.0/.editorconfig
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      168 2016-04-19 19:04:57.000000 pysu-0.2.0/.coveragerc
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2702 2016-05-06 18:33:07.000000 pysu-0.2.0/setup.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2696 2016-04-19 19:04:57.000000 pysu-0.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1302 2016-04-19 19:04:57.000000 pysu-0.2.0/LICENSE
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     2168 2016-05-06 18:35:24.000000 pysu-0.2.0/PKG-INFO
--rw-rw-r--   0 ionel     (1000) ionel     (1000)     1030 2016-04-19 19:04:57.000000 pysu-0.2.0/.cookiecutterrc
-drwxrwxr-x   0 ionel     (1000) ionel     (1000)        0 2016-05-06 18:35:24.000000 pysu-0.2.0/tests/
--rw-rw-r--   0 ionel     (1000) ionel     (1000)       71 2016-04-19 19:04:57.000000 pysu-0.2.0/tests/test_pysu.py
--rw-rw-r--   0 ionel     (1000) ionel     (1000)      239 2016-05-06 18:32:34.000000 pysu-0.2.0/CHANGELOG.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.224209 pysu-1.0.0/
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      605 2024-04-11 23:38:17.000000 pysu-1.0.0/.bumpversion.cfg
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1541 2024-04-11 23:38:17.000000 pysu-1.0.0/.cookiecutterrc
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      172 2024-04-11 13:41:26.000000 pysu-1.0.0/.coveragerc
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       27 2024-04-11 13:05:36.000000 pysu-1.0.0/.dockerignore
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)      353 2024-04-11 13:41:26.000000 pysu-1.0.0/.editorconfig
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.219209 pysu-1.0.0/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.221209 pysu-1.0.0/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3973 2024-04-11 13:41:26.000000 pysu-1.0.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      702 2024-04-11 13:47:47.000000 pysu-1.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       70 2024-04-11 13:41:26.000000 pysu-1.0.0/AUTHORS.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      461 2024-04-11 23:32:09.000000 pysu-1.0.0/CHANGELOG.rst
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2313 2024-04-11 13:41:26.000000 pysu-1.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)     1337 2024-04-11 13:41:26.000000 pysu-1.0.0/LICENSE
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      424 2024-04-11 16:29:05.000000 pysu-1.0.0/MANIFEST.in
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2726 2024-04-11 23:38:31.224209 pysu-1.0.0/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2132 2024-04-11 23:38:17.000000 pysu-1.0.0/README.rst
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2867 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/bootstrap.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py27/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py27/Dockerfile
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py34/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py34/Dockerfile
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/py35/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3160 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/py35/Dockerfile
+-rw-rw-r--   0 ionel     (1000) ionel     (1000)       72 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/requirements.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/templates/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.220209 pysu-1.0.0/ci/templates/.github/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/ci/templates/.github/workflows/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1812 2024-04-11 13:41:26.000000 pysu-1.0.0/ci/templates/.github/workflows/github-actions.yml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3170 2024-04-11 13:05:36.000000 pysu-1.0.0/ci/templates/Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1352 2024-04-11 13:41:26.000000 pysu-1.0.0/pyproject.toml
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      901 2024-04-11 13:41:26.000000 pysu-1.0.0/pytest.ini
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       38 2024-04-11 23:38:31.224209 pysu-1.0.0/setup.cfg
+-rwxr-xr-x   0 ionel     (1000) ionel     (1000)     2819 2024-04-11 23:38:17.000000 pysu-1.0.0/setup.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.220209 pysu-1.0.0/src/
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.222209 pysu-1.0.0/src/pysu/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       22 2024-04-11 23:38:17.000000 pysu-1.0.0/src/pysu/__init__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      378 2024-04-11 13:47:13.000000 pysu-1.0.0/src/pysu/__main__.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3055 2024-04-11 16:09:52.000000 pysu-1.0.0/src/pysu/cli.py
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.223209 pysu-1.0.0/src/pysu.egg-info/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     2726 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/PKG-INFO
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      767 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/SOURCES.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/dependency_links.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)       39 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/entry_points.txt
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        1 2024-04-11 23:38:30.000000 pysu-1.0.0/src/pysu.egg-info/not-zip-safe
+-rw-r--r--   0 ionel     (1000) ionel     (1000)        5 2024-04-11 23:38:31.000000 pysu-1.0.0/src/pysu.egg-info/top_level.txt
+drwxr-xr-x   0 ionel     (1000) ionel     (1000)        0 2024-04-11 23:38:31.223209 pysu-1.0.0/tests/
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3165 2024-04-11 16:08:38.000000 pysu-1.0.0/tests/test-alpine.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     3281 2024-04-11 16:08:45.000000 pysu-1.0.0/tests/test-debian.Dockerfile
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      404 2024-04-11 23:32:03.000000 pysu-1.0.0/tests/test_docker.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)      347 2024-04-11 15:01:08.000000 pysu-1.0.0/tests/test_pysu.py
+-rw-r--r--   0 ionel     (1000) ionel     (1000)     1487 2024-04-11 13:41:26.000000 pysu-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysu-0.2.0/README.rst` & `pysu-1.0.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -4,65 +4,62 @@
 
 .. start-badges
 
 .. list-table::
     :stub-columns: 1
 
     * - tests
-      - | |travis| |requires|
-        |
+      - |github-actions|
     * - package
-      - |version| |downloads| |wheel| |supported-versions| |supported-implementations|
+      - |version| |wheel| |supported-versions| |supported-implementations| |commits-since|
 
-.. |docs| image:: https://readthedocs.org/projects/python-su/badge/?style=flat
-    :target: https://readthedocs.org/projects/python-su
-    :alt: Documentation Status
+.. |github-actions| image:: https://github.com/ionelmc/python-su/actions/workflows/github-actions.yml/badge.svg
+    :alt: GitHub Actions Build Status
+    :target: https://github.com/ionelmc/python-su/actions
 
-.. |travis| image:: https://travis-ci.org/ionelmc/python-su.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.org/ionelmc/python-su
-
-.. |requires| image:: https://requires.io/github/ionelmc/python-su/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/ionelmc/python-su/requirements/?branch=master
-
-.. |version| image:: https://img.shields.io/pypi/v/pysu.svg?style=flat
+.. |version| image:: https://img.shields.io/pypi/v/pysu.svg
     :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/pysu
+    :target: https://pypi.org/project/pysu
 
-.. |downloads| image:: https://img.shields.io/pypi/dm/pysu.svg?style=flat
-    :alt: PyPI Package monthly downloads
-    :target: https://pypi.python.org/pypi/pysu
-
-.. |wheel| image:: https://img.shields.io/pypi/wheel/pysu.svg?style=flat
+.. |wheel| image:: https://img.shields.io/pypi/wheel/pysu.svg
     :alt: PyPI Wheel
-    :target: https://pypi.python.org/pypi/pysu
+    :target: https://pypi.org/project/pysu
 
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pysu.svg?style=flat
+.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/pysu.svg
     :alt: Supported versions
-    :target: https://pypi.python.org/pypi/pysu
+    :target: https://pypi.org/project/pysu
 
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pysu.svg?style=flat
+.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/pysu.svg
     :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/pysu
+    :target: https://pypi.org/project/pysu
+
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ionelmc/python-su/v1.0.0.svg
+    :alt: Commits since latest release
+    :target: https://github.com/ionelmc/python-su/compare/v1.0.0...master
+
 
 
 .. end-badges
 
 Simple Python-based setuid+setgid+setgroups+exec. A port of https://github.com/tianon/gosu
 
-* Free software: BSD license
+* Free software: BSD 2-Clause License
 
 Installation
 ============
 
 ::
 
     pip install pysu
 
+You can also install the in-development version with::
+
+    pip install https://github.com/ionelmc/python-su/archive/master.zip
+
+
 Documentation
 =============
 
 Usage: pysu [-h] user[:group] command
 
 Change user and exec command.
 
@@ -72,10 +69,27 @@
 
 optional arguments:
   -h, --help  show this help message and exit
 
 Development
 ===========
 
-To run the all tests run::
+To run all the tests run::
 
     tox
+
+Note, to combine the coverage data from all the tox environments run:
+
+.. list-table::
+    :widths: 10 90
+    :stub-columns: 1
+
+    - - Windows
+      - ::
+
+            set PYTEST_ADDOPTS=--cov-append
+            tox
+
+    - - Other
+      - ::
+
+            PYTEST_ADDOPTS=--cov-append tox
```

### Comparing `pysu-0.2.0/tox.ini` & `pysu-1.0.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,71 @@
-; a generative tox configuration, see: https://testrun.org/tox/latest/config.html#generative-envlist
+[testenv:bootstrap]
+deps =
+    jinja2
+    tox
+skip_install = true
+commands =
+    python ci/bootstrap.py --no-env
+passenv =
+    *
 
+; a generative tox configuration, see: https://tox.wiki/en/latest/user_guide.html#generative-environments
 [tox]
 envlist =
+    clean,
     check,
-    py{27,34,35}
+    {py38,py39,py310,py311,py312,pypy38,pypy39,pypy310},
+    report
+ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    pypy: {env:TOXPYTHON:pypy}
-    {py27,docs,spell}: {env:TOXPYTHON:python2.7}
-    py33: {env:TOXPYTHON:python3.3}
-    py34: {env:TOXPYTHON:python3.4}
-    py35: {env:TOXPYTHON:python3.5}
-    {clean,check,report,coveralls,codecov}: python3.5
-    bootstrap: python
+    pypy38: {env:TOXPYTHON:pypy3.8}
+    pypy39: {env:TOXPYTHON:pypy3.9}
+    pypy310: {env:TOXPYTHON:pypy3.10}
+    py38: {env:TOXPYTHON:python3.8}
+    py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
+    py311: {env:TOXPYTHON:python3.11}
+    py312: {env:TOXPYTHON:python3.12}
+    {bootstrap,clean,check,report}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
 usedevelop = false
 deps =
+    pytest
+    pytest-cov
 commands =
-    docker build --file=ci/{envname}/Dockerfile .
-whitelist_externals =
-    docker
-
-[testenv:bootstrap]
-deps =
-    jinja2
-    matrix
-skip_install = true
-commands =
-    python ci/bootstrap.py
-passenv =
-    *
+    {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
-    flake8
+    pre-commit
     readme-renderer
     pygments
     isort
 skip_install = true
 commands =
     python setup.py check --strict --metadata --restructuredtext
-    check-manifest {toxinidir}
-    flake8 src tests setup.py
-    isort --verbose --check-only --diff --recursive src tests setup.py
+    check-manifest .
+    pre-commit run --all-files --show-diff-on-failure
 
+[testenv:report]
+deps =
+    coverage
+skip_install = true
+commands =
+    coverage report
+    coverage html
+
+[testenv:clean]
+commands =
+    python setup.py clean
+    coverage erase
+skip_install = true
+deps =
+    coverage
```

### Comparing `pysu-0.2.0/ci/py35/Dockerfile` & `pysu-1.0.0/ci/py35/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-0.2.0/ci/py27/Dockerfile` & `pysu-1.0.0/ci/py27/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-0.2.0/ci/templates/Dockerfile` & `pysu-1.0.0/ci/templates/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-0.2.0/ci/py34/Dockerfile` & `pysu-1.0.0/ci/py34/Dockerfile`

 * *Files identical despite different names*

### Comparing `pysu-0.2.0/src/pysu.egg-info/SOURCES.txt` & `pysu-1.0.0/src/pysu.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .dockerignore
 .editorconfig
-.travis.yml
+.pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
+pytest.ini
 setup.py
 tox.ini
+.github/workflows/github-actions.yml
 ci/bootstrap.py
+ci/requirements.txt
 ci/py27/Dockerfile
 ci/py34/Dockerfile
 ci/py35/Dockerfile
-ci/templates/.travis.yml
 ci/templates/Dockerfile
+ci/templates/.github/workflows/github-actions.yml
 src/pysu/__init__.py
 src/pysu/__main__.py
 src/pysu/cli.py
 src/pysu.egg-info/PKG-INFO
 src/pysu.egg-info/SOURCES.txt
 src/pysu.egg-info/dependency_links.txt
 src/pysu.egg-info/entry_points.txt
 src/pysu.egg-info/not-zip-safe
 src/pysu.egg-info/top_level.txt
+tests/test-alpine.Dockerfile
+tests/test-debian.Dockerfile
+tests/test_docker.py
 tests/test_pysu.py
```

### Comparing `pysu-0.2.0/CONTRIBUTING.rst` & `pysu-1.0.0/CONTRIBUTING.rst`

 * *Files 20% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 
 To set up `python-su` for local development:
 
 1. Fork `python-su <https://github.com/ionelmc/python-su>`_
    (look for the "Fork" button).
 2. Clone your fork locally::
 
-    git clone git@github.com:your_name_here/python-su.git
+    git clone git@github.com:YOURGITHUBNAME/python-su.git
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes, run all the checks, doc builder and spell checker with `tox <http://tox.readthedocs.org/en/latest/install.html>`_ one command::
+4. When you're done making changes run all the checks and docs builder with one command::
 
     tox
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
@@ -64,27 +64,22 @@
 Pull Request Guidelines
 -----------------------
 
 If you need some code review or feedback while you're developing the code just make the pull request.
 
 For merging, you should:
 
-1. Include passing tests (run ``tox``) [1]_.
+1. Include passing tests (run ``tox``).
 2. Update documentation when there's new API, functionality etc.
 3. Add a note to ``CHANGELOG.rst`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/ionelmc/python-su/pull_requests>`_ for each change you add in the pull request.
-
-       It will be slower though ...
-
 Tips
 ----
 
 To run a subset of tests::
 
-    tox -e envname -- py.test -k test_myfeature
+    tox -e envname -- pytest -k test_myfeature
 
-To run all the test environments in *parallel* (you need to ``pip install detox``)::
+To run all the test environments in *parallel*::
 
-    detox
+    tox -p auto
```

### Comparing `pysu-0.2.0/LICENSE` & `pysu-1.0.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,10 @@
-Copyright (c) 2016, Ionel Cristian Mărieș
-All rights reserved.
+BSD 2-Clause License
 
-Redistribution and use in source and binary forms, with or without modification, are permitted provided that the
-following conditions are met:
+Copyright (c) 2016-2024, Ionel Cristian Mărieș. All rights reserved.
 
-1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following
-disclaimer.
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following
-disclaimer in the documentation and/or other materials provided with the distribution.
+    1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+    2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
-THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

