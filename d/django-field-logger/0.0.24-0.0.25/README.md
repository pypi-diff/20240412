# Comparing `tmp/django-field-logger-0.0.24.tar.gz` & `tmp/django-field-logger-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-field-logger-0.0.24.tar", last modified: Thu Apr 11 16:55:48 2024, max compression
+gzip compressed data, was "django-field-logger-0.0.25.tar", last modified: Fri Apr 12 03:16:25 2024, max compression
```

## Comparing `django-field-logger-0.0.24.tar` & `django-field-logger-0.0.25.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.24/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.24/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9200 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7601 2024-04-11 16:53:44.000000 django-field-logger-0.0.24/README.rst
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/django_field_logger.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9200 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      530 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-11 16:55:48.000000 django-field-logger-0.0.24/django_field_logger.egg-info/top_level.txt
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/fieldlogger/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.24/fieldlogger/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.24/fieldlogger/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.24/fieldlogger/config.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.24/fieldlogger/fieldlogger.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.24/fieldlogger/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2621 2024-04-11 07:22:36.000000 django-field-logger-0.0.24/fieldlogger/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.24/fieldlogger/signals.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.24/fieldlogger/utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.24/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      670 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       96 2024-04-11 16:55:39.000000 django-field-logger-0.0.24/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-11 16:55:48.645359 django-field-logger-0.0.24/tests/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.24/tests/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.24/tests/settings.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.24/tests/test_utils.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.24/tests/tests.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2024-01-16 20:01:32.000000 django-field-logger-0.0.25/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-field-logger-0.0.25/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9881 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     7673 2024-04-12 03:10:09.000000 django-field-logger-0.0.25/README.rst
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/django_field_logger.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     9881 2024-04-12 03:16:25.000000 django-field-logger-0.0.25/django_field_logger.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      530 2024-04-12 03:16:25.000000 django-field-logger-0.0.25/django_field_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-04-12 03:16:25.000000 django-field-logger-0.0.25/django_field_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-12 03:16:25.000000 django-field-logger-0.0.25/django_field_logger.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       12 2024-04-12 03:16:25.000000 django-field-logger-0.0.25/django_field_logger.egg-info/top_level.txt
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/fieldlogger/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-01-16 20:05:29.000000 django-field-logger-0.0.25/fieldlogger/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      219 2024-01-16 20:51:47.000000 django-field-logger-0.0.25/fieldlogger/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3135 2024-04-08 14:39:49.000000 django-field-logger-0.0.25/fieldlogger/config.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      862 2024-04-01 09:39:30.000000 django-field-logger-0.0.25/fieldlogger/fieldlogger.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      350 2024-01-17 04:38:48.000000 django-field-logger-0.0.25/fieldlogger/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2622 2024-04-12 03:07:50.000000 django-field-logger-0.0.25/fieldlogger/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1563 2024-04-08 14:41:10.000000 django-field-logger-0.0.25/fieldlogger/signals.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      296 2024-03-27 00:36:10.000000 django-field-logger-0.0.25/fieldlogger/utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      415 2024-04-01 09:32:10.000000 django-field-logger-0.0.25/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1136 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/setup.cfg
+-rwxr-xr-x   0 nibblex   (1000) nibblex   (1000)       96 2024-04-11 16:55:39.000000 django-field-logger-0.0.25/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-04-12 03:16:25.385675 django-field-logger-0.0.25/tests/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2024-03-27 02:22:33.000000 django-field-logger-0.0.25/tests/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2913 2024-04-11 07:12:55.000000 django-field-logger-0.0.25/tests/settings.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3943 2024-04-11 07:23:31.000000 django-field-logger-0.0.25/tests/test_utils.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1788 2024-04-11 07:26:07.000000 django-field-logger-0.0.25/tests/tests.py
```

### Comparing `django-field-logger-0.0.24/LICENSE` & `django-field-logger-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/PKG-INFO` & `django-field-logger-0.0.25/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,53 @@
-Metadata-Version: 2.1
-Name: django-field-logger
-Version: 0.0.24
-Summary: A Django app for logging changes in model fields.
-Home-page: https://github.com/nibblex/django-field-logger
-Author: Sergio Rodríguez
-Author-email: srodriguez3441@gmail.com
-Maintainer: Sergio Rodríguez
-Maintainer-email: srodriguez3441@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-License-File: LICENSE
-
 Django Field Logger
 ===================
 
 A Django app for logging changes in model fields.
 
 How to set up?
 ~~~~~~~~~~~~~~
 
 1) Add ``fieldlogger`` to your ``INSTALLED_APPS``
 2) Run ``python manage.py migrate`` to initialize the model
 3) Add ``FIELD_LOGGER_SETTINGS`` to your ``settings.py`` file.
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'ENCODER': 'path.to.your.json.Encoder', # (default: None)
-       'DECODER': 'path.to.your.json.Decoder', # (default: None)
-       'LOGGING_ENABLED': True, # (default: True)
-       'FAIL_SILENTLY': True, # (default: True)
-       'LOGGING_APPS': {
-           'your_app': {
-               'logging_enabled': True, # (default: True)
-               'fail_silently': True, # (default: True)
-               'models': {
-                   'YourModel': {
-                       'logging_enabled': True, # (default: True)
-                       'fail_silently': True, # (default: True)
-                       'fields': ['field1', 'field2'], # (default: [])
-                       'exclude_fields': ['field3', 'field4'], # (default: [])
-                       'callbacks': [
-                           lambda instance, fields, logs: print(instance, fields, logs),
-                           'yourapp.app.callbacks.your_function_name'
-                       ], # (default: [])
-                   },
-               },
-               'callbacks': [
-                   lambda instances, fields, logs: print(instances, fields, logs),
-                   'yourapp.app.callbacks.your_function_name'
-               ], # (default: [])
-           },
-       },
-       'CALLBACKS': [
-           lambda instance, fields, logs: print(instance, fields, logs),
-           'yourapp.app.callbacks.your_function_name'
-       ], # (default: [])
-   }
+    FIELD_LOGGER_SETTINGS={
+        'ENCODER': 'path.to.your.json.Encoder', # (default: None)
+        'DECODER': 'path.to.your.json.Decoder', # (default: None)
+        'LOGGING_ENABLED': True, # (default: True)
+        'FAIL_SILENTLY': True, # (default: True)
+        'LOGGING_APPS': {
+            'your_app': {
+                'logging_enabled': True, # (default: True)
+                'fail_silently': True, # (default: True)
+                'models': {
+                    'YourModel': {
+                        'logging_enabled': True, # (default: True)
+                        'fail_silently': True, # (default: True)
+                        'fields': ['field1', 'field2'], # (default: [])
+                        'exclude_fields': ['field3', 'field4'], # (default: [])
+                        'callbacks': [
+                            lambda instance, fields, logs: print(instance, fields, logs),
+                            'yourapp.app.callbacks.your_function_name'
+                        ], # (default: [])
+                    },
+                },
+                'callbacks': [
+                    lambda instances, fields, logs: print(instances, fields, logs),
+                    'yourapp.app.callbacks.your_function_name'
+                ], # (default: [])
+            },
+        },
+        'CALLBACKS': [
+            lambda instance, fields, logs: print(instance, fields, logs),
+            'yourapp.app.callbacks.your_function_name'
+        ], # (default: [])
+    }
 
 -  ``ENCODER`` and ``DECODER`` are optional. If you want to
    encode/decode your model instance fields, you can specify your
    encoder/decoder classes here. Your encoder/decoder classes must be
    subclasses of ``json.JSONEncoder`` and ``json.JSONDecoder``
    respectively.
 -  ``LOGGING_ENABLED`` is optional. If you want to disable logging
@@ -109,108 +93,108 @@
 
 This section serves as a small example to demonstrate how to use this package.
 
 Supposing you have this configuration in your settings.py file:
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'LOGGING_APPS': {
-           'drivers': {
-               'models': {
-                   'Driver': {
-                       'fields': ['driver_name']
-                   },
-               },
-           },
-       },
-   }
+    FIELD_LOGGER_SETTINGS={
+        'LOGGING_APPS': {
+            'drivers': {
+                'models': {
+                    'Driver': {
+                        'fields': ['driver_name']
+                    },
+                },
+            },
+        },
+    }
 
 Supposing you have a model called ``Driver`` with fields called
 ``latest_speed``, ``driver_name``, ``driver_id``:
 
 .. code:: python
 
-       driver = Driver.objects.last()
-       driver.latest_speed = 5
-       driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
-
-       driver.driver_name = 'John Doe'
-       driver.save()  # a record with this driver is created
-
-       driver.driver_name = 'Jane Doe'
-       driver.save()  # a record with this driver is created
-
-       instance_id = driver.id
-       app_label = driver._meta.app_label
-       model = driver._meta.model_name
+    driver = Driver.objects.last()
+    driver.latest_speed = 5
+    driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
+
+    driver.driver_name = 'John Doe'
+    driver.save()  # a record with this driver is created
+
+    driver.driver_name = 'Jane Doe'
+    driver.save()  # a record with this driver is created
+
+    instance_id = driver.id
+    app_label = driver._meta.app_label
+    model = driver._meta.model_name
 
-       log = FieldLog.objects.filter(instance_id=instance_id, app_label=app_label, table_name=model).last()
-       print(log.field, log.old_value, log.new_value)  # prints: driver_name John Doe Jane Doe
+    log = FieldLog.objects.filter(instance_id=instance_id, app_label=app_label, table_name=model).last()
+    print(log.field, log.old_value, log.new_value)  # prints: driver_name John Doe Jane Doe
 
 Callback example
 ~~~~~~~~~~~~~~~~
 
 Supposing you have this function in yourapp/callbacks.py which sets the
 ``extra_data`` field of the ``FieldLog`` model:
 
 .. code:: python
 
-   def set_extra_data_for_driver_name(instance, fields, logs):
-       log = logs.get('driver_name')
-       if log:
-           log.extra_data = {
-               'name_length': len(log.new_value)
-           }
-           log.save()
+    def set_extra_data_for_driver_name(instance, fields, logs):
+        log = logs.get('driver_name')
+        if log:
+            log.extra_data = {
+                'name_length': len(log.new_value)
+            }
+            log.save()
 
 Then you can add this callback function to your configuration like this:
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'LOGGING_APPS': {
-           'drivers': {
-               'models': {
-                   'Driver': {
-                       'fields': ['driver_name'],
-                       'callbacks': [
-                           'yourapp.callbacks.set_extra_data_for_driver_name'
-                       ]
-                   },
-               },
-           },
-       },
-   }
+    FIELD_LOGGER_SETTINGS={
+        'LOGGING_APPS': {
+            'drivers': {
+                'models': {
+                    'Driver': {
+                        'fields': ['driver_name'],
+                        'callbacks': [
+                            'yourapp.callbacks.set_extra_data_for_driver_name'
+                        ]
+                    },
+                },
+            },
+        },
+    }
 
 .. note::
 
     You can also add lambda functions to your callbacks
 
 The model structure
 ~~~~~~~~~~~~~~~~~~~
 
 This package provides you a django model which is called ``FieldLog``;
 which tracks each change to a model instance specified in your
 configuration mapping. An example record is as follows:
 
 ::
 
-   {
-    'id': 2,
-    'app_label': 'drivers',
-    'model': 'driver',
-    'instance_id': 1,
-    'field': 'latest_speed',
-    'timestamp': datetime.datetime(2024, 1, 16, 9, 1, 14, 619568, tzinfo=<UTC>),
-    'old_value': 'John Doe',
-    'new_value': 'Jane Doe',
-    'extra_data': {}, # this is a JSONField, you can store any extra data here using callbacks or by overriding it directly
-    'created': False, # this is a boolean field, if it is True, it means that instance is a newly created instance
-   }
+    {
+        'id': 2,
+        'app_label': 'drivers',
+        'model': 'driver',
+        'instance_id': 1,
+        'field': 'latest_speed',
+        'timestamp': datetime.datetime(2024, 1, 16, 9, 1, 14, 619568, tzinfo=<UTC>),
+        'old_value': 'John Doe',
+        'new_value': 'Jane Doe',
+        'extra_data': {}, # this is a JSONField, you can store any extra data here using callbacks or by overriding it directly
+        'created': False, # this is a boolean field, if it is True, it means that instance is a newly created instance
+    }
 
 Additionally, ``FieldLog`` model provides the following properties:
 
 -  ``model_class``: returns the model class of the instance that is
    being logged.
 -  ``instance``: returns the instance that is being logged.
 -  ``previous_log``: returns the previous log of the instance that is
@@ -225,31 +209,9 @@
 
 -  ``fieldlog_set`` since the ``FieldLog`` model has not a direct
    relation to the model that is being logged, you can use this property
    to get the logs of the instance that is being logged.
 
    .. code:: python
 
-       driver = Driver.objects.last()
-       logs = driver.fieldlog_set.all()
-
-MIT License
-
-Copyright (c) 2024 Sergio Rodríguez
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+        driver = Driver.objects.last()
+        logs = driver.fieldlog_set.all()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django-field-logger-0.0.24/django_field_logger.egg-info/PKG-INFO` & `django-field-logger-0.0.25/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,33 @@
 Metadata-Version: 2.1
 Name: django-field-logger
-Version: 0.0.24
+Version: 0.0.25
 Summary: A Django app for logging changes in model fields.
 Home-page: https://github.com/nibblex/django-field-logger
 Author: Sergio Rodríguez
 Author-email: srodriguez3441@gmail.com
 Maintainer: Sergio Rodríguez
 Maintainer-email: srodriguez3441@gmail.com
 License: MIT
-Classifier: Programming Language :: Python :: 3
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Django Field Logger
 ===================
 
 A Django app for logging changes in model fields.
@@ -24,46 +37,46 @@
 
 1) Add ``fieldlogger`` to your ``INSTALLED_APPS``
 2) Run ``python manage.py migrate`` to initialize the model
 3) Add ``FIELD_LOGGER_SETTINGS`` to your ``settings.py`` file.
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'ENCODER': 'path.to.your.json.Encoder', # (default: None)
-       'DECODER': 'path.to.your.json.Decoder', # (default: None)
-       'LOGGING_ENABLED': True, # (default: True)
-       'FAIL_SILENTLY': True, # (default: True)
-       'LOGGING_APPS': {
-           'your_app': {
-               'logging_enabled': True, # (default: True)
-               'fail_silently': True, # (default: True)
-               'models': {
-                   'YourModel': {
-                       'logging_enabled': True, # (default: True)
-                       'fail_silently': True, # (default: True)
-                       'fields': ['field1', 'field2'], # (default: [])
-                       'exclude_fields': ['field3', 'field4'], # (default: [])
-                       'callbacks': [
-                           lambda instance, fields, logs: print(instance, fields, logs),
-                           'yourapp.app.callbacks.your_function_name'
-                       ], # (default: [])
-                   },
-               },
-               'callbacks': [
-                   lambda instances, fields, logs: print(instances, fields, logs),
-                   'yourapp.app.callbacks.your_function_name'
-               ], # (default: [])
-           },
-       },
-       'CALLBACKS': [
-           lambda instance, fields, logs: print(instance, fields, logs),
-           'yourapp.app.callbacks.your_function_name'
-       ], # (default: [])
-   }
+    FIELD_LOGGER_SETTINGS={
+        'ENCODER': 'path.to.your.json.Encoder', # (default: None)
+        'DECODER': 'path.to.your.json.Decoder', # (default: None)
+        'LOGGING_ENABLED': True, # (default: True)
+        'FAIL_SILENTLY': True, # (default: True)
+        'LOGGING_APPS': {
+            'your_app': {
+                'logging_enabled': True, # (default: True)
+                'fail_silently': True, # (default: True)
+                'models': {
+                    'YourModel': {
+                        'logging_enabled': True, # (default: True)
+                        'fail_silently': True, # (default: True)
+                        'fields': ['field1', 'field2'], # (default: [])
+                        'exclude_fields': ['field3', 'field4'], # (default: [])
+                        'callbacks': [
+                            lambda instance, fields, logs: print(instance, fields, logs),
+                            'yourapp.app.callbacks.your_function_name'
+                        ], # (default: [])
+                    },
+                },
+                'callbacks': [
+                    lambda instances, fields, logs: print(instances, fields, logs),
+                    'yourapp.app.callbacks.your_function_name'
+                ], # (default: [])
+            },
+        },
+        'CALLBACKS': [
+            lambda instance, fields, logs: print(instance, fields, logs),
+            'yourapp.app.callbacks.your_function_name'
+        ], # (default: [])
+    }
 
 -  ``ENCODER`` and ``DECODER`` are optional. If you want to
    encode/decode your model instance fields, you can specify your
    encoder/decoder classes here. Your encoder/decoder classes must be
    subclasses of ``json.JSONEncoder`` and ``json.JSONDecoder``
    respectively.
 -  ``LOGGING_ENABLED`` is optional. If you want to disable logging
@@ -109,108 +122,108 @@
 
 This section serves as a small example to demonstrate how to use this package.
 
 Supposing you have this configuration in your settings.py file:
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'LOGGING_APPS': {
-           'drivers': {
-               'models': {
-                   'Driver': {
-                       'fields': ['driver_name']
-                   },
-               },
-           },
-       },
-   }
+    FIELD_LOGGER_SETTINGS={
+        'LOGGING_APPS': {
+            'drivers': {
+                'models': {
+                    'Driver': {
+                        'fields': ['driver_name']
+                    },
+                },
+            },
+        },
+    }
 
 Supposing you have a model called ``Driver`` with fields called
 ``latest_speed``, ``driver_name``, ``driver_id``:
 
 .. code:: python
 
-       driver = Driver.objects.last()
-       driver.latest_speed = 5
-       driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
-
-       driver.driver_name = 'John Doe'
-       driver.save()  # a record with this driver is created
-
-       driver.driver_name = 'Jane Doe'
-       driver.save()  # a record with this driver is created
-
-       instance_id = driver.id
-       app_label = driver._meta.app_label
-       model = driver._meta.model_name
+    driver = Driver.objects.last()
+    driver.latest_speed = 5
+    driver.save()  # fieldlogger won't create a record since 'latest_speed' was not among the loggable fields
+
+    driver.driver_name = 'John Doe'
+    driver.save()  # a record with this driver is created
+
+    driver.driver_name = 'Jane Doe'
+    driver.save()  # a record with this driver is created
+
+    instance_id = driver.id
+    app_label = driver._meta.app_label
+    model = driver._meta.model_name
 
-       log = FieldLog.objects.filter(instance_id=instance_id, app_label=app_label, table_name=model).last()
-       print(log.field, log.old_value, log.new_value)  # prints: driver_name John Doe Jane Doe
+    log = FieldLog.objects.filter(instance_id=instance_id, app_label=app_label, table_name=model).last()
+    print(log.field, log.old_value, log.new_value)  # prints: driver_name John Doe Jane Doe
 
 Callback example
 ~~~~~~~~~~~~~~~~
 
 Supposing you have this function in yourapp/callbacks.py which sets the
 ``extra_data`` field of the ``FieldLog`` model:
 
 .. code:: python
 
-   def set_extra_data_for_driver_name(instance, fields, logs):
-       log = logs.get('driver_name')
-       if log:
-           log.extra_data = {
-               'name_length': len(log.new_value)
-           }
-           log.save()
+    def set_extra_data_for_driver_name(instance, fields, logs):
+        log = logs.get('driver_name')
+        if log:
+            log.extra_data = {
+                'name_length': len(log.new_value)
+            }
+            log.save()
 
 Then you can add this callback function to your configuration like this:
 
 .. code:: python
 
-   FIELD_LOGGER_SETTINGS={
-       'LOGGING_APPS': {
-           'drivers': {
-               'models': {
-                   'Driver': {
-                       'fields': ['driver_name'],
-                       'callbacks': [
-                           'yourapp.callbacks.set_extra_data_for_driver_name'
-                       ]
-                   },
-               },
-           },
-       },
-   }
+    FIELD_LOGGER_SETTINGS={
+        'LOGGING_APPS': {
+            'drivers': {
+                'models': {
+                    'Driver': {
+                        'fields': ['driver_name'],
+                        'callbacks': [
+                            'yourapp.callbacks.set_extra_data_for_driver_name'
+                        ]
+                    },
+                },
+            },
+        },
+    }
 
 .. note::
 
     You can also add lambda functions to your callbacks
 
 The model structure
 ~~~~~~~~~~~~~~~~~~~
 
 This package provides you a django model which is called ``FieldLog``;
 which tracks each change to a model instance specified in your
 configuration mapping. An example record is as follows:
 
 ::
 
-   {
-    'id': 2,
-    'app_label': 'drivers',
-    'model': 'driver',
-    'instance_id': 1,
-    'field': 'latest_speed',
-    'timestamp': datetime.datetime(2024, 1, 16, 9, 1, 14, 619568, tzinfo=<UTC>),
-    'old_value': 'John Doe',
-    'new_value': 'Jane Doe',
-    'extra_data': {}, # this is a JSONField, you can store any extra data here using callbacks or by overriding it directly
-    'created': False, # this is a boolean field, if it is True, it means that instance is a newly created instance
-   }
+    {
+        'id': 2,
+        'app_label': 'drivers',
+        'model': 'driver',
+        'instance_id': 1,
+        'field': 'latest_speed',
+        'timestamp': datetime.datetime(2024, 1, 16, 9, 1, 14, 619568, tzinfo=<UTC>),
+        'old_value': 'John Doe',
+        'new_value': 'Jane Doe',
+        'extra_data': {}, # this is a JSONField, you can store any extra data here using callbacks or by overriding it directly
+        'created': False, # this is a boolean field, if it is True, it means that instance is a newly created instance
+    }
 
 Additionally, ``FieldLog`` model provides the following properties:
 
 -  ``model_class``: returns the model class of the instance that is
    being logged.
 -  ``instance``: returns the instance that is being logged.
 -  ``previous_log``: returns the previous log of the instance that is
@@ -225,16 +238,16 @@
 
 -  ``fieldlog_set`` since the ``FieldLog`` model has not a direct
    relation to the model that is being logged, you can use this property
    to get the logs of the instance that is being logged.
 
    .. code:: python
 
-       driver = Driver.objects.last()
-       logs = driver.fieldlog_set.all()
+        driver = Driver.objects.last()
+        logs = driver.fieldlog_set.all()
 
 MIT License
 
 Copyright (c) 2024 Sergio Rodríguez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `django-field-logger-0.0.24/django_field_logger.egg-info/SOURCES.txt` & `django-field-logger-0.0.25/django_field_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/fieldlogger/config.py` & `django-field-logger-0.0.25/fieldlogger/config.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/fieldlogger/fieldlogger.py` & `django-field-logger-0.0.25/fieldlogger/fieldlogger.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/fieldlogger/models.py` & `django-field-logger-0.0.25/fieldlogger/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         instance.instance_id = int(iid) if iid.isdigit() else iid
         instance.old_value = (
             cls.from_db_field(field_class, instance.old_value)
             if not instance.created
             else None
         )
         instance.new_value = cls.from_db_field(field_class, instance.new_value)
+
         return instance
 
     @property
     def model_class(self):
         return apps.get_model(self.app_label, self.model)
 
     @property
```

### Comparing `django-field-logger-0.0.24/fieldlogger/signals.py` & `django-field-logger-0.0.25/fieldlogger/signals.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/tests/settings.py` & `django-field-logger-0.0.25/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/tests/test_utils.py` & `django-field-logger-0.0.25/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-field-logger-0.0.24/tests/tests.py` & `django-field-logger-0.0.25/tests/tests.py`

 * *Files identical despite different names*

