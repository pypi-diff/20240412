# Comparing `tmp/django-plans-payments-1.2.2.tar.gz` & `tmp/django-plans-payments-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-payments-1.2.2.tar", last modified: Wed Dec 20 07:32:02 2023, max compression
+gzip compressed data, was "django-plans-payments-1.3.0.tar", last modified: Fri Apr 12 12:29:43 2024, max compression
```

## Comparing `django-plans-payments-1.2.2.tar` & `django-plans-payments-1.3.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/
--rw-rw-r--   0 petr      (1000) petr      (1000)      207 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.181259 django-plans-payments-1.2.2/.github/
--rw-rw-r--   0 petr      (1000) petr      (1000)      350 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.181259 django-plans-payments-1.2.2/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2770 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      158 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/AUTHORS.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3330 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/CONTRIBUTING.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1033 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/HISTORY.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      182 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1557 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)     4588 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2672 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/README.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.181259 django-plans-payments-1.2.2/django_plans_payments.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4588 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1855 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       29 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       15 2023-12-20 07:32:02.000000 django-plans-payments-1.2.2/django_plans_payments.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.181259 django-plans-payments-1.2.2/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/authors.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8443 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/contributing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       28 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/history.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/make.bat
--rw-rw-r--   0 petr      (1000) petr      (1000)       27 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/readme.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      452 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/docs/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      329 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      191 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/mypy.ini
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.181259 django-plans-payments-1.2.2/plans_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1695 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      122 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4514 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      424 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/0002_payment_transaction_fee.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      716 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/0003_auto_20201006_0855.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      513 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/0004_payment_billing_phone.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      633 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7619 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.177259 django-plans-payments-1.2.2/plans_payments/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/static/img/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3674 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/static/img/visa-logo.svg
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.177259 django-plans-payments-1.2.2/plans_payments/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)       49 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/mail/renew_cvv_3ds_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       36 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/mail/renew_cvv_3ds_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      197 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/plans/order_detail.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/templates/plans_payments/
--rw-rw-r--   0 petr      (1000) petr      (1000)       77 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/plans_payments/failure.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      217 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/plans_payments/payment.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      777 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/plans_payments/payment_buttons.html
--rw-rw-r--   0 petr      (1000) petr      (1000)       85 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templates/plans_payments/success.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/plans_payments/templatetags/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templatetags/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/templatetags/payment_buttons.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      385 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2717 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/plans_payments/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       86 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       34 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/requirements_dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      187 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/requirements_test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      575 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/runtests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      325 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/setup.cfg
--rwxrwxr-x   0 petr      (1000) petr      (1000)     2395 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/setup.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1872 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/tests/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)       49 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/templates/base.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:02.185259 django-plans-payments-1.2.2/tests/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)    10702 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3522 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      345 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tests/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      586 2023-12-20 07:32:01.000000 django-plans-payments-1.2.2/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      207 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/.github/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      350 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3278 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      161 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/AUTHORS.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3330 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/HISTORY.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1075 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      182 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1557 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/Makefile
+-rw-r--r--   0 petr      (1000) petr      (1000)     4871 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2790 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/README.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/django_plans_payments.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     4871 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1855 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       15 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/django_plans_payments.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6778 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/authors.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8443 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/contributing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/history.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      452 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6467 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/make.bat
+-rw-rw-r--   0 petr      (1000) petr      (1000)       27 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/readme.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/docs/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      329 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      191 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/mypy.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/plans_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1695 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      122 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/plans_payments/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4514 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      424 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/0002_payment_transaction_fee.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      716 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/0003_auto_20201006_0855.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      513 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/0004_payment_billing_phone.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      633 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7953 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.819961 django-plans-payments-1.3.0/plans_payments/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.823960 django-plans-payments-1.3.0/plans_payments/static/img/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3674 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/static/img/visa-logo.svg
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.819961 django-plans-payments-1.3.0/plans_payments/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/plans_payments/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/mail/renew_cvv_3ds_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       36 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/mail/renew_cvv_3ds_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/plans_payments/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      197 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/plans/order_detail.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/plans_payments/templates/plans_payments/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       77 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/plans_payments/failure.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      217 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/plans_payments/payment.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      777 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/plans_payments/payment_buttons.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)       85 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templates/plans_payments/success.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/plans_payments/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      353 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/templatetags/payment_buttons.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      385 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2717 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/plans_payments/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       93 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       34 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/requirements_dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      187 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/requirements_test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      575 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/runtests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      325 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/setup.cfg
+-rwxrwxr-x   0 petr      (1000) petr      (1000)     2402 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/setup.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1984 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/tests/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       49 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/templates/base.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.827959 django-plans-payments-1.3.0/tests/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)    14633 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3522 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      345 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tests/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      758 2024-04-12 12:29:43.000000 django-plans-payments-1.3.0/tox.ini
```

### Comparing `django-plans-payments-1.2.2/CONTRIBUTING.rst` & `django-plans-payments-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/HISTORY.rst` & `django-plans-payments-1.3.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 .. :changelog:
 
 History
 -------
 
+1.3.0 (2024-04-12)
+++++++++++++++++++
+
+* add optional returning orders when payments are refunded
+
 1.2.2 (2023-12-20)
 ++++++++++++++++++
 
 * add change_reason for django-simple-history
 
 1.2.1 (2023-12-19)
 ++++++++++++++++++
```

### Comparing `django-plans-payments-1.2.2/LICENSE` & `django-plans-payments-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/Makefile` & `django-plans-payments-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/PKG-INFO` & `django-plans-payments-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-payments
-Version: 1.2.2
+Version: 1.3.0
 Summary: Integration between django-plans and django-payments.
 Home-page: https://github.com/PetrDlouhy/django-plans-payments
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-payments
 Classifier: Development Status :: 3 - Alpha
@@ -17,30 +17,32 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-plans>=1.0.7
+Requires-Dist: django-payments
 
 =============================
 Django plans payments
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-payments.svg
     :target: https://badge.fury.io/py/django-plans-payments
 
-.. image:: https://travis-ci.org/PetrDlouhy/django-plans-payments.svg?branch=master
-    :target: https://travis-ci.org/PetrDlouhy/django-plans-payments
+.. image:: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml
 
 .. image:: https://codecov.io/gh/PetrDlouhy/django-plans-payments/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/PetrDlouhy/django-plans-payments
 
 Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-payments <https://github.com/mirumee/django-payments>`_.
-This will add payment buttons to the order page and automatically confirm the `Order` after the payment.
+This will add payment buttons to the order page and automatically confirm the `Order` after the payment. Optionally, it can return the corresponding order when a payment is refunded.
 
 Documentation
 -------------
 
 The full documentation is at https://django-plans-payments.readthedocs.io.
 
 Quickstart
@@ -113,14 +115,19 @@
 
 
 
 
 History
 -------
 
+1.3.0 (2024-04-12)
+++++++++++++++++++
+
+* add optional returning orders when payments are refunded
+
 1.2.2 (2023-12-20)
 ++++++++++++++++++
 
 * add change_reason for django-simple-history
 
 1.2.1 (2023-12-19)
 ++++++++++++++++++
```

### Comparing `django-plans-payments-1.2.2/README.rst` & `django-plans-payments-1.3.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 =============================
 Django plans payments
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-payments.svg
     :target: https://badge.fury.io/py/django-plans-payments
 
-.. image:: https://travis-ci.org/PetrDlouhy/django-plans-payments.svg?branch=master
-    :target: https://travis-ci.org/PetrDlouhy/django-plans-payments
+.. image:: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml
 
 .. image:: https://codecov.io/gh/PetrDlouhy/django-plans-payments/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/PetrDlouhy/django-plans-payments
 
 Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-payments <https://github.com/mirumee/django-payments>`_.
-This will add payment buttons to the order page and automatically confirm the `Order` after the payment.
+This will add payment buttons to the order page and automatically confirm the `Order` after the payment. Optionally, it can return the corresponding order when a payment is refunded.
 
 Documentation
 -------------
 
 The full documentation is at https://django-plans-payments.readthedocs.io.
 
 Quickstart
```

### Comparing `django-plans-payments-1.2.2/django_plans_payments.egg-info/PKG-INFO` & `django-plans-payments-1.3.0/django_plans_payments.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans-payments
-Version: 1.2.2
+Version: 1.3.0
 Summary: Integration between django-plans and django-payments.
 Home-page: https://github.com/PetrDlouhy/django-plans-payments
 Author: Petr Dlouhý
 Author-email: petr.dlouhy@email.cz
 License: MIT
 Keywords: django-plans-payments
 Classifier: Development Status :: 3 - Alpha
@@ -17,30 +17,32 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: django-plans>=1.0.7
+Requires-Dist: django-payments
 
 =============================
 Django plans payments
 =============================
 
 .. image:: https://badge.fury.io/py/django-plans-payments.svg
     :target: https://badge.fury.io/py/django-plans-payments
 
-.. image:: https://travis-ci.org/PetrDlouhy/django-plans-payments.svg?branch=master
-    :target: https://travis-ci.org/PetrDlouhy/django-plans-payments
+.. image:: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml/badge.svg
+    :target: https://github.com/PetrDlouhy/django-plans-payments/actions/workflows/main.yml
 
 .. image:: https://codecov.io/gh/PetrDlouhy/django-plans-payments/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/PetrDlouhy/django-plans-payments
 
 Almost automatic integration between `django-plans <https://github.com/django-getpaid/django-plans>`_ and `django-payments <https://github.com/mirumee/django-payments>`_.
-This will add payment buttons to the order page and automatically confirm the `Order` after the payment.
+This will add payment buttons to the order page and automatically confirm the `Order` after the payment. Optionally, it can return the corresponding order when a payment is refunded.
 
 Documentation
 -------------
 
 The full documentation is at https://django-plans-payments.readthedocs.io.
 
 Quickstart
@@ -113,14 +115,19 @@
 
 
 
 
 History
 -------
 
+1.3.0 (2024-04-12)
+++++++++++++++++++
+
+* add optional returning orders when payments are refunded
+
 1.2.2 (2023-12-20)
 ++++++++++++++++++
 
 * add change_reason for django-simple-history
 
 1.2.1 (2023-12-19)
 ++++++++++++++++++
```

### Comparing `django-plans-payments-1.2.2/django_plans_payments.egg-info/SOURCES.txt` & `django-plans-payments-1.3.0/django_plans_payments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/docs/Makefile` & `django-plans-payments-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/docs/conf.py` & `django-plans-payments-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/docs/make.bat` & `django-plans-payments-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/admin.py` & `django-plans-payments-1.3.0/plans_payments/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/migrations/0001_initial.py` & `django-plans-payments-1.3.0/plans_payments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/migrations/0003_auto_20201006_0855.py` & `django-plans-payments-1.3.0/plans_payments/migrations/0003_auto_20201006_0855.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/migrations/0004_payment_billing_phone.py` & `django-plans-payments-1.3.0/plans_payments/migrations/0004_payment_billing_phone.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py` & `django-plans-payments-1.3.0/plans_payments/migrations/0005_payment_plans_payme_status_9ad17d_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/models.py` & `django-plans-payments-1.3.0/plans_payments/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -148,22 +148,32 @@
     payment = kwargs["instance"]
     order = payment.order
     if payment.status == PaymentStatus.CONFIRMED:
         if hasattr(order.user.userplan, "recurring"):
             order.user.userplan.recurring.token_verified = True
             order.user.userplan.recurring.save()
         order.complete_order()
-    if order.status != Order.STATUS.COMPLETED and payment.status not in (
+    if (
+        getattr(settings, "PLANS_PAYMENTS_RETURN_ORDER_WHEN_PAYMENT_REFUNDED", False)
+        and payment.status == PaymentStatus.REFUNDED
+    ):
+        order._change_reason = (
+            f"Django-plans-payments: Payment status changed to {payment.status}"
+        )
+        order.return_order()
+    elif order.status != Order.STATUS.COMPLETED and payment.status not in (
         PaymentStatus.CONFIRMED,
         PaymentStatus.WAITING,
         PaymentStatus.INPUT,
     ):
         order.status = Order.STATUS.CANCELED
         # In case django-simples-history is installed
-        order._change_reason = f"Django-plans-payments: Payment status changed to {payment.status}"
+        order._change_reason = (
+            f"Django-plans-payments: Payment status changed to {payment.status}"
+        )
         order.save()
         if hasattr(order.user.userplan, "recurring"):
             order.user.userplan.recurring.token_verified = False
             order.user.userplan.recurring.save()
 
 
 @receiver(account_automatic_renewal)
```

### Comparing `django-plans-payments-1.2.2/plans_payments/static/img/visa-logo.svg` & `django-plans-payments-1.3.0/plans_payments/static/img/visa-logo.svg`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/templates/plans_payments/payment_buttons.html` & `django-plans-payments-1.3.0/plans_payments/templates/plans_payments/payment_buttons.html`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/plans_payments/views.py` & `django-plans-payments-1.3.0/plans_payments/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/runtests.py` & `django-plans-payments-1.3.0/runtests.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/setup.py` & `django-plans-payments-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     author_email="petr.dlouhy@email.cz",
     url="https://github.com/PetrDlouhy/django-plans-payments",
     packages=[
         "plans_payments",
     ],
     include_package_data=True,
     install_requires=[
-        "django-plans",
+        "django-plans>=1.0.7",
         "django-payments",
     ],
     license="MIT",
     zip_safe=False,
     keywords="django-plans-payments",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `django-plans-payments-1.2.2/tests/settings.py` & `django-plans-payments-1.3.0/tests/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8
 from typing import Dict, Tuple
 
+import django
+
 DEBUG = True
 USE_TZ = True
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "-#5o&sf4iu8&-@na$ad*(t)0gl6_gnw-7_=mk5!zcck)p0w&30"
 
 DATABASES = {
@@ -70,7 +72,10 @@
     "issuer_tax_number": "CZ 123 456 789",
 }
 PLANS_CURRENCY = "USD"
 PLANS_TAXATION_POLICY = "plans.taxation.eu.EUTaxationPolicy"
 PLANS_TAX_COUNTRY = "CZ"
 PLANS_DEFAULT_COUNTRY = "CZ"
 PLANS_GET_COUNTRY_FROM_IP = True
+
+if django.VERSION >= (4, 1):
+    FORM_RENDERER = "django.forms.renderers.DjangoDivFormRenderer"
```

### Comparing `django-plans-payments-1.2.2/tests/test_models.py` & `django-plans-payments-1.3.0/tests/test_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Tests for `django-plans-payments` models module.
 """
 import json
 from datetime import datetime
 from decimal import Decimal
 
 import pytz
-from django.test import TestCase
+from django.test import TestCase, override_settings
 from freezegun import freeze_time
 from model_bakery import baker
 from payments import PaymentStatus
 from plans.models import Invoice, Order
 
 from plans_payments import models
 
@@ -204,25 +204,27 @@
         self.assertEqual(userplan.recurring.card_masked_number, "1234")
         self.assertEqual(userplan.recurring.has_automatic_renewal, True)
 
     def test_change_payment_status(self):
         p = models.Payment(order=baker.make("Order", status=Order.STATUS.NEW))
         models.change_payment_status("sender", instance=p)
         self.assertEqual(p.status, "waiting")
+        self.assertEqual(p.order.status, Order.STATUS.NEW)
 
     def test_change_payment_status_confirmed(self):
         p = models.Payment(
             order=baker.make("Order", status=Order.STATUS.NEW),
             status=PaymentStatus.CONFIRMED,
         )
         userplan = baker.make("UserPlan", user=p.order.user)
         recurring_user_plan = baker.make("RecurringUserPlan", user_plan=userplan)
         models.change_payment_status("sender", instance=p)
         self.assertEqual(p.status, "confirmed")
         self.assertEqual(recurring_user_plan.token_verified, True)
+        self.assertEqual(p.order.status, Order.STATUS.COMPLETED)
 
     @freeze_time("2018-01-01")
     def test_change_payment_status_confirmed_double_submit(self):
         """Test double submit of payment status_changed signal"""
         p = models.Payment(
             order=baker.make("Order", status=Order.STATUS.NEW),
             status=PaymentStatus.CONFIRMED,
@@ -247,23 +249,104 @@
             order=baker.make("Order", status=Order.STATUS.NEW),
             status=PaymentStatus.REJECTED,
         )
         userplan = baker.make("UserPlan", user=p.order.user)
         baker.make("RecurringUserPlan", user_plan=userplan)
         models.change_payment_status("sender", instance=p)
         self.assertEqual(p.status, "rejected")
+        self.assertEqual(p.order.status, Order.STATUS.CANCELED)
+
+    def test_change_payment_status_rejected_order_completed(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.COMPLETED),
+            status=PaymentStatus.REJECTED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "rejected")
+        self.assertEqual(p.order.status, Order.STATUS.COMPLETED)
+
+    def test_change_payment_status_refunded(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.COMPLETED),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.COMPLETED)
+
+    @override_settings(PLANS_PAYMENTS_RETURN_ORDER_WHEN_PAYMENT_REFUNDED=True)
+    def test_change_payment_status_refunded_return_enabled(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.COMPLETED),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.RETURNED)
+
+    def test_change_payment_status_refunded_order_not_valid(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.NOT_VALID),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.CANCELED)
+
+    @override_settings(PLANS_PAYMENTS_RETURN_ORDER_WHEN_PAYMENT_REFUNDED=True)
+    def test_change_payment_status_refunded_order_not_valid_return_enabled(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.NOT_VALID),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.RETURNED)
+
+    # This should not happen practically but with Django Admin, anything can happen...
+    def test_change_payment_status_refunded_order_canceled(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.CANCELED),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.CANCELED)
+
+    # This should not happen practically but with Django Admin, anything can happen...
+    @override_settings(PLANS_PAYMENTS_RETURN_ORDER_WHEN_PAYMENT_REFUNDED=True)
+    def test_change_payment_status_refunded_order_canceled_return_enabled(self):
+        p = models.Payment(
+            order=baker.make("Order", status=Order.STATUS.CANCELED),
+            status=PaymentStatus.REFUNDED,
+        )
+        baker.make("UserPlan", user=p.order.user)
+        with self.assertRaisesRegex(
+            ValueError,
+            r"^Cannot return order with status other than COMPLETED and NOT_VALID: 4$",
+        ):
+            models.change_payment_status("sender", instance=p)
+        self.assertEqual(p.status, "refunded")
+        self.assertEqual(p.order.status, Order.STATUS.CANCELED)
 
     def test_change_payment_status_confirmed_no_recurring(self):
         p = models.Payment(
             order=baker.make("Order", status=Order.STATUS.NEW),
             status=PaymentStatus.CONFIRMED,
         )
         baker.make("UserPlan", user=p.order.user)
         models.change_payment_status("sender", instance=p)
         self.assertEqual(p.status, "confirmed")
+        self.assertEqual(p.order.status, Order.STATUS.COMPLETED)
 
     def test_renew_accounts_no_variant(self):
         p = models.Payment()
         user = baker.make("User")
         userplan = baker.make("UserPlan", user=user)
         baker.make("RecurringUserPlan", user_plan=userplan)
         models.renew_accounts("sender", user, p)
```

### Comparing `django-plans-payments-1.2.2/tests/test_views.py` & `django-plans-payments-1.3.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-payments-1.2.2/tox.ini` & `django-plans-payments-1.3.0/tox.ini`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 [tox]
 envlist =
     py{310,39,38}
-    py{310,39,38}-dj{40,41},
+    py{312,311,310}-dj50,
+    py{312,311,310,39,38}-dj42,
+    py{311,310,39,38}-dj41,
+    py{310,39,38}-dj40,
     py{310,39,38,37,36}-dj32,
-    py{39,38,37,36}-dj{30,31},
-    py{38,37,36,35}-dj{20,21,22},
+    py{39,38,37,36}-dj31,
 
 [testenv]
 setenv =
     PYTHONPATH = {toxinidir}:{toxinidir}/plans_payments
 commands =
+    python --version
+    python manage.py --version
     python -W error::DeprecationWarning -m coverage run manage.py test
 deps =
-    django-31: Django>=3.1,<3.2
-    django-32: Django>=3.2,<3.3
-    django-40: Django>=4.0,<4.1
-    django-41: Django>=4.1,<4.2
     -r{toxinidir}/requirements_test.txt
+    dj31: Django>=3.1,<3.2
+    dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
+    dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
+    dj50: Django>=5.0,<5.1
 basepython =
     py37: python3.7
     py38: python3.8
     py39: python3.9
     py310: python3.10
+    py311: python3.11
+    py312: python3.12
```

