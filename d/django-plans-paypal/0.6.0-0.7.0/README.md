# Comparing `tmp/django-plans-paypal-0.6.0.tar.gz` & `tmp/django-plans-paypal-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-paypal-0.6.0.tar", last modified: Wed Mar 22 16:49:07 2023, max compression
+gzip compressed data, was "django-plans-paypal-0.7.0.tar", last modified: Fri Apr 12 13:13:10 2024, max compression
```

## Comparing `django-plans-paypal-0.6.0.tar` & `django-plans-paypal-0.7.0.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      229 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.684781 django-plans-paypal-0.6.0/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      348 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.684781 django-plans-paypal-0.6.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2596 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      432 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      469 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/.travis.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3306 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2508 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      179 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1549 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)     8532 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.684781 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     8532 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1229 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       87 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       19 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/django_plans_paypal.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8421 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      450 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      227 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      438 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      330 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      195 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/plans_paypal/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      721 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/apps.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4429 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/hooks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/plans_paypal/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1392 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2002 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/migrations/0002_auto_20211130_1117.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      618 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.684781 django-plans-paypal-0.6.0/plans_paypal/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/plans_paypal/templates/paypal_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)      157 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/templates/paypal_payments/payment.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/plans_paypal/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     8439 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/tests/test_hooks.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2141 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      594 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4109 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/plans_paypal/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      123 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      150 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      419 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2827 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1659 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/tests/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-03-22 16:49:07.688781 django-plans-paypal-0.6.0/tests/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/tests/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      226 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      388 2023-03-22 16:49:07.000000 django-plans-paypal-0.6.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      229 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.470719 django-plans-paypal-0.7.0/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      348 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.470719 django-plans-paypal-0.7.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3177 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      432 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      469 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/.travis.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3306 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2742 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1549 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6975 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6975 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1314 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       87 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       19 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/django_plans_paypal.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8421 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      450 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      227 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      438 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      330 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      195 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      721 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/apps.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4532 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/hooks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1392 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2002 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0002_auto_20211130_1117.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2146 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      618 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.466719 django-plans-paypal-0.7.0/plans_paypal/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/templates/paypal_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      157 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/templates/paypal_payments/payment.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.474719 django-plans-paypal-0.7.0/plans_paypal/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10620 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/test_hooks.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2141 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      594 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4289 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/plans_paypal/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      123 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      150 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      419 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2827 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1659 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:13:10.478720 django-plans-paypal-0.7.0/tests/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      226 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      388 2024-04-12 13:13:10.000000 django-plans-paypal-0.7.0/tox.ini
```

### Comparing `django-plans-paypal-0.6.0/.github/workflows/main.yml` & `django-plans-paypal-0.7.0/.github/workflows/main.yml`

 * *Files 22% similar despite different names*

```diff
@@ -15,37 +15,58 @@
 
 # A workflow run is made up of one or more jobs that can run sequentially or in parallel
 jobs:
   # This workflow contains a single job called "build"
   tests:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
-        
+
     strategy:
       matrix:
-        DJANGO_VERSION: ['3.1.*', '3.2.*', '4.0.*', '4.1.*']
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        DJANGO_VERSION: ['3.1.*', '3.2.*', '4.0.*', '4.1.*', '4.2.*', '5.0.*']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', '3.12']
         exclude:
-          - DJANGO_VERSION: '4.1.*'
-            python-version: '3.7'
-          - DJANGO_VERSION: '4.0.*'
-            python-version: '3.7'
           - DJANGO_VERSION: '3.1.*'
             python-version: '3.10'
           - DJANGO_VERSION: '3.1.*'
             python-version: '3.11'
+          - DJANGO_VERSION: '3.1.*'
+            python-version: '3.12'
+
           - DJANGO_VERSION: '3.2.*'
             python-version: '3.11'
+          - DJANGO_VERSION: '3.2.*'
+            python-version: '3.12'
+
+          - DJANGO_VERSION: '4.0.*'
+            python-version: '3.7'
           - DJANGO_VERSION: '4.0.*'
             python-version: '3.11'
+          - DJANGO_VERSION: '4.0.*'
+            python-version: '3.12'
+
+          - DJANGO_VERSION: '4.1.*'
+            python-version: '3.7'
+          - DJANGO_VERSION: '4.1.*'
+            python-version: '3.12'
+
+          - DJANGO_VERSION: '4.2.*'
+            python-version: '3.7'
+
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.7'
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.8'
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.9'
 
       fail-fast: false
     steps:
       - uses: actions/checkout@v2
-      
+
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
             python-version: ${{ matrix.python-version }}
       - uses: actions/cache@v2
         with:
           path: ~/.cache/pip
```

### Comparing `django-plans-paypal-0.6.0/CONTRIBUTING.rst` & `django-plans-paypal-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/HISTORY.rst` & `django-plans-paypal-0.7.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+0.7.0 (2024-04-12)
+++++++++++++++++++
+* migrate code to RecurringUserPlan.renewal_triggered_by
+* migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
+
 0.6.0 (2023-03-22)
 +++++++++++++++++++
 * Fix amount received on recurring payments, add tests
 
 0.5.1 (2023-02-11)
 +++++++++++++++++++
 * allow only logged users to access the failure view
```

### Comparing `django-plans-paypal-0.6.0/LICENSE` & `django-plans-paypal-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/Makefile` & `django-plans-paypal-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/PKG-INFO` & `django-plans-paypal-0.7.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,249 +1,255 @@
 Metadata-Version: 2.1
 Name: django-plans-paypal
-Version: 0.6.0
+Version: 0.7.0
 Summary: Integration between django-plans and django-paypal.
 Home-page: https://github.com/PetrDlouhy/django-plans-paypal
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
-Description: =============================
-        Django plans paypal
-        =============================
-        
-        .. image:: https://badge.fury.io/py/django-plans-paypal.svg
-            :target: https://badge.fury.io/py/django-plans-paypal
-        
-        .. image:: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml/badge.svg
-            :target: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml
-        
-        .. image:: https://codecov.io/gh/PetrDlouhy/django-plans-paypal/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/PetrDlouhy/django-plans-paypal
-        
-        Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-paypal <https://github.com/spookylukey/django-paypal>`_.
-        This will add subscribe buttons to the order page and automatically confirm the `Order` after the payment.
-        
-        Currently it is in experimetal stage, wher only recurring payments (subscribtions) are supported.
-        
-        
-        Documentation
-        -------------
-        
-        The full documentation is at https://django-plans-paypal.readthedocs.io.
-        
-        Quickstart
-        ----------
-        
-        Install and configure ``django-plans`` and ``django-paypal`` apps.
-        Capture mode is not yet supported, so ``PAYMENT_VARINANTS`` with ``'capture': False`` will not get confirmed.
-        
-        Install Django plans paypal::
-        
-            pip install django-plans-paypal
-        
-        Add it to your ``INSTALLED_APPS``, before the ``plans``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'payments',
-                'paypal.standard.ipn',
-                'plans_paypal',
-                ...
-            )
-        
-        Add your bussiness account e-mail address to settings:
-        
-        .. code-block:: python
-        
-           PAYPAL_BUSSINESS_EMAIL = "foo@bar.com"
-        
-           # To enable encrypted PayPal form:
-           PAYPAL_ENCRYPTED_FORM = True
-           PAYPAL_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
-           PAYPAL_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
-           PAYPAL_CERT = os.path.join(BASE_DIR, 'certs/paypal_cert.pem')
-           PAYPAL_CERT_ID = 'xxxxx'
-        
-        
-        Add Django ``plans_paypal`` to the URL patterns:
-        
-        .. code-block:: python
-        
-            urlpatterns = [
-                ...
-                url(r'^plans-paypal', include('plans_paypal.urls')),
-                ...
-            ]
-        
-        Override `django-plans` class `CreateOrderView` so that `get_success_url()` returns url of `paypal-payment` view:
-        
-        .. code-block:: python
-        
-            def get_success_url(self):
-               return reverse("paypal-payment", kwargs={'order_id': self.object.id})
-        
-        Sandbox testing
-        ---------------
-        
-        Set following settings:
-        
-        .. code-block:: python
-        
-           PAYPAL_TEST_BUSSINESS_EMAIL = "foo@bar.com"
-           PAYPAL_TEST = True
-        
-           # For encrypted PayPal sandbox form:
-           PAYPAL_TEST_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
-           PAYPAL_TEST_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
-           PAYPAL_TEST_CERT = os.path.join(BASE_DIR, 'certs/paypal_sandbox_cert.pem')
-           PAYPAL_TEST_CERT_ID = 'xxxx'
-        
-        
-        Redirect user to `paypal-payment-sandbox` instead of `paypal-payment` view.
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Running Tests
-        -------------
-        
-        Does the code actually work?
-        
-        ::
-        
-            source <YOURVIRTUALENV>/bin/activate
-            (myenv) $ pip install tox
-            (myenv) $ tox
-        
-        Credits
-        -------
-        
-        Tools used in rendering this package:
-        
-        *  Cookiecutter_
-        *  `cookiecutter-djangopackage`_
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
-        
-        
-        
-        
-        History
-        -------
-        
-        0.6.0 (2023-03-22)
-        +++++++++++++++++++
-        * Fix amount received on recurring payments, add tests
-        
-        0.5.1 (2023-02-11)
-        +++++++++++++++++++
-        * allow only logged users to access the failure view
-        
-        0.5.0 (2022-12-14)
-        +++++++++++++++++++
-        
-        * Fix tax received on recurring payments
-        * More robust receiving original Order ID (if PayPal fails to handle custom_data)
-        * update to Django 4.1
-        * fix completing recurring payments if first order status is returned
-        * only log error if custom data can't be parsed
-        
-        0.4.10 (2022-04-29)
-        +++++++++++++++++++
-        * fix problem with duplicate payments
-        * PayPalPaymentAdmin: display connected IPN fields
-        
-        0.4.9 (2022-03-07)
-        ++++++++++++++++++
-        * make parsing custom_data more robust
-        
-        0.4.8 (2022-01-19)
-        ++++++++++++++++++
-        * fix last release
-        * add tests and test on all supported Django/Python versions through GitHub actions
-        
-        0.4.7 (2022-01-13)
-        ++++++++++++++++++
-        * fix problem if there was ' in custom payment data
-        
-        0.4.6 (2021-12-02)
-        ++++++++++++++++++
-        * fix problem with creating bad JSON
-        
-        0.4.5 (2021-12-01)
-        ++++++++++++++++++
-        * fix IPN field editing in PayPalPaymentAdmin
-        * store also user e-mail in custom to enable search in IPN admin
-        
-        0.4.4 (2021-12-01)
-        ++++++++++++++++++
-        * create PayPalPayment before completing the order
-        
-        0.4.3 (2021-11-30)
-        ++++++++++++++++++
-        * fix problem with recurring payments
-        * add created/modified/author auto fields
-        
-        0.4.2 (2021-11-08)
-        ++++++++++++++++++
-        * fix problem with other IPN types
-        
-        0.4.1 (2021-10-18)
-        ++++++++++++++++++
-        * cancel order after returning to failure URL
-        
-        0.4.0 (2021-10-18)
-        ++++++++++++++++++
-        * allow to set up encrypted PayPal form
-        
-        0.3.0 (2021-10-15)
-        ++++++++++++++++++
-        * fixes and improvements to the sandbox/production functionality
-        * reverse sandbox logic - if no `PAYPAL_TEST`, the sandbox view would return production so nobody can pay through sandbox on production server
-        
-        0.2.2 (2021-10-12)
-        ++++++++++++++++++
-        * fix foregotten pudb
-        
-        0.2.1 (2021-10-12)
-        ++++++++++++++++++
-        * add sandbox view, so both production and sandbox can be used on one server
-        
-        0.2.0 (2021-10-11)
-        ++++++++++++++++++
-        * fix periods to complain with PayPal maximal durations
-        
-        0.1.0 (2021-10-08)
-        ++++++++++++++++++
-        * hook ipn.PayPalIpn object with plans.Order (for later usage e.g. determining PayPal fee)
-        * set plan renewal for django-plans
-        
-        0.0.2 (2018-08-05)
-        ++++++++++++++++++
-        
-        * Payment process without capturing should work
-        * Automatic buttons generation
-        
-        0.0.1 (2018-07-23)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
 Keywords: django-plans-paypal
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=============================
+Django plans paypal
+=============================
+
+.. image:: https://badge.fury.io/py/django-plans-paypal.svg
+    :target: https://badge.fury.io/py/django-plans-paypal
+
+.. image:: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml
+
+.. image:: https://codecov.io/gh/PetrDlouhy/django-plans-paypal/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/django-plans-paypal
+
+Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-paypal <https://github.com/spookylukey/django-paypal>`_.
+This will add subscribe buttons to the order page and automatically confirm the `Order` after the payment.
+
+Currently it is in experimetal stage, wher only recurring payments (subscribtions) are supported.
+
+
+Documentation
+-------------
+
+The full documentation is at https://django-plans-paypal.readthedocs.io.
+
+Quickstart
+----------
+
+Install and configure ``django-plans`` and ``django-paypal`` apps.
+Capture mode is not yet supported, so ``PAYMENT_VARINANTS`` with ``'capture': False`` will not get confirmed.
+
+Install Django plans paypal::
+
+    pip install django-plans-paypal
+
+Add it to your ``INSTALLED_APPS``, before the ``plans``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        'payments',
+        'paypal.standard.ipn',
+        'plans_paypal',
+        ...
+    )
+
+Add your bussiness account e-mail address to settings:
+
+.. code-block:: python
+
+   PAYPAL_BUSSINESS_EMAIL = "foo@bar.com"
+
+   # To enable encrypted PayPal form:
+   PAYPAL_ENCRYPTED_FORM = True
+   PAYPAL_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
+   PAYPAL_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
+   PAYPAL_CERT = os.path.join(BASE_DIR, 'certs/paypal_cert.pem')
+   PAYPAL_CERT_ID = 'xxxxx'
+
+
+Add Django ``plans_paypal`` to the URL patterns:
+
+.. code-block:: python
+
+    urlpatterns = [
+        ...
+        url(r'^plans-paypal', include('plans_paypal.urls')),
+        ...
+    ]
+
+Override `django-plans` class `CreateOrderView` so that `get_success_url()` returns url of `paypal-payment` view:
+
+.. code-block:: python
+
+    def get_success_url(self):
+       return reverse("paypal-payment", kwargs={'order_id': self.object.id})
+
+Sandbox testing
+---------------
+
+Set following settings:
+
+.. code-block:: python
+
+   PAYPAL_TEST_BUSSINESS_EMAIL = "foo@bar.com"
+   PAYPAL_TEST = True
+
+   # For encrypted PayPal sandbox form:
+   PAYPAL_TEST_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
+   PAYPAL_TEST_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
+   PAYPAL_TEST_CERT = os.path.join(BASE_DIR, 'certs/paypal_sandbox_cert.pem')
+   PAYPAL_TEST_CERT_ID = 'xxxx'
+
+
+Redirect user to `paypal-payment-sandbox` instead of `paypal-payment` view.
+
+Features
+--------
+
+* TODO
+
+Running Tests
+-------------
+
+Does the code actually work?
+
+::
+
+    source <YOURVIRTUALENV>/bin/activate
+    (myenv) $ pip install tox
+    (myenv) $ tox
+
+Credits
+-------
+
+Tools used in rendering this package:
+
+*  Cookiecutter_
+*  `cookiecutter-djangopackage`_
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
+
+
+
+
+History
+-------
+
+0.7.0 (2024-04-12)
+++++++++++++++++++
+* migrate code to RecurringUserPlan.renewal_triggered_by
+* migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
+
+0.6.0 (2023-03-22)
++++++++++++++++++++
+* Fix amount received on recurring payments, add tests
+
+0.5.1 (2023-02-11)
++++++++++++++++++++
+* allow only logged users to access the failure view
+
+0.5.0 (2022-12-14)
++++++++++++++++++++
+
+* Fix tax received on recurring payments
+* More robust receiving original Order ID (if PayPal fails to handle custom_data)
+* update to Django 4.1
+* fix completing recurring payments if first order status is returned
+* only log error if custom data can't be parsed
+
+0.4.10 (2022-04-29)
++++++++++++++++++++
+* fix problem with duplicate payments
+* PayPalPaymentAdmin: display connected IPN fields
+
+0.4.9 (2022-03-07)
+++++++++++++++++++
+* make parsing custom_data more robust
+
+0.4.8 (2022-01-19)
+++++++++++++++++++
+* fix last release
+* add tests and test on all supported Django/Python versions through GitHub actions
+
+0.4.7 (2022-01-13)
+++++++++++++++++++
+* fix problem if there was ' in custom payment data
+
+0.4.6 (2021-12-02)
+++++++++++++++++++
+* fix problem with creating bad JSON
+
+0.4.5 (2021-12-01)
+++++++++++++++++++
+* fix IPN field editing in PayPalPaymentAdmin
+* store also user e-mail in custom to enable search in IPN admin
+
+0.4.4 (2021-12-01)
+++++++++++++++++++
+* create PayPalPayment before completing the order
+
+0.4.3 (2021-11-30)
+++++++++++++++++++
+* fix problem with recurring payments
+* add created/modified/author auto fields
+
+0.4.2 (2021-11-08)
+++++++++++++++++++
+* fix problem with other IPN types
+
+0.4.1 (2021-10-18)
+++++++++++++++++++
+* cancel order after returning to failure URL
+
+0.4.0 (2021-10-18)
+++++++++++++++++++
+* allow to set up encrypted PayPal form
+
+0.3.0 (2021-10-15)
+++++++++++++++++++
+* fixes and improvements to the sandbox/production functionality
+* reverse sandbox logic - if no `PAYPAL_TEST`, the sandbox view would return production so nobody can pay through sandbox on production server
+
+0.2.2 (2021-10-12)
+++++++++++++++++++
+* fix foregotten pudb
+
+0.2.1 (2021-10-12)
+++++++++++++++++++
+* add sandbox view, so both production and sandbox can be used on one server
+
+0.2.0 (2021-10-11)
+++++++++++++++++++
+* fix periods to complain with PayPal maximal durations
+
+0.1.0 (2021-10-08)
+++++++++++++++++++
+* hook ipn.PayPalIpn object with plans.Order (for later usage e.g. determining PayPal fee)
+* set plan renewal for django-plans
+
+0.0.2 (2018-08-05)
+++++++++++++++++++
+
+* Payment process without capturing should work
+* Automatic buttons generation
+
+0.0.1 (2018-07-23)
+++++++++++++++++++
+
+* First release on PyPI.
```

### Comparing `django-plans-paypal-0.6.0/README.rst` & `django-plans-paypal-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/django_plans_paypal.egg-info/PKG-INFO` & `django-plans-paypal-0.7.0/django_plans_paypal.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,249 +1,255 @@
 Metadata-Version: 2.1
 Name: django-plans-paypal
-Version: 0.6.0
+Version: 0.7.0
 Summary: Integration between django-plans and django-paypal.
 Home-page: https://github.com/PetrDlouhy/django-plans-paypal
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
-Description: =============================
-        Django plans paypal
-        =============================
-        
-        .. image:: https://badge.fury.io/py/django-plans-paypal.svg
-            :target: https://badge.fury.io/py/django-plans-paypal
-        
-        .. image:: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml/badge.svg
-            :target: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml
-        
-        .. image:: https://codecov.io/gh/PetrDlouhy/django-plans-paypal/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/PetrDlouhy/django-plans-paypal
-        
-        Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-paypal <https://github.com/spookylukey/django-paypal>`_.
-        This will add subscribe buttons to the order page and automatically confirm the `Order` after the payment.
-        
-        Currently it is in experimetal stage, wher only recurring payments (subscribtions) are supported.
-        
-        
-        Documentation
-        -------------
-        
-        The full documentation is at https://django-plans-paypal.readthedocs.io.
-        
-        Quickstart
-        ----------
-        
-        Install and configure ``django-plans`` and ``django-paypal`` apps.
-        Capture mode is not yet supported, so ``PAYMENT_VARINANTS`` with ``'capture': False`` will not get confirmed.
-        
-        Install Django plans paypal::
-        
-            pip install django-plans-paypal
-        
-        Add it to your ``INSTALLED_APPS``, before the ``plans``:
-        
-        .. code-block:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'payments',
-                'paypal.standard.ipn',
-                'plans_paypal',
-                ...
-            )
-        
-        Add your bussiness account e-mail address to settings:
-        
-        .. code-block:: python
-        
-           PAYPAL_BUSSINESS_EMAIL = "foo@bar.com"
-        
-           # To enable encrypted PayPal form:
-           PAYPAL_ENCRYPTED_FORM = True
-           PAYPAL_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
-           PAYPAL_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
-           PAYPAL_CERT = os.path.join(BASE_DIR, 'certs/paypal_cert.pem')
-           PAYPAL_CERT_ID = 'xxxxx'
-        
-        
-        Add Django ``plans_paypal`` to the URL patterns:
-        
-        .. code-block:: python
-        
-            urlpatterns = [
-                ...
-                url(r'^plans-paypal', include('plans_paypal.urls')),
-                ...
-            ]
-        
-        Override `django-plans` class `CreateOrderView` so that `get_success_url()` returns url of `paypal-payment` view:
-        
-        .. code-block:: python
-        
-            def get_success_url(self):
-               return reverse("paypal-payment", kwargs={'order_id': self.object.id})
-        
-        Sandbox testing
-        ---------------
-        
-        Set following settings:
-        
-        .. code-block:: python
-        
-           PAYPAL_TEST_BUSSINESS_EMAIL = "foo@bar.com"
-           PAYPAL_TEST = True
-        
-           # For encrypted PayPal sandbox form:
-           PAYPAL_TEST_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
-           PAYPAL_TEST_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
-           PAYPAL_TEST_CERT = os.path.join(BASE_DIR, 'certs/paypal_sandbox_cert.pem')
-           PAYPAL_TEST_CERT_ID = 'xxxx'
-        
-        
-        Redirect user to `paypal-payment-sandbox` instead of `paypal-payment` view.
-        
-        Features
-        --------
-        
-        * TODO
-        
-        Running Tests
-        -------------
-        
-        Does the code actually work?
-        
-        ::
-        
-            source <YOURVIRTUALENV>/bin/activate
-            (myenv) $ pip install tox
-            (myenv) $ tox
-        
-        Credits
-        -------
-        
-        Tools used in rendering this package:
-        
-        *  Cookiecutter_
-        *  `cookiecutter-djangopackage`_
-        
-        .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-        .. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
-        
-        
-        
-        
-        History
-        -------
-        
-        0.6.0 (2023-03-22)
-        +++++++++++++++++++
-        * Fix amount received on recurring payments, add tests
-        
-        0.5.1 (2023-02-11)
-        +++++++++++++++++++
-        * allow only logged users to access the failure view
-        
-        0.5.0 (2022-12-14)
-        +++++++++++++++++++
-        
-        * Fix tax received on recurring payments
-        * More robust receiving original Order ID (if PayPal fails to handle custom_data)
-        * update to Django 4.1
-        * fix completing recurring payments if first order status is returned
-        * only log error if custom data can't be parsed
-        
-        0.4.10 (2022-04-29)
-        +++++++++++++++++++
-        * fix problem with duplicate payments
-        * PayPalPaymentAdmin: display connected IPN fields
-        
-        0.4.9 (2022-03-07)
-        ++++++++++++++++++
-        * make parsing custom_data more robust
-        
-        0.4.8 (2022-01-19)
-        ++++++++++++++++++
-        * fix last release
-        * add tests and test on all supported Django/Python versions through GitHub actions
-        
-        0.4.7 (2022-01-13)
-        ++++++++++++++++++
-        * fix problem if there was ' in custom payment data
-        
-        0.4.6 (2021-12-02)
-        ++++++++++++++++++
-        * fix problem with creating bad JSON
-        
-        0.4.5 (2021-12-01)
-        ++++++++++++++++++
-        * fix IPN field editing in PayPalPaymentAdmin
-        * store also user e-mail in custom to enable search in IPN admin
-        
-        0.4.4 (2021-12-01)
-        ++++++++++++++++++
-        * create PayPalPayment before completing the order
-        
-        0.4.3 (2021-11-30)
-        ++++++++++++++++++
-        * fix problem with recurring payments
-        * add created/modified/author auto fields
-        
-        0.4.2 (2021-11-08)
-        ++++++++++++++++++
-        * fix problem with other IPN types
-        
-        0.4.1 (2021-10-18)
-        ++++++++++++++++++
-        * cancel order after returning to failure URL
-        
-        0.4.0 (2021-10-18)
-        ++++++++++++++++++
-        * allow to set up encrypted PayPal form
-        
-        0.3.0 (2021-10-15)
-        ++++++++++++++++++
-        * fixes and improvements to the sandbox/production functionality
-        * reverse sandbox logic - if no `PAYPAL_TEST`, the sandbox view would return production so nobody can pay through sandbox on production server
-        
-        0.2.2 (2021-10-12)
-        ++++++++++++++++++
-        * fix foregotten pudb
-        
-        0.2.1 (2021-10-12)
-        ++++++++++++++++++
-        * add sandbox view, so both production and sandbox can be used on one server
-        
-        0.2.0 (2021-10-11)
-        ++++++++++++++++++
-        * fix periods to complain with PayPal maximal durations
-        
-        0.1.0 (2021-10-08)
-        ++++++++++++++++++
-        * hook ipn.PayPalIpn object with plans.Order (for later usage e.g. determining PayPal fee)
-        * set plan renewal for django-plans
-        
-        0.0.2 (2018-08-05)
-        ++++++++++++++++++
-        
-        * Payment process without capturing should work
-        * Automatic buttons generation
-        
-        0.0.1 (2018-07-23)
-        ++++++++++++++++++
-        
-        * First release on PyPI.
-        
 Keywords: django-plans-paypal
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=============================
+Django plans paypal
+=============================
+
+.. image:: https://badge.fury.io/py/django-plans-paypal.svg
+    :target: https://badge.fury.io/py/django-plans-paypal
+
+.. image:: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/PetrDlouhy/django-plans-paypal/actions/workflows/main.yml
+
+.. image:: https://codecov.io/gh/PetrDlouhy/django-plans-paypal/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/PetrDlouhy/django-plans-paypal
+
+Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-paypal <https://github.com/spookylukey/django-paypal>`_.
+This will add subscribe buttons to the order page and automatically confirm the `Order` after the payment.
+
+Currently it is in experimetal stage, wher only recurring payments (subscribtions) are supported.
+
+
+Documentation
+-------------
+
+The full documentation is at https://django-plans-paypal.readthedocs.io.
+
+Quickstart
+----------
+
+Install and configure ``django-plans`` and ``django-paypal`` apps.
+Capture mode is not yet supported, so ``PAYMENT_VARINANTS`` with ``'capture': False`` will not get confirmed.
+
+Install Django plans paypal::
+
+    pip install django-plans-paypal
+
+Add it to your ``INSTALLED_APPS``, before the ``plans``:
+
+.. code-block:: python
+
+    INSTALLED_APPS = (
+        ...
+        'payments',
+        'paypal.standard.ipn',
+        'plans_paypal',
+        ...
+    )
+
+Add your bussiness account e-mail address to settings:
+
+.. code-block:: python
+
+   PAYPAL_BUSSINESS_EMAIL = "foo@bar.com"
+
+   # To enable encrypted PayPal form:
+   PAYPAL_ENCRYPTED_FORM = True
+   PAYPAL_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
+   PAYPAL_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
+   PAYPAL_CERT = os.path.join(BASE_DIR, 'certs/paypal_cert.pem')
+   PAYPAL_CERT_ID = 'xxxxx'
+
+
+Add Django ``plans_paypal`` to the URL patterns:
+
+.. code-block:: python
+
+    urlpatterns = [
+        ...
+        url(r'^plans-paypal', include('plans_paypal.urls')),
+        ...
+    ]
+
+Override `django-plans` class `CreateOrderView` so that `get_success_url()` returns url of `paypal-payment` view:
+
+.. code-block:: python
+
+    def get_success_url(self):
+       return reverse("paypal-payment", kwargs={'order_id': self.object.id})
+
+Sandbox testing
+---------------
+
+Set following settings:
+
+.. code-block:: python
+
+   PAYPAL_TEST_BUSSINESS_EMAIL = "foo@bar.com"
+   PAYPAL_TEST = True
+
+   # For encrypted PayPal sandbox form:
+   PAYPAL_TEST_PRIVATE_CERT = os.path.join(BASE_DIR, 'certs/paypal_private.pem')
+   PAYPAL_TEST_PUBLIC_CERT = os.path.join(BASE_DIR, 'certs/paypal_public.pem')
+   PAYPAL_TEST_CERT = os.path.join(BASE_DIR, 'certs/paypal_sandbox_cert.pem')
+   PAYPAL_TEST_CERT_ID = 'xxxx'
+
+
+Redirect user to `paypal-payment-sandbox` instead of `paypal-payment` view.
+
+Features
+--------
+
+* TODO
+
+Running Tests
+-------------
+
+Does the code actually work?
+
+::
+
+    source <YOURVIRTUALENV>/bin/activate
+    (myenv) $ pip install tox
+    (myenv) $ tox
+
+Credits
+-------
+
+Tools used in rendering this package:
+
+*  Cookiecutter_
+*  `cookiecutter-djangopackage`_
+
+.. _Cookiecutter: https://github.com/audreyr/cookiecutter
+.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
+
+
+
+
+History
+-------
+
+0.7.0 (2024-04-12)
+++++++++++++++++++
+* migrate code to RecurringUserPlan.renewal_triggered_by
+* migrate data of RecurringUserPlans with payment_provider="paypal-recurring" and renewal_triggered_by=TASK to renewal_triggered_by=OTHER
+
+0.6.0 (2023-03-22)
++++++++++++++++++++
+* Fix amount received on recurring payments, add tests
+
+0.5.1 (2023-02-11)
++++++++++++++++++++
+* allow only logged users to access the failure view
+
+0.5.0 (2022-12-14)
++++++++++++++++++++
+
+* Fix tax received on recurring payments
+* More robust receiving original Order ID (if PayPal fails to handle custom_data)
+* update to Django 4.1
+* fix completing recurring payments if first order status is returned
+* only log error if custom data can't be parsed
+
+0.4.10 (2022-04-29)
++++++++++++++++++++
+* fix problem with duplicate payments
+* PayPalPaymentAdmin: display connected IPN fields
+
+0.4.9 (2022-03-07)
+++++++++++++++++++
+* make parsing custom_data more robust
+
+0.4.8 (2022-01-19)
+++++++++++++++++++
+* fix last release
+* add tests and test on all supported Django/Python versions through GitHub actions
+
+0.4.7 (2022-01-13)
+++++++++++++++++++
+* fix problem if there was ' in custom payment data
+
+0.4.6 (2021-12-02)
+++++++++++++++++++
+* fix problem with creating bad JSON
+
+0.4.5 (2021-12-01)
+++++++++++++++++++
+* fix IPN field editing in PayPalPaymentAdmin
+* store also user e-mail in custom to enable search in IPN admin
+
+0.4.4 (2021-12-01)
+++++++++++++++++++
+* create PayPalPayment before completing the order
+
+0.4.3 (2021-11-30)
+++++++++++++++++++
+* fix problem with recurring payments
+* add created/modified/author auto fields
+
+0.4.2 (2021-11-08)
+++++++++++++++++++
+* fix problem with other IPN types
+
+0.4.1 (2021-10-18)
+++++++++++++++++++
+* cancel order after returning to failure URL
+
+0.4.0 (2021-10-18)
+++++++++++++++++++
+* allow to set up encrypted PayPal form
+
+0.3.0 (2021-10-15)
+++++++++++++++++++
+* fixes and improvements to the sandbox/production functionality
+* reverse sandbox logic - if no `PAYPAL_TEST`, the sandbox view would return production so nobody can pay through sandbox on production server
+
+0.2.2 (2021-10-12)
+++++++++++++++++++
+* fix foregotten pudb
+
+0.2.1 (2021-10-12)
+++++++++++++++++++
+* add sandbox view, so both production and sandbox can be used on one server
+
+0.2.0 (2021-10-11)
+++++++++++++++++++
+* fix periods to complain with PayPal maximal durations
+
+0.1.0 (2021-10-08)
+++++++++++++++++++
+* hook ipn.PayPalIpn object with plans.Order (for later usage e.g. determining PayPal fee)
+* set plan renewal for django-plans
+
+0.0.2 (2018-08-05)
+++++++++++++++++++
+
+* Payment process without capturing should work
+* Automatic buttons generation
+
+0.0.1 (2018-07-23)
+++++++++++++++++++
+
+* First release on PyPI.
```

### Comparing `django-plans-paypal-0.6.0/django_plans_paypal.egg-info/SOURCES.txt` & `django-plans-paypal-0.7.0/django_plans_paypal.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 plans_paypal/apps.py
 plans_paypal/hooks.py
 plans_paypal/models.py
 plans_paypal/urls.py
 plans_paypal/views.py
 plans_paypal/migrations/0001_initial.py
 plans_paypal/migrations/0002_auto_20211130_1117.py
+plans_paypal/migrations/0003_recurringuserplan_renewal_triggered_by_task_to_other.py
 plans_paypal/migrations/__init__.py
 plans_paypal/templates/paypal_payments/payment.html
 plans_paypal/tests/__init__.py
 plans_paypal/tests/test_hooks.py
 plans_paypal/tests/test_views.py
 tests/__init__.py
 tests/settings.py
```

### Comparing `django-plans-paypal-0.6.0/docs/Makefile` & `django-plans-paypal-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/docs/conf.py` & `django-plans-paypal-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/docs/make.bat` & `django-plans-paypal-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/admin.py` & `django-plans-paypal-0.7.0/plans_paypal/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/hooks.py` & `django-plans-paypal-0.7.0/plans_paypal/hooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import logging
 
 from django.conf import settings
 from paypal.standard.ipn.signals import valid_ipn_received
 from paypal.standard.models import ST_PP_COMPLETED, ST_PP_PENDING
+from plans.base.models import AbstractRecurringUserPlan
 from plans.models import Order
 
 from .models import PayPalPayment
 
 
 logger = logging.getLogger(__name__)
 
@@ -109,15 +110,15 @@
                 currency=ipn_obj.mc_currency,
             )
         user_plan.set_plan_renewal(
             order,
             token=ipn_obj.subscr_id,
             payment_provider="paypal-recurring"
             + ("-sandbox" if ipn_obj.test_ipn else ""),
-            has_automatic_renewal=True,
+            renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
             token_verified=True,
         )
         paypal_payment = PayPalPayment.objects.create(
             paypal_ipn=ipn_obj, user_plan=user_plan, order=order
         )  # use the new order
         order.complete_order()
         return paypal_payment
```

### Comparing `django-plans-paypal-0.6.0/plans_paypal/migrations/0001_initial.py` & `django-plans-paypal-0.7.0/plans_paypal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/migrations/0002_auto_20211130_1117.py` & `django-plans-paypal-0.7.0/plans_paypal/migrations/0002_auto_20211130_1117.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/models.py` & `django-plans-paypal-0.7.0/plans_paypal/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/tests/test_hooks.py` & `django-plans-paypal-0.7.0/plans_paypal/tests/test_hooks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from decimal import Decimal
 from unittest.mock import patch
 
 from django.test import TestCase, override_settings
 from model_bakery import baker
 from paypal.standard.models import ST_PP_COMPLETED
+from plans.base.models import AbstractRecurringUserPlan
 from plans.models import Invoice, Order
 
 from plans_paypal.hooks import parse_custom, receive_ipn
 
 
 class HooksTests(TestCase):
     def test_receive_ipn_no_subscription(self):
@@ -42,14 +43,16 @@
             f"'user_plan_id': {user_plan.id},"
             "}",
         )
         self.assertEqual(receive_ipn(ipn), None)
         mock_logger.error.assert_called_with(
             "IPN with unknown status", extra={"ipn_obj": ipn, "ipn_status": ""}
         )
+        user_plan.refresh_from_db()
+        self.assertFalse(hasattr(user_plan, "recurring"))
 
     def test_receive_ipn_completed_email_does_not_match(self):
         user_plan = baker.make("UserPlan")
         order = baker.make("Order", user=user_plan.user)
         ipn = baker.make(
             "PayPalIPN",
             txn_type="subscr_payment",
@@ -59,14 +62,16 @@
             f"'user_plan_id': {user_plan.id},"
             "}",
         )
         with self.assertRaisesRegex(
             Exception, "Returned email doesn't match: '' != 'fake@email.com'"
         ):
             receive_ipn(ipn)
+        user_plan.refresh_from_db()
+        self.assertFalse(hasattr(user_plan, "recurring"))
 
     def test_receive_ipn_completed(self):
         user = baker.make("User", username="foobar")
         user_plan = baker.make("UserPlan", user=user)
         order = baker.make("Order", user=user, amount=100)
         order.user.save()
         pricing = baker.make("Pricing")
@@ -81,14 +86,24 @@
             f"'user_plan_id': {user_plan.id},"
             f"'pricing_id': {pricing.id},"
             "}",
         )
         paypal_payment = receive_ipn(ipn)
         self.assertEqual(paypal_payment.paypal_ipn, ipn)
         self.assertEqual(paypal_payment.order, order)
+        user.userplan.refresh_from_db()
+        self.assertEqual(user.userplan.recurring.amount, Decimal("100.00"))
+        self.assertIsNone(user.userplan.recurring.tax)
+        self.assertEqual(user.userplan.recurring.token, "")
+        self.assertEqual(user.userplan.recurring.payment_provider, "paypal-recurring")
+        self.assertEqual(
+            user.userplan.recurring.renewal_triggered_by,
+            AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+        )
+        self.assertTrue(user.userplan.recurring.token_verified)
 
     def test_receive_ipn_completed_order_completed(self):
         """
         Test completed IPN status when the previous order is completed
         and we need to make new order
         """
         user = baker.make("User", username="foobar")
@@ -109,14 +124,24 @@
             f"'user_plan_id': {user_plan.id},"
             f"'pricing_id': {pricing.id},"
             "}",
         )
         paypal_payment = receive_ipn(ipn)
         self.assertEqual(paypal_payment.paypal_ipn, ipn)
         self.assertNotEqual(paypal_payment.order, order)
+        user.userplan.refresh_from_db()
+        self.assertEqual(user.userplan.recurring.amount, Decimal("100.00"))
+        self.assertIsNone(user.userplan.recurring.tax)
+        self.assertEqual(user.userplan.recurring.token, "")
+        self.assertEqual(user.userplan.recurring.payment_provider, "paypal-recurring")
+        self.assertEqual(
+            user.userplan.recurring.renewal_triggered_by,
+            AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+        )
+        self.assertTrue(user.userplan.recurring.token_verified)
 
     @override_settings(
         PLANS_INVOICE_ISSUER={
             "issuer_name": "Foo bar company",
             "issuer_street": "Foo",
             "issuer_city": "Bar",
             "issuer_zipcode": "12345",
@@ -158,14 +183,21 @@
         self.assertEqual(paypal_payment.order.amount, 100.00)
         self.assertEqual(paypal_payment.order.tax, 12.0)
         self.assertEqual(paypal_payment.order.total(), 112.00)
         user.userplan.refresh_from_db()
         new_recurring_plan = user.userplan.recurring
         self.assertEqual(new_recurring_plan.amount, Decimal("100.00"))
         self.assertEqual(new_recurring_plan.tax, 12.0)
+        self.assertEqual(new_recurring_plan.token, "")
+        self.assertEqual(new_recurring_plan.payment_provider, "paypal-recurring")
+        self.assertEqual(
+            new_recurring_plan.renewal_triggered_by,
+            AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+        )
+        self.assertTrue(new_recurring_plan.token_verified)
         invoice = Invoice.objects.get(type=Invoice.INVOICE_TYPES.INVOICE)
         self.assertEqual(invoice.total, 112.00)
         self.assertEqual(invoice.total_net, 100.00)
         self.assertEqual(invoice.tax_total, 12.0)
         self.assertEqual(invoice.tax, 12.0)
 
     def test_receive_ipn_renewal_wrong_amount(self):
@@ -192,14 +224,24 @@
             f"'first_order_id': {order.id},"
             f"'user_plan_id': {user_plan.id},"
             f"'pricing_id': {pricing.id},"
             "}",
         )
         with self.assertRaisesRegex(Exception, "Received amount doesn't match"):
             receive_ipn(ipn)
+        user.userplan.refresh_from_db()
+        self.assertIsNone(user.userplan.recurring.amount)
+        self.assertIsNone(user.userplan.recurring.tax)
+        self.assertIsNone(user.userplan.recurring.token)
+        self.assertIsNone(user.userplan.recurring.payment_provider)
+        self.assertEqual(
+            user.userplan.recurring.renewal_triggered_by,
+            AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+        )
+        self.assertFalse(user.userplan.recurring.token_verified)
 
     def test_receive_ipn_cancellation(self):
         """
         Test cancellation IPN status.
         Should delete recurring plan.
         """
         user = baker.make("User", username="foobar")
```

### Comparing `django-plans-paypal-0.6.0/plans_paypal/tests/test_views.py` & `django-plans-paypal-0.7.0/plans_paypal/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/urls.py` & `django-plans-paypal-0.7.0/plans_paypal/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/plans_paypal/views.py` & `django-plans-paypal-0.7.0/plans_paypal/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             else settings.PAYPAL_BUSSINESS_EMAIL
         ),
         "a3": str(order.total()),  # monthly price
         "p3": period,  # duration of each unit (depends on unit)
         "t3": duration_unit,  # duration unit ("M for Month")
         "src": "1",  # make payments recur
         "sra": "1",  # reattempt payment on payment error
+        "srt": "52",  # reattempt count
         "no_note": "1",  # remove extra notes (optional)
         "item_name": f"{order.name} Order ID: {order.pk}",
         "notify_url": request.build_absolute_uri(reverse("paypal-ipn")),
         "return": request.build_absolute_uri(
             reverse("order_payment_success", kwargs={"pk": order_id})
         ),
         "cancel_return": request.build_absolute_uri(
@@ -111,9 +112,11 @@
     return render(request, "paypal_payments/payment.html", context)
 
 
 class PaymentFailureView(LoginRequiredMixin, View):
     def get(self, request, *args, order_id=None, payment_variant=None):
         order = get_object_or_404(Order, pk=order_id, user=request.user)
         order.status = Order.STATUS.CANCELED
+        # In case django-simple-history is installed
+        order._change_reason = "Django-payments-paypal: Payment failed by cancel view"
         order.save()
         return redirect(reverse("order_payment_failure", kwargs={"pk": order_id}))
```

### Comparing `django-plans-paypal-0.6.0/runtests.py` & `django-plans-paypal-0.7.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/setup.py` & `django-plans-paypal-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-paypal-0.6.0/tests/settings.py` & `django-plans-paypal-0.7.0/tests/settings.py`

 * *Files identical despite different names*

