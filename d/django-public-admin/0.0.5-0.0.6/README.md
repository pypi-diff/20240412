# Comparing `tmp/django-public-admin-0.0.5.tar.gz` & `tmp/django_public_admin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-public-admin-0.0.5.tar", last modified: Thu Oct 22 16:02:55 2020, max compression
+gzip compressed data, was "django_public_admin-0.0.6.tar", max compression
```

## Comparing `django-public-admin-0.0.5.tar` & `django_public_admin-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1059 2020-03-30 20:26:10.710718 django-public-admin-0.0.5/LICENSE
--rw-r--r--   0        0        0     1564 2020-04-04 22:43:11.974428 django-public-admin-0.0.5/README.md
--rw-r--r--   0        0        0        0 2020-04-04 17:51:01.797429 django-public-admin-0.0.5/public_admin/__init__.py
--rw-r--r--   0        0        0     1067 2020-04-04 21:38:40.359311 django-public-admin-0.0.5/public_admin/admin.py
--rw-r--r--   0        0        0      182 2020-10-22 15:47:41.490764 django-public-admin-0.0.5/public_admin/exceptions.py
--rw-r--r--   0        0        0     4046 2020-10-22 15:50:44.660374 django-public-admin-0.0.5/public_admin/sites.py
--rw-r--r--   0        0        0      239 2020-10-05 13:28:03.951086 django-public-admin-0.0.5/public_admin/templates/admin/base.html
--rw-r--r--   0        0        0      161 2020-10-05 13:28:03.951086 django-public-admin-0.0.5/public_admin/templates/admin/index.html
--rw-r--r--   0        0        0     1327 2020-10-22 16:01:55.587433 django-public-admin-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2325 2020-10-22 16:02:56.223662 django-public-admin-0.0.5/setup.py
--rw-r--r--   0        0        0     2651 2020-10-22 16:02:56.223928 django-public-admin-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-11 22:35:22.952526 django_public_admin-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1564 2024-04-11 22:35:22.952788 django_public_admin-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 22:35:22.958130 django_public_admin-0.0.6/public_admin/__init__.py
+-rw-r--r--   0        0        0     1068 2024-04-11 22:49:32.907727 django_public_admin-0.0.6/public_admin/admin.py
+-rw-r--r--   0        0        0      182 2024-04-11 22:35:22.958396 django_public_admin-0.0.6/public_admin/exceptions.py
+-rw-r--r--   0        0        0     4046 2024-04-11 22:35:22.958552 django_public_admin-0.0.6/public_admin/sites.py
+-rw-r--r--   0        0        0      239 2024-04-11 22:35:22.959006 django_public_admin-0.0.6/public_admin/templates/admin/base.html
+-rw-r--r--   0        0        0      161 2024-04-11 22:35:22.959264 django_public_admin-0.0.6/public_admin/templates/admin/index.html
+-rw-r--r--   0        0        0     1153 2024-04-11 23:42:30.481514 django_public_admin-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2578 1970-01-01 00:00:00.000000 django_public_admin-0.0.6/PKG-INFO
```

### Comparing `django-public-admin-0.0.5/LICENSE` & `django_public_admin-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-public-admin-0.0.5/README.md` & `django_public_admin-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `django-public-admin-0.0.5/public_admin/admin.py` & `django_public_admin-0.0.6/public_admin/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.contrib.admin import ModelAdmin
+
 from public_admin.sites import PublicAdminSite
 
 
 class PublicModelAdmin(ModelAdmin):
     """This mimics the Django's native ModelAdmin but filters URLs that should
     not exist in a public admin, and deals with request-based permissions."""
```

### Comparing `django-public-admin-0.0.5/public_admin/sites.py` & `django_public_admin-0.0.6/public_admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-public-admin-0.0.5/pyproject.toml` & `django_public_admin-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 [tool.poetry]
 name = "django-public-admin"
-version = "0.0.5"
+version = "0.0.6"
 description = "A public read-only version of the Django Admin"
 authors = ["Eduardo Cuducos <cuducos@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuducos/django-public-admin"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Topic :: Software Development",
   "Framework :: Django",
-  "Framework :: Django :: 2.0",
-  "Framework :: Django :: 2.1",
-  "Framework :: Django :: 2.2",
-  "Framework :: Django :: 3.0",
-  "Framework :: Django :: 3.1",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9"
+  "Framework :: Django :: 3.2",
+  "Framework :: Django :: 4.2",
+  "Framework :: Django :: 5.0",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 packages = [
     {include = "public_admin"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-django = ">=2"
+python = "^3.9"
+django = ">=3.2"
 
 [tool.poetry.dev-dependencies]
-black = { version = "*", allow-prereleases = true }
-flake8 = "^3.7.9"
-pip = "^20.0.2"
-pytest-black = "^0.3.8"
-pytest-flake8 = "^1.0.4"
-pytest-mock = "^2.0.0"
-readthedocs-sphinx-ext = "^1.0.1"
-sphinx = "^2.4.4"
-sphinx_rtd_theme = "^0.4.3"
-tox = "^3.14.6"
+pytest-ruff = "^0.3.1"
+readthedocs-sphinx-ext = "^2.2.5"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
+tox = "^4.14.2"
 
 [tool.pytest.ini_options]
-flake8-max-line-length = 88
-addopts = "--black --flake8"
+addopts = "--ruff --ruff-format"
+
+[tool.ruff.lint]
+select = ["E", "F", "I"]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django-public-admin-0.0.5/setup.py` & `django_public_admin-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,56 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-public-admin
+Version: 0.0.6
+Summary: A public read-only version of the Django Admin
+Home-page: https://github.com/cuducos/django-public-admin
+License: MIT
+Author: Eduardo Cuducos
+Author-email: cuducos@users.noreply.github.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Requires-Dist: django (>=3.2)
+Project-URL: Repository, https://github.com/cuducos/django-public-admin
+Description-Content-Type: text/markdown
+
+[![PyPI](https://img.shields.io/pypi/v/django-public-admin)](https://pypi.org/project/django-public-admin/) [![Documentation Status](https://readthedocs.org/projects/django-public-admin/badge/?version=latest)](https://django-public-admin.readthedocs.io/en/latest/?badge=latest) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-public-admin)](https://pypi.org/project/django-public-admin/) [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-public-admin)](https://pypi.org/project/django-public-admin/)
+
+# Django Public Admin
+
+
+A public and read-only version of the [Django Admin](https://docs.djangoproject.com/en/3.0/ref/contrib/admin/). A drop-in replacement for Django's native `AdminSite` and `ModelAdmin` for publicly accessible data. Check the [documentation](https://django-public-admin.readthedocs.io/en/latest/?badge=latest) for more information on how to use it.
+
+## Contributing
+
+We use `tox` to Run tests with Python 3.6, 3.7 and 3.8, and with Django 2 and 3. Also we use Black and `flake8`:
+
+```console
+$ poetry install
+$ poetry run tox
+```
+
+### Docs
+
+To build the docs we use [Sphinx](https://www.sphinx-doc.org/en/):
+
+```
+$ poetry run sphinx-build docs docs/_build/
+```
 
-packages = \
-['public_admin']
+Them just jump to `docs/_build/index.html`.
 
-package_data = \
-{'': ['*'], 'public_admin': ['templates/admin/*']}
+## License & Credits
 
-install_requires = \
-['django>=2']
-
-setup_kwargs = {
-    'name': 'django-public-admin',
-    'version': '0.0.5',
-    'description': 'A public read-only version of the Django Admin',
-    'long_description': "[![PyPI](https://img.shields.io/pypi/v/django-public-admin)](https://pypi.org/project/django-public-admin/) [![Documentation Status](https://readthedocs.org/projects/django-public-admin/badge/?version=latest)](https://django-public-admin.readthedocs.io/en/latest/?badge=latest) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-public-admin)](https://pypi.org/project/django-public-admin/) [![PyPI - Django Version](https://img.shields.io/pypi/djversions/django-public-admin)](https://pypi.org/project/django-public-admin/)\n\n# Django Public Admin\n\n\nA public and read-only version of the [Django Admin](https://docs.djangoproject.com/en/3.0/ref/contrib/admin/). A drop-in replacement for Django's native `AdminSite` and `ModelAdmin` for publicly accessible data. Check the [documentation](https://django-public-admin.readthedocs.io/en/latest/?badge=latest) for more information on how to use it.\n\n## Contributing\n\nWe use `tox` to Run tests with Python 3.6, 3.7 and 3.8, and with Django 2 and 3. Also we use Black and `flake8`:\n\n```console\n$ poetry install\n$ poetry run tox\n```\n\n### Docs\n\nTo build the docs we use [Sphinx](https://www.sphinx-doc.org/en/):\n\n```\n$ poetry run sphinx-build docs docs/_build/\n```\n\nThem just jump to `docs/_build/index.html`.\n\n## License & Credits\n\nThis package is licensed under [MIT license](/LICENSE) and acknowledge [Serenata de Amor](https://github.com/okfn-brasil/serenata-de-amor) (© [Open Knowledge Brasil](https://br.okfn.org) and, previously, © [Data Science Brigade](https://github.com/datasciencebr)).\n",
-    'author': 'Eduardo Cuducos',
-    'author_email': 'cuducos@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/cuducos/django-public-admin',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
+This package is licensed under [MIT license](/LICENSE) and acknowledge [Serenata de Amor](https://github.com/okfn-brasil/serenata-de-amor) (© [Open Knowledge Brasil](https://br.okfn.org) and, previously, © [Data Science Brigade](https://github.com/datasciencebr)).
 
-
-setup(**setup_kwargs)
```

