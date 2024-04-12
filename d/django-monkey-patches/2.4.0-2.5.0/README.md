# Comparing `tmp/django_monkey_patches-2.4.0.tar.gz` & `tmp/django_monkey_patches-2.5.0.tar.gz`

## Comparing `django_monkey_patches-2.4.0.tar` & `django_monkey_patches-2.5.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39086 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    14772 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/COPYING.LESSER
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/README.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    12932 2020-02-02 00:00:00.000000 django_monkey_patches-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/README_printable.md
+-rwxr-xr-x   0        0        0     1592 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/build_readme.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    24374 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.0/PKG-INFO
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
-The goal of dev_side_code files is to keep code that should not be used
+----------------------------------------------------------------------
+The goal of dev_side_code files is to keep code
+that should not be used
 but was used to create the best code possible in some patches.
 Below, is the code for micro-optimisations of
 retrieve_forward_cache_callback_for_foreign_key.
 """
 
 # pylint: disable=too-many-lines
 
@@ -1325,202 +1331,202 @@
 callbacks.update(
     {
         "c_field_list_list": cc_field_list_list("field_name"),
         "c_field_id_list_list": cc_field_id_list_list("field_name"),
         "c_field_not_none_list_list": cc_field_not_none_list_list(
             "field_name"
         ),
-        "c_field_id_not_none_list_list": cc_field_id_not_none_list_list(
-            "field_name"
+        "c_field_id_not_none_list_list": (
+            cc_field_id_not_none_list_list("field_name")
         ),
         "c_field_none_list_list": cc_field_none_list_list(
             "field_name"
         ),
         "c_field_id_none_list_list": cc_field_id_none_list_list(
             "field_name"
         ),
         "c_field_tuple_tuple": cc_field_tuple_tuple("field_name"),
         "c_field_id_tuple_tuple": cc_field_id_tuple_tuple(
             "field_name"
         ),
         "c_field_not_none_tuple_tuple": cc_field_not_none_tuple_tuple(
             "field_name"
         ),
-        "c_field_id_not_none_tuple_tuple": cc_field_id_not_none_tuple_tuple(
-            "field_name"
+        "c_field_id_not_none_tuple_tuple": (
+            cc_field_id_not_none_tuple_tuple("field_name")
         ),
         "c_field_none_tuple_tuple": cc_field_none_tuple_tuple(
             "field_name"
         ),
         "c_field_id_none_tuple_tuple": cc_field_id_none_tuple_tuple(
             "field_name"
         ),
         "c_field_list_tuple": cc_field_list_tuple("field_name"),
         "c_field_id_list_tuple": cc_field_id_list_tuple("field_name"),
         "c_field_not_none_list_tuple": cc_field_not_none_list_tuple(
             "field_name"
         ),
-        "c_field_id_not_none_list_tuple": cc_field_id_not_none_list_tuple(
-            "field_name"
+        "c_field_id_not_none_list_tuple": (
+            cc_field_id_not_none_list_tuple("field_name")
         ),
         "c_field_none_list_tuple": cc_field_none_list_tuple(
             "field_name"
         ),
         "c_field_id_none_list_tuple": cc_field_id_none_list_tuple(
             "field_name"
         ),
         "c_field_tuple_list": cc_field_tuple_list("field_name"),
         "c_field_id_tuple_list": cc_field_id_tuple_list("field_name"),
         "c_field_not_none_tuple_list": cc_field_not_none_tuple_list(
             "field_name"
         ),
-        "c_field_id_not_none_tuple_list": cc_field_id_not_none_tuple_list(
-            "field_name"
+        "c_field_id_not_none_tuple_list": (
+            cc_field_id_not_none_tuple_list("field_name")
         ),
         "c_field_none_tuple_list": cc_field_none_tuple_list(
             "field_name"
         ),
         "c_field_id_none_tuple_list": cc_field_id_none_tuple_list(
             "field_name"
         ),
         "c_field_tuple_empty": cc_field_tuple_empty("field_name"),
         "c_field_id_tuple_empty": cc_field_id_tuple_empty(
             "field_name"
         ),
         "c_field_not_none_tuple_empty": cc_field_not_none_tuple_empty(
             "field_name"
         ),
-        "c_field_id_not_none_tuple_empty": cc_field_id_not_none_tuple_empty(
-            "field_name"
+        "c_field_id_not_none_tuple_empty": (
+            cc_field_id_not_none_tuple_empty("field_name")
         ),
         "c_field_none_tuple_empty": cc_field_none_tuple_empty(
             "field_name"
         ),
         "c_field_id_none_tuple_empty": cc_field_id_none_tuple_empty(
             "field_name"
         ),
         "c_field_list_empty": cc_field_list_empty("field_name"),
         "c_field_id_list_empty": cc_field_id_list_empty("field_name"),
         "c_field_not_none_list_empty": cc_field_not_none_list_empty(
             "field_name"
         ),
-        "c_field_id_not_none_list_empty": cc_field_id_not_none_list_empty(
-            "field_name"
+        "c_field_id_not_none_list_empty": (
+            cc_field_id_not_none_list_empty("field_name")
         ),
         "c_field_none_list_empty": cc_field_none_list_empty(
             "field_name"
         ),
         "c_field_id_none_list_empty": cc_field_id_none_list_empty(
             "field_name"
         ),
         "c_field_list_list_nnl": cc_field_list_list_nnl("field_name"),
         "c_field_id_list_list_nnl": cc_field_id_list_list_nnl(
             "field_name"
         ),
-        "c_field_not_none_list_list_nnl": cc_field_not_none_list_list_nnl(
-            "field_name"
+        "c_field_not_none_list_list_nnl": (
+            cc_field_not_none_list_list_nnl("field_name")
         ),
-        "c_field_id_not_none_list_list_nnl": cc_field_id_not_none_list_list_nnl(
-            "field_name"
+        "c_field_id_not_none_list_list_nnl": (
+            cc_field_id_not_none_list_list_nnl("field_name")
         ),
         "c_field_none_list_list_nnl": cc_field_none_list_list_nnl(
             "field_name"
         ),
-        "c_field_id_none_list_list_nnl": cc_field_id_none_list_list_nnl(
-            "field_name"
+        "c_field_id_none_list_list_nnl": (
+            cc_field_id_none_list_list_nnl("field_name")
         ),
         "c_field_tuple_tuple_nnl": cc_field_tuple_tuple_nnl(
             "field_name"
         ),
         "c_field_id_tuple_tuple_nnl": cc_field_id_tuple_tuple_nnl(
             "field_name"
         ),
-        "c_field_not_none_tuple_tuple_nnl": cc_field_not_none_tuple_tuple_nnl(
-            "field_name"
+        "c_field_not_none_tuple_tuple_nnl": (
+            cc_field_not_none_tuple_tuple_nnl("field_name")
         ),
-        "c_field_id_not_none_tuple_tuple_nnl": cc_field_id_not_none_tuple_tuple_nnl(
-            "field_name"
+        "c_field_id_not_none_tuple_tuple_nnl": (
+            cc_field_id_not_none_tuple_tuple_nnl("field_name")
         ),
-        "c_field_none_tuple_tuple_nnl": cc_field_none_tuple_tuple_nnl(
-            "field_name"
+        "c_field_none_tuple_tuple_nnl": (
+            cc_field_none_tuple_tuple_nnl("field_name")
         ),
-        "c_field_id_none_tuple_tuple_nnl": cc_field_id_none_tuple_tuple_nnl(
-            "field_name"
+        "c_field_id_none_tuple_tuple_nnl": (
+            cc_field_id_none_tuple_tuple_nnl("field_name")
         ),
-        "c_field_list_tuple_nnl": cc_field_list_tuple_nnl(
-            "field_name"
+        "c_field_list_tuple_nnl": (
+            cc_field_list_tuple_nnl("field_name")
         ),
         "c_field_id_list_tuple_nnl": cc_field_id_list_tuple_nnl(
             "field_name"
         ),
-        "c_field_not_none_list_tuple_nnl": cc_field_not_none_list_tuple_nnl(
-            "field_name"
+        "c_field_not_none_list_tuple_nnl": (
+            cc_field_not_none_list_tuple_nnl("field_name")
         ),
-        "c_field_id_not_none_list_tuple_nnl": cc_field_id_not_none_list_tuple_nnl(
-            "field_name"
+        "c_field_id_not_none_list_tuple_nnl": (
+            cc_field_id_not_none_list_tuple_nnl("field_name")
         ),
         "c_field_none_list_tuple_nnl": cc_field_none_list_tuple_nnl(
             "field_name"
         ),
-        "c_field_id_none_list_tuple_nnl": cc_field_id_none_list_tuple_nnl(
-            "field_name"
+        "c_field_id_none_list_tuple_nnl": (
+            cc_field_id_none_list_tuple_nnl("field_name")
         ),
         "c_field_tuple_list_nnl": cc_field_tuple_list_nnl(
             "field_name"
         ),
         "c_field_id_tuple_list_nnl": cc_field_id_tuple_list_nnl(
             "field_name"
         ),
-        "c_field_not_none_tuple_list_nnl": cc_field_not_none_tuple_list_nnl(
-            "field_name"
+        "c_field_not_none_tuple_list_nnl": (
+            cc_field_not_none_tuple_list_nnl("field_name")
         ),
-        "c_field_id_not_none_tuple_list_nnl": cc_field_id_not_none_tuple_list_nnl(
-            "field_name"
+        "c_field_id_not_none_tuple_list_nnl": (
+            cc_field_id_not_none_tuple_list_nnl("field_name")
         ),
         "c_field_none_tuple_list_nnl": cc_field_none_tuple_list_nnl(
             "field_name"
         ),
-        "c_field_id_none_tuple_list_nnl": cc_field_id_none_tuple_list_nnl(
-            "field_name"
+        "c_field_id_none_tuple_list_nnl": (
+            cc_field_id_none_tuple_list_nnl("field_name")
         ),
         "c_field_tuple_empty_nnl": cc_field_tuple_empty_nnl(
             "field_name"
         ),
         "c_field_id_tuple_empty_nnl": cc_field_id_tuple_empty_nnl(
             "field_name"
         ),
-        "c_field_not_none_tuple_empty_nnl": cc_field_not_none_tuple_empty_nnl(
-            "field_name"
+        "c_field_not_none_tuple_empty_nnl": (
+            cc_field_not_none_tuple_empty_nnl("field_name")
         ),
-        "c_field_id_not_none_tuple_empty_nnl": cc_field_id_not_none_tuple_empty_nnl(
-            "field_name"
+        "c_field_id_not_none_tuple_empty_nnl": (
+            cc_field_id_not_none_tuple_empty_nnl("field_name")
         ),
         "c_field_none_tuple_empty_nnl": cc_field_none_tuple_empty_nnl(
             "field_name"
         ),
-        "c_field_id_none_tuple_empty_nnl": cc_field_id_none_tuple_empty_nnl(
-            "field_name"
+        "c_field_id_none_tuple_empty_nnl": (
+            cc_field_id_none_tuple_empty_nnl("field_name")
         ),
         "c_field_list_empty_nnl": cc_field_list_empty_nnl(
             "field_name"
         ),
         "c_field_id_list_empty_nnl": cc_field_id_list_empty_nnl(
             "field_name"
         ),
-        "c_field_not_none_list_empty_nnl": cc_field_not_none_list_empty_nnl(
-            "field_name"
+        "c_field_not_none_list_empty_nnl": (
+            cc_field_not_none_list_empty_nnl("field_name")
         ),
-        "c_field_id_not_none_list_empty_nnl": cc_field_id_not_none_list_empty_nnl(
-            "field_name"
+        "c_field_id_not_none_list_empty_nnl": (
+            cc_field_id_not_none_list_empty_nnl("field_name")
         ),
         "c_field_none_list_empty_nnl": cc_field_none_list_empty_nnl(
             "field_name"
         ),
-        "c_field_id_none_list_empty_nnl": cc_field_id_none_list_empty_nnl(
-            "field_name"
+        "c_field_id_none_list_empty_nnl": (
+            cc_field_id_none_list_empty_nnl("field_name")
         ),
     }
 )
 
 NUMBER_OF_ITERATIONS = 1000000
 
 
@@ -1555,14 +1561,14 @@
             f" Sans FK: {data['time_without_fk']}"
         )
 
 
 # Benchmark each callback.
 benchmark(callbacks)
 
-print("-------------------------------------------------------")
+print("-------------------------------------------------------------")
 
 # Benchmark each callback in random order.
 keys = list(callbacks.keys())
 random.shuffle(keys)
 callbacks_2 = {key: callbacks[key] for key in keys}
 benchmark(callbacks_2)
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 A collection of functions to make the key used by the cache.
 As of now, it is only for tests.
 """
 
 import os
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 To optimize some queries, you may need to add prefetches
 that apply only to some of the instances.
 It is very convenient when you have some expensive prefetches
 that concerns only a few instances.
 Hence, I added a filter_callback argument to Prefetch.
 #ClimateChangeBrake
 Note that I also submitted a ticket and a PR:
@@ -62,36 +67,48 @@
                     for obj2 in obj.needed_ps:
                         obj.needed_p_by[obj2.c_id] = obj2
 
         return query_set.prefetch_related(
             f"{prefix}p2",
             Prefetch(
                 f"{prefix}s",
-                post_prefetch_callback=create_post_prefetch_callback_add_backward_multiple(
-                    retrieve_forward_cache_callback=lambda o: [o.s] if o.s_id else [],
+                post_prefetch_callback=(
+                  create_post_prefetch_callback_add_backward_multiple(
+                    retrieve_forward_cache_callback=lambda o: [o.s]
+                    if o.s_id
+                    else [],
                     backward_cache_name="current_o_ancestors",
+                  )
                 ),
             ),
             Prefetch(
                 f"{prefix}c2",
-                post_prefetch_callback=create_post_prefetch_callback_add_backward_multiple(
-                    retrieve_forward_cache_callback=lambda o:[o.c2] if o.c2_id else [],
+                post_prefetch_callback=(
+                  create_post_prefetch_callback_add_backward_multiple(
+                    retrieve_forward_cache_callback=lambda o:[o.c2]
+                    if o.c2_id
+                    else [],
                     backward_cache_name="current_order_ancestors",
+                  )
                 ),
             ),
             Prefetch(
                 f"{prefix}s__ps",
                 queryset=(
                     P.objects.filter(c_id=c_id)
                     if c_id
                     else P.objects.all()
                 ),
                 to_attr="needed_ps",
-                filter_callback=lambda p: hasattr(p, "_prefetched_objects_cache")
-                and p._prefetched_objects_cache.get("current_order_ancestors")
+                filter_callback=(
+                  lambda p: hasattr(p, "_prefetched_objects_cache")
+                )
+                and p._prefetched_objects_cache.get(
+                    "current_order_ancestors"
+                )
                 and any(
                     map(
                         lambda o: o.c2_id is not None,
                         p._prefetched_objects_cache.get(
                             "current_o_ancestors"
                         ).values(),
                     )
@@ -114,15 +131,17 @@
                         to_attr="needed_ps",
                         post_prefetch_callback=ventilate_ps_by_c_id,
                     ),
                 ),
                 to_attr="needed_u",
                 filter_callback=lambda c: (
                     hasattr(c2, "_prefetched_objects_cache")
-                    and c2._prefetched_objects_cache.get("current_o_ancestors")
+                    and c2._prefetched_objects_cache.get(
+                        "current_o_ancestors"
+                    )
                     and any(
                         map(
                             lambda o: o.c2_id is not None
                             and o.s_id is None,
                             c._prefetched_objects_cache.get(
                                 "current_o_ancestors"
                             ).values(),
@@ -163,17 +182,23 @@
                 ).select_related("r2"),
                 to_attr="pertinent_r3",
             ),
         )
 
         return query_set
 
-So maybe now you understand why I do not understand framework maintainers
+So maybe now, you understand why
+I do not understand framework maintainers
 that block any new feature not coming from them.
 I think we don't live in code of the same complexity.
+I did a second PR,
+mainly because it can help (but it was rejected as usual),
+and because it can help for understanding this patch,
+and see that the modifications needed are only minor:
+https://github.com/django/django/pull/18003
 """
 
 import importlib
 
 # pylint: disable-next=import-error
 from django.db.models import Prefetch, query
 
@@ -275,21 +300,23 @@
         "done_queries = {}",
         'done_queries = {"": model_instances}',
     )
     .replace(
         "if lookup.prefetch_to in done_queries:",
         "if lookup.prefetch_to in done_queries:\n"
         "            if lookup.post_prefetch_callback:\n"
-        "                lookup.post_prefetch_callback(lookup, done_queries)\n",
+        "                lookup.post_prefetch_callback("
+        "lookup, done_queries)\n",
     )
     .replace(
         "obj_list = new_obj_list",
         "obj_list = new_obj_list\n"
         "        if lookup.post_prefetch_callback:\n"
-        "            lookup.post_prefetch_callback(lookup, done_queries)\n",
+        "            lookup.post_prefetch_callback("
+        "lookup, done_queries)\n",
     )
 )
 
 
 # local value needed for the exec
 prefetch_one_level = patched_prefetch_one_level_v1
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 In older versions of Django, a prefetch use the ordering defined
 on the class prefetched.
 class Meta:
     ordering = ...
 But when you prefetch and there is a single value per current object
 that will recieve the prefetch in its cache,
 then the ordering is totally useless.
@@ -40,15 +45,16 @@
 
 # pylint: disable-next=import-error
 from django.db.models.fields.related_descriptors import (
     ForwardManyToOneDescriptor,
     ReverseOneToOneDescriptor,
 )
 
-# In old versions of Django, the method is called get_prefetch_queryset().
+# In old versions of Django,
+# the method is called get_prefetch_queryset().
 # It is deprecated in Django 5 and will be removed in Django 6.
 # Apply the patch that corresponds to your version.
 # pylint: disable-next=invalid-name
 original_forward_many_to_one_get_prefetch_queryset = None
 if hasattr(ForwardManyToOneDescriptor, "get_prefetch_queryset"):
     original_forward_many_to_one_get_prefetch_queryset = (
         ForwardManyToOneDescriptor.get_prefetch_queryset
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
 
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
 """
 
 # pylint: disable-next=import-error
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
 
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
-There is an inconsistency in behavior of current QuerySet.get_or_create():
+----------------------------------------------------------------------
+There is an inconsistency in behavior
+of current QuerySet.get_or_create():
 It avoids unnecessary DB query for related object given as argument
 only if created is True.
 I gave a script demonstrating this here:
 https://code.djangoproject.com/ticket/34884
 The patch of get_or_create() can be replaced by
 a more general patch on QuerySet.get().
 """
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
 
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
-There is an inconsistency in behavior of current QuerySet.get_or_create():
+----------------------------------------------------------------------
+There is an inconsistency in behavior
+of current QuerySet.get_or_create():
 It avoids unnecessary DB query for related object given as argument
 only if created is True.
 I gave a script demonstrating this here:
 https://code.djangoproject.com/ticket/34884
 In my tests, this patch yields a speed up of almost 10 %,
 since it avoids many unnecessary queries.
 """
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 r"""
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 Choose between flaky tests by default,
 and slow tests by default.
 The topic is complex,
 because you may end up having tests
-where most of the time is spent on the same cache filling over and over.
+where most of the time is spent
+on the same cache filling over and over.
 But the good news is that you can apply or not this patch at will.
 
 /!\/!\/!\ cache.clear() can do a lot of harm
-if you have a cache infrastructure shared between your test environment
-and your production environment,
+if you have a cache infrastructure shared
+between your test environment and your production environment,
 or shared between your Django application and another application.
-As the Django doc states at https://docs.djangoproject.com/en/dev/topics/cache/ :
-> Finally, if you want to delete all the keys in the cache, use cache.clear().
+As the Django doc states at
+https://docs.djangoproject.com/en/dev/topics/cache/:
+> Finally, if you want to delete all the keys in the cache,
+> use cache.clear().
 > Be careful with this; clear() will remove everything from the cache,
 > not just the keys set by your application.
 Better solutions exist by searching for cache keys with some prefix,
 and then using cache.delete_many().
 But there is no uniform way yet, across cache backends,
 to get cache keys with some prefix.
 See:
-https://stackoverflow.com/questions/9048257/get-list-of-cache-keys-in-django
+https://stackoverflow.com/questions/9048257/\
+  get-list-of-cache-keys-in-django
 For this solution and Redis,
 you will have to choose v2 and modify your caches settings
 according to your use case.
 
-/!\ Make sure you call super().tearDown() in your custom tearDown() methods.
+/!\ Make sure you call super().tearDown()
+in your custom tearDown() methods.
 """
 
 import os
 from typing import Dict
 
 # pylint: disable-next=import-error
 from django.conf import settings
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 Django Rest Framework is considered "feature-complete".
 But if you had the chance to work with an in-house framework
 like I did in PHP for 8,5 years,
-you know that there is no such thing as a "feature-complete" framework ;).
-The goal of this patch is to shorten application code with small helpers
-for accessing request in serializers.
+you know that there is no such thing as
+a "feature-complete" framework ;).
+The goal of this patch is to shorten application code
+with small helpers for accessing request in serializers.
 https://github.com/encode/django-rest-framework/issues/8457
-Field class introduces the context property and BaseSerializer inherits of Field,
+Field class introduces the context property,
+and BaseSerializer inherits of Field,
 so the right place to add this helper functions is Field.
 """
 
 # pylint: disable-next=import-error
 from rest_framework.fields import Field
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-2.5.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 """
 This file is part of django-monkey-patches library.
 
-django-monkey-patches is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-django-monkey-patches is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.    See the
-GNU Lesser General Public License for more details.
+django-monkey-patches is free software:
+you can redistribute it and/or modify it under the terms
+of the GNU Lesser General Public License
+as published by the Free Software Foundation,
+either version 3 of the License,
+or (at your option) any later version.
+
+django-monkey-patches is distributed in the hope
+that it will be useful,
+but WITHOUT ANY WARRANTY;
+without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+See the GNU Lesser General Public License for more details.
 
-You should have received a copy of the GNU Lesser General Public License
+You should have received a copy of
+the GNU Lesser General Public License
 along with django-monkey-patches.
 If not, see <http://www.gnu.org/licenses/>.
 
 ©Copyright 2023-2024 Laurent Lyaudet
--------------------------------------------------------------------------
+----------------------------------------------------------------------
 Django Rest Framework is considered "feature-complete".
 But if you had the chance to work with an in-house framework
 like I did in PHP for 8,5 years,
-you know that there is no such thing as a "feature-complete" framework ;).
-The goal of this patch is to have a sensible place to add unconventional prefetches.
+you know that there is no such thing as
+a "feature-complete" framework :(.
+The goal of this patch is to have a sensible place
+to add unconventional prefetches.
 You may apply the patch,
-or use patched_to_representation_v1 in a class inheriting from ListSerializer.
+or use patched_to_representation_v1
+in a class inheriting from ListSerializer.
 """
 
 # pylint: disable-next=import-error
 from django.db import models
 
 # pylint: disable-next=import-error
 from rest_framework.serializers import ListSerializer
```

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.4.0/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-2.5.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.4.0/COPYING` & `django_monkey_patches-2.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.4.0/COPYING.LESSER` & `django_monkey_patches-2.5.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.4.0/README.md` & `django_monkey_patches-2.5.0/README_printable.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,131 @@
 # django-monkey-patches
 
-[![pypi-version]][pypi]
-[![Downloads](https://img.shields.io/pypi/dm/django-monkey-patches)](https://pypistats.org/packages/django-monkey-patches)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches/badge)](https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/c928d2b8b724abcb2913/maintainability)](https://codeclimate.com/github/LLyaudet/django-monkey-patches/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/de6280433b32447684458fb655c3a4b3)](https://app.codacy.com/gh/LLyaudet/django-monkey-patches/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/django-monkey-patches)
-![GitHub License](https://img.shields.io/github/license/llyaudet/django-monkey-patches)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-monkey-patches)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/django-monkey-patches)
-[![GitHub Sponsors](https://img.shields.io/github/sponsors/LLyaudet)](https://github.com/sponsors/LLyaudet)
+[![PyPI-version-badge]][PyPI-package-page]
+[![Downloads-badge]][PyPIStats-package-page]
+[![Code-style:black:badge]][Black-GitHub.com]
+[![Imports:isort:badge]][Isort-GitHub.io]
+[![Linting:pylint:badge]][Pylint-GitHub.com]
+[![CodeFactor-badge]][CodeFactor-package-page]
+[![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
+[![Codacy-badge]][Codacy-package-page]
+![GitHub-top-language-badge]
+![GitHub-license-badge]
+![PyPI-python-version-badge]
+![GitHub-code-size-in-bytes-badge]
+[![GitHub-sponsors-badge]][GitHub-sponsors-page]
 
-|     **A collection of monkey patches to improve Django framework**     |
+| **A collection of monkey patches to improve Django framework** |
 
 
 ## Use
 
-Each monkey-patch `beautiful_patch` should be available with a function `apply_beautiful_patch()`.
+Each monkey-patch `beautiful_patch` should be available
+with a function `apply_beautiful_patch()`.
 Hence, all you have to do is:
 
 ```python
-from django_monkey_patches.django__beautiful_class__beautiful_patch import apply_beautiful_patch
+from django_monkey_patches.django__beautiful_class__beautiful_patch\
+    import apply_beautiful_patch
 
 apply_beautiful_patch()
 ```
 
-For example, you can do it in your Django settings.py file or in a file imported in settings.py.
+For example, you can do it in your Django settings.py file
+or in a file imported in settings.py.
 
 
 ## Choosing a patch
 
 Look at the source code on GitHub.
 The rational behind each patch is given in the source code file.
-If you cannot bother reading the source code of a patch of ten or twenty lines,
+If you cannot bother reading the source code
+of a patch of ten or twenty lines,
 you probably should not apply it anyway ;).
 
 
 ## F.A.Q.
 
 ### Why does the version not follow Django versions?
 
-Because I plan to add monkey-patches for other packages around Django itself.
-For example, Django Rest Framework (DRF) is in "maintenance mode only".
-It does not accept new features and is only updated to keep compatibility with new versions of Django.
-Moreover, many patches wil be plainly compatible with most versions of Django,
+Because I plan to add monkey-patches for other packages
+around Django itself.
+For example, Django Rest Framework (DRF)
+is in "maintenance mode only".
+It does not accept new features
+and is only updated to keep compatibility
+with new versions of Django.
+Moreover,
+many patches wil be plainly compatible with most versions of Django,
 and I don't see the need of multiplying versions.
-So instead, I use semantic versioning relative to the proposed patches.
+So instead,
+I use semantic versioning relative to the proposed patches.
 
 ### Why is Django not a dependency?
 
 See previous question.
 
 ### Why is there no tests folder?
 
 See previous question.
 
-[pypi-version]: https://img.shields.io/pypi/v/django-monkey-patches.svg
-[pypi]: https://pypi.org/project/django-monkey-patches/
+[PyPI-version-badge]: https://img.shields.io/pypi/v/\
+django-monkey-patches.svg
+
+[PyPI-package-page]: https://pypi.org/project/django-monkey-patches/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/\
+django-monkey-patches
+
+[PyPIStats-package-page]: https://pypistats.org/packages/\
+django-monkey-patches
+
+[Code-style:black:badge]: https://img.shields.io/badge/\
+code%20style-black-000000.svg
+
+[Black-GitHub.com]: https://github.com/psf/black
+
+[Imports:isort:badge]: https://img.shields.io/badge/\
+%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+
+[Isort-GitHub.io]: https://pycqa.github.io/isort/
+
+[Linting:pylint:badge]: https://img.shields.io/badge/\
+linting-pylint-yellowgreen
+
+[Pylint-GitHub.com]: https://github.com/pylint-dev/pylint
+
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/\
+llyaudet/django-monkey-patches/badge
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/\
+github/llyaudet/django-monkey-patches
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/\
+badges/c928d2b8b724abcb2913/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/\
+github/LLyaudet/django-monkey-patches/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/\
+de6280433b32447684458fb655c3a4b3
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/\
+django-monkey-patches/dashboard?utm_source=gh&utm_medium=referral\
+&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/\
+languages/top/llyaudet/django-monkey-patches
+
+[GitHub-license-badge]: https://img.shields.io/github/license/\
+llyaudet/django-monkey-patches
+
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/\
+django-monkey-patches
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/\
+languages/code-size/llyaudet/django-monkey-patches
+
+[GitHub-sponsors-badge]: https://img.shields.io/github/sponsors/\
+LLyaudet
+
+[GitHub-sponsors-page]: https://github.com/sponsors/LLyaudet
```

### Comparing `django_monkey_patches-2.4.0/pyproject.toml` & `django_monkey_patches-2.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "2.4.0"
-description = "Add monkey-patches to correct and enhance your favorite framework"
+version = "2.5.0"
+description = """\
+Add monkey-patches to correct and enhance your favorite framework\
+"""
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
 license = { file = "COPYING.LESSER" }
 classifiers = [
-    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
+    """\
+License :: OSI Approved :: \
+GNU Lesser General Public License v3 or later (LGPLv3+)\
+""",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["Django", "monkey-patch"]
 dependencies = [
 ]
@@ -29,15 +34,17 @@
   "black",
   "isort",
   "pylint",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LLyaudet/django-monkey-patches"
-"Bug Tracker" = "https://github.com/LLyaudet/django-monkey-patches/issues"
+"Bug Tracker" = """\
+https://github.com/LLyaudet/django-monkey-patches/issues\
+"""
 
 [tool.black]
 line-length = 70
 
 [tool.isort]
 profile = "black"
 line_length = 70
```

### Comparing `django_monkey_patches-2.4.0/PKG-INFO` & `django_monkey_patches-2.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 2.4.0
+Version: 2.5.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -182,67 +182,118 @@
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pylint; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # django-monkey-patches
 
-[![pypi-version]][pypi]
-[![Downloads](https://img.shields.io/pypi/dm/django-monkey-patches)](https://pypistats.org/packages/django-monkey-patches)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-[![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
-[![CodeFactor](https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches/badge)](https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches)
-[![CodeClimateMaintainability](https://api.codeclimate.com/v1/badges/c928d2b8b724abcb2913/maintainability)](https://codeclimate.com/github/LLyaudet/django-monkey-patches/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/de6280433b32447684458fb655c3a4b3)](https://app.codacy.com/gh/LLyaudet/django-monkey-patches/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
-![GitHub top language](https://img.shields.io/github/languages/top/llyaudet/django-monkey-patches)
-![GitHub License](https://img.shields.io/github/license/llyaudet/django-monkey-patches)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-monkey-patches)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/llyaudet/django-monkey-patches)
-[![GitHub Sponsors](https://img.shields.io/github/sponsors/LLyaudet)](https://github.com/sponsors/LLyaudet)
+[![PyPI-version-badge]][PyPI-package-page]
+[![Downloads-badge]][PyPIStats-package-page]
+[![Code-style:black:badge]][Black-GitHub.com]
+[![Imports:isort:badge]][Isort-GitHub.io]
+[![Linting:pylint:badge]][Pylint-GitHub.com]
+[![CodeFactor-badge]][CodeFactor-package-page]
+[![CodeClimateMaintainability-badge]][CodeClimateM13y-package-page]
+[![Codacy-badge]][Codacy-package-page]
+![GitHub-top-language-badge]
+![GitHub-license-badge]
+![PyPI-python-version-badge]
+![GitHub-code-size-in-bytes-badge]
+[![GitHub-sponsors-badge]][GitHub-sponsors-page]
 
-|     **A collection of monkey patches to improve Django framework**     |
+| **A collection of monkey patches to improve Django framework** |
 
 
 ## Use
 
-Each monkey-patch `beautiful_patch` should be available with a function `apply_beautiful_patch()`.
+Each monkey-patch `beautiful_patch` should be available
+with a function `apply_beautiful_patch()`.
 Hence, all you have to do is:
 
 ```python
-from django_monkey_patches.django__beautiful_class__beautiful_patch import apply_beautiful_patch
+from django_monkey_patches.django__beautiful_class__beautiful_patch\
+    import apply_beautiful_patch
 
 apply_beautiful_patch()
 ```
 
-For example, you can do it in your Django settings.py file or in a file imported in settings.py.
+For example, you can do it in your Django settings.py file
+or in a file imported in settings.py.
 
 
 ## Choosing a patch
 
 Look at the source code on GitHub.
 The rational behind each patch is given in the source code file.
-If you cannot bother reading the source code of a patch of ten or twenty lines,
+If you cannot bother reading the source code
+of a patch of ten or twenty lines,
 you probably should not apply it anyway ;).
 
 
 ## F.A.Q.
 
 ### Why does the version not follow Django versions?
 
-Because I plan to add monkey-patches for other packages around Django itself.
-For example, Django Rest Framework (DRF) is in "maintenance mode only".
-It does not accept new features and is only updated to keep compatibility with new versions of Django.
-Moreover, many patches wil be plainly compatible with most versions of Django,
+Because I plan to add monkey-patches for other packages
+around Django itself.
+For example, Django Rest Framework (DRF)
+is in "maintenance mode only".
+It does not accept new features
+and is only updated to keep compatibility
+with new versions of Django.
+Moreover,
+many patches wil be plainly compatible with most versions of Django,
 and I don't see the need of multiplying versions.
-So instead, I use semantic versioning relative to the proposed patches.
+So instead,
+I use semantic versioning relative to the proposed patches.
 
 ### Why is Django not a dependency?
 
 See previous question.
 
 ### Why is there no tests folder?
 
 See previous question.
 
-[pypi-version]: https://img.shields.io/pypi/v/django-monkey-patches.svg
-[pypi]: https://pypi.org/project/django-monkey-patches/
+[PyPI-version-badge]: https://img.shields.io/pypi/v/django-monkey-patches.svg
+
+[PyPI-package-page]: https://pypi.org/project/django-monkey-patches/
+
+[Downloads-badge]: https://img.shields.io/pypi/dm/django-monkey-patches
+
+[PyPIStats-package-page]: https://pypistats.org/packages/django-monkey-patches
+
+[Code-style:black:badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+
+[Black-GitHub.com]: https://github.com/psf/black
+
+[Imports:isort:badge]: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+
+[Isort-GitHub.io]: https://pycqa.github.io/isort/
+
+[Linting:pylint:badge]: https://img.shields.io/badge/linting-pylint-yellowgreen
+
+[Pylint-GitHub.com]: https://github.com/pylint-dev/pylint
+
+[CodeFactor-badge]: https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches/badge
+
+[CodeFactor-package-page]: https://www.codefactor.io/repository/github/llyaudet/django-monkey-patches
+
+[CodeClimateMaintainability-badge]: https://api.codeclimate.com/v1/badges/c928d2b8b724abcb2913/maintainability
+
+[CodeClimateM13y-package-page]: https://codeclimate.com/github/LLyaudet/django-monkey-patches/maintainability
+
+[Codacy-badge]: https://app.codacy.com/project/badge/Grade/de6280433b32447684458fb655c3a4b3
+
+[Codacy-package-page]: https://app.codacy.com/gh/LLyaudet/django-monkey-patches/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade
+
+[GitHub-top-language-badge]: https://img.shields.io/github/languages/top/llyaudet/django-monkey-patches
+
+[GitHub-license-badge]: https://img.shields.io/github/license/llyaudet/django-monkey-patches
+
+[PyPI-python-version-badge]: https://img.shields.io/pypi/pyversions/django-monkey-patches
+
+[GitHub-code-size-in-bytes-badge]: https://img.shields.io/github/languages/code-size/llyaudet/django-monkey-patches
+
+[GitHub-sponsors-badge]: https://img.shields.io/github/sponsors/LLyaudet
+
+[GitHub-sponsors-page]: https://github.com/sponsors/LLyaudet
```

