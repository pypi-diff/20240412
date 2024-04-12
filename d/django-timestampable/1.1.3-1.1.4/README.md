# Comparing `tmp/django-timestampable-1.1.3.tar.gz` & `tmp/django-timestampable-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-timestampable-1.1.3.tar", last modified: Fri Sep  1 21:10:04 2023, max compression
+gzip compressed data, was "django-timestampable-1.1.4.tar", last modified: Fri Apr 12 10:14:48 2024, max compression
```

## Comparing `django-timestampable-1.1.3.tar` & `django-timestampable-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-09-01 21:10:04.401973 django-timestampable-1.1.3/
--rw-r--r--   0 dmp593     (501) staff       (20)     1063 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/LICENSE
--rw-r--r--   0 dmp593     (501) staff       (20)       58 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/MANIFEST.in
--rw-r--r--   0 dmp593     (501) staff       (20)    10073 2023-09-01 21:10:04.402043 django-timestampable-1.1.3/PKG-INFO
--rw-r--r--   0 dmp593     (501) staff       (20)     8718 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/README.md
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-09-01 21:10:04.400687 django-timestampable-1.1.3/django_timestampable.egg-info/
--rw-r--r--   0 dmp593     (501) staff       (20)    10073 2023-09-01 21:10:04.000000 django-timestampable-1.1.3/django_timestampable.egg-info/PKG-INFO
--rw-r--r--   0 dmp593     (501) staff       (20)      558 2023-09-01 21:10:04.000000 django-timestampable-1.1.3/django_timestampable.egg-info/SOURCES.txt
--rw-r--r--   0 dmp593     (501) staff       (20)        1 2023-09-01 21:10:04.000000 django-timestampable-1.1.3/django_timestampable.egg-info/dependency_links.txt
--rw-r--r--   0 dmp593     (501) staff       (20)       60 2023-09-01 21:10:04.000000 django-timestampable-1.1.3/django_timestampable.egg-info/requires.txt
--rw-r--r--   0 dmp593     (501) staff       (20)       11 2023-09-01 21:10:04.000000 django-timestampable-1.1.3/django_timestampable.egg-info/top_level.txt
--rw-r--r--   0 dmp593     (501) staff       (20)     1337 2023-09-01 21:10:04.402320 django-timestampable-1.1.3/setup.cfg
--rw-r--r--   0 dmp593     (501) staff       (20)      134 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/setup.py
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-09-01 21:10:04.401269 django-timestampable-1.1.3/timestamps/
--rw-r--r--   0 dmp593     (501) staff       (20)        0 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/__init__.py
--rw-r--r--   0 dmp593     (501) staff       (20)       95 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/apps.py
-drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2023-09-01 21:10:04.401867 django-timestampable-1.1.3/timestamps/drf/
--rw-r--r--   0 dmp593     (501) staff       (20)      371 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/__init__.py
--rw-r--r--   0 dmp593     (501) staff       (20)     4705 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/mixins.py
--rw-r--r--   0 dmp593     (501) staff       (20)      469 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/permissions.py
--rw-r--r--   0 dmp593     (501) staff       (20)     2152 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/routers.py
--rw-r--r--   0 dmp593     (501) staff       (20)      414 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/utils.py
--rw-r--r--   0 dmp593     (501) staff       (20)      682 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/drf/viewsets.py
--rw-r--r--   0 dmp593     (501) staff       (20)      921 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/managers.py
--rw-r--r--   0 dmp593     (501) staff       (20)     1853 2023-09-01 21:01:58.000000 django-timestampable-1.1.3/timestamps/models.py
--rw-r--r--   0 dmp593     (501) staff       (20)      613 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/querysets.py
--rw-r--r--   0 dmp593     (501) staff       (20)      140 2023-07-03 09:16:32.000000 django-timestampable-1.1.3/timestamps/signals.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2024-04-12 10:14:48.076330 django-timestampable-1.1.4/
+-rw-r--r--   0 dmp593     (501) staff       (20)     1063 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/LICENSE
+-rw-r--r--   0 dmp593     (501) staff       (20)       58 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/MANIFEST.in
+-rw-r--r--   0 dmp593     (501) staff       (20)    10163 2024-04-12 10:14:48.076402 django-timestampable-1.1.4/PKG-INFO
+-rw-r--r--   0 dmp593     (501) staff       (20)     8718 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/README.md
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2024-04-12 10:14:48.074808 django-timestampable-1.1.4/django_timestampable.egg-info/
+-rw-r--r--   0 dmp593     (501) staff       (20)    10163 2024-04-12 10:14:48.000000 django-timestampable-1.1.4/django_timestampable.egg-info/PKG-INFO
+-rw-r--r--   0 dmp593     (501) staff       (20)      558 2024-04-12 10:14:48.000000 django-timestampable-1.1.4/django_timestampable.egg-info/SOURCES.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)        1 2024-04-12 10:14:48.000000 django-timestampable-1.1.4/django_timestampable.egg-info/dependency_links.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)       60 2024-04-12 10:14:48.000000 django-timestampable-1.1.4/django_timestampable.egg-info/requires.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)       11 2024-04-12 10:14:48.000000 django-timestampable-1.1.4/django_timestampable.egg-info/top_level.txt
+-rw-r--r--   0 dmp593     (501) staff       (20)     1405 2024-04-12 10:14:48.078330 django-timestampable-1.1.4/setup.cfg
+-rw-r--r--   0 dmp593     (501) staff       (20)      134 2024-04-12 10:06:56.000000 django-timestampable-1.1.4/setup.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2024-04-12 10:14:48.075533 django-timestampable-1.1.4/timestamps/
+-rw-r--r--   0 dmp593     (501) staff       (20)        0 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/__init__.py
+-rw-r--r--   0 dmp593     (501) staff       (20)       95 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/apps.py
+drwxr-xr-x   0 dmp593     (501) staff       (20)        0 2024-04-12 10:14:48.076234 django-timestampable-1.1.4/timestamps/drf/
+-rw-r--r--   0 dmp593     (501) staff       (20)      371 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/drf/__init__.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     4784 2024-04-12 09:54:12.000000 django-timestampable-1.1.4/timestamps/drf/mixins.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      469 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/drf/permissions.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     2152 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/drf/routers.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      414 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/drf/utils.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      682 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/drf/viewsets.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      921 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/managers.py
+-rw-r--r--   0 dmp593     (501) staff       (20)     1853 2023-09-01 21:01:58.000000 django-timestampable-1.1.4/timestamps/models.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      613 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/querysets.py
+-rw-r--r--   0 dmp593     (501) staff       (20)      140 2023-07-03 09:16:32.000000 django-timestampable-1.1.4/timestamps/signals.py
```

### Comparing `django-timestampable-1.1.3/LICENSE` & `django-timestampable-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/PKG-INFO` & `django-timestampable-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: django-timestampable
-Version: 1.1.3
+Version: 1.1.4
 Summary: Timestamps and Soft Delete Patterns in Django Models
 Home-page: https://github.com/xgeekshq/django-timestampable/
 Author: Daniel Pinto
 Author-email: dmp593@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: drf
 License-File: LICENSE
```

### Comparing `django-timestampable-1.1.3/README.md` & `django-timestampable-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/django_timestampable.egg-info/PKG-INFO` & `django-timestampable-1.1.4/django_timestampable.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: django-timestampable
-Version: 1.1.3
+Version: 1.1.4
 Summary: Timestamps and Soft Delete Patterns in Django Models
 Home-page: https://github.com/xgeekshq/django-timestampable/
 Author: Daniel Pinto
 Author-email: dmp593@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: drf
 License-File: LICENSE
```

### Comparing `django-timestampable-1.1.3/django_timestampable.egg-info/SOURCES.txt` & `django-timestampable-1.1.4/django_timestampable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/setup.cfg` & `django-timestampable-1.1.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-timestampable
-version = 1.1.3
+version = 1.1.4
 description = Timestamps and Soft Delete Patterns in Django Models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/xgeekshq/django-timestampable/
 author = Daniel Pinto
 author_email = dmp593@gmail.com
 license = MIT
@@ -12,26 +12,28 @@
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
+	Framework :: Django :: 5.0
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Application Frameworks
 
 [options]
 include_package_data = true
 packages = 
 	timestamps
```

### Comparing `django-timestampable-1.1.3/timestamps/drf/mixins.py` & `django-timestampable-1.1.4/timestamps/drf/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 # without the need to use all the views mixins, extended in CoreModelViewSet.
 @aspectlib.Aspect
 def __get_queryset(*args, **kwargs):
     queryset = yield aspectlib.Proceed
 
     view = args[0]
 
+    if not hasattr(view, 'action'):
+        yield aspectlib.Return(queryset) 
+
     mixin = {
         'list_with_deleted': ListWithDeletedModelMixin,
         'retrieve_with_deleted': RetrieveWithDeletedModelMixin,
     }
 
     if is_hard_delete_request(view):
         mixin['destroy'] = DestroyModelMixin
```

### Comparing `django-timestampable-1.1.3/timestamps/drf/routers.py` & `django-timestampable-1.1.4/timestamps/drf/routers.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/timestamps/drf/viewsets.py` & `django-timestampable-1.1.4/timestamps/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/timestamps/managers.py` & `django-timestampable-1.1.4/timestamps/managers.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/timestamps/models.py` & `django-timestampable-1.1.4/timestamps/models.py`

 * *Files identical despite different names*

### Comparing `django-timestampable-1.1.3/timestamps/querysets.py` & `django-timestampable-1.1.4/timestamps/querysets.py`

 * *Files identical despite different names*

