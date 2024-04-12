# Comparing `tmp/django-bootstrap5-23.4.tar.gz` & `tmp/django-bootstrap5-24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-bootstrap5-23.4.tar", last modified: Thu Dec 28 14:27:31 2023, max compression
+gzip compressed data, was "django-bootstrap5-24.1.tar", last modified: Fri Apr 12 08:20:08 2024, max compression
```

## Comparing `django-bootstrap5-23.4.tar` & `django-bootstrap5-24.1.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.188296 django-bootstrap5-23.4/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.175544 django-bootstrap5-23.4/.github/
--rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/.github/dependabot.yml
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.175828 django-bootstrap5-23.4/.github/workflows/
--rw-r--r--   0 dylan      (501) staff       (20)     1525 2023-06-29 05:37:28.000000 django-bootstrap5-23.4/.github/workflows/dependabot-auto-approve-and-merge.yml
--rw-r--r--   0 dylan      (501) staff       (20)     2967 2023-12-28 14:12:07.000000 django-bootstrap5-23.4/.github/workflows/test.yml
--rw-r--r--   0 dylan      (501) staff       (20)      587 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/.gitignore
--rw-r--r--   0 dylan      (501) staff       (20)      206 2023-12-28 14:11:48.000000 django-bootstrap5-23.4/.readthedocs.yml
--rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/AUTHORS
--rw-r--r--   0 dylan      (501) staff       (20)     5281 2023-12-28 14:27:26.000000 django-bootstrap5-23.4/CHANGELOG.md
--rw-r--r--   0 dylan      (501) staff       (20)     2348 2023-12-28 14:11:48.000000 django-bootstrap5-23.4/CONTRIBUTING.md
--rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)     1151 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/MIGRATE.md
--rw-r--r--   0 dylan      (501) staff       (20)     1090 2023-12-28 14:22:09.000000 django-bootstrap5-23.4/Makefile
--rw-r--r--   0 dylan      (501) staff       (20)     5570 2023-12-28 14:27:31.188057 django-bootstrap5-23.4/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2346 2023-12-24 09:23:31.000000 django-bootstrap5-23.4/README.md
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.177595 django-bootstrap5-23.4/docs/
--rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/changelog.rst
--rw-r--r--   0 dylan      (501) staff       (20)      566 2023-12-28 14:11:48.000000 django-bootstrap5-23.4/docs/conf.py
--rw-r--r--   0 dylan      (501) staff       (20)       34 2023-06-03 11:33:19.000000 django-bootstrap5-23.4/docs/contributing.rst
--rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/example_template.rst
--rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/forms.rst
--rw-r--r--   0 dylan      (501) staff       (20)      265 2023-06-03 14:37:18.000000 django-bootstrap5-23.4/docs/index.rst
--rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/installation.rst
--rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/migrate.rst
--rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/quickstart.rst
--rw-r--r--   0 dylan      (501) staff       (20)       55 2023-12-28 14:22:35.000000 django-bootstrap5-23.4/docs/requirements.txt
--rw-r--r--   0 dylan      (501) staff       (20)     3275 2022-10-14 14:58:03.000000 django-bootstrap5-23.4/docs/settings.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/templates.rst
--rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/docs/templatetags.rst
--rw-r--r--   0 dylan      (501) staff       (20)      799 2023-06-03 13:26:35.000000 django-bootstrap5-23.4/docs/widgets.rst
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.178045 django-bootstrap5-23.4/example/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.178365 django-bootstrap5-23.4/example/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     4215 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/app/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)     2785 2022-02-27 06:07:14.000000 django-bootstrap5-23.4/example/app/views.py
--rwxr-xr-x   0 dylan      (501) staff       (20)      242 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     5231 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/settings.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.173142 django-bootstrap5-23.4/example/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.179659 django-bootstrap5-23.4/example/templates/app/
--rw-r--r--   0 dylan      (501) staff       (20)     1327 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/base.html
--rw-r--r--   0 dylan      (501) staff       (20)      125 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/bootstrap.html
--rw-r--r--   0 dylan      (501) staff       (20)      397 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/form.html
--rw-r--r--   0 dylan      (501) staff       (20)      549 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/form_by_field.html
--rw-r--r--   0 dylan      (501) staff       (20)      429 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/form_horizontal.html
--rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/form_inline.html
--rw-r--r--   0 dylan      (501) staff       (20)      417 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/form_with_files.html
--rw-r--r--   0 dylan      (501) staff       (20)      443 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/formset.html
--rw-r--r--   0 dylan      (501) staff       (20)      205 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/home.html
--rw-r--r--   0 dylan      (501) staff       (20)      274 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/misc.html
--rw-r--r--   0 dylan      (501) staff       (20)      489 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/example/templates/app/pagination.html
--rw-r--r--   0 dylan      (501) staff       (20)      898 2023-04-23 11:11:29.000000 django-bootstrap5-23.4/example/urls.py
--rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/manage.py
--rw-r--r--   0 dylan      (501) staff       (20)     2565 2023-12-28 14:27:26.000000 django-bootstrap5-23.4/pyproject.toml
--rw-r--r--   0 dylan      (501) staff       (20)      117 2023-12-28 14:22:36.000000 django-bootstrap5-23.4/requirements-dev.txt
--rw-r--r--   0 dylan      (501) staff       (20)       78 2023-12-28 14:22:35.000000 django-bootstrap5-23.4/requirements-test.txt
--rw-r--r--   0 dylan      (501) staff       (20)       38 2023-12-28 14:27:31.188335 django-bootstrap5-23.4/setup.cfg
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.173317 django-bootstrap5-23.4/src/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.181398 django-bootstrap5-23.4/src/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-28 14:11:02.000000 django-bootstrap5-23.4/src/django_bootstrap5/__about__.py
--rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-03 11:33:19.000000 django-bootstrap5-23.4/src/django_bootstrap5/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-23.4/src/django_bootstrap5/components.py
--rw-r--r--   0 dylan      (501) staff       (20)     2692 2023-11-09 15:16:48.000000 django-bootstrap5-23.4/src/django_bootstrap5/core.py
--rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/css.py
--rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-23.4/src/django_bootstrap5/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/html.py
--rw-r--r--   0 dylan      (501) staff       (20)    21264 2023-12-24 09:23:31.000000 django-bootstrap5-23.4/src/django_bootstrap5/renderers.py
--rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/size.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.173427 django-bootstrap5-23.4/src/django_bootstrap5/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.182781 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/
--rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
--rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
--rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.183163 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/
--rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
--rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
--rw-r--r--   0 dylan      (501) staff       (20)      670 2022-10-15 06:09:49.000000 django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.183394 django-bootstrap5-23.4/src/django_bootstrap5/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    19503 2023-11-09 15:16:52.000000 django-bootstrap5-23.4/src/django_bootstrap5/templatetags/django_bootstrap5.py
--rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/src/django_bootstrap5/widgets.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.187731 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)     5570 2023-12-28 14:27:31.000000 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     3454 2023-12-28 14:27:31.000000 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2023-12-28 14:27:31.000000 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)       12 2023-12-28 14:27:31.000000 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/requires.txt
--rw-r--r--   0 dylan      (501) staff       (20)       18 2023-12-28 14:27:31.000000 django-bootstrap5-23.4/src/django_bootstrap5.egg-info/top_level.txt
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.187228 django-bootstrap5-23.4/tests/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/__init__.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2023-12-28 14:27:31.187562 django-bootstrap5-23.4/tests/app/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/app/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/app/settings.py
--rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/app/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      549 2023-06-29 05:37:28.000000 django-bootstrap5-23.4/tests/base.py
--rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/image.py
--rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_alert.py
--rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_button.py
--rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_css_and_js_tags.py
--rw-r--r--   0 dylan      (501) staff       (20)     3282 2023-12-28 14:11:02.000000 django-bootstrap5-23.4/tests/test_bootstrap_field.py
--rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_datetime.py
--rw-r--r--   0 dylan      (501) staff       (20)     3797 2023-12-28 14:11:02.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_input_checkbox.py
--rw-r--r--   0 dylan      (501) staff       (20)     2120 2023-06-29 05:47:36.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_input_color.py
--rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_input_file.py
--rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_input_range.py
--rw-r--r--   0 dylan      (501) staff       (20)    12847 2023-12-28 14:11:02.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_input_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_parameters.py
--rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_radio_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     2240 2023-06-29 05:55:16.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_select.py
--rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_field_textarea.py
--rw-r--r--   0 dylan      (501) staff       (20)     8031 2023-12-28 14:11:02.000000 django-bootstrap5-23.4/tests/test_bootstrap_form.py
--rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_bootstrap_formset.py
--rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-23.4/tests/test_bootstrap_label.py
--rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-23.4/tests/test_bootstrap_messages.py
--rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django-bootstrap5-23.4/tests/test_bootstrap_pagination.py
--rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_components.py
--rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_css.py
--rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_html.py
--rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_settings.py
--rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_size.py
--rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_templates.py
--rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_text.py
--rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django-bootstrap5-23.4/tests/test_urls.py
--rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-23.4/tests/test_version.py
--rw-r--r--   0 dylan      (501) staff       (20)      983 2023-12-28 14:11:48.000000 django-bootstrap5-23.4/tox.ini
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.774009 django-bootstrap5-24.1/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.755661 django-bootstrap5-24.1/.github/
+-rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/.github/dependabot.yml
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.756079 django-bootstrap5-24.1/.github/workflows/
+-rw-r--r--   0 dylan      (501) staff       (20)     1525 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/.github/workflows/dependabot-auto-approve-and-merge.yml
+-rw-r--r--   0 dylan      (501) staff       (20)     2967 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/.github/workflows/test.yml
+-rw-r--r--   0 dylan      (501) staff       (20)      587 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/.gitignore
+-rw-r--r--   0 dylan      (501) staff       (20)      206 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/.readthedocs.yml
+-rw-r--r--   0 dylan      (501) staff       (20)      757 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/AUTHORS
+-rw-r--r--   0 dylan      (501) staff       (20)     5411 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/CHANGELOG.md
+-rw-r--r--   0 dylan      (501) staff       (20)     2348 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/CONTRIBUTING.md
+-rw-r--r--   0 dylan      (501) staff       (20)     1533 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     1151 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/MIGRATE.md
+-rw-r--r--   0 dylan      (501) staff       (20)     1090 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/Makefile
+-rw-r--r--   0 dylan      (501) staff       (20)     5570 2024-04-12 08:20:08.773780 django-bootstrap5-24.1/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     2346 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/README.md
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.757995 django-bootstrap5-24.1/docs/
+-rw-r--r--   0 dylan      (501) staff       (20)       30 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/changelog.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      566 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/docs/conf.py
+-rw-r--r--   0 dylan      (501) staff       (20)       34 2023-06-03 11:33:19.000000 django-bootstrap5-24.1/docs/contributing.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      577 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/example_template.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     3276 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/forms.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      265 2023-06-03 14:37:18.000000 django-bootstrap5-24.1/docs/index.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      585 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/installation.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       28 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/migrate.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      665 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/quickstart.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       55 2024-04-12 08:13:48.000000 django-bootstrap5-24.1/docs/requirements.txt
+-rw-r--r--   0 dylan      (501) staff       (20)     3275 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/docs/settings.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     1364 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/templates.rst
+-rw-r--r--   0 dylan      (501) staff       (20)     2217 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/docs/templatetags.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      799 2023-06-03 13:26:35.000000 django-bootstrap5-24.1/docs/widgets.rst
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.758584 django-bootstrap5-24.1/example/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.759143 django-bootstrap5-24.1/example/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4215 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/app/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2785 2022-02-27 06:07:14.000000 django-bootstrap5-24.1/example/app/views.py
+-rwxr-xr-x   0 dylan      (501) staff       (20)      242 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     5231 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/settings.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752555 django-bootstrap5-24.1/example/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.761206 django-bootstrap5-24.1/example/templates/app/
+-rw-r--r--   0 dylan      (501) staff       (20)     1327 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/base.html
+-rw-r--r--   0 dylan      (501) staff       (20)      125 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/bootstrap.html
+-rw-r--r--   0 dylan      (501) staff       (20)      397 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form.html
+-rw-r--r--   0 dylan      (501) staff       (20)      549 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_by_field.html
+-rw-r--r--   0 dylan      (501) staff       (20)      429 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_horizontal.html
+-rw-r--r--   0 dylan      (501) staff       (20)      441 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_inline.html
+-rw-r--r--   0 dylan      (501) staff       (20)      417 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/form_with_files.html
+-rw-r--r--   0 dylan      (501) staff       (20)      443 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/formset.html
+-rw-r--r--   0 dylan      (501) staff       (20)      205 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/home.html
+-rw-r--r--   0 dylan      (501) staff       (20)      274 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/misc.html
+-rw-r--r--   0 dylan      (501) staff       (20)      489 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/example/templates/app/pagination.html
+-rw-r--r--   0 dylan      (501) staff       (20)      898 2023-04-23 11:11:29.000000 django-bootstrap5-24.1/example/urls.py
+-rwxr-xr-x   0 dylan      (501) staff       (20)      252 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2565 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/pyproject.toml
+-rw-r--r--   0 dylan      (501) staff       (20)      117 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/requirements-dev.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       78 2024-04-12 08:19:55.000000 django-bootstrap5-24.1/requirements-test.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2024-04-12 08:20:08.774050 django-bootstrap5-24.1/setup.cfg
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752745 django-bootstrap5-24.1/src/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.763904 django-bootstrap5-24.1/src/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)       93 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/__about__.py
+-rw-r--r--   0 dylan      (501) staff       (20)       69 2023-06-03 11:33:19.000000 django-bootstrap5-24.1/src/django_bootstrap5/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2351 2022-08-05 14:34:59.000000 django-bootstrap5-24.1/src/django_bootstrap5/components.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2692 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/src/django_bootstrap5/core.py
+-rw-r--r--   0 dylan      (501) staff       (20)      621 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/css.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1482 2022-10-15 06:32:49.000000 django-bootstrap5-24.1/src/django_bootstrap5/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)      870 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/html.py
+-rw-r--r--   0 dylan      (501) staff       (20)    21369 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/renderers.py
+-rw-r--r--   0 dylan      (501) staff       (20)      901 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/size.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.752873 django-bootstrap5-24.1/src/django_bootstrap5/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.765510 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/
+-rw-r--r--   0 dylan      (501) staff       (20)     1079 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html
+-rw-r--r--   0 dylan      (501) staff       (20)       95 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/field_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)       79 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/field_help_text.html
+-rw-r--r--   0 dylan      (501) staff       (20)      122 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/form_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)      206 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/messages.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1762 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.766012 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/
+-rw-r--r--   0 dylan      (501) staff       (20)      895 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1052 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html
+-rw-r--r--   0 dylan      (501) staff       (20)      829 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.766365 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    19503 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/src/django_bootstrap5/templatetags/django_bootstrap5.py
+-rw-r--r--   0 dylan      (501) staff       (20)      467 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1497 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)      745 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/src/django_bootstrap5/widgets.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.773445 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)     5570 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     3510 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       12 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/requires.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       18 2024-04-12 08:20:08.000000 django-bootstrap5-24.1/src/django_bootstrap5.egg-info/top_level.txt
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.772873 django-bootstrap5-24.1/tests/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/__init__.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2024-04-12 08:20:08.773251 django-bootstrap5-24.1/tests/app/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1703 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)       17 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/app/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      549 2023-06-29 05:37:28.000000 django-bootstrap5-24.1/tests/base.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3439 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/image.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1595 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_alert.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2698 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_button.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2024 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_css_and_js_tags.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3282 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3343 2021-12-27 05:56:30.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_datetime.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3797 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_checkbox.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2120 2023-06-29 05:47:36.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_color.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3150 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_file.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2003 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_range.py
+-rw-r--r--   0 dylan      (501) staff       (20)    12847 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_input_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     3657 2023-04-23 08:55:44.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_parameters.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4590 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4545 2024-04-12 08:10:50.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select_button_group.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2240 2023-06-29 05:55:16.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_select.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1340 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_field_textarea.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8031 2023-12-29 08:24:07.000000 django-bootstrap5-24.1/tests/test_bootstrap_form.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1634 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_bootstrap_formset.py
+-rw-r--r--   0 dylan      (501) staff       (20)      869 2022-10-15 06:31:02.000000 django-bootstrap5-24.1/tests/test_bootstrap_label.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2934 2022-08-05 14:34:59.000000 django-bootstrap5-24.1/tests/test_bootstrap_messages.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6807 2023-04-25 10:31:45.000000 django-bootstrap5-24.1/tests/test_bootstrap_pagination.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2600 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_components.py
+-rw-r--r--   0 dylan      (501) staff       (20)      839 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_css.py
+-rw-r--r--   0 dylan      (501) staff       (20)      511 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_html.py
+-rw-r--r--   0 dylan      (501) staff       (20)      515 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_settings.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1149 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_size.py
+-rw-r--r--   0 dylan      (501) staff       (20)      852 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_templates.py
+-rw-r--r--   0 dylan      (501) staff       (20)      556 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_text.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1257 2023-04-23 08:55:44.000000 django-bootstrap5-24.1/tests/test_urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)      315 2021-12-12 13:22:34.000000 django-bootstrap5-24.1/tests/test_version.py
+-rw-r--r--   0 dylan      (501) staff       (20)      983 2023-12-29 08:22:50.000000 django-bootstrap5-24.1/tox.ini
```

### Comparing `django-bootstrap5-23.4/.github/workflows/dependabot-auto-approve-and-merge.yml` & `django-bootstrap5-24.1/.github/workflows/dependabot-auto-approve-and-merge.yml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     runs-on: ubuntu-latest
     # Check the actor, only run for Dependabot PRs, prevent failing on non-Dependabot PRs.
     if: ${{ github.actor == 'dependabot[bot]' }}
     steps:
       # This step will fail (without approval) if there's no metadata.
       - name: Dependabot metadata
         id: dependabot-metadata
-        uses: dependabot/fetch-metadata@v1.6.0
+        uses: dependabot/fetch-metadata@v1.7.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
       # Approve the PR.
       - name: Approve a PR
         run: gh pr review --approve "$PR_URL"
         env:
           PR_URL: ${{ github.event.pull_request.html_url }}
```

### Comparing `django-bootstrap5-23.4/.github/workflows/test.yml` & `django-bootstrap5-24.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/.gitignore` & `django-bootstrap5-24.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/AUTHORS` & `django-bootstrap5-24.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/CHANGELOG.md` & `django-bootstrap5-24.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 24.1 (2024-04-12)
+
+- Fix RadioSelectButtonGroup rendering and add 'disabled' attribute to radio button group template (#447).
+
 ## 23.4 (2023-12-28)
 
 - Use ruff instead of black for formatting (#536).
 - Drop support for Python 3.7 in test matrix (#533).
 - Fix support for Django 4.2 in test matrix (#533).
 - Pass "horizontal_field_offset_class" to child renderers (#391, #521).
 - Add support for Django 5.0 (#538).
```

### Comparing `django-bootstrap5-23.4/CONTRIBUTING.md` & `django-bootstrap5-24.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/LICENSE` & `django-bootstrap5-24.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/MIGRATE.md` & `django-bootstrap5-24.1/MIGRATE.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/Makefile` & `django-bootstrap5-24.1/Makefile`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/PKG-INFO` & `django-bootstrap5-24.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 23.4
+Version: 24.1
 Summary: Bootstrap 5 for Django
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: BSD 3-Clause License
         
         Copyright (c) Zostera B.V. and individual contributors
         All rights reserved.
```

### Comparing `django-bootstrap5-23.4/README.md` & `django-bootstrap5-24.1/README.md`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/conf.py` & `django-bootstrap5-24.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/example_template.rst` & `django-bootstrap5-24.1/docs/example_template.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/forms.rst` & `django-bootstrap5-24.1/docs/forms.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/installation.rst` & `django-bootstrap5-24.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/quickstart.rst` & `django-bootstrap5-24.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/settings.rst` & `django-bootstrap5-24.1/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/templates.rst` & `django-bootstrap5-24.1/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/templatetags.rst` & `django-bootstrap5-24.1/docs/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/docs/widgets.rst` & `django-bootstrap5-24.1/docs/widgets.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/app/forms.py` & `django-bootstrap5-24.1/example/app/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/app/views.py` & `django-bootstrap5-24.1/example/app/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/settings.py` & `django-bootstrap5-24.1/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/templates/app/base.html` & `django-bootstrap5-24.1/example/templates/app/base.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/templates/app/form_by_field.html` & `django-bootstrap5-24.1/example/templates/app/form_by_field.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/example/urls.py` & `django-bootstrap5-24.1/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/pyproject.toml` & `django-bootstrap5-24.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 dependencies = ["Django>=3.2"]
 description = "Bootstrap 5 for Django"
 license = {file = "LICENSE"}
 name = "django-bootstrap5"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "23.4"
+version = "24.1"
 
 [project.urls]
 Changelog = "https://github.com/zostera/django-bootstrap5/blob/main/CHANGELOG.md"
 Documentation = "https://django-bootstrap5.readthedocs.io/"
 Homepage = "https://github.com/zostera/django-bootstrap5"
 Issues = "https://github.com/zostera/django-bootstrap5/issues"
 Source = "https://github.com/zostera/django-bootstrap5"
```

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/components.py` & `django-bootstrap5-24.1/src/django_bootstrap5/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/core.py` & `django-bootstrap5-24.1/src/django_bootstrap5/core.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/css.py` & `django-bootstrap5-24.1/src/django_bootstrap5/css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/forms.py` & `django-bootstrap5-24.1/src/django_bootstrap5/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/html.py` & `django-bootstrap5-24.1/src/django_bootstrap5/html.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/renderers.py` & `django-bootstrap5-24.1/src/django_bootstrap5/renderers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from .core import get_bootstrap_setting
 from .css import merge_css_classes
 from .forms import render_field, render_form, render_label
 from .size import DEFAULT_SIZE, SIZE_MD, get_size_class, parse_size
 from .text import text_value
 from .utils import render_template_file
-from .widgets import ReadOnlyPasswordHashWidget, is_widget_with_placeholder
+from .widgets import RadioSelectButtonGroup, ReadOnlyPasswordHashWidget, is_widget_with_placeholder
 
 
 class BaseRenderer:
     """A content renderer."""
 
     # Template paths for overriding in custom subclasses.
     field_errors_template = "django_bootstrap5/field_errors.html"
@@ -343,15 +343,17 @@
         if self.is_multi_widget:
             widgets = self.widget.widgets
         else:
             widgets = [self.widget]
         for widget in widgets:
             self.add_widget_class_attrs(widget)
             self.add_placeholder_attrs(widget)
-            if isinstance(widget, (RadioSelect, CheckboxSelectMultiple)):
+            if isinstance(widget, (RadioSelect, CheckboxSelectMultiple)) and not isinstance(
+                widget, RadioSelectButtonGroup
+            ):
                 widget.template_name = "django_bootstrap5/widgets/radio_select.html"
             elif isinstance(widget, ClearableFileInput):
                 widget.template_name = "django_bootstrap5/widgets/clearable_file_input.html"
 
     def get_label_class(self, horizontal=False):
         """Return CSS class for label."""
         label_classes = [text_value(self.label_class)]
```

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/size.py` & `django-bootstrap5-24.1/src/django_bootstrap5/size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html` & `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/bootstrap5.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/pagination.html` & `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html` & `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html` & `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html` & `django-bootstrap5-24.1/src/django_bootstrap5/templates/django_bootstrap5/widgets/radio_select_button_group.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 <div{% if widget.attrs.id %} id="{{ widget.attrs.id }}"{% endif %} class="btn-group" role="group">
   {% for group, options, index in widget.optgroups %}
     {% for option in options %}
-      <input type="{{ option.type }}" class="{{ widget.attrs.class|add:' btn-check' }}" autocomplete="off" name="{{ option.name }}" id="{{ option.attrs.id }}"{% if option.value != None %} value="{{ option.value|stringformat:'s' }}"{% if option.attrs.checked %} checked="checked"{% endif %}{% endif %}{% if widget.required %} required{% endif %}>
+      <input type="{{ option.type }}"
+             class="{{ widget.attrs.class|add:' btn-check' }}"
+             autocomplete="off"
+             name="{{ option.name }}"
+             id="{{ option.attrs.id }}"
+             {% if option.value != None %} value="{{ option.value|stringformat:'s' }}"
+              {% if option.attrs.checked %} checked="checked"{% endif %}{% endif %}
+             {% if widget.attrs.disabled %} disabled{% endif %}
+             {% if widget.required %} required{% endif %}>
       <label class="btn btn-outline-primary" for="{{ option.attrs.id }}">{{ option.label }}</label>
     {% endfor %}
   {% endfor %}
 </div>
```

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/templatetags/django_bootstrap5.py` & `django-bootstrap5-24.1/src/django_bootstrap5/templatetags/django_bootstrap5.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/utils.py` & `django-bootstrap5-24.1/src/django_bootstrap5/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5/widgets.py` & `django-bootstrap5-24.1/src/django_bootstrap5/widgets.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5.egg-info/PKG-INFO` & `django-bootstrap5-24.1/src/django_bootstrap5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bootstrap5
-Version: 23.4
+Version: 24.1
 Summary: Bootstrap 5 for Django
 Author-email: Dylan Verheul <dylan@dyve.net>
 License: BSD 3-Clause License
         
         Copyright (c) Zostera B.V. and individual contributors
         All rights reserved.
```

### Comparing `django-bootstrap5-23.4/src/django_bootstrap5.egg-info/SOURCES.txt` & `django-bootstrap5-24.1/src/django_bootstrap5.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 tests/test_bootstrap_field_input_checkbox.py
 tests/test_bootstrap_field_input_color.py
 tests/test_bootstrap_field_input_file.py
 tests/test_bootstrap_field_input_range.py
 tests/test_bootstrap_field_input_text.py
 tests/test_bootstrap_field_parameters.py
 tests/test_bootstrap_field_radio_select.py
+tests/test_bootstrap_field_radio_select_button_group.py
 tests/test_bootstrap_field_select.py
 tests/test_bootstrap_field_textarea.py
 tests/test_bootstrap_form.py
 tests/test_bootstrap_formset.py
 tests/test_bootstrap_label.py
 tests/test_bootstrap_messages.py
 tests/test_bootstrap_pagination.py
```

### Comparing `django-bootstrap5-23.4/tests/app/settings.py` & `django-bootstrap5-24.1/tests/app/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/base.py` & `django-bootstrap5-24.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/image.py` & `django-bootstrap5-24.1/tests/image.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_alert.py` & `django-bootstrap5-24.1/tests/test_bootstrap_alert.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_button.py` & `django-bootstrap5-24.1/tests/test_bootstrap_button.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_css_and_js_tags.py` & `django-bootstrap5-24.1/tests/test_bootstrap_css_and_js_tags.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_datetime.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_datetime.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_input_checkbox.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_input_checkbox.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_input_color.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_input_color.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_input_file.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_input_file.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_input_range.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_input_range.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_input_text.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_input_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_parameters.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_parameters.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_radio_select.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_radio_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_select.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_select.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_field_textarea.py` & `django-bootstrap5-24.1/tests/test_bootstrap_field_textarea.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_form.py` & `django-bootstrap5-24.1/tests/test_bootstrap_form.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_formset.py` & `django-bootstrap5-24.1/tests/test_bootstrap_formset.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_label.py` & `django-bootstrap5-24.1/tests/test_bootstrap_label.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_messages.py` & `django-bootstrap5-24.1/tests/test_bootstrap_messages.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_bootstrap_pagination.py` & `django-bootstrap5-24.1/tests/test_bootstrap_pagination.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_components.py` & `django-bootstrap5-24.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_css.py` & `django-bootstrap5-24.1/tests/test_css.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_settings.py` & `django-bootstrap5-24.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_size.py` & `django-bootstrap5-24.1/tests/test_size.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_templates.py` & `django-bootstrap5-24.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_text.py` & `django-bootstrap5-24.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tests/test_urls.py` & `django-bootstrap5-24.1/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap5-23.4/tox.ini` & `django-bootstrap5-24.1/tox.ini`

 * *Files identical despite different names*

