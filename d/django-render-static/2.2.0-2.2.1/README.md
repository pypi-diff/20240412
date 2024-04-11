# Comparing `tmp/django_render_static-2.2.0.tar.gz` & `tmp/django_render_static-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_render_static-2.2.0.tar", max compression
+gzip compressed data, was "django_render_static-2.2.1.tar", max compression
```

## Comparing `django_render_static-2.2.0.tar` & `django_render_static-2.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1073 2023-11-08 22:34:36.090325 django_render_static-2.2.0/LICENSE
--rw-r--r--   0        0        0    11929 2023-12-22 06:58:18.231241 django_render_static-2.2.0/README.rst
--rw-r--r--   0        0        0     4430 2024-02-28 01:52:06.712880 django_render_static-2.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1302 2024-02-28 01:52:06.713131 django_render_static-2.2.0/render_static/__init__.py
--rwxr-xr-x   0        0        0      152 2023-12-22 06:59:26.300794 django_render_static-2.2.0/render_static/apps.py
--rwxr-xr-x   0        0        0    10616 2024-02-28 01:52:06.713508 django_render_static-2.2.0/render_static/backends.py
--rw-r--r--   0        0        0     6485 2024-02-28 01:52:06.713829 django_render_static-2.2.0/render_static/context.py
--rw-r--r--   0        0        0    27809 2024-02-28 01:52:06.714083 django_render_static-2.2.0/render_static/engine.py
--rw-r--r--   0        0        0      637 2023-12-22 06:59:26.310866 django_render_static-2.2.0/render_static/exceptions.py
--rw-r--r--   0        0        0      403 2024-02-28 00:29:16.706609 django_render_static-2.2.0/render_static/loaders/__init__.py
--rw-r--r--   0        0        0     8006 2024-02-28 01:52:06.714593 django_render_static-2.2.0/render_static/loaders/django.py
--rw-r--r--   0        0        0     5462 2024-02-28 01:52:06.714959 django_render_static-2.2.0/render_static/loaders/jinja2.py
--rw-r--r--   0        0        0     1519 2024-02-27 20:27:03.802654 django_render_static-2.2.0/render_static/loaders/mixins.py
--rw-r--r--   0        0        0      781 2024-02-28 01:52:06.715276 django_render_static-2.2.0/render_static/loaders/utils.py
--rwxr-xr-x   0        0        0        0 2023-11-08 22:34:36.093265 django_render_static-2.2.0/render_static/management/__init__.py
--rwxr-xr-x   0        0        0        0 2023-11-08 22:34:36.093343 django_render_static-2.2.0/render_static/management/commands/__init__.py
--rwxr-xr-x   0        0        0     6782 2024-02-28 01:52:06.715666 django_render_static-2.2.0/render_static/management/commands/renderstatic.py
--rw-r--r--   0        0        0     1089 2023-12-22 06:59:26.318042 django_render_static-2.2.0/render_static/origin.py
--rw-r--r--   0        0        0     7424 2023-12-22 07:03:28.814145 django_render_static-2.2.0/render_static/placeholders.py
--rw-r--r--   0        0        0     2805 2024-01-24 05:28:02.082521 django_render_static-2.2.0/render_static/resource.py
--rw-r--r--   0        0        0      180 2023-11-08 22:34:36.093892 django_render_static-2.2.0/render_static/static_templates/render_static/defines.js
--rw-r--r--   0        0        0      164 2023-11-08 22:34:36.093963 django_render_static-2.2.0/render_static/static_templates/render_static/enums.js
--rw-r--r--   0        0        0      265 2023-11-08 22:34:36.094044 django_render_static-2.2.0/render_static/static_templates/render_static/urls.js
--rwxr-xr-x   0        0        0        0 2023-11-08 22:34:36.094122 django_render_static-2.2.0/render_static/templatetags/__init__.py
--rwxr-xr-x   0        0        0    17265 2024-02-28 01:52:06.716088 django_render_static-2.2.0/render_static/templatetags/render_static.py
--rw-r--r--   0        0        0    19673 2024-02-28 01:52:06.720916 django_render_static-2.2.0/render_static/transpilers/__init__.py
--rw-r--r--   0        0        0     8216 2023-12-22 07:28:37.406597 django_render_static-2.2.0/render_static/transpilers/defines_to_js.py
--rw-r--r--   0        0        0    25311 2024-02-28 01:52:06.721256 django_render_static-2.2.0/render_static/transpilers/enums_to_js.py
--rw-r--r--   0        0        0    56297 2024-02-28 01:52:06.721498 django_render_static-2.2.0/render_static/transpilers/urls_to_js.py
--rw-r--r--   0        0        0    13951 1970-01-01 00:00:00.000000 django_render_static-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 17:34:27.093376 django_render_static-2.2.1/LICENSE
+-rw-r--r--   0        0        0    10809 2024-04-11 23:03:58.311389 django_render_static-2.2.1/README.md
+-rw-r--r--   0        0        0     4459 2024-04-11 23:03:58.311872 django_render_static-2.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1302 2024-04-11 23:03:58.312911 django_render_static-2.2.1/render_static/__init__.py
+-rwxr-xr-x   0        0        0      152 2024-04-11 17:34:27.099462 django_render_static-2.2.1/render_static/apps.py
+-rwxr-xr-x   0        0        0    10616 2024-04-11 17:34:27.099938 django_render_static-2.2.1/render_static/backends.py
+-rw-r--r--   0        0        0     6485 2024-04-11 17:34:27.100602 django_render_static-2.2.1/render_static/context.py
+-rw-r--r--   0        0        0    27809 2024-04-11 17:34:27.100855 django_render_static-2.2.1/render_static/engine.py
+-rw-r--r--   0        0        0      637 2024-04-11 17:34:27.101081 django_render_static-2.2.1/render_static/exceptions.py
+-rw-r--r--   0        0        0      403 2024-04-11 17:34:27.101345 django_render_static-2.2.1/render_static/loaders/__init__.py
+-rw-r--r--   0        0        0     8006 2024-04-11 17:34:27.101982 django_render_static-2.2.1/render_static/loaders/django.py
+-rw-r--r--   0        0        0     5462 2024-04-11 17:34:27.102562 django_render_static-2.2.1/render_static/loaders/jinja2.py
+-rw-r--r--   0        0        0     1519 2024-04-11 17:34:27.102730 django_render_static-2.2.1/render_static/loaders/mixins.py
+-rw-r--r--   0        0        0      781 2024-04-11 17:34:27.102894 django_render_static-2.2.1/render_static/loaders/utils.py
+-rwxr-xr-x   0        0        0        0 2024-04-11 17:34:27.103044 django_render_static-2.2.1/render_static/management/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-04-11 17:34:27.103212 django_render_static-2.2.1/render_static/management/commands/__init__.py
+-rwxr-xr-x   0        0        0     6782 2024-04-11 17:34:27.103855 django_render_static-2.2.1/render_static/management/commands/renderstatic.py
+-rw-r--r--   0        0        0     1089 2024-04-11 17:34:27.104018 django_render_static-2.2.1/render_static/origin.py
+-rw-r--r--   0        0        0     7424 2024-04-11 17:34:27.104609 django_render_static-2.2.1/render_static/placeholders.py
+-rw-r--r--   0        0        0     2805 2024-04-11 17:34:27.104780 django_render_static-2.2.1/render_static/resource.py
+-rw-r--r--   0        0        0      180 2024-04-11 17:34:27.105109 django_render_static-2.2.1/render_static/static_templates/render_static/defines.js
+-rw-r--r--   0        0        0      164 2024-04-11 17:34:27.105236 django_render_static-2.2.1/render_static/static_templates/render_static/enums.js
+-rw-r--r--   0        0        0      265 2024-04-11 17:34:27.105373 django_render_static-2.2.1/render_static/static_templates/render_static/urls.js
+-rwxr-xr-x   0        0        0        0 2024-04-11 17:34:27.105516 django_render_static-2.2.1/render_static/templatetags/__init__.py
+-rwxr-xr-x   0        0        0    17265 2024-04-11 17:34:27.105759 django_render_static-2.2.1/render_static/templatetags/render_static.py
+-rw-r--r--   0        0        0    19673 2024-04-11 17:34:27.128093 django_render_static-2.2.1/render_static/transpilers/__init__.py
+-rw-r--r--   0        0        0     8216 2024-04-11 17:34:27.128402 django_render_static-2.2.1/render_static/transpilers/defines_to_js.py
+-rw-r--r--   0        0        0    25311 2024-04-11 17:34:27.128594 django_render_static-2.2.1/render_static/transpilers/enums_to_js.py
+-rw-r--r--   0        0        0    56068 2024-04-11 23:03:58.313159 django_render_static-2.2.1/render_static/transpilers/urls_to_js.py
+-rw-r--r--   0        0        0    12834 1970-01-01 00:00:00.000000 django_render_static-2.2.1/PKG-INFO
```

### Comparing `django_render_static-2.2.0/LICENSE` & `django_render_static-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/README.rst` & `django_render_static-2.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,91 @@
-|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPi djversions| |PyPI status| |Documentation Status|
-|Code Cov| |Test Status| |Code Style|
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static/)
+[![PyPI djversions](https://img.shields.io/pypi/djversions/django-render-static.svg)](https://pypi.org/project/django-render-static/)
+[![PyPI status](https://img.shields.io/pypi/status/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static)
+[![Documentation Status](https://readthedocs.org/projects/django-render-static/badge/?version=latest)](http://django-render-static.readthedocs.io/?badge=latest/)
+[![Code Cov](https://codecov.io/gh/bckohan/django-render-static/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-render-static)
+[![Test Status](https://github.com/bckohan/django-render-static/workflows/test/badge.svg)](https://github.com/bckohan/django-render-static/actions/workflows/test.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-   :target: https://lbesson.mit-license.org/
-
-.. |PyPI version fury.io| image:: https://badge.fury.io/py/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static/
-
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static/
-
-.. |PyPI djversions| image:: https://img.shields.io/pypi/djversions/django-render-static.svg
-   :target: https://pypi.org/project/django-render-static/
-
-.. |PyPI status| image:: https://img.shields.io/pypi/status/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static
-
-.. |Documentation Status| image:: https://readthedocs.org/projects/django-render-static/badge/?version=latest
-   :target: http://django-render-static.readthedocs.io/?badge=latest/
-
-.. |Code Cov| image:: https://codecov.io/gh/bckohan/django-render-static/branch/main/graph/badge.svg?token=0IZOKN2DYL
-   :target: https://codecov.io/gh/bckohan/django-render-static
-
-.. |Test Status| image:: https://github.com/bckohan/django-render-static/workflows/test/badge.svg
-   :target: https://github.com/bckohan/django-render-static/actions
-
-.. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-
-django-render-static
-#######################
+# django-render-static
 
 Use Django's template engines to render static files that are collected
 during the ``collectstatic`` routine and likely served above Django at runtime.
 Files rendered by django-render-static are immediately available to participate
 in the normal static file collection pipeline.
 
-For example, a frequently occurring pattern that violates the `DRY principle <https://en.wikipedia.org/wiki/Don%27t_repeat_yourself>`_
-is the presence of defines, or enum like structures in server side Python code that are simply replicated in client
-side JavaScript. Another example might be rebuilding Django URLs from arguments in a `Single Page Application <https://en.wikipedia.org/wiki/Single-page_application>`_.
-Single-sourcing these structures by transpiling client side code from the server side code keeps the stack bone DRY.
-
-`django-render-static` includes Python to Javascript transpilers for:
-    - Django's `reverse` function (`urls_to_js`)
-    - PEP 435 style Python enumerations (`enums_to_js`)
-    - Plain data define-like structures in Python classes and modules
-      (`defines_to_js`)
+For example, a frequently occurring pattern that violates the
+[DRY principle](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) is the presence of defines,
+or enum like structures in server side Python code that are simply replicated in client side
+JavaScript. Another example might be rebuilding Django URLs from arguments in a
+[Single Page Application](https://en.wikipedia.org/wiki/Single-page_application). Single-sourcing
+these structures by transpiling client side code from the server side code keeps the stack bone DRY.
+
+**`django-render-static` includes Python to Javascript transpilers for:**
+
+* Django's `reverse` function (`urls_to_js`)
+* PEP 435 style Python enumerations (`enums_to_js`)
+* Plain data define-like structures in Python classes and modules
+    (`defines_to_js`)
 
 Transpilation is extremely flexible and may be customized by using override blocks or extending the provided 
 transpilers.
 
 `django-render-static` also formalizes the concept of a package-time or deployment-time
 static file rendering step. It piggybacks off the existing templating engines and configurations
 and should therefore be familiar to Django developers. It supports both standard Django templating
 and Jinja templates and allows contexts to be specified in python, json or YAML.
 
 You can report bugs and discuss features on the
-`issues page <https://github.com/bckohan/django-render-static/issues>`_.
+[issues page](https://github.com/bckohan/django-render-static/issues).
 
-`Contributions <https://github.com/bckohan/django-render-static/blob/main/CONTRIBUTING.rst>`_ are
+[Contributions](https://github.com/bckohan/django-render-static/blob/main/CONTRIBUTING.rst) are
 encouraged!
 
-`Full documentation at read the docs. <https://django-render-static.readthedocs.io/en/latest/>`_
-
-Installation
-------------
-
-1. Clone django-render-static from GitHub_ or install a release off PyPI_ :
+[Full documentation at read the docs.](https://django-render-static.readthedocs.io/en/latest/)
 
-.. code:: bash
+## Installation
 
-       pip install django-render-static
+1. Clone django-render-static from [GitHub](http://github.com/bckohan/django-render-static) or install a release off [PyPI](http://pypi.python.org/pypi/django-render-static):
 
+```shell
+pip install django-render-static
+```
 
 2. Add 'render_static' to your ``INSTALLED_APPS`` :
 
-.. code:: python
-
-       INSTALLED_APPS = [
-           'render_static',
-       ]
-
+```python
+INSTALLED_APPS = [
+    'render_static',
+]
+```
 
 3. Add a ``STATIC_TEMPLATES`` configuration directive to your settings file:
 
-.. code:: python
-
-        STATIC_TEMPLATES = {
-            'templates' : [
-                ('path/to/template':, {'context' {'variable': 'value'})
-            ]
-        }
+```python
 
+STATIC_TEMPLATES = {
+    'templates' : [
+        ('path/to/template':, {'context' {'variable': 'value'})
+    ]
+}
+```
 
 4. Run ``renderstatic`` preceding every run of ``collectstatic`` :
 
-.. code:: bash
-
-        $> manage.py renderstatic
-        $> manage.py collectstatic
-
+```shell
+$> manage.py renderstatic
+$> manage.py collectstatic
+```
 
-.. _GitHub: http://github.com/bckohan/django-render-static
-.. _PyPI: http://pypi.python.org/pypi/django-render-static
-.. _django-enum: http://pypi.python.org/pypi/django-enum
-.. _enum-properties: http://pypi.python.org/pypi/enum-properties
+## Usage
 
-
-Usage
------
-
-Transpiling Model Field Choices
--------------------------------
+### Transpiling Model Field Choices
 
 You have an app with a model with a character field that has several valid choices defined in an
 enumeration type way, and you'd like to export those defines to JavaScript. You'd like to include
 a template for other's using your app to use to generate a defines.js file. Say your app structure
 looks like this::
 
     .
@@ -129,265 +98,257 @@
         │   └── examples
         │       └── defines.js
         └── urls.py
 
 
 Your defines/model classes might look like this:
 
-.. code:: python
-
-    class ExampleModel(Defines, models.Model):
+```python
+class ExampleModel(Defines, models.Model):
 
-        DEFINE1 = 'D1'
-        DEFINE2 = 'D2'
-        DEFINE3 = 'D3'
-        DEFINES = (
-            (DEFINE1, 'Define 1'),
-            (DEFINE2, 'Define 2'),
-            (DEFINE3, 'Define 3')
-        )
-
-        define_field = models.CharField(choices=DEFINES, max_length=2)
+    DEFINE1 = 'D1'
+    DEFINE2 = 'D2'
+    DEFINE3 = 'D3'
+    DEFINES = (
+        (DEFINE1, 'Define 1'),
+        (DEFINE2, 'Define 2'),
+        (DEFINE3, 'Define 3')
+    )
 
+    define_field = models.CharField(choices=DEFINES, max_length=2)
+```
 
 And your defines.js template might look like this:
 
-.. code:: js+django
-
-    {% defines_to_js modules="examples.models" %}
-
+```js+django
+{% defines_to_js modules="examples.models" %}
+```
 
 If someone wanted to use your defines template to generate a JavaScript version of your Python
 class their settings file might look like this:
 
-.. code:: python
-
-    STATIC_TEMPLATES = {
-        'templates': [
-            'examples/defines.js'
-        ]
-    }
+```python
+STATIC_TEMPLATES = {
+    'templates': [
+        'examples/defines.js'
+    ]
+}
+```
 
 
 And then of course they would call `renderstatic` before `collectstatic`:
 
-.. code:: bash
-
-    $> ./manage.py renderstatic
-    $> ./manage.py collectstatic
-
+```shell
+$> ./manage.py renderstatic
+$> ./manage.py collectstatic
+```
 
 This would create the following file::
 
     .
     └── examples
         └── static
             └── examples
                 └── defines.js
 
 Which would look like this:
 
-.. code:: javascript
-
-    const defines = {
-        ExampleModel: {
-            DEFINE1: "D1",
-            DEFINE2: "D2",
-            DEFINE3: "D3",
-            DEFINES: [["D1", "Define 1"], ["D2", "Define 2"], ["D3", "Define 3"]]
-        }
-    };
-
-
-Transpiling Enumerations
-------------------------
+```javascript
+const defines = {
+    ExampleModel: {
+        DEFINE1: "D1",
+        DEFINE2: "D2",
+        DEFINE3: "D3",
+        DEFINES: [["D1", "Define 1"], ["D2", "Define 2"], ["D3", "Define 3"]]
+    }
+};
+```
 
-Say instead of the usual choices tuple you're using PEP 435 style python
-enumerations as model fields using django-enum_ and enum-properties_. For example
-we might define a simple color enumeration like so:
+### Transpiling Enumerations
 
-.. code:: python
+Say instead of the usual choices tuple you're using PEP 435 style python enumerations as model
+fields using [django-enum](http://pypi.python.org/pypi/django-enum) and
+[enum-properties](http://pypi.python.org/pypi/enum-properties). For example we might define a
+simple color enumeration like so:
 
-    from django.db import models
-    from django_enum import EnumField, TextChoices
-    from enum_properties import p, s
+```python
+from django.db import models
+from django_enum import EnumField, TextChoices
+from enum_properties import p, s
 
-    class ExampleModel(models.Model):
+class ExampleModel(models.Model):
 
-        class Color(TextChoices, s('rgb'), s('hex', case_fold=True)):
+    class Color(TextChoices, s('rgb'), s('hex', case_fold=True)):
 
-            # name   value   label       rgb       hex
-            RED   =   'R',   'Red',   (1, 0, 0), 'ff0000'
-            GREEN =   'G',   'Green', (0, 1, 0), '00ff00'
-            BLUE  =   'B',   'Blue',  (0, 0, 1), '0000ff'
+        # name   value   label       rgb       hex
+        RED   =   'R',   'Red',   (1, 0, 0), 'ff0000'
+        GREEN =   'G',   'Green', (0, 1, 0), '00ff00'
+        BLUE  =   'B',   'Blue',  (0, 0, 1), '0000ff'
 
-        color = EnumField(Color, null=True, default=None)
+    color = EnumField(Color, null=True, default=None)
+```
 
 If we define an enum.js template that looks like this:
 
-.. code:: js+django
+```js+django
 
     {% enums_to_js enums="examples.models.ExampleModel.Color" %}
+```
 
 It will contain a javascript class transpilation of the Color enum that looks
 like this:
 
-.. code:: javascript
+```javascript
 
-    class Color {
+class Color {
 
-        static RED = new Color("R", "RED", "Red", [1, 0, 0], "ff0000");
-        static GREEN = new Color("G", "GREEN", "Green", [0, 1, 0], "00ff00");
-        static BLUE = new Color("B", "BLUE", "Blue", [0, 0, 1], "0000ff");
-
-        constructor (value, name, label, rgb, hex) {
-            this.value = value;
-            this.name = name;
-            this.label = label;
-            this.rgb = rgb;
-            this.hex = hex;
-        }
+    static RED = new Color("R", "RED", "Red", [1, 0, 0], "ff0000");
+    static GREEN = new Color("G", "GREEN", "Green", [0, 1, 0], "00ff00");
+    static BLUE = new Color("B", "BLUE", "Blue", [0, 0, 1], "0000ff");
+
+    constructor (value, name, label, rgb, hex) {
+        this.value = value;
+        this.name = name;
+        this.label = label;
+        this.rgb = rgb;
+        this.hex = hex;
+    }
 
-        toString() {
-            return this.value;
-        }
+    toString() {
+        return this.value;
+    }
 
-        static get(value) {
-            switch(value) {
-                case "R":
-                    return Color.RED;
-                case "G":
-                    return Color.GREEN;
-                case "B":
-                    return Color.BLUE;
-            }
-            throw new TypeError(`No Color enumeration maps to value ${value}`);
+    static get(value) {
+        switch(value) {
+            case "R":
+                return Color.RED;
+            case "G":
+                return Color.GREEN;
+            case "B":
+                return Color.BLUE;
         }
+        throw new TypeError(`No Color enumeration maps to value ${value}`);
+    }
 
-        static [Symbol.iterator]() {
-            return [Color.RED, Color.GREEN, Color.BLUE][Symbol.iterator]();
-        }
+    static [Symbol.iterator]() {
+        return [Color.RED, Color.GREEN, Color.BLUE][Symbol.iterator]();
     }
+}
+```
 
 We can now use our enumeration like so:
 
-.. code:: javascript
-
-    Color.BLUE === Color.get('B');
-    for (const color of Color) {
-        console.log(color);
-    }
-
+```javascript
+Color.BLUE === Color.get('B');
+for (const color of Color) {
+    console.log(color);
+}
+```
 
-Transpiling URL reversal
-------------------------
+### Transpiling URL reversal
 
 You'd like to be able to call something like `reverse` on path names from your client JavaScript
 code the same way you do from Python Django code.
 
 Your settings file might look like:
 
-.. code:: python
-
+```python
     STATIC_TEMPLATES={
         'ENGINES': [{
             'BACKEND': 'render_static.backends.StaticDjangoTemplates',
             'OPTIONS': {
                 'loaders': [
                     ('render_static.loaders.StaticLocMemLoader', {
                         'urls.js': '{% urls_to_js %}'
                     })
                 ]
             },
         }],
         'templates': ['urls.js']
     }
+```
 
+Then call `renderstatic` before `collectstatic`:
 
-Then call `renderstatic` before `collectstatic`::
-
-    $> ./manage.py renderstatic
-    $> ./manage.py collectstatic
+```shell
+$> ./manage.py renderstatic
+$> ./manage.py collectstatic
+```
 
 If your root urls.py looks like this:
 
-.. code:: python
-
-    from django.contrib import admin
-    from django.urls import path
-
-    from .views import MyView
-
-    urlpatterns = [
-        path('admin/', admin.site.urls),
-        path('simple', MyView.as_view(), name='simple'),
-        path('simple/<int:arg1>', MyView.as_view(), name='simple'),
-        path('different/<int:arg1>/<str:arg2>', MyView.as_view(), name='different'),
-    ]
-
+```python
+from django.contrib import admin
+from django.urls import path
+
+from .views import MyView
+
+urlpatterns = [
+    path('admin/', admin.site.urls),
+    path('simple', MyView.as_view(), name='simple'),
+    path('simple/<int:arg1>', MyView.as_view(), name='simple'),
+    path('different/<int:arg1>/<str:arg2>', MyView.as_view(), name='different'),
+]
+```
 
 So you can now fetch paths like this, in a way that is roughly API-equivalent
 to Django's `reverse` function:
 
-.. code:: javascript
-
-    import { URLResolver } from '/static/urls.js';
+```javascript
+import { URLResolver } from '/static/urls.js';
 
-    const urls = new URLResolver();
+const urls = new URLResolver();
 
-    // /different/143/emma
-    urls.reverse('different', {kwargs: {'arg1': 143, 'arg2': 'emma'}});
+// /different/143/emma
+urls.reverse('different', {kwargs: {'arg1': 143, 'arg2': 'emma'}});
 
-    // reverse also supports query parameters
-    // /different/143/emma?intarg=0&listarg=A&listarg=B&listarg=C
-    urls.reverse(
-        'different',
-        {
-            kwargs: {arg1: 143, arg2: 'emma'},
-            query: {
-                intarg: 0,
-                listarg: ['A', 'B', 'C']
-            }
+// reverse also supports query parameters
+// /different/143/emma?intarg=0&listarg=A&listarg=B&listarg=C
+urls.reverse(
+    'different',
+    {
+        kwargs: {arg1: 143, arg2: 'emma'},
+        query: {
+            intarg: 0,
+            listarg: ['A', 'B', 'C']
         }
-    );
-    
+    }
+);
+```
 
-URLGenerationFailed Exceptions & Placeholders
----------------------------------------------
+### URLGenerationFailed Exceptions & Placeholders
 
 If you encounter a ``URLGenerationFailed`` exception you most likely need to register a placeholder for the argument in question. A placeholder is just a string or object that can be coerced to a string that matches the regular expression for the argument:
 
-.. code:: python
-
-   from render_static.placeholders import register_variable_placeholder
+```python
+from render_static.placeholders import register_variable_placeholder
 
-   app_name = 'year_app'
-   urlpatterns = [
-       re_path(r'^fetch/(?P<year>\d{4})/$', YearView.as_view(), name='fetch_year')
-   ]
+app_name = 'year_app'
+urlpatterns = [
+    re_path(r'^fetch/(?P<year>\d{4})/$', YearView.as_view(), name='fetch_year')
+]
 
-   register_variable_placeholder('year', 2000, app_name=app_name)
+register_variable_placeholder('year', 2000, app_name=app_name)
+```
 
 Users should typically use a path instead of re_path and register their own custom converters when needed. Placeholders can be directly registered on the converter (and are then conveniently available to users of your app!):
 
-.. code:: python
-
-   from django.urls.converters import register_converter
-
-   class YearConverter:
-       regex = '[0-9]{4}'
-       placeholder = 2000  # this attribute is used by `url_to_js` to reverse paths
-
-       def to_python(self, value):
-           return int(value)
+```python
+from django.urls.converters import register_converter
 
-       def to_url(self, value):
-           return str(value)
+class YearConverter:
+    regex = '[0-9]{4}'
+    placeholder = 2000  # this attribute is used by `url_to_js` to reverse paths
 
+    def to_python(self, value):
+        return int(value)
 
-   register_converter(YearConverter, 'year')
+    def to_url(self, value):
+        return str(value)
 
-   urlpatterns = [
-       path('fetch/<year:year>', YearView.as_view(), name='fetch_year')
-   ]
 
+register_converter(YearConverter, 'year')
 
+urlpatterns = [
+    path('fetch/<year:year>', YearView.as_view(), name='fetch_year')
+]
+```
```

### Comparing `django_render_static-2.2.0/pyproject.toml` & `django_render_static-2.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "django-render-static"
-version = "2.2.0"
+version = "2.2.1"
 description = "Use Django's template engine to render static files at deployment or package time. Includes transpilers for extending Django's url reversal and enums to JavaScript."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/bckohan/django-render-static"
 homepage = "https://django-render-static.readthedocs.io"
 keywords = ["django", "static", "templates", "javascript", "url", "reverse", "defines", "transpiler", "transpile", "enum"]
 classifiers = [
     "Environment :: Console",
     "Framework :: Django",
     "Operating System :: OS Independent",
@@ -64,15 +64,15 @@
 mypy = "^1.8"
 isort = "^5.13.0"
 doc8 = "^1.1.0"
 pytest-cov = "^4.1.0"
 pylint = "^3.0.0"
 deepdiff = "^6.7.0"
 safety = "^2.3.0"
-readme-renderer = ">=42"
+readme-renderer = {extras = ["md"], version = "^43.0"}
 types-PyYAML = "^6.0"
 coverage = "^7.3.0"
 importlib-metadata = "^7.0.0"
 selenium = "^4.16.0"
 python-dateutil = "^2.8.2"
 ipdb = "^0.13.13"
 black = "^23.12.0"
```

### Comparing `django_render_static-2.2.0/render_static/__init__.py` & `django_render_static-2.2.1/render_static/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from .context import resolve_context
 from .resource import resource
 from .transpilers.defines_to_js import DefaultDefineTranspiler
 from .transpilers.enums_to_js import EnumClassWriter
 from .transpilers.urls_to_js import ClassURLWriter, SimpleURLWriter
 
-VERSION = (2, 2, 0)
+VERSION = (2, 2, 1)
 
 __title__ = "Django Render Static"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2020-2024 Brian Kohan"
```

### Comparing `django_render_static-2.2.0/render_static/backends.py` & `django_render_static-2.2.1/render_static/backends.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/context.py` & `django_render_static-2.2.1/render_static/context.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/engine.py` & `django_render_static-2.2.1/render_static/engine.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/exceptions.py` & `django_render_static-2.2.1/render_static/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/loaders/django.py` & `django_render_static-2.2.1/render_static/loaders/django.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/loaders/jinja2.py` & `django_render_static-2.2.1/render_static/loaders/jinja2.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/loaders/mixins.py` & `django_render_static-2.2.1/render_static/loaders/mixins.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/loaders/utils.py` & `django_render_static-2.2.1/render_static/loaders/utils.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/management/commands/renderstatic.py` & `django_render_static-2.2.1/render_static/management/commands/renderstatic.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/origin.py` & `django_render_static-2.2.1/render_static/origin.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/placeholders.py` & `django_render_static-2.2.1/render_static/placeholders.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/resource.py` & `django_render_static-2.2.1/render_static/resource.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/templatetags/render_static.py` & `django_render_static-2.2.1/render_static/templatetags/render_static.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/transpilers/__init__.py` & `django_render_static-2.2.1/render_static/transpilers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/transpilers/defines_to_js.py` & `django_render_static-2.2.1/render_static/transpilers/defines_to_js.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/transpilers/enums_to_js.py` & `django_render_static-2.2.1/render_static/transpilers/enums_to_js.py`

 * *Files identical despite different names*

### Comparing `django_render_static-2.2.0/render_static/transpilers/urls_to_js.py` & `django_render_static-2.2.1/render_static/transpilers/urls_to_js.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,76 +486,74 @@
                 try:
                     if unnamed:
                         placeholder_url = reverse(qname, args=placeholders)
                     else:
                         placeholder_url = reverse(
                             qname, kwargs={**kwargs, **(endpoint.default_args or {})}
                         )
+                except (NoReverseMatch, TypeError, AttributeError, ValueError):
+                    continue
 
-                    replacements = []
+                replacements = []
 
-                    mtch = composite_regex.search(placeholder_url.lstrip("/"))
+                mtch = composite_regex.search(placeholder_url.lstrip("/"))
 
-                    if mtch:
-                        # there might be group matches that aren't part of
-                        # our kwargs, we go through this extra work to
-                        # make sure we aren't subbing spans that aren't
-                        # kwargs
-                        grp_mp = {
-                            idx: var for var, idx in composite_regex.groupindex.items()
-                        }
-
-                        for idx, value in enumerate(  # pylint: disable=W0612
-                            mtch.groups(), start=1
-                        ):
-                            if unnamed:
+                if mtch:
+                    # there might be group matches that aren't part of
+                    # our kwargs, we go through this extra work to
+                    # make sure we aren't subbing spans that aren't
+                    # kwargs
+                    grp_mp = {
+                        idx: var for var, idx in composite_regex.groupindex.items()
+                    }
+
+                    for idx, value in enumerate(  # pylint: disable=W0612
+                        mtch.groups(), start=1
+                    ):
+                        if unnamed:
+                            replacements.append((mtch.span(idx), Substitute(idx - 1)))
+                        else:
+                            # if the regex has non-capturing groups we
+                            # need to filter those out
+                            if idx in grp_mp:
                                 replacements.append(
-                                    (mtch.span(idx), Substitute(idx - 1))
+                                    (mtch.span(idx), Substitute(grp_mp[idx]))
                                 )
-                            else:
-                                # if the regex has non-capturing groups we
-                                # need to filter those out
-                                if idx in grp_mp:
-                                    replacements.append(
-                                        (mtch.span(idx), Substitute(grp_mp[idx]))
-                                    )
-
-                        url_idx = 0
-                        path = []
-                        for rpl in replacements:
-                            while url_idx <= rpl[0][0]:
-                                path.append(placeholder_url[url_idx])
-                                url_idx += 1
-                            path.append(rpl[1])
-                            url_idx += rpl[0][1] - rpl[0][0]
-                        if url_idx < len(placeholder_url):
-                            path.append(placeholder_url[url_idx:])
-
-                        yield from self.visit_path(
-                            path,
-                            list(kwargs.keys()),
-                            endpoint.default_args if num_patterns > 1 else None,
-                        )
 
-                    else:
-                        # if we're here it means this path was overridden
-                        # further down the tree
-                        yield (
-                            f"/* Path {composite_regex.pattern} overruled "
-                            "with: "
-                            + (
-                                f"args={unnamed} */"
-                                if unnamed
-                                else f"kwargs={list(params.keys())} */"
-                            )
+                    url_idx = 0
+                    path = []
+                    for rpl in replacements:
+                        while url_idx <= rpl[0][0]:
+                            path.append(placeholder_url[url_idx])
+                            url_idx += 1
+                        path.append(rpl[1])
+                        url_idx += rpl[0][1] - rpl[0][0]
+                    if url_idx < len(placeholder_url):
+                        path.append(placeholder_url[url_idx:])
+
+                    yield from self.visit_path(
+                        path,
+                        list(kwargs.keys()),
+                        endpoint.default_args if num_patterns > 1 else None,
+                    )
+
+                else:
+                    # if we're here it means this path was overridden
+                    # further down the tree
+                    yield (
+                        f"/* Path {composite_regex.pattern} overruled "
+                        "with: "
+                        + (
+                            f"args={unnamed} */"
+                            if unnamed
+                            else f"kwargs={list(params.keys())} */"
                         )
-                    return
+                    )
+                return
 
-                except NoReverseMatch:
-                    continue
         else:
             # this is a simple url with no params
             if not composite_regex.search(reverse(qname).lstrip("/")):
                 yield f"/* Path '{composite_regex.pattern}' overruled */"
             else:
                 yield from self.visit_path([reverse(qname)], [])
             return
```

### Comparing `django_render_static-2.2.0/PKG-INFO` & `django_render_static-2.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-render-static
-Version: 2.2.0
+Version: 2.2.1
 Summary: Use Django's template engine to render static files at deployment or package time. Includes transpilers for extending Django's url reversal and enums to JavaScript.
 Home-page: https://django-render-static.readthedocs.io
 License: MIT
 Keywords: django,static,templates,javascript,url,reverse,defines,transpiler,transpile,enum
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -36,131 +36,100 @@
 Provides-Extra: yaml
 Requires-Dist: Django (>=3.2,<6.0)
 Requires-Dist: Jinja2 (>=2.9,<4.0) ; extra == "jinja2" or extra == "all"
 Requires-Dist: PyYAML (>=5.1,<7.0) ; extra == "yaml" or extra == "all"
 Requires-Dist: django-typer (>=1.0.0,<2.0.0)
 Requires-Dist: importlib-resources (>=1.3.0) ; python_version < "3.9"
 Project-URL: Repository, https://github.com/bckohan/django-render-static
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-|MIT license| |PyPI version fury.io| |PyPI pyversions| |PyPi djversions| |PyPI status| |Documentation Status|
-|Code Cov| |Test Status| |Code Style|
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static/)
+[![PyPI djversions](https://img.shields.io/pypi/djversions/django-render-static.svg)](https://pypi.org/project/django-render-static/)
+[![PyPI status](https://img.shields.io/pypi/status/django-render-static.svg)](https://pypi.python.org/pypi/django-render-static)
+[![Documentation Status](https://readthedocs.org/projects/django-render-static/badge/?version=latest)](http://django-render-static.readthedocs.io/?badge=latest/)
+[![Code Cov](https://codecov.io/gh/bckohan/django-render-static/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://codecov.io/gh/bckohan/django-render-static)
+[![Test Status](https://github.com/bckohan/django-render-static/workflows/test/badge.svg)](https://github.com/bckohan/django-render-static/actions/workflows/test.yml)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-.. |MIT license| image:: https://img.shields.io/badge/License-MIT-blue.svg
-   :target: https://lbesson.mit-license.org/
-
-.. |PyPI version fury.io| image:: https://badge.fury.io/py/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static/
-
-.. |PyPI pyversions| image:: https://img.shields.io/pypi/pyversions/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static/
-
-.. |PyPI djversions| image:: https://img.shields.io/pypi/djversions/django-render-static.svg
-   :target: https://pypi.org/project/django-render-static/
-
-.. |PyPI status| image:: https://img.shields.io/pypi/status/django-render-static.svg
-   :target: https://pypi.python.org/pypi/django-render-static
-
-.. |Documentation Status| image:: https://readthedocs.org/projects/django-render-static/badge/?version=latest
-   :target: http://django-render-static.readthedocs.io/?badge=latest/
-
-.. |Code Cov| image:: https://codecov.io/gh/bckohan/django-render-static/branch/main/graph/badge.svg?token=0IZOKN2DYL
-   :target: https://codecov.io/gh/bckohan/django-render-static
-
-.. |Test Status| image:: https://github.com/bckohan/django-render-static/workflows/test/badge.svg
-   :target: https://github.com/bckohan/django-render-static/actions
-
-.. |Code Style| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-
-
-django-render-static
-#######################
+# django-render-static
 
 Use Django's template engines to render static files that are collected
 during the ``collectstatic`` routine and likely served above Django at runtime.
 Files rendered by django-render-static are immediately available to participate
 in the normal static file collection pipeline.
 
-For example, a frequently occurring pattern that violates the `DRY principle <https://en.wikipedia.org/wiki/Don%27t_repeat_yourself>`_
-is the presence of defines, or enum like structures in server side Python code that are simply replicated in client
-side JavaScript. Another example might be rebuilding Django URLs from arguments in a `Single Page Application <https://en.wikipedia.org/wiki/Single-page_application>`_.
-Single-sourcing these structures by transpiling client side code from the server side code keeps the stack bone DRY.
-
-`django-render-static` includes Python to Javascript transpilers for:
-    - Django's `reverse` function (`urls_to_js`)
-    - PEP 435 style Python enumerations (`enums_to_js`)
-    - Plain data define-like structures in Python classes and modules
-      (`defines_to_js`)
+For example, a frequently occurring pattern that violates the
+[DRY principle](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) is the presence of defines,
+or enum like structures in server side Python code that are simply replicated in client side
+JavaScript. Another example might be rebuilding Django URLs from arguments in a
+[Single Page Application](https://en.wikipedia.org/wiki/Single-page_application). Single-sourcing
+these structures by transpiling client side code from the server side code keeps the stack bone DRY.
+
+**`django-render-static` includes Python to Javascript transpilers for:**
+
+* Django's `reverse` function (`urls_to_js`)
+* PEP 435 style Python enumerations (`enums_to_js`)
+* Plain data define-like structures in Python classes and modules
+    (`defines_to_js`)
 
 Transpilation is extremely flexible and may be customized by using override blocks or extending the provided 
 transpilers.
 
 `django-render-static` also formalizes the concept of a package-time or deployment-time
 static file rendering step. It piggybacks off the existing templating engines and configurations
 and should therefore be familiar to Django developers. It supports both standard Django templating
 and Jinja templates and allows contexts to be specified in python, json or YAML.
 
 You can report bugs and discuss features on the
-`issues page <https://github.com/bckohan/django-render-static/issues>`_.
+[issues page](https://github.com/bckohan/django-render-static/issues).
 
-`Contributions <https://github.com/bckohan/django-render-static/blob/main/CONTRIBUTING.rst>`_ are
+[Contributions](https://github.com/bckohan/django-render-static/blob/main/CONTRIBUTING.rst) are
 encouraged!
 
-`Full documentation at read the docs. <https://django-render-static.readthedocs.io/en/latest/>`_
-
-Installation
-------------
-
-1. Clone django-render-static from GitHub_ or install a release off PyPI_ :
+[Full documentation at read the docs.](https://django-render-static.readthedocs.io/en/latest/)
 
-.. code:: bash
+## Installation
 
-       pip install django-render-static
+1. Clone django-render-static from [GitHub](http://github.com/bckohan/django-render-static) or install a release off [PyPI](http://pypi.python.org/pypi/django-render-static):
 
+```shell
+pip install django-render-static
+```
 
 2. Add 'render_static' to your ``INSTALLED_APPS`` :
 
-.. code:: python
-
-       INSTALLED_APPS = [
-           'render_static',
-       ]
-
+```python
+INSTALLED_APPS = [
+    'render_static',
+]
+```
 
 3. Add a ``STATIC_TEMPLATES`` configuration directive to your settings file:
 
-.. code:: python
-
-        STATIC_TEMPLATES = {
-            'templates' : [
-                ('path/to/template':, {'context' {'variable': 'value'})
-            ]
-        }
+```python
 
+STATIC_TEMPLATES = {
+    'templates' : [
+        ('path/to/template':, {'context' {'variable': 'value'})
+    ]
+}
+```
 
 4. Run ``renderstatic`` preceding every run of ``collectstatic`` :
 
-.. code:: bash
-
-        $> manage.py renderstatic
-        $> manage.py collectstatic
-
+```shell
+$> manage.py renderstatic
+$> manage.py collectstatic
+```
 
-.. _GitHub: http://github.com/bckohan/django-render-static
-.. _PyPI: http://pypi.python.org/pypi/django-render-static
-.. _django-enum: http://pypi.python.org/pypi/django-enum
-.. _enum-properties: http://pypi.python.org/pypi/enum-properties
+## Usage
 
-
-Usage
------
-
-Transpiling Model Field Choices
--------------------------------
+### Transpiling Model Field Choices
 
 You have an app with a model with a character field that has several valid choices defined in an
 enumeration type way, and you'd like to export those defines to JavaScript. You'd like to include
 a template for other's using your app to use to generate a defines.js file. Say your app structure
 looks like this::
 
     .
@@ -173,266 +142,258 @@
         │   └── examples
         │       └── defines.js
         └── urls.py
 
 
 Your defines/model classes might look like this:
 
-.. code:: python
-
-    class ExampleModel(Defines, models.Model):
+```python
+class ExampleModel(Defines, models.Model):
 
-        DEFINE1 = 'D1'
-        DEFINE2 = 'D2'
-        DEFINE3 = 'D3'
-        DEFINES = (
-            (DEFINE1, 'Define 1'),
-            (DEFINE2, 'Define 2'),
-            (DEFINE3, 'Define 3')
-        )
-
-        define_field = models.CharField(choices=DEFINES, max_length=2)
+    DEFINE1 = 'D1'
+    DEFINE2 = 'D2'
+    DEFINE3 = 'D3'
+    DEFINES = (
+        (DEFINE1, 'Define 1'),
+        (DEFINE2, 'Define 2'),
+        (DEFINE3, 'Define 3')
+    )
 
+    define_field = models.CharField(choices=DEFINES, max_length=2)
+```
 
 And your defines.js template might look like this:
 
-.. code:: js+django
-
-    {% defines_to_js modules="examples.models" %}
-
+```js+django
+{% defines_to_js modules="examples.models" %}
+```
 
 If someone wanted to use your defines template to generate a JavaScript version of your Python
 class their settings file might look like this:
 
-.. code:: python
-
-    STATIC_TEMPLATES = {
-        'templates': [
-            'examples/defines.js'
-        ]
-    }
+```python
+STATIC_TEMPLATES = {
+    'templates': [
+        'examples/defines.js'
+    ]
+}
+```
 
 
 And then of course they would call `renderstatic` before `collectstatic`:
 
-.. code:: bash
-
-    $> ./manage.py renderstatic
-    $> ./manage.py collectstatic
-
+```shell
+$> ./manage.py renderstatic
+$> ./manage.py collectstatic
+```
 
 This would create the following file::
 
     .
     └── examples
         └── static
             └── examples
                 └── defines.js
 
 Which would look like this:
 
-.. code:: javascript
-
-    const defines = {
-        ExampleModel: {
-            DEFINE1: "D1",
-            DEFINE2: "D2",
-            DEFINE3: "D3",
-            DEFINES: [["D1", "Define 1"], ["D2", "Define 2"], ["D3", "Define 3"]]
-        }
-    };
-
-
-Transpiling Enumerations
-------------------------
+```javascript
+const defines = {
+    ExampleModel: {
+        DEFINE1: "D1",
+        DEFINE2: "D2",
+        DEFINE3: "D3",
+        DEFINES: [["D1", "Define 1"], ["D2", "Define 2"], ["D3", "Define 3"]]
+    }
+};
+```
 
-Say instead of the usual choices tuple you're using PEP 435 style python
-enumerations as model fields using django-enum_ and enum-properties_. For example
-we might define a simple color enumeration like so:
+### Transpiling Enumerations
 
-.. code:: python
+Say instead of the usual choices tuple you're using PEP 435 style python enumerations as model
+fields using [django-enum](http://pypi.python.org/pypi/django-enum) and
+[enum-properties](http://pypi.python.org/pypi/enum-properties). For example we might define a
+simple color enumeration like so:
 
-    from django.db import models
-    from django_enum import EnumField, TextChoices
-    from enum_properties import p, s
+```python
+from django.db import models
+from django_enum import EnumField, TextChoices
+from enum_properties import p, s
 
-    class ExampleModel(models.Model):
+class ExampleModel(models.Model):
 
-        class Color(TextChoices, s('rgb'), s('hex', case_fold=True)):
+    class Color(TextChoices, s('rgb'), s('hex', case_fold=True)):
 
-            # name   value   label       rgb       hex
-            RED   =   'R',   'Red',   (1, 0, 0), 'ff0000'
-            GREEN =   'G',   'Green', (0, 1, 0), '00ff00'
-            BLUE  =   'B',   'Blue',  (0, 0, 1), '0000ff'
+        # name   value   label       rgb       hex
+        RED   =   'R',   'Red',   (1, 0, 0), 'ff0000'
+        GREEN =   'G',   'Green', (0, 1, 0), '00ff00'
+        BLUE  =   'B',   'Blue',  (0, 0, 1), '0000ff'
 
-        color = EnumField(Color, null=True, default=None)
+    color = EnumField(Color, null=True, default=None)
+```
 
 If we define an enum.js template that looks like this:
 
-.. code:: js+django
+```js+django
 
     {% enums_to_js enums="examples.models.ExampleModel.Color" %}
+```
 
 It will contain a javascript class transpilation of the Color enum that looks
 like this:
 
-.. code:: javascript
+```javascript
 
-    class Color {
+class Color {
 
-        static RED = new Color("R", "RED", "Red", [1, 0, 0], "ff0000");
-        static GREEN = new Color("G", "GREEN", "Green", [0, 1, 0], "00ff00");
-        static BLUE = new Color("B", "BLUE", "Blue", [0, 0, 1], "0000ff");
-
-        constructor (value, name, label, rgb, hex) {
-            this.value = value;
-            this.name = name;
-            this.label = label;
-            this.rgb = rgb;
-            this.hex = hex;
-        }
+    static RED = new Color("R", "RED", "Red", [1, 0, 0], "ff0000");
+    static GREEN = new Color("G", "GREEN", "Green", [0, 1, 0], "00ff00");
+    static BLUE = new Color("B", "BLUE", "Blue", [0, 0, 1], "0000ff");
+
+    constructor (value, name, label, rgb, hex) {
+        this.value = value;
+        this.name = name;
+        this.label = label;
+        this.rgb = rgb;
+        this.hex = hex;
+    }
 
-        toString() {
-            return this.value;
-        }
+    toString() {
+        return this.value;
+    }
 
-        static get(value) {
-            switch(value) {
-                case "R":
-                    return Color.RED;
-                case "G":
-                    return Color.GREEN;
-                case "B":
-                    return Color.BLUE;
-            }
-            throw new TypeError(`No Color enumeration maps to value ${value}`);
+    static get(value) {
+        switch(value) {
+            case "R":
+                return Color.RED;
+            case "G":
+                return Color.GREEN;
+            case "B":
+                return Color.BLUE;
         }
+        throw new TypeError(`No Color enumeration maps to value ${value}`);
+    }
 
-        static [Symbol.iterator]() {
-            return [Color.RED, Color.GREEN, Color.BLUE][Symbol.iterator]();
-        }
+    static [Symbol.iterator]() {
+        return [Color.RED, Color.GREEN, Color.BLUE][Symbol.iterator]();
     }
+}
+```
 
 We can now use our enumeration like so:
 
-.. code:: javascript
-
-    Color.BLUE === Color.get('B');
-    for (const color of Color) {
-        console.log(color);
-    }
-
+```javascript
+Color.BLUE === Color.get('B');
+for (const color of Color) {
+    console.log(color);
+}
+```
 
-Transpiling URL reversal
-------------------------
+### Transpiling URL reversal
 
 You'd like to be able to call something like `reverse` on path names from your client JavaScript
 code the same way you do from Python Django code.
 
 Your settings file might look like:
 
-.. code:: python
-
+```python
     STATIC_TEMPLATES={
         'ENGINES': [{
             'BACKEND': 'render_static.backends.StaticDjangoTemplates',
             'OPTIONS': {
                 'loaders': [
                     ('render_static.loaders.StaticLocMemLoader', {
                         'urls.js': '{% urls_to_js %}'
                     })
                 ]
             },
         }],
         'templates': ['urls.js']
     }
+```
 
+Then call `renderstatic` before `collectstatic`:
 
-Then call `renderstatic` before `collectstatic`::
-
-    $> ./manage.py renderstatic
-    $> ./manage.py collectstatic
+```shell
+$> ./manage.py renderstatic
+$> ./manage.py collectstatic
+```
 
 If your root urls.py looks like this:
 
-.. code:: python
-
-    from django.contrib import admin
-    from django.urls import path
-
-    from .views import MyView
-
-    urlpatterns = [
-        path('admin/', admin.site.urls),
-        path('simple', MyView.as_view(), name='simple'),
-        path('simple/<int:arg1>', MyView.as_view(), name='simple'),
-        path('different/<int:arg1>/<str:arg2>', MyView.as_view(), name='different'),
-    ]
-
+```python
+from django.contrib import admin
+from django.urls import path
+
+from .views import MyView
+
+urlpatterns = [
+    path('admin/', admin.site.urls),
+    path('simple', MyView.as_view(), name='simple'),
+    path('simple/<int:arg1>', MyView.as_view(), name='simple'),
+    path('different/<int:arg1>/<str:arg2>', MyView.as_view(), name='different'),
+]
+```
 
 So you can now fetch paths like this, in a way that is roughly API-equivalent
 to Django's `reverse` function:
 
-.. code:: javascript
-
-    import { URLResolver } from '/static/urls.js';
+```javascript
+import { URLResolver } from '/static/urls.js';
 
-    const urls = new URLResolver();
+const urls = new URLResolver();
 
-    // /different/143/emma
-    urls.reverse('different', {kwargs: {'arg1': 143, 'arg2': 'emma'}});
+// /different/143/emma
+urls.reverse('different', {kwargs: {'arg1': 143, 'arg2': 'emma'}});
 
-    // reverse also supports query parameters
-    // /different/143/emma?intarg=0&listarg=A&listarg=B&listarg=C
-    urls.reverse(
-        'different',
-        {
-            kwargs: {arg1: 143, arg2: 'emma'},
-            query: {
-                intarg: 0,
-                listarg: ['A', 'B', 'C']
-            }
+// reverse also supports query parameters
+// /different/143/emma?intarg=0&listarg=A&listarg=B&listarg=C
+urls.reverse(
+    'different',
+    {
+        kwargs: {arg1: 143, arg2: 'emma'},
+        query: {
+            intarg: 0,
+            listarg: ['A', 'B', 'C']
         }
-    );
-    
+    }
+);
+```
 
-URLGenerationFailed Exceptions & Placeholders
----------------------------------------------
+### URLGenerationFailed Exceptions & Placeholders
 
 If you encounter a ``URLGenerationFailed`` exception you most likely need to register a placeholder for the argument in question. A placeholder is just a string or object that can be coerced to a string that matches the regular expression for the argument:
 
-.. code:: python
-
-   from render_static.placeholders import register_variable_placeholder
+```python
+from render_static.placeholders import register_variable_placeholder
 
-   app_name = 'year_app'
-   urlpatterns = [
-       re_path(r'^fetch/(?P<year>\d{4})/$', YearView.as_view(), name='fetch_year')
-   ]
+app_name = 'year_app'
+urlpatterns = [
+    re_path(r'^fetch/(?P<year>\d{4})/$', YearView.as_view(), name='fetch_year')
+]
 
-   register_variable_placeholder('year', 2000, app_name=app_name)
+register_variable_placeholder('year', 2000, app_name=app_name)
+```
 
 Users should typically use a path instead of re_path and register their own custom converters when needed. Placeholders can be directly registered on the converter (and are then conveniently available to users of your app!):
 
-.. code:: python
-
-   from django.urls.converters import register_converter
-
-   class YearConverter:
-       regex = '[0-9]{4}'
-       placeholder = 2000  # this attribute is used by `url_to_js` to reverse paths
-
-       def to_python(self, value):
-           return int(value)
+```python
+from django.urls.converters import register_converter
 
-       def to_url(self, value):
-           return str(value)
+class YearConverter:
+    regex = '[0-9]{4}'
+    placeholder = 2000  # this attribute is used by `url_to_js` to reverse paths
 
+    def to_python(self, value):
+        return int(value)
 
-   register_converter(YearConverter, 'year')
+    def to_url(self, value):
+        return str(value)
 
-   urlpatterns = [
-       path('fetch/<year:year>', YearView.as_view(), name='fetch_year')
-   ]
 
+register_converter(YearConverter, 'year')
 
+urlpatterns = [
+    path('fetch/<year:year>', YearView.as_view(), name='fetch_year')
+]
+```
```

