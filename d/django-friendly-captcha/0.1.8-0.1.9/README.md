# Comparing `tmp/django-friendly-captcha-0.1.8.tar.gz` & `tmp/django-friendly-captcha-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-friendly-captcha-0.1.8.tar", last modified: Tue Aug  1 18:16:37 2023, max compression
+gzip compressed data, was "django-friendly-captcha-0.1.9.tar", last modified: Tue Feb 27 13:35:27 2024, max compression
```

## Comparing `django-friendly-captcha-0.1.8.tar` & `django-friendly-captcha-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:16:36.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 18:16:37.000000 django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.031075 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/friendly_captcha/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:16:37.035075 django-friendly-captcha-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-01 18:16:26.000000 django-friendly-captcha-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-27 13:35:27.000000 django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/friendly_captcha/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.632526 django-friendly-captcha-0.1.9/friendly_captcha/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.632526 django-friendly-captcha-0.1.9/friendly_captcha/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/friendly_captcha/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.632526 django-friendly-captcha-0.1.9/friendly_captcha/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/friendly_captcha/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/friendly_captcha/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 13:35:27.636526 django-friendly-captcha-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-27 13:35:20.000000 django-friendly-captcha-0.1.9/setup.py
```

### Comparing `django-friendly-captcha-0.1.8/LICENSE` & `django-friendly-captcha-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.8/PKG-INFO` & `django-friendly-captcha-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-friendly-captcha
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django library for friendly captcha
 Home-page: https://github.com/christianwgd/django-friendly-captcha
 Download-URL: 
 Author: Christian Wiegand
 Author-email: christianwgd@gmail.com
 Maintainer: Christian Wiegand
 Maintainer-email: christianwgd@gmail.com
@@ -13,21 +13,21 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: django
+Requires-Dist: requests
 
 Django Friendly Captcha
 =======================
 
 .. image:: https://img.shields.io/pypi/v/django-friendly-captcha
     :target: https://pypi.python.org/pypi/django-friendly-captcha
 
@@ -80,15 +80,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
+Version 0.1.9 includes friendly captcha version 0.9.14 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.8/README.rst` & `django-friendly-captcha-0.1.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
+Version 0.1.9 includes friendly captcha version 0.9.14 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/PKG-INFO` & `django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-friendly-captcha
-Version: 0.1.8
+Version: 0.1.9
 Summary: Django library for friendly captcha
 Home-page: https://github.com/christianwgd/django-friendly-captcha
 Download-URL: 
 Author: Christian Wiegand
 Author-email: christianwgd@gmail.com
 Maintainer: Christian Wiegand
 Maintainer-email: christianwgd@gmail.com
@@ -13,21 +13,21 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: django
+Requires-Dist: requests
 
 Django Friendly Captcha
 =======================
 
 .. image:: https://img.shields.io/pypi/v/django-friendly-captcha
     :target: https://pypi.python.org/pypi/django-friendly-captcha
 
@@ -80,15 +80,15 @@
                 'name', 'email', 'subject', 'text'
             )
 
         captcha = FrcCaptchaField()
 
 As of version 0.1.7 the javascript static assets are included in
 the widget, so there is no need to do that in your project templates.
-Version 0.1.8 includes friendly captcha version 0.9.12 javascript files.
+Version 0.1.9 includes friendly captcha version 0.9.14 javascript files.
 If you need a different version you can set these by providing
 them in your settings:
 
 .. code-block::
 
     FRC_WIDGET_MODULE_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.module.min.js'
     FRC_WIDGET_JS = 'https://unpkg.com/friendly-challenge@0.9.8/widget.min.js'
```

### Comparing `django-friendly-captcha-0.1.8/django_friendly_captcha.egg-info/SOURCES.txt` & `django-friendly-captcha-0.1.9/django_friendly_captcha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.8/friendly_captcha/fields.py` & `django-friendly-captcha-0.1.9/friendly_captcha/fields.py`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.8/friendly_captcha/locale/de/LC_MESSAGES/django.po` & `django-friendly-captcha-0.1.9/friendly_captcha/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.8/friendly_captcha/locale/en/LC_MESSAGES/django.po` & `django-friendly-captcha-0.1.9/friendly_captcha/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-friendly-captcha-0.1.8/friendly_captcha/widgets.py` & `django-friendly-captcha-0.1.9/friendly_captcha/widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 class FrcCaptchaWidget(Widget):
 
     def __init__(self):
         super().__init__()
         self.site_key = getattr(settings, 'FRC_CAPTCHA_SITE_KEY', None)
         self.frc_widget_module_js = getattr(
             settings, 'FRC_WIDGET_MODULE_JS',
-            'https://unpkg.com/friendly-challenge@0.9.12/widget.module.min.js',
+            'https://unpkg.com/friendly-challenge@0.9.14/widget.module.min.js',
         )
         self.frc_widget_js = getattr(
             settings, 'FRC_WIDGET_JS',
-            'https://unpkg.com/friendly-challenge@0.9.12/widget.min.js'
+            'https://unpkg.com/friendly-challenge@0.9.14/widget.min.js'
         )
 
     def render(self, name, value, attrs=None, renderer=None):
         attrs['data-lang'] = translation.get_language()
         attrs['data-sitekey'] = self.site_key
         attrs['data-solution-field-name'] = name
         attrs['class'] = 'frc-captcha'
```

### Comparing `django-friendly-captcha-0.1.8/setup.py` & `django-friendly-captcha-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='django-friendly-captcha',
-    version='0.1.8',
+    version='0.1.9',
     description='Django library for friendly captcha',
     long_description=read('README.rst'),
     url='https://github.com/christianwgd/django-friendly-captcha',
     download_url='',
     author='Christian Wiegand',
     author_email='christianwgd@gmail.com',
     maintainer='Christian Wiegand',
@@ -29,15 +29,13 @@
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     zip_safe=False,
 )
```

