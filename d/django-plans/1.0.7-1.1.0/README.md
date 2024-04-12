# Comparing `tmp/django-plans-1.0.7.tar.gz` & `tmp/django-plans-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-1.0.7.tar", last modified: Tue Apr  9 10:06:48 2024, max compression
+gzip compressed data, was "django-plans-1.1.0.tar", last modified: Fri Apr 12 12:33:50 2024, max compression
```

## Comparing `django-plans-1.0.7.tar` & `django-plans-1.1.0.tar`

### file list

```diff
@@ -1,286 +1,288 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-09 10:06:47.000000 django-plans-1.0.7/.coveragerc
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.979654 django-plans-1.0.7/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2024-04-09 10:06:47.000000 django-plans-1.0.7/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      343 2024-04-09 10:06:47.000000 django-plans-1.0.7/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      616 2024-04-09 10:06:47.000000 django-plans-1.0.7/.travis.yml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/.tx/
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/.tx/config
--rw-rw-r--   0 petr      (1000) petr      (1000)       83 2024-04-09 10:06:47.000000 django-plans-1.0.7/AUTHORS
--rw-rw-r--   0 petr      (1000) petr      (1000)     5506 2024-04-09 10:06:47.000000 django-plans-1.0.7/CHANGELOG
--rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2024-04-09 10:06:47.000000 django-plans-1.0.7/CODE_OF_CONDUCT.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-04-09 10:06:47.000000 django-plans-1.0.7/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/MANIFEST.in
--rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-09 10:06:48.011654 django-plans-1.0.7/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2024-04-09 10:06:47.000000 django-plans-1.0.7/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2024-04-09 10:06:47.000000 django-plans-1.0.7/conftest.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/fixtures/initial_data.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/forms.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      279 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/foo/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/foo/templates/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)      591 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_confirm_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_form.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/templates/foo/foo_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      402 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/foo/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.987654 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      378 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      603 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      904 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      495 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      804 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      858 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      693 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_plans.json
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      119 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      117 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      116 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    30867 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/sample_plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.991654 django-plans-1.0.7/demo/example/sample_plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/sample_plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      744 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/templates/plans/upgrade.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/sample_plans/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/css/example.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/demo/example/static/img/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/static/img/messages/
--rw-rw-r--   0 petr      (1000) petr      (1000)      294 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_alert.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_error.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/static/img/messages/icon_success.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      823 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/home.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      757 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/plans/billing_info_update.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/demo/example/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)      718 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      605 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/example/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/fabfile.py
--rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/demo/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/django_plans.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     8397 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-09 10:06:47.000000 django-plans-1.0.7/django_plans.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.995654 django-plans-1.0.7/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.999654 django-plans-1.0.7/docs/source/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/docs/source/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.999654 django-plans-1.0.7/docs/source/_static/images/
--rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-1.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-2.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/_static/images/django-plans-3.png
--rw-rw-r--   0 petr      (1000) petr      (1000)      860 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/caveats.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/customize_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1703 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/integration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/invoicing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_change.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      847 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_expiration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2246 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/plans_recurrence.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/quota_validators.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/south.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/taxation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2024-04-09 10:06:47.000000 django-plans-1.0.7/docs/source/templating.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      296 2024-04-09 10:06:47.000000 django-plans-1.0.7/fabfile.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9052 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      277 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/base/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/base/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    46940 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/base/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      273 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/context_processors.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/contrib.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/enumeration.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/fixtures/test_django-plans_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/forms.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      351 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/importer.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/listeners.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.003654 django-plans-1.0.7/plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      930 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      417 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      291 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      890 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0002_auto_20180901_1744.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0003_make_plans_unique.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      480 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0004_create_user_plans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0005_recurring_payments.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      665 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0006_auto_20200504_1541.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0007_recurringuserplan_card_masked_number.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      625 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0008_recurringuserplan_token_verified.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      456 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0009_auto_20210303_1134.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0010_auto_20220113_1317.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0011_auto_20220208_1344.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      531 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/0012_planpricing_visible.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/mixins.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/plan_change.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/quota.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/signals.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2079 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/taxation/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/eu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/taxation/ru.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.983654 django-plans-1.0.7/plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.007654 django-plans-1.0.7/plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/templates/plans/upgrade.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)       29 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2213 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/test_autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    58966 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/tests/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:48.011654 django-plans-1.0.7/plans_i18n/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      815 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       65 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      764 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/translation.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       26 2024-04-09 10:06:47.000000 django-plans-1.0.7/plans_i18n/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      371 2024-04-09 10:06:48.011654 django-plans-1.0.7/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2024-04-09 10:06:47.000000 django-plans-1.0.7/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      624 2024-04-09 10:06:47.000000 django-plans-1.0.7/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-12 12:33:50.000000 django-plans-1.1.0/.coveragerc
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2024-04-12 12:33:50.000000 django-plans-1.1.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      343 2024-04-12 12:33:50.000000 django-plans-1.1.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      616 2024-04-12 12:33:50.000000 django-plans-1.1.0/.travis.yml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/.tx/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/.tx/config
+-rw-rw-r--   0 petr      (1000) petr      (1000)       83 2024-04-12 12:33:50.000000 django-plans-1.1.0/AUTHORS
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6906 2024-04-12 12:33:50.000000 django-plans-1.1.0/CHANGELOG
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2024-04-12 12:33:50.000000 django-plans-1.1.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-04-12 12:33:50.000000 django-plans-1.1.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/MANIFEST.in
+-rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-12 12:33:50.937353 django-plans-1.1.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2024-04-12 12:33:50.000000 django-plans-1.1.0/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2024-04-12 12:33:50.000000 django-plans-1.1.0/conftest.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/demo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/fixtures/initial_data.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/forms.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      279 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/foo/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/templates/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      591 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_confirm_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_form.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      402 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      378 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      603 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      904 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      495 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      804 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      858 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      693 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      119 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      117 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      116 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    31516 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/sample_plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      744 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/upgrade.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/css/example.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/static/img/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/static/img/messages/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      294 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_alert.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_error.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_success.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      823 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/home.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      757 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/billing_info_update.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      718 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      605 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/fabfile.py
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/django_plans.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8584 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/source/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/docs/source/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/source/_static/images/
+-rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-1.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-2.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-3.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)      860 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/caveats.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/customize_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1703 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/integration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/invoicing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_change.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      847 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_expiration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2417 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_recurrence.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/quota_validators.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/south.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/taxation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/templating.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      296 2024-04-12 12:33:50.000000 django-plans-1.1.0/fabfile.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9022 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      277 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/base/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/base/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    50345 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/base/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      273 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/context_processors.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/contrib.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/enumeration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/forms.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      351 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/importer.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/listeners.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      930 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      417 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      291 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      890 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0002_auto_20180901_1744.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0003_make_plans_unique.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      480 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0004_create_user_plans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0005_recurring_payments.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      665 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0006_auto_20200504_1541.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0007_recurringuserplan_card_masked_number.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      625 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0008_recurringuserplan_token_verified.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      456 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0009_auto_20210303_1134.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0010_auto_20220113_1317.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0011_auto_20220208_1344.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      531 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0012_planpricing_visible.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1457 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3085 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/mixins.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/plan_change.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/quota.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/signals.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2176 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/taxation/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/eu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/ru.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/upgrade.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       29 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3309 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/test_autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    68912 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans_i18n/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      815 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       65 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      764 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/translation.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       26 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      371 2024-04-12 12:33:50.937353 django-plans-1.1.0/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2024-04-12 12:33:50.000000 django-plans-1.1.0/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      624 2024-04-12 12:33:50.000000 django-plans-1.1.0/tox.ini
```

### Comparing `django-plans-1.0.7/.coveragerc` & `django-plans-1.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/.github/workflows/main.yml` & `django-plans-1.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/.travis.yml` & `django-plans-1.1.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/CODE_OF_CONDUCT.md` & `django-plans-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/LICENSE` & `django-plans-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/PKG-INFO` & `django-plans-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.0.7
+Version: 1.1.0
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-plans-1.0.7/README.rst` & `django-plans-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/conftest.py` & `django-plans-1.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/fixtures/initial_data.json` & `django-plans-1.1.0/demo/example/foo/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/migrations/0001_initial.py` & `django-plans-1.1.0/demo/example/foo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/templates/foo/foo_confirm_delete.html` & `django-plans-1.1.0/demo/example/foo/templates/foo/foo_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/templates/foo/foo_form.html` & `django-plans-1.1.0/demo/example/foo/templates/foo/foo_form.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/templates/foo/foo_list.html` & `django-plans-1.1.0/demo/example/foo/templates/foo/foo_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/foo/views.py` & `django-plans-1.1.0/demo/example/foo/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/en/LC_MESSAGES/django.po` & `django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/fixtures/initial_plan.json` & `django-plans-1.1.0/demo/example/sample_plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_auth.json` & `django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/fixtures/test_django-plans_plans.json` & `django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/migrations/0001_initial.py` & `django-plans-1.1.0/demo/example/sample_plans/migrations/0001_initial.py`

 * *Files 7% similar despite different names*

```diff
@@ -331,16 +331,27 @@
                         max_digits=4,
                         null=True,
                         verbose_name="tax",
                     ),
                 ),
                 ("currency", models.CharField(max_length=3, verbose_name="currency")),
                 (
-                    "has_automatic_renewal",
+                    "renewal_triggered_by",
+                    models.IntegerField(
+                        choices=[(1, "other"), (2, "user"), (3, "task")],
+                        db_index=True,
+                        default=2,
+                        help_text="The source of the associated plan's renewal (USER = user-initiated renewal, TASK = autorenew_account-task-initiated renewal, OTHER = renewal is triggered using another mechanism).",
+                        verbose_name="renewal triggered by",
+                    ),
+                ),
+                (
+                    "_has_automatic_renewal_backup_deprecated",
                     models.BooleanField(
+                        db_column="has_automatic_renewal",
                         default=False,
                         help_text="Automatic renewal is enabled for associated plan. If False, the plan renewal can be still initiated by user.",
                         verbose_name="has automatic plan renewal",
                     ),
                 ),
                 (
                     "token_verified",
```

### Comparing `django-plans-1.0.7/demo/example/sample_plans/models.py` & `django-plans-1.1.0/demo/example/sample_plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/mail/change_plan_body.txt` & `django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/mail/expired_account_body.txt` & `django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/mail/extend_account_body.txt` & `django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/mail/remind_expire_body.txt` & `django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/account_activation.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/billing_info_update.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/create_order.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/current.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/expiration_messages.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/extend.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_detail_table.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/order_list.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/pagination.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/templates/plans/plan_table.html` & `django-plans-1.1.0/demo/example/sample_plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/sample_plans/tests.py` & `django-plans-1.1.0/demo/example/sample_plans/tests.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/settings.py` & `django-plans-1.1.0/demo/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/static/css/example.css` & `django-plans-1.1.0/demo/example/static/css/example.css`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/static/img/messages/icon_error.png` & `django-plans-1.1.0/demo/example/static/img/messages/icon_error.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/static/img/messages/icon_success.png` & `django-plans-1.1.0/demo/example/static/img/messages/icon_success.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/templates/base.html` & `django-plans-1.1.0/demo/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/templates/home.html` & `django-plans-1.1.0/demo/example/templates/home.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/templates/plans/billing_info_create.html` & `django-plans-1.1.0/demo/example/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/templates/plans/billing_info_update.html` & `django-plans-1.1.0/demo/example/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/templates/registration/login.html` & `django-plans-1.1.0/demo/example/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/urls.py` & `django-plans-1.1.0/demo/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/example/wsgi.py` & `django-plans-1.1.0/demo/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/demo/manage.py` & `django-plans-1.1.0/demo/manage.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/django_plans.egg-info/PKG-INFO` & `django-plans-1.1.0/django_plans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.0.7
+Version: 1.1.0
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
```

### Comparing `django-plans-1.0.7/django_plans.egg-info/SOURCES.txt` & `django-plans-1.1.0/django_plans.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,16 @@
 plans/migrations/0006_auto_20200504_1541.py
 plans/migrations/0007_recurringuserplan_card_masked_number.py
 plans/migrations/0008_recurringuserplan_token_verified.py
 plans/migrations/0009_auto_20210303_1134.py
 plans/migrations/0010_auto_20220113_1317.py
 plans/migrations/0011_auto_20220208_1344.py
 plans/migrations/0012_planpricing_visible.py
+plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py
+plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py
 plans/migrations/__init__.py
 plans/taxation/__init__.py
 plans/taxation/eu.py
 plans/taxation/ru.py
 plans/templates/mail/change_plan_body.txt
 plans/templates/mail/change_plan_title.txt
 plans/templates/mail/expired_account_body.txt
```

### Comparing `django-plans-1.0.7/docs/Makefile` & `django-plans-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/_static/images/django-plans-1.png` & `django-plans-1.1.0/docs/source/_static/images/django-plans-1.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/_static/images/django-plans-2.png` & `django-plans-1.1.0/docs/source/_static/images/django-plans-2.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/_static/images/django-plans-3.png` & `django-plans-1.1.0/docs/source/_static/images/django-plans-3.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/caveats.rst` & `django-plans-1.1.0/docs/source/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/conf.py` & `django-plans-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/customize_models.rst` & `django-plans-1.1.0/docs/source/customize_models.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/index.rst` & `django-plans-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/installation.rst` & `django-plans-1.1.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/integration.rst` & `django-plans-1.1.0/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/invoicing.rst` & `django-plans-1.1.0/docs/source/invoicing.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/plans.rst` & `django-plans-1.1.0/docs/source/plans.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/plans_change.rst` & `django-plans-1.1.0/docs/source/plans_change.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/plans_expiration.rst` & `django-plans-1.1.0/docs/source/plans_expiration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/plans_recurrence.rst` & `django-plans-1.1.0/docs/source/plans_recurrence.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Plans recurrence and automatic renewal
 ======================================
 
 To support renewal of plans, use ``RecurringUserPlan`` model to store information about the recurrence.
 
-The plans can be renewed automatically, or the ``RecurringUserPlan`` information can be used only to store information for one-click user initiated renewal (with ``automatic_renewal=False``).
+The plans can be renewed automatically using this app, the ``RecurringUserPlan`` information can be used only to store information for one-click user initiated renewal (with ``renewal_triggered_by=USER``), or the ``RecurringUserPlan`` can indicate that another mechanism is used to automatically renew the plans (``renewal_triggered_by=OTHER``).
 
-For plans, that should be renewed automatically fill in information about the recurrence::
+For plans, that should be renewed automatically using this app fill in information about the recurrence::
 
    self.order.user.userplan.set_plan_renewal(
        order=self.order,
-       automatic_renewal=True,
+       renewal_triggered_by=TASK,
        ...
        # Not required
        payment_provider='FooProvider',
        token=token,
        card_expire_year=card_expire_year,
        card_expire_month=card_expire_month,
        ...
    )
 
-Then all active ``UserPlan`` with ``RecurringUserPlan.has_automatic_renewal=True`` will be picked by ``autorenew_account`` task, that will send ``account_automatic_renewal`` signal.
+Then all active ``UserPlan`` with ``RecurringUserPlan.renewal_triggered_by=TASK`` will be picked by ``autorenew_account`` task, that will send ``account_automatic_renewal`` signal.
 This signal can be used for your implementation of automatic plan renewal. You should implement following steps::
 
    @receiver(account_automatic_renewal)
    def renew_accounts(sender, user, *args, **kwargs):
        order = user.userplan.recurring.create_renew_order()
 
        ...
```

### Comparing `django-plans-1.0.7/docs/source/quota_validators.rst` & `django-plans-1.1.0/docs/source/quota_validators.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/settings.rst` & `django-plans-1.1.0/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/south.rst` & `django-plans-1.1.0/docs/source/south.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/taxation.rst` & `django-plans-1.1.0/docs/source/taxation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/docs/source/templating.rst` & `django-plans-1.1.0/docs/source/templating.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/admin.py` & `django-plans-1.1.0/plans/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -257,26 +257,26 @@
 class UserPlanAdmin(UserLinkMixin, admin.ModelAdmin):
     list_filter = (
         "active",
         "expire",
         "plan__name",
         "plan__available",
         "plan__visible",
-        "recurring__has_automatic_renewal",
+        "recurring__renewal_triggered_by",
         "recurring__payment_provider",
         "recurring__token_verified",
         "recurring__pricing",
     )
     search_fields = ("user__username", "user__email", "plan__name", "recurring__token")
     list_display = (
         "user",
         "plan",
         "expire",
         "active",
-        "recurring__automatic_renewal",
+        "recurring__renewal_triggered_by",
         "recurring__token_verified",
         "recurring__payment_provider",
         "recurring__pricing",
     )
     list_display_links = list_display
     list_select_related = True
     readonly_fields = ("user_link", "created", "updated_at")
@@ -286,20 +286,21 @@
     ]
     fields = ("user", "user_link", "plan", "expire", "active", "created", "updated_at")
     raw_id_fields = [
         "user",
         "plan",
     ]
 
-    def recurring__automatic_renewal(self, obj):
-        return obj.recurring.has_automatic_renewal
+    def recurring__renewal_triggered_by(self, obj):
+        return obj.recurring.renewal_triggered_by
 
-    recurring__automatic_renewal.admin_order_field = "recurring__has_automatic_renewal"
-    recurring__automatic_renewal.boolean = True
-    recurring__automatic_renewal.short_description = "Automatic renewal"
+    recurring__renewal_triggered_by.admin_order_field = (
+        "recurring__renewal_triggered_by"
+    )
+    recurring__renewal_triggered_by.short_description = "Renewal triggered by"
 
     def recurring__token_verified(self, obj):
         return obj.recurring.token_verified
 
     recurring__token_verified.admin_order_field = "recurring__token_verified"
     recurring__token_verified.boolean = True
     recurring__token_verified.short_description = "Renewal token verified"
@@ -309,15 +310,15 @@
 
     recurring__payment_provider.admin_order_field = "recurring__payment_provider"
     recurring__payment_provider.short_description = "Renewal payment_provider"
 
     def recurring__pricing(self, obj):
         return obj.recurring.pricing
 
-    recurring__automatic_renewal.admin_order_field = "recurring__pricing"
+    recurring__pricing.admin_order_field = "recurring__pricing"
 
 
 admin.site.register(Quota, QuotaAdmin)
 admin.site.register(Plan, PlanAdmin)
 admin.site.register(UserPlan, UserPlanAdmin)
 admin.site.register(Pricing)
 admin.site.register(Order, OrderAdmin)
```

### Comparing `django-plans-1.0.7/plans/base/models.py` & `django-plans-1.1.0/plans/base/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import unicode_literals
 
 import logging
 import re
+import warnings
 from datetime import date, timedelta
 from decimal import Decimal
 
 import stdnum.eu.vat
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import models, transaction
@@ -295,15 +296,16 @@
         if not self.is_expired() and self.expire is not None and self.plan == plan:
             return self.expire
         return date.today()
 
     def has_automatic_renewal(self):
         return (
             hasattr(self, "recurring")
-            and self.recurring.has_automatic_renewal
+            and self.recurring.renewal_triggered_by
+            != self.recurring.RENEWAL_TRIGGERED_BY.USER
             and self.recurring.token_verified
         )
 
     def get_plan_extended_until(self, plan, pricing):
         if plan.is_free():
             return None
         if pricing is None:
@@ -328,32 +330,59 @@
             plans_autorenew_before_hours = getattr(
                 settings, "PLANS_AUTORENEW_BEFORE_HOURS", 0
             )
             return self.expire - timedelta(
                 days=plans_autorenew_before_days, hours=plans_autorenew_before_hours
             )
 
-    def set_plan_renewal(self, order, has_automatic_renewal=True, **kwargs):
+    def set_plan_renewal(
+        self,
+        order,
+        # TODO: has_automatic_renewal deprecated. Remove in the next major release.
+        has_automatic_renewal=None,
+        # TODO: renewal_triggered_by=None deprecated. Set to TASK in the next major release.
+        renewal_triggered_by=None,
+        **kwargs,
+    ):
         """
         Creates or updates plan renewal information for this userplan with given order
         """
         if not hasattr(self, "recurring"):
             self.recurring = AbstractRecurringUserPlan.get_concrete_model()()
 
+        if has_automatic_renewal is None and renewal_triggered_by is None:
+            has_automatic_renewal = True
+        if has_automatic_renewal is not None:
+            warnings.warn(
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+                DeprecationWarning,
+            )
+        if renewal_triggered_by is None:
+            warnings.warn(
+                "renewal_triggered_by=None is deprecated. "
+                "Set an AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY instead.",
+                DeprecationWarning,
+            )
+            renewal_triggered_by = (
+                self.recurring.RENEWAL_TRIGGERED_BY.TASK
+                if has_automatic_renewal
+                else self.recurring.RENEWAL_TRIGGERED_BY.USER
+            )
+
         # Erase values of all fields
         # We don't want to mix the old and new values
         self.recurring.set_all_fields_default()
 
         # Set new values
         self.recurring.user_plan = self
         self.recurring.pricing = order.pricing
         self.recurring.amount = order.amount
         self.recurring.tax = order.tax
         self.recurring.currency = order.currency
-        self.recurring.has_automatic_renewal = has_automatic_renewal
+        self.recurring.renewal_triggered_by = renewal_triggered_by
         for k, v in kwargs.items():
             setattr(self.recurring, k, v)
         self.recurring.save()
         return self.recurring
 
     def extend_account(self, plan, pricing):
         """
@@ -505,14 +534,22 @@
 
 class AbstractRecurringUserPlan(BaseMixin, models.Model):
     """
     OneToOne model associated with UserPlan that stores information about the plan recurrence.
     More about recurring payments in docs.
     """
 
+    RENEWAL_TRIGGERED_BY = Enumeration(
+        [
+            (1, "OTHER", pgettext_lazy("Renewal triggered by", "other")),
+            (2, "USER", pgettext_lazy("Renewal triggered by", "user")),
+            (3, "TASK", pgettext_lazy("Renewal triggered by", "task")),
+        ]
+    )
+
     user_plan = models.OneToOneField(
         "UserPlan", on_delete=models.CASCADE, related_name="recurring"
     )
     token = models.CharField(
         _("recurring token"),
         help_text=_(
             "Token, that will be used for payment renewal. Depends on used payment provider"
@@ -546,20 +583,34 @@
         null=True,
         blank=True,
     )
     tax = models.DecimalField(
         _("tax"), max_digits=4, decimal_places=2, db_index=True, null=True, blank=True
     )  # Tax=None is when tax is not applicable
     currency = models.CharField(_("currency"), max_length=3)
-    has_automatic_renewal = models.BooleanField(
+    renewal_triggered_by = models.IntegerField(
+        _("renewal triggered by"),
+        choices=RENEWAL_TRIGGERED_BY,
+        help_text=_(
+            "The source of the associated plan's renewal (USER = user-initiated renewal, "
+            "TASK = autorenew_account-task-initiated renewal, OTHER = renewal is triggered using another mechanism)."
+        ),
+        default=RENEWAL_TRIGGERED_BY.USER,
+        db_index=True,
+    )
+    # A backup of the old has_automatic_renewal field to support data migration to the new renewal_triggered_by field.
+    # Do not make any other modifications to the field in order to let user's auto-migrations detect the renaming.
+    # TODO: _has_automatic_renewal_backup_deprecated deprecated. Remove in the next major release.
+    _has_automatic_renewal_backup_deprecated = models.BooleanField(
         _("has automatic plan renewal"),
         help_text=_(
             "Automatic renewal is enabled for associated plan. "
             "If False, the plan renewal can be still initiated by user.",
         ),
+        db_column="has_automatic_renewal",
         default=False,
     )
     token_verified = models.BooleanField(
         _("token has been verified by payment"),
         help_text=_(
             "The recurring token has been verified by at least one payment to be working.",
         ),
@@ -568,14 +619,43 @@
     card_expire_year = models.IntegerField(null=True, blank=True)
     card_expire_month = models.IntegerField(null=True, blank=True)
     card_masked_number = models.CharField(null=True, blank=True, max_length=255)
 
     class Meta:
         abstract = True
 
+    # TODO: has_automatic_renewal deprecated. Remove in the next major release.
+    @property
+    def has_automatic_renewal(self):
+        warnings.warn(
+            "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            DeprecationWarning,
+        )
+        return self.renewal_triggered_by != self.RENEWAL_TRIGGERED_BY.USER
+
+    # TODO: has_automatic_renewal deprecated. Remove in the next major release.
+    @has_automatic_renewal.setter
+    def has_automatic_renewal(self, value):
+        warnings.warn(
+            "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            DeprecationWarning,
+        )
+        self.renewal_triggered_by = (
+            self.RENEWAL_TRIGGERED_BY.TASK if value else self.RENEWAL_TRIGGERED_BY.USER
+        )
+
+    # TODO: has_automatic_renewal deprecated. Remove in the next major release.
+    @has_automatic_renewal.deleter
+    def has_automatic_renewal(self):
+        warnings.warn(
+            "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            DeprecationWarning,
+        )
+        del self.renewal_triggered_by
+
     def create_renew_order(self):
         """
         Create order for plan renewal
         """
         userplan = self.user_plan
         order = AbstractOrder.get_concrete_model().objects.create(
             user=userplan.user,
@@ -601,15 +681,15 @@
         """
         self.token = None
         self.payment_provider = None
         self.pricing = None
         self.amount = None
         self.tax = None
         self.currency = None
-        self.has_automatic_renewal = False
+        self.renewal_triggered_by = self.RENEWAL_TRIGGERED_BY.USER
         self.token_verified = False
         self.card_expire_year = None
         self.card_expire_month = None
         self.card_masked_number = None
 
 
 class AbstractPricing(BaseMixin, models.Model):
```

### Comparing `django-plans-1.0.7/plans/context_processors.py` & `django-plans-1.1.0/plans/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/contrib.py` & `django-plans-1.1.0/plans/contrib.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/enumeration.py` & `django-plans-1.1.0/plans/enumeration.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/fixtures/initial_plan.json` & `django-plans-1.1.0/plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/fixtures/test_django-plans_auth.json` & `django-plans-1.1.0/plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/fixtures/test_django-plans_plans.json` & `django-plans-1.1.0/plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/forms.py` & `django-plans-1.1.0/plans/forms.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/listeners.py` & `django-plans-1.1.0/plans/listeners.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/en/LC_MESSAGES/django.po` & `django-plans-1.1.0/plans/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.mo` & `django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/management/commands/autorenew_accounts.py` & `django-plans-1.1.0/plans/management/commands/autorenew_accounts.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0001_initial.py` & `django-plans-1.1.0/plans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0002_auto_20180901_1744.py` & `django-plans-1.1.0/plans/migrations/0002_auto_20180901_1744.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0003_make_plans_unique.py` & `django-plans-1.1.0/plans/migrations/0003_make_plans_unique.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0005_recurring_payments.py` & `django-plans-1.1.0/plans/migrations/0005_recurring_payments.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0006_auto_20200504_1541.py` & `django-plans-1.1.0/plans/migrations/0006_auto_20200504_1541.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0008_recurringuserplan_token_verified.py` & `django-plans-1.1.0/plans/migrations/0008_recurringuserplan_token_verified.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0010_auto_20220113_1317.py` & `django-plans-1.1.0/plans/migrations/0010_auto_20220113_1317.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0011_auto_20220208_1344.py` & `django-plans-1.1.0/plans/migrations/0011_auto_20220208_1344.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/migrations/0012_planpricing_visible.py` & `django-plans-1.1.0/plans/migrations/0012_planpricing_visible.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/mixins.py` & `django-plans-1.1.0/plans/mixins.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/models.py` & `django-plans-1.1.0/plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/plan_change.py` & `django-plans-1.1.0/plans/plan_change.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/signals.py` & `django-plans-1.1.0/plans/signals.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/tasks.py` & `django-plans-1.1.0/plans/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import logging
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 
+from .base.models import AbstractRecurringUserPlan
 from .signals import account_automatic_renewal
 
 User = get_user_model()
 logger = logging.getLogger("plans.tasks")
 
 
 def get_active_plans():
@@ -20,15 +21,15 @@
 
 def autorenew_account(providers=None):
     logger.info("Started automatic account renewal")
     PLANS_AUTORENEW_BEFORE_DAYS = getattr(settings, "PLANS_AUTORENEW_BEFORE_DAYS", 0)
     PLANS_AUTORENEW_BEFORE_HOURS = getattr(settings, "PLANS_AUTORENEW_BEFORE_HOURS", 0)
 
     accounts_for_renewal = get_active_plans().filter(
-        userplan__recurring__has_automatic_renewal=True,
+        userplan__recurring__renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
         userplan__recurring__token_verified=True,
         userplan__expire__lt=datetime.date.today()
         + datetime.timedelta(
             days=PLANS_AUTORENEW_BEFORE_DAYS, hours=PLANS_AUTORENEW_BEFORE_HOURS
         ),
     )
```

### Comparing `django-plans-1.0.7/plans/taxation/__init__.py` & `django-plans-1.1.0/plans/taxation/__init__.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/taxation/eu.py` & `django-plans-1.1.0/plans/taxation/eu.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/taxation/ru.py` & `django-plans-1.1.0/plans/taxation/ru.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/mail/change_plan_body.txt` & `django-plans-1.1.0/plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/mail/expired_account_body.txt` & `django-plans-1.1.0/plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/mail/extend_account_body.txt` & `django-plans-1.1.0/plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/mail/remind_expire_body.txt` & `django-plans-1.1.0/plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/account_activation.html` & `django-plans-1.1.0/plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.1.0/plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/create_order.html` & `django-plans-1.1.0/plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/current.html` & `django-plans-1.1.0/plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/expiration_messages.html` & `django-plans-1.1.0/plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/extend.html` & `django-plans-1.1.0/plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.1.0/plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.1.0/plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/order_detail.html` & `django-plans-1.1.0/plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/order_detail_table.html` & `django-plans-1.1.0/plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/order_list.html` & `django-plans-1.1.0/plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/pagination.html` & `django-plans-1.1.0/plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/templates/plans/plan_table.html` & `django-plans-1.1.0/plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/tests/test_autorenew_accounts.py` & `django-plans-1.1.0/plans/tests/test_autorenew_accounts.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,58 +2,81 @@
 from decimal import Decimal
 from io import StringIO
 
 from django.core.management import call_command
 from django.test import TestCase
 from model_bakery import baker
 
+from plans.models import AbstractRecurringUserPlan
+
 
 class ManagementCommandTests(TestCase):
     def test_command_output(self):
         out = StringIO()
         call_command("autorenew_accounts", stdout=out)
         self.assertEqual(out.getvalue(), "Starting renewal\nNo accounts autorenewed\n")
 
     def test_renewal(self):
-        self.user = baker.make("User", username="testuser")
-        plan_pricing = baker.make(
-            "PlanPricing", plan=baker.make("Plan", name="Foo plan")
-        )
-        baker.make(
-            "UserPlan",
-            user=self.user,
-            plan=plan_pricing.plan,
-            recurring__payment_provider="internal-payment-recurring",
-            recurring__amount=Decimal(123),
-            recurring__pricing=plan_pricing.pricing,
-            recurring__currency="USD",
-            recurring__has_automatic_renewal=True,
-            recurring__token_verified=True,
-            expire=datetime.date(2020, 1, 2),
+        _make_user(
+            userplan__expire=datetime.date(2020, 1, 2),
+            userplan__recurring__renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            userplan__recurring__token_verified=True,
         )
         out = StringIO()
         call_command("autorenew_accounts", stdout=out)
         self.assertEqual(
             out.getvalue().strip(),
             "Starting renewal\nAccounts submitted to renewal:\n\tinternal-payment-recurring\t\ttestuser",
         )
 
-    def test_renewal_providers(self):
-        self.user = baker.make("User", username="testuser")
-        plan_pricing = baker.make(
-            "PlanPricing", plan=baker.make("Plan", name="Foo plan")
+    def test_renewal_triggered_by_user(self):
+        _make_user(
+            userplan__expire=datetime.date(2020, 1, 2),
+            userplan__recurring__renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+            userplan__recurring__token_verified=True,
         )
-        baker.make(
-            "UserPlan",
-            user=self.user,
-            plan=plan_pricing.plan,
-            recurring__payment_provider="internal-payment-recurring",
-            recurring__amount=Decimal(123),
-            recurring__pricing=plan_pricing.pricing,
-            recurring__currency="USD",
-            recurring__has_automatic_renewal=True,
-            recurring__token_verified=True,
-            expire=datetime.date(2020, 1, 2),
+        out = StringIO()
+        call_command("autorenew_accounts", stdout=out)
+        self.assertEqual(out.getvalue(), "Starting renewal\nNo accounts autorenewed\n")
+
+    def test_renewal_triggered_by_other(self):
+        _make_user(
+            userplan__expire=datetime.date(2020, 1, 2),
+            userplan__recurring__renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+            userplan__recurring__token_verified=True,
+        )
+        out = StringIO()
+        call_command("autorenew_accounts", stdout=out)
+        self.assertEqual(out.getvalue(), "Starting renewal\nNo accounts autorenewed\n")
+
+    def test_renewal_providers(self):
+        _make_user(
+            userplan__expire=datetime.date(2020, 1, 2),
+            userplan__recurring__renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            userplan__recurring__payment_provider="internal-payment-recurring",
+            userplan__recurring__token_verified=True,
         )
         out = StringIO()
         call_command("autorenew_accounts", providers="foo", stdout=out)
         self.assertEqual(out.getvalue(), "Starting renewal\nNo accounts autorenewed\n")
+
+
+def _make_user(
+    userplan__expire,
+    userplan__recurring__renewal_triggered_by,
+    userplan__recurring__token_verified,
+    userplan__recurring__payment_provider="internal-payment-recurring",
+):
+    user = baker.make("User", username="testuser")
+    plan_pricing = baker.make("PlanPricing", plan=baker.make("Plan", name="Foo plan"))
+    baker.make(
+        "UserPlan",
+        user=user,
+        plan=plan_pricing.plan,
+        recurring__payment_provider=userplan__recurring__payment_provider,
+        recurring__amount=Decimal(123),
+        recurring__pricing=plan_pricing.pricing,
+        recurring__currency="USD",
+        recurring__renewal_triggered_by=userplan__recurring__renewal_triggered_by,
+        recurring__token_verified=userplan__recurring__token_verified,
+        expire=userplan__expire,
+    )
```

### Comparing `django-plans-1.0.7/plans/tests/test_views.py` & `django-plans-1.1.0/plans/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/tests/tests.py` & `django-plans-1.1.0/plans/tests/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import random
 import re
+import warnings
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from io import StringIO
 from unittest import mock
 from unittest.mock import patch
 
 import requests
@@ -27,14 +28,15 @@
 from plans.base.models import (
     AbstractBillingInfo,
     AbstractInvoice,
     AbstractOrder,
     AbstractPlan,
     AbstractPlanPricing,
     AbstractPricing,
+    AbstractRecurringUserPlan,
     AbstractUserPlan,
 )
 from plans.plan_change import PlanChangePolicy, StandardPlanChangePolicy
 from plans.quota import get_user_quota
 from plans.taxation.eu import EUTaxationPolicy
 from plans.validators import ModelCountValidator
 from plans.views import CreateOrderView
@@ -1486,24 +1488,146 @@
 
 
 class RecurringPlansTestCase(TestCase):
     def test_set_plan_renewal(self):
         """Test that UserPlan.set_plan_renewal() method"""
         up = baker.make("UserPlan")
         o = baker.make("Order", amount=10)
-        up.set_plan_renewal(order=o, card_masked_number="1234")
-        self.assertEqual(up.recurring.amount, 10)
-        self.assertEqual(up.recurring.card_masked_number, "1234")
-        old_id = up.recurring.id
-
-        # test setting new values
-        up.set_plan_renewal(order=o)
-        self.assertEqual(up.recurring.amount, 10)
-        self.assertEqual(up.recurring.card_masked_number, None)
-        self.assertEqual(up.recurring.id, old_id)
+
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+
+            up.set_plan_renewal(
+                order=o,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+                card_masked_number="1234",
+            )
+            self.assertEqual(up.recurring.amount, 10)
+            self.assertEqual(up.recurring.card_masked_number, "1234")
+            self.assertFalse(caught_warnings)
+            old_id = up.recurring.id
+
+            # test setting new values
+            up.set_plan_renewal(
+                order=o,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            )
+            self.assertEqual(up.recurring.amount, 10)
+            self.assertEqual(up.recurring.card_masked_number, None)
+            self.assertEqual(up.recurring.id, old_id)
+            self.assertFalse(caught_warnings)
+
+            # test renewal_triggered_by overrides has_automatic_renewal
+            up.set_plan_renewal(
+                order=o,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+                has_automatic_renewal=False,
+            )
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+            up.set_plan_renewal(
+                order=o,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+                has_automatic_renewal=True,
+            )
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+            up.set_plan_renewal(
+                order=o,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+                has_automatic_renewal=True,
+            )
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            # test deprecated backward compatibility
+            up.set_plan_renewal(order=o)
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            )
+            self.assertEqual(len(caught_warnings), 2)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "renewal_triggered_by=None is deprecated. "
+                "Set an AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY instead.",
+            )
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+            up.set_plan_renewal(order=o, has_automatic_renewal=True)
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            )
+            self.assertEqual(len(caught_warnings), 2)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "renewal_triggered_by=None is deprecated. "
+                "Set an AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY instead.",
+            )
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+            up.set_plan_renewal(order=o, has_automatic_renewal=False)
+            self.assertEqual(
+                up.recurring.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+            )
+            self.assertEqual(len(caught_warnings), 2)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "renewal_triggered_by=None is deprecated. "
+                "Set an AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY instead.",
+            )
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
 
     def test_plan_autorenew_at(self):
         """Test that UserPlan.plan_autorenew_at() method"""
         up = baker.make("UserPlan")
         self.assertEqual(up.plan_autorenew_at(), None)
 
     def test_plan_autorenew_at_expire(self):
@@ -1516,23 +1640,33 @@
         PLANS_AUTORENEW_BEFORE_HOURS=24,
     )
     def test_plan_autorenew_at_settings(self):
         """Test that UserPlan.plan_autorenew_at() method"""
         up = baker.make("UserPlan", expire=date(2020, 1, 5))
         self.assertEqual(up.plan_autorenew_at(), date(2020, 1, 1))
 
-    def test_has_automatic_renewal(self):
+    def test_userplan_has_automatic_renewal(self):
         """Test UserPlan.has_automatic_renewal() method"""
         user_plan = baker.make("UserPlan")
         order = baker.make("Order", amount=10)
-        user_plan.set_plan_renewal(order=order, card_masked_number="1234")
-        self.assertEqual(user_plan.has_automatic_renewal(), False)
 
-        user_plan.recurring.token_verified = True
-        self.assertEqual(user_plan.has_automatic_renewal(), True)
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+
+            user_plan.set_plan_renewal(
+                order=order,
+                renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+                card_masked_number="1234",
+            )
+            self.assertEqual(user_plan.has_automatic_renewal(), False)
+            self.assertFalse(caught_warnings)
+
+            user_plan.recurring.token_verified = True
+            self.assertEqual(user_plan.has_automatic_renewal(), True)
+            self.assertFalse(caught_warnings)
 
     def test_create_new_order(self):
         rup = baker.make(
             "RecurringUserPlan",
             user_plan__user__billinginfo__country="CZ",
             amount=10,
         )
@@ -1549,27 +1683,112 @@
             amount=10,
             tax=11,
         )
         with no_connection():
             order = rup.create_renew_order()
         self.assertEqual(order.tax, 11)
 
+    def test_has_automatic_renewal(self):
+        rup = baker.make("RecurringUserPlan")
+
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            warnings.simplefilter("always")
+
+            rup.renewal_triggered_by = (
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER
+            )
+            self.assertFalse(rup.has_automatic_renewal)
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            rup.renewal_triggered_by = (
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK
+            )
+            self.assertTrue(rup.has_automatic_renewal)
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            rup.renewal_triggered_by = (
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.OTHER
+            )
+            self.assertTrue(rup.has_automatic_renewal)
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            rup.has_automatic_renewal = False
+            self.assertEqual(
+                rup.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            rup.has_automatic_renewal = True
+            self.assertEqual(
+                rup.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
+            del rup.has_automatic_renewal
+            self.assertEqual(
+                rup.renewal_triggered_by,
+                AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.USER,
+            )
+            self.assertEqual(len(caught_warnings), 1)
+            caught_warning = caught_warnings.pop()
+            self.assertTrue(issubclass(caught_warning.category, DeprecationWarning))
+            self.assertEqual(
+                str(caught_warning.message),
+                "has_automatic_renewal is deprecated. Use renewal_triggered_by instead.",
+            )
+
 
 class TasksTestCase(TestCase):
     def setUp(self):
         self.user = baker.make("User", email="foo@bar.cz", username="foo bar")
 
     def test_expire_account_task(self):
         order = baker.make("Order", amount=10)
         userplan = baker.make("UserPlan", user=self.user)
         userplan.expire = date.today() - timedelta(days=1)
         userplan.active = True
 
         # If the automatic renewal didn't go through, even automatic renewal plans has to go
-        userplan.set_plan_renewal(order=order, card_masked_number="1234")
+        userplan.set_plan_renewal(
+            order=order,
+            renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            card_masked_number="1234",
+        )
 
         userplan.save()
         tasks.expire_account()
 
         userplan.refresh_from_db()
         self.assertEqual(userplan.active, False)
         self.assertEqual(len(mail.outbox), 1)
@@ -1581,15 +1800,19 @@
     def test_expire_account_task_notify(self):
         order = baker.make("Order", amount=10)
         userplan = baker.make("UserPlan", user=self.user)
         userplan.expire = date.today() + timedelta(days=3)
         userplan.active = True
 
         # If the automatic renewal didn't go through, even automatic renewal plans has to go
-        userplan.set_plan_renewal(order=order, card_masked_number="1234")
+        userplan.set_plan_renewal(
+            order=order,
+            renewal_triggered_by=AbstractRecurringUserPlan.RENEWAL_TRIGGERED_BY.TASK,
+            card_masked_number="1234",
+        )
 
         userplan.save()
         tasks.expire_account()
 
         userplan.refresh_from_db()
         self.assertEqual(userplan.active, True)
         self.assertEqual(len(mail.outbox), 1)
```

### Comparing `django-plans-1.0.7/plans/urls.py` & `django-plans-1.1.0/plans/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/utils.py` & `django-plans-1.1.0/plans/utils.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/validators.py` & `django-plans-1.1.0/plans/validators.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans/views.py` & `django-plans-1.1.0/plans/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans_i18n/README.rst` & `django-plans-1.1.0/plans_i18n/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans_i18n/admin.py` & `django-plans-1.1.0/plans_i18n/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/plans_i18n/translation.py` & `django-plans-1.1.0/plans_i18n/translation.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/setup.py` & `django-plans-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.0.7/tox.ini` & `django-plans-1.1.0/tox.ini`

 * *Files identical despite different names*

