# Comparing `tmp/cubicweb-counters-0.4.0.tar.gz` & `tmp/cubicweb-counters-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-counters-0.4.0.tar", last modified: Fri Apr  8 20:36:40 2022, max compression
+gzip compressed data, was "cubicweb-counters-0.5.0.tar", last modified: Fri Apr 12 12:25:21 2024, max compression
```

## Comparing `cubicweb-counters-0.4.0.tar` & `cubicweb-counters-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)      340 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      444 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       41 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:36:40.603187 cubicweb-counters-0.4.0/cubicweb_counters/
--rw-rw-rw-   0 root         (0) root         (0)       71 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/cubicweb_counters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/cubicweb_counters/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2834 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/cubicweb_counters/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/cubicweb_counters/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1395 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/cubicweb_counters/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/
--rw-r--r--   0 root         (0) root         (0)      444 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-04-08 20:36:40.000000 cubicweb-counters-0.4.0/cubicweb_counters.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2601 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-08 20:36:40.607187 cubicweb-counters-0.4.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)      961 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/test/unittest_counters.py
--rw-rw-rw-   0 root         (0) root         (0)     1941 2022-04-08 20:36:05.000000 cubicweb-counters-0.4.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:25:21.084534 cubicweb-counters-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-12 12:25:21.084534 cubicweb-counters-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:25:21.076533 cubicweb-counters-0.5.0/cubicweb_counters/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/cubicweb_counters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/cubicweb_counters/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2794 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/cubicweb_counters/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/cubicweb_counters/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/cubicweb_counters/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:25:21.080534 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-12 12:25:21.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-12 12:25:20.000000 cubicweb-counters-0.5.0/cubicweb_counters.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 12:25:21.084534 cubicweb-counters-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:25:21.080534 cubicweb-counters-0.5.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:25:21.080534 cubicweb-counters-0.5.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/test/unittest_counters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-04-12 12:24:58.000000 cubicweb-counters-0.5.0/tox.ini
```

### Comparing `cubicweb-counters-0.4.0/cubicweb_counters/__pkginfo__.py` & `cubicweb-counters-0.5.0/cubicweb_counters/__pkginfo__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-counters application packaging information"""
 
 modname = "cubicweb_counters"
 distname = "cubicweb-counters"
 
-numversion = (0, 4, 0)
+numversion = (0, 5, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "sequence/counter classes"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    "cubicweb": ">= 3.33.0, < 3.38.0",
+    "cubicweb": ">= 3.33.0, < 3.39.0",
 }
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python :: 3",
```

### Comparing `cubicweb-counters-0.4.0/cubicweb_counters/entities.py` & `cubicweb-counters-0.5.0/cubicweb_counters/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2011-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2011-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -53,35 +53,34 @@
 
 class PeriodicallyResetCounter(AnyEntity):
     __regid__ = "PeriodicallyResetCounter"
 
     def dc_title(self):
         if self.name:
             return self.name
-        return "{} #{}".format(self.dc_type(), self.eid)
+        return f"{self.dc_type()} #{self.eid}"
 
     def next_value(self):
         """repository only method to use to retrieve next counter value"""
         # update to lock the row
         self._cw.system_sql(
             "UPDATE cw_%s SET cw_value=cw_value+%s WHERE cw_eid=%s"
             % (self.__regid__, self.increment, self.eid)
         )
         cu = self._cw.system_sql(
-            """SELECT cw_value, cw_reset_on, cw_reset_every FROM cw_%s
-            WHERE cw_eid=%s"""
-            % (self.__regid__, self.eid)
+            f"""SELECT cw_value, cw_reset_on, cw_reset_every
+            FROM cw_{self.__regid__}
+            WHERE cw_eid={self.eid}"""
         )
         value, reset_on, reset_mode = cu.fetchone()
         # check if we've to reset the counter
         if need_reset(reset_on, reset_mode):
             value = self.initial_value + self.increment
             self._cw.system_sql(
-                """UPDATE cw_%s SET cw_value=%%(value)s,
-                cw_reset_on=%%(now)s WHERE cw_eid=%s"""
-                % (self.__regid__, self.eid),
+                f"""UPDATE cw_{self.__regid__} SET cw_value=%(value)s,
+                cw_reset_on=%(now)s WHERE cw_eid={self.eid}""",
                 {"value": value, "now": datetime.now()},
             )
         return value
 
 
 # XXX creation hook to initialise cw_value
```

### Comparing `cubicweb-counters-0.4.0/cubicweb_counters/hooks.py` & `cubicweb-counters-0.5.0/cubicweb_counters/hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2011-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2011-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-counters-0.4.0/cubicweb_counters/schema.py` & `cubicweb-counters-0.5.0/cubicweb_counters/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2011-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2011-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-counters-0.4.0/cubicweb_counters.egg-info/SOURCES.txt` & `cubicweb-counters-0.5.0/cubicweb_counters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-counters-0.4.0/setup.py` & `cubicweb-counters-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of a cubicweb-counters.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -51,17 +51,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-counters-0.4.0/test/unittest_counters.py` & `cubicweb-counters-0.5.0/test/unittest_counters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-counters-0.4.0/tox.ini` & `cubicweb-counters-0.5.0/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -6,19 +6,19 @@
   pytest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
   {envpython} -m pytest {posargs}
 
 [testenv:flake8]
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   flake8
 deps =
   flake8
-commands = flake8
+commands = flake8 --show-source
 
 [pytest]
 python_files = *test_*.py
 testpaths = test
 addopts = -r fEs
 
 [testenv:check-manifest]
@@ -28,28 +28,28 @@
 commands =
   {envpython} -m check_manifest {toxinidir}
 
 [testenv:black]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
-  black >= 19.10b0
+  black >= 22.12
 commands = black .
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -57,15 +57,15 @@
   twine check dist/*
   twine upload --skip-existing dist/*
 
 [testenv:deb-publish]
 passenv = JENKINS_USER JENKINS_TOKEN
 basepython = python3
 skip_install = true
-whitelist_externals =
+allowlist_externals =
   rm
   sh
   hg
   python3
 deps =
   httpie
 commands =
@@ -83,7 +83,14 @@
   http -f POST https://{env:JENKINS_USER}:{env:JENKINS_TOKEN}@jenkins.intra.logilab.fr/job/pkg-from-dsc/buildWithParameters DIST=buster source.zip@dist/latest.zip REPO=buster PUBLISH=true
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
+
+[flake8]
+basepython = python3
+format = pylint
+ignore = W503, E203, E731, E231, E501
+max-line-length = 100
+exclude = .tox/*
```

