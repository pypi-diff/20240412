# Comparing `tmp/django-admin-charts-1.3.0.tar.gz` & `tmp/django-admin-charts-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-charts-1.3.0.tar", last modified: Sat Feb 11 18:25:43 2023, max compression
+gzip compressed data, was "django-admin-charts-1.3.1.tar", last modified: Fri Apr 12 13:45:33 2024, max compression
```

## Comparing `django-admin-charts-1.3.0.tar` & `django-admin-charts-1.3.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.057686 django-admin-charts-1.3.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      154 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/.coveragerc
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/.coveralls.yml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.041686 django-admin-charts-1.3.0/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.045686 django-admin-charts-1.3.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3706 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      437 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)     8405 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/CHANGELOG.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      226 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/CONTRIBUTORS
--rw-rw-r--   0 petr      (1000) petr      (1000)      154 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     1154 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/MIT-LICENSE.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)    12344 2023-02-11 18:25:43.057686 django-admin-charts-1.3.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     8935 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       12 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/TODO
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.045686 django-admin-charts-1.3.0/admin_tools_stats/
--rw-rw-r--   0 petr      (1000) petr      (1000)      611 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.045686 django-admin-charts-1.3.0/admin_tools_stats/__pycache__/
--rw-rw-r--   0 petr      (1000) petr      (1000)      353 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 petr      (1000) petr      (1000)     5054 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3429 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/app_label_renamer.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      160 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/apps.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/charts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.045686 django-admin-charts-1.3.0/admin_tools_stats/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      364 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/fixtures/10_dashboardstatscriteria_status.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      766 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/fixtures/20_dashboardstatscriteria_call_type.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      922 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/fixtures/initial_data.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     4098 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/forms.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.041686 django-admin-charts-1.3.0/admin_tools_stats/management/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.045686 django-admin-charts-1.3.0/admin_tools_stats/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5364 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/management/commands/recalculate_charts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     6760 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0002_auto_20190920_1058.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3314 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0003_auto_20191007_0950.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      699 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0004_dashboardstats_y_tick_format.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2638 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0005_auto_20200203_1537.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4051 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0006_auto_20200205_0944.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1961 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0007_auto_20200205_1054.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1076 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0008_auto_20200911_1400.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      811 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0009_auto_20200928_1003.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0010_dashboardstats_show_to_users.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2240 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0011_auto_20210204_1206.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3048 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0012_auto_20210207_0859.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1514 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0013_auto_20210221_1247.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9787 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0014_auto_20211122_1511.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      963 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0015_auto_20211209_0822.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      447 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0016_dashboardstats_cache_values.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1517 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0017_alter_dashboardstats_options_and_more.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      436 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0018_alter_dashboardstats_options.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0019_criteriatostatsm2m_recalculate.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      866 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0020_alter_dashboardstats_graph_key.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1256 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/0021_auto_20230210_1102.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    38767 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3216 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/modules.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/south_migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     7765 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0001_initial_migration.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4217 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0002_add_sum_field_name.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5289 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0003_add_operation_field_name.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/south_migrations/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/templates/admin/
--rw-rw-r--   0 petr      (1000) petr      (1000)      565 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin/index.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2646 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/admin_charts.js
--rw-rw-r--   0 petr      (1000) petr      (1000)     2405 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/analytics.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      106 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/analytics_chart.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      196 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/analytics_user.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      364 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/chart_container.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      278 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/chart_containers.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      496 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/chart_data.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1150 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/chart_form.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/modules/
--rw-rw-r--   0 petr      (1000) petr      (1000)      497 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/modules/chart.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      269 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templates/include_nvd3.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/templatetags/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templatetags/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1401 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/templatetags/admin_chart_tags.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.049686 django-admin-charts-1.3.0/admin_tools_stats/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9610 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/test_admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      582 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/test_forms.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    67338 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    22209 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1030 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/tests/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      882 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1203 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7493 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/admin_tools_stats/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/.coveralls.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)       11 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4947 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/dashboard.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/demoproject/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/demoproject/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1214 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/fixtures/auth_user.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     3065 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/fixtures/test_data.json
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/demoproject/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)      972 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/migrations/0002_auto_20210221_0541.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      714 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/migrations/0003_testkid_author.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      384 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/migrations/0004_testkid_height.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      555 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     8098 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/demoproject/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/demoproject/demoproject/templates/admin/
--rw-rw-r--   0 petr      (1000) petr      (1000)      542 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/templates/admin/base_site.html
--rw-rw-r--   0 petr      (1000) petr      (1000)       89 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/templates/home.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      206 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1436 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/demoproject/wsgi.py
--rwxrwxr-x   0 petr      (1000) petr      (1000)      255 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/menu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      101 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      489 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/demoproject/test_settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/django_admin_charts.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)    12344 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     5140 2023-02-11 18:25:43.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)      191 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       30 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/django_admin_charts.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4666 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/docs/source/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/docs/source/_static/
--rw-rw-r--   0 petr      (1000) petr      (1000)    20957 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/Snímek obrazovky_2022-03-04_17-29-58.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   104856 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/Snímek obrazovky_2022-03-04_17-31-16.png
--rw-rw-r--   0 petr      (1000) petr      (1000)    55556 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/admin_dashboard.png
--rw-rw-r--   0 petr      (1000) petr      (1000)    50767 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/aoe_chart.png
--rw-rw-r--   0 petr      (1000) petr      (1000)    30123 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/bar_chart.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.053686 django-admin-charts-1.3.0/docs/source/_static/images/
--rw-rw-r--   0 petr      (1000) petr      (1000)   122086 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/images/admin_screenshot.png
--rw-rw-r--   0 petr      (1000) petr      (1000)    53145 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/_static/stacked_area_chart.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     7480 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/conf.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.057686 django-admin-charts-1.3.0/docs/source/developer-doc/
--rw-rw-r--   0 petr      (1000) petr      (1000)      364 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/developer-doc/modules.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1228 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/developer-doc/objects-description.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      221 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/developer-doc/pre-requisite.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      571 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/developer-doc/testing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      286 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/developer-doc.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-02-11 18:25:43.057686 django-admin-charts-1.3.0/docs/source/includes/
--rw-rw-r--   0 petr      (1000) petr      (1000)      229 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/includes/introduction.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      783 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       93 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/docs/source/introduction.rst
--rwxrwxr-x   0 petr      (1000) petr      (1000)      260 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      201 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/mypy.ini
--rw-rw-r--   0 petr      (1000) petr      (1000)       57 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/pyproject.toml
--rw-rw-r--   0 petr      (1000) petr      (1000)      175 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      403 2023-02-11 18:25:43.057686 django-admin-charts-1.3.0/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     2690 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      114 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/test_requirements.txt
--rwxrwxr-x   0 petr      (1000) petr      (1000)      597 2023-02-11 18:25:42.000000 django-admin-charts-1.3.0/update_version.sh
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      154 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/.coveragerc
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/.coveralls.yml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.439213 django-admin-charts-1.3.1/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.443213 django-admin-charts-1.3.1/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3814 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      437 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8496 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/CHANGELOG.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      226 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/CONTRIBUTORS
+-rw-rw-r--   0 petr      (1000) petr      (1000)      154 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1154 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/MIT-LICENSE.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9991 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8989 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       12 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/TODO
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.443213 django-admin-charts-1.3.1/admin_tools_stats/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      611 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.443213 django-admin-charts-1.3.1/admin_tools_stats/__pycache__/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      382 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/admin_tools_stats/__pycache__/__init__.cpython-311.pyc
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5135 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3429 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/app_label_renamer.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/apps.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/charts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.443213 django-admin-charts-1.3.1/admin_tools_stats/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      364 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/fixtures/10_dashboardstatscriteria_status.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      766 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/fixtures/20_dashboardstatscriteria_call_type.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      922 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/fixtures/initial_data.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4146 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/forms.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.439213 django-admin-charts-1.3.1/admin_tools_stats/management/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.443213 django-admin-charts-1.3.1/admin_tools_stats/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5364 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/management/commands/recalculate_charts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6760 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0002_auto_20190920_1058.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3314 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0003_auto_20191007_0950.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      699 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0004_dashboardstats_y_tick_format.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2638 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0005_auto_20200203_1537.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4051 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0006_auto_20200205_0944.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1961 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0007_auto_20200205_1054.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1076 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0008_auto_20200911_1400.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      811 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0009_auto_20200928_1003.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0010_dashboardstats_show_to_users.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2240 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0011_auto_20210204_1206.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3048 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0012_auto_20210207_0859.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1514 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0013_auto_20210221_1247.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9787 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0014_auto_20211122_1511.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      963 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0015_auto_20211209_0822.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      447 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0016_dashboardstats_cache_values.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1517 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0017_alter_dashboardstats_options_and_more.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      436 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0018_alter_dashboardstats_options.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0019_criteriatostatsm2m_recalculate.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      866 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0020_alter_dashboardstats_graph_key.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1256 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/0021_auto_20230210_1102.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    38766 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3216 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/modules.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/south_migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7765 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0001_initial_migration.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4217 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0002_add_sum_field_name.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5289 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0003_add_operation_field_name.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/south_migrations/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/templates/admin/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      565 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin/index.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2646 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/admin_charts.js
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2405 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/analytics.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/analytics_chart.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      196 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/analytics_user.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      364 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/chart_container.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      278 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/chart_containers.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      496 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/chart_data.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1150 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/chart_form.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/modules/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      497 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/modules/chart.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      269 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templates/include_nvd3.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.447213 django-admin-charts-1.3.1/admin_tools_stats/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1401 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/templatetags/admin_chart_tags.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/admin_tools_stats/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9968 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/test_admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      582 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/test_forms.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    67338 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    22209 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1030 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/tests/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1203 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7493 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/admin_tools_stats/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/.coveralls.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)       11 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4947 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/dashboard.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/demoproject/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/demoproject/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1214 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/fixtures/auth_user.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3065 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/fixtures/test_data.json
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/demoproject/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      972 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/migrations/0002_auto_20210221_0541.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/migrations/0003_testkid_author.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      384 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/migrations/0004_testkid_height.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      555 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8098 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/demoproject/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/demoproject/demoproject/templates/admin/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      542 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/templates/admin/base_site.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)       89 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/templates/home.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      206 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1437 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/demoproject/wsgi.py
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      255 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/menu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      101 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      489 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/demoproject/test_settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/django_admin_charts.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9991 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5140 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)      191 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       30 2024-04-12 13:45:33.000000 django-admin-charts-1.3.1/django_admin_charts.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.451213 django-admin-charts-1.3.1/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4666 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/docs/source/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/docs/source/_static/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    20957 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/Snímek obrazovky_2022-03-04_17-29-58.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   104856 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/Snímek obrazovky_2022-03-04_17-31-16.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)    55556 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/admin_dashboard.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)    50767 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/aoe_chart.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)    30123 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/bar_chart.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/docs/source/_static/images/
+-rw-rw-r--   0 petr      (1000) petr      (1000)   122086 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/images/admin_screenshot.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)    53145 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/_static/stacked_area_chart.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7480 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/conf.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/docs/source/developer-doc/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      364 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/developer-doc/modules.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1228 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/developer-doc/objects-description.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      221 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/developer-doc/pre-requisite.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      571 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/developer-doc/testing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      286 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/developer-doc.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/docs/source/includes/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      229 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/includes/introduction.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      783 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       93 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/docs/source/introduction.rst
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      260 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      201 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/mypy.ini
+-rw-rw-r--   0 petr      (1000) petr      (1000)       57 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/pyproject.toml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      175 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      403 2024-04-12 13:45:33.455212 django-admin-charts-1.3.1/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2690 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      114 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/test_requirements.txt
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      597 2024-04-12 13:45:32.000000 django-admin-charts-1.3.1/update_version.sh
```

### Comparing `django-admin-charts-1.3.0/.github/workflows/main.yml` & `django-admin-charts-1.3.1/.github/workflows/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,26 +18,37 @@
   # This workflow contains a single job called "build"
   tests:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
         
     strategy:
       matrix:
-        DJANGO_VERSION: ['3.2.*', '4.0.*', '4.1.*']
+        DJANGO_VERSION: ['3.2.*', '4.0.*', '4.1.*', '4.2.*']
         DB_ENGINE: [ 'postgres', 'mysql' ]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', '3.12']
         exclude:
-          - DJANGO_VERSION: '4.1.*'
-            python-version: '3.7'
-          - DJANGO_VERSION: '4.0.*'
-            python-version: '3.7'
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
+          - DJANGO_VERSION: '4.2.*'
+            python-version: '3.12'
+
+          - DJANGO_VERSION: '4.2.*'
+            python-version: '3.7'
       fail-fast: false
 
     services:
       postgres:
         image: postgres
         env:
           POSTGRES_PASSWORD: postgres
@@ -45,15 +56,15 @@
           --health-cmd pg_isready
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
         ports:
           - 5432:5432
       mysql:
-        image: mysql:5.7
+        image: mysql:8.3
         env:
           MYSQL_DATABASE: test_db
           MYSQL_USER: db_user
           MYSQL_PASSWORD: mysql
           MYSQL_ROOT_PASSWORD: rootpassword
         options: >-
           --health-cmd "mysqladmin ping"
@@ -79,17 +90,14 @@
         run: |
            pip install -e .
            pip install --upgrade --upgrade-strategy eager -r demoproject/requirements.txt
            pip install --upgrade --upgrade-strategy eager -r requirements.txt
            pip install Django==${{ matrix.DJANGO_VERSION }}
            pip install codecov
 
-      - name: Install django-jsonfield for older Django versions
-        if: ${{ matrix.DJANGO_VERSION == '2.2.*' || matrix.DJANGO_VERSION == '3.0.*' }}
-        run: pip install django-jsonfield
       - name: Testing
         run: |
           if [ "$matrix.DB_ENGINE" = 'mysql' ]; then
             mysql_tzinfo_to_sql /usr/share/zoneinfo | mysql -u db_user -p mysql mysql
           fi
           python manage.py makemigrations --check --dry-run
           python -W error::DeprecationWarning -m coverage run manage.py test
```

### Comparing `django-admin-charts-1.3.0/CHANGELOG.rst` & `django-admin-charts-1.3.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+1.3.1 (2024-04-12)
+------------------
+
+* fix for Django 5.0 DashboardStats admin add view
+
 1.3.0 (2023-02-10)
 ------------------
 
 * set BigAutoField as app default
 * remove support for Django<=3.1
 * fix hardcoded url in admin_charts.js template
```

### Comparing `django-admin-charts-1.3.0/MIT-LICENSE.txt` & `django-admin-charts-1.3.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/PKG-INFO` & `django-admin-charts-1.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,321 +1,320 @@
 Metadata-Version: 2.1
 Name: django-admin-charts
-Version: 1.3.0
+Version: 1.3.1
 Summary: django-admin-charts - Easily configurable charts statistics for `django-admin` and `django-admin-tools`
 Home-page: https://github.com/PetrDlouhy/django-admin-charts
 Author: Petr Dlouhy
 Author-email: petr.dlouhy@email.cz
 License: MIT License
-Description: ===================
-        Django admin charts
-        ===================
-        
-        :Description: Easily configurable charts statistics for ``django-admin`` and ``django-admin-tools``.
-        :Documentation: http://django-admin-charts.readthedocs.org/en/latest/
-        
-        .. image:: https://travis-ci.org/PetrDlouhy/django-admin-charts.svg?branch=master
-            :target: https://travis-ci.org/PetrDlouhy/django-admin-charts
-        
-        .. image:: https://img.shields.io/pypi/v/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/pyversions/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/pypi/l/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: License
-        
-        .. inclusion-marker-do-not-remove
-        
-        Create beautiful configurable charts from your models and display them on the ``django-admin`` index page or on ``django-admin-tools`` dashboard.
-        The charts are based on models and criterias defined through admin interface and some chart parameters are configurable in live view.
-        
-        This is application is fork of `django-admin-tools-stats <https://github.com/areski/django-admin-tools-stats/>`_ which has been reworked to display all charts through Ajax and made work with plain ``django-admin``. The ``django-admin-tools`` are supported but not needed.
-        
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/stacked_area_chart.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/bar_chart.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/aoe_chart.png
-        
-        ============
-        Requirements
-        ============
-        
-        * ``Django>=2.0``
-        * ``Python>3.6``
-        * PostgreSQL (MySQL is experimental, other databases probably not working but PRs are welcome)
-        * ``simplejson`` for charts based on ``DecimalField`` values
-        
-        ============
-        Installation
-        ============
-        
-        Install django-admin-charts with these commands:
-        
-            $ pip install django-admin-charts
-        
-        
-        
-        Basic setup for ``django-admin``
-        --------------------------------
-        
-        Add ``admin_tools_stats`` (the Django admin charts application) & ``django_nvd3`` into INSTALLED_APPS in settings.py:
-        
-        .. code:: python
-        
-            INSTALLED_APPS = (
-                'admin_tools_stats',  # this must be BEFORE 'admin_tools' and 'django.contrib.admin'
-                'django_nvd3',
-                ...
-                'django.contrib.admin',
-            )
-        
-        Register chart views in your ``urls.py``:
-        
-        .. code:: python
-        
-            from django.urls import include, path
-            urlpatterns = [
-                path('admin_tools_stats/', include('admin_tools_stats.urls')),
-            ]
-        
-        Ensure, you have ``default`` cache set up: https://docs.djangoproject.com/en/3.2/topics/cache/#memcached
-        
-        Run migrations:
-        
-        .. code:: sh
-        
-            $ python manage.py migrate
-        
-        Open Django admin root and add your ``Dashboard Stats`` configuration:
-        
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-29-58.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-31-16.png
-        
-        Then the charts will appear on the root of Django admin page as well as on analytics page (``/admin_tools_stats/analytics/``).
-        
-        ======================
-        Special configurations
-        ======================
-        
-        Update from ``django-admin-tools-stats``
-        ----------------------------------------
-        
-        Uninstall ``django-admin-tools-stats``.
-        
-        Follow ``django-admin-charts`` installation according to previous section. Especially pay attention to these steps:
-        - Move ``admin_tools_stats`` in ``INSTALLED_APPS`` before ``admin_tools`` and ``django.contrib.admin``.
-        - Configure ``urls.py``.
-        
-        Change ``DashboardCharts`` to ``DashboardChart`` in dashboard definition (this is recomended even if dummy class is left for compatibility reasons).
-        
-        Check any overridden template from ``admin_tools_stats`` or ``DashboardChart(s)`` class that might interfere with the changes.
-        
-        Configure javascript libraries
-        ----------------------------------------------------------
-        
-        By default the nvd3/d3 libraries are taken from unpkg.
-        If you want to install those libraries on your own, you can set their path by following settings:
-        
-        .. code:: python
-        
-           ADMIN_CHARTS_NVD3_JS_PATH = 'bow/nvd3/build/nv.d3.js'
-           ADMIN_CHARTS_NVD3_CSS_PATH = 'bow/nvd3/build/nv.d3.css'
-           ADMIN_CHARTS_D3_JS_PATH = 'bow/d3/d3.js'
-        
-        The settings can accept either full path (with http...) or there can be static file path.
-        Note that versions ``nvd3==1.8.6`` and ``d3==3.3.13`` are the only tested to be working.
-        
-        
-        Installation of javascript libraries with ``django-bower``
-        ----------------------------------------------------------
-        
-        Add ``django-bower`` to INSTALLED_APPS in settings.py:
-        
-        .. code:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'djangobower'
-            )
-        
-        Add the following properties to you settings.py file:
-        
-        .. code:: python
-        
-            # Specifie path to components root (you need to use absolute path)
-            BOWER_COMPONENTS_ROOT = os.path.join(PROJECT_ROOT, 'components')
-        
-        
-            BOWER_INSTALLED_APPS = (
-                'd3#3.3.13',
-                'nvd3#1.8.6',
-            )
-        
-        Add django-bower finder to your static file finders:
-        
-        .. code:: python
-        
-            STATICFILES_FINDERS = (
-                ...
-                'djangobower.finders.BowerFinder',
-            )
-        
-        Run the following commands. These will download nvd3.js and its dependencies using bower and throw them in to you static folder for access by your application:
-        
-        .. code:: sh
-        
-            $ python manage.py bower_install
-            $ python manage.py collectstatic
-        
-        
-        
-        Usage with ``django-admin-tools``
-        ----------------------------------
-        
-        Configure ``admin_tools``
-        
-        Add following code to dashboard.py:
-        
-        .. code:: python
-        
-            from admin_tools_stats.modules import DashboardChart, get_active_graph
-        
-            # append an app list module
-            self.children.append(modules.AppList(
-                _('Dashboard Stats Settings'),
-                models=('admin_tools_stats.*', ),
-            ))
-        
-            # Copy following code into your custom dashboard
-            # append following code after recent actions module or
-            # a link list module for "quick links"
-            if context['request'].user.has_perm('admin_tools_stats.view_dashboardstats'):
-                    graph_list = get_active_graph()
-                else:
-                    graph_list = []
-        
-            for i in graph_list:
-                kwargs = {}
-                kwargs['require_chart_jscss'] = True
-                kwargs['graph_key'] = i.graph_key
-        
-                for key in context['request'].POST:
-                    if key.startswith('select_box_'):
-                        kwargs[key] = context['request'].POST[key]
-        
-                self.children.append(DashboardChart(**kwargs))
-        
-        
-        You may also need to add some includes to your template admin base, see an example on the demo project::
-        
-            demoproject/demoproject/templates/admin/base_site.html
-        
-        
-        Usage on DB that doesn't support JSONFields
-        -------------------------------------------
-        
-        You can add following line to your settings in order to use JSONField from `django-jsonfield` instead of native Django JSONField:
-        
-        .. code:: python
-        
-           ADMIN_CHARTS_USE_JSONFIELD = False
-        
-        This can become handy, when deploying on MySQL<5.7 (Like AWS RDS Aurora)
-        
-        
-        ============
-        Running demo
-        ============
-        
-        Run following commands:
-        
-        .. code:: sh
-        
-           export DB_ENGINE='sqlite'
-           pip install -r requirements.txt
-           python manage.py migrate
-           python manage.py loaddata demoproject/fixtures/auth_user.json
-           python manage.py loaddata demoproject/fixtures/test_data.json
-           python manage.py bower install
-           python manage.py runserver
-        
-        And log in with username `admin` and password `admin` to the `localhost:8000/admin` site.
-        
-        ===========
-        Development
-        ===========
-        
-        Dependencies
-        ------------
-        
-        django-admin-charts is a django based application, the major requirements are:
-        
-        - django-jsonfield
-        - django-nvd3
-        - django-bower
-        
-        
-        Running tests
-        -------------
-        
-        Test can be run with:
-        
-        .. code:: sh
-        
-            DB_ENGINE="postgres" coverage run ./manage.py test --keepdb
-        
-        
-        Contributing
-        ------------
-        
-        If you've found a bug, add a feature or improve django-admin-charts and
-        think it is useful then please consider contributing.
-        Patches, pull requests or just suggestions are always welcome!
-        
-        Source code: http://github.com/PetrDlouhy/django-admin-charts
-        
-        Bug tracker: https://github.com/PetrDlouhy/django-admin-charts/issues
-        
-        
-        Debugging charts
-        ----------------
-        
-        For chart data view (/admin_tools_stats/chart_data/payments/) the URL query
-        parameter `&debug=True` can be added, in order to get Django debug page or
-        Django debug toolbar.
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available on 'Read the Docs':
-        http://readthedocs.org/docs/django-admin-charts/
-        
-        
-        License
-        -------
-        
-        django-admin-charts is licensed under MIT, see ``MIT-LICENSE.txt``.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+
+===================
+Django admin charts
+===================
+
+:Description: Easily configurable charts statistics for ``django-admin`` and ``django-admin-tools``.
+:Documentation: http://django-admin-charts.readthedocs.org/en/latest/
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml/badge.svg?branch=master
+    :target: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml
+
+.. image:: https://img.shields.io/pypi/v/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/dm/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/pyversions/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/l/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: License
+
+.. inclusion-marker-do-not-remove
+
+Create beautiful configurable charts from your models and display them on the ``django-admin`` index page or on ``django-admin-tools`` dashboard.
+The charts are based on models and criterias defined through admin interface and some chart parameters are configurable in live view.
+
+This is application is fork of `django-admin-tools-stats <https://github.com/areski/django-admin-tools-stats/>`_ which has been reworked to display all charts through Ajax and made work with plain ``django-admin``. The ``django-admin-tools`` are supported but not needed.
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/stacked_area_chart.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/bar_chart.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/aoe_chart.png
+
+============
+Requirements
+============
+
+* ``Django>=2.0``
+* ``Python>3.6``
+* PostgreSQL (MySQL is experimental, other databases probably not working but PRs are welcome)
+* ``simplejson`` for charts based on ``DecimalField`` values
+
+============
+Installation
+============
+
+Install django-admin-charts with these commands:
+
+    $ pip install django-admin-charts
+
+
+
+Basic setup for ``django-admin``
+--------------------------------
+
+Add ``admin_tools_stats`` (the Django admin charts application) & ``django_nvd3`` into INSTALLED_APPS in settings.py:
+
+.. code:: python
+
+    INSTALLED_APPS = (
+        'admin_tools_stats',  # this must be BEFORE 'admin_tools' and 'django.contrib.admin'
+        'django_nvd3',
+        ...
+        'django.contrib.admin',
+    )
+
+Register chart views in your ``urls.py``:
+
+.. code:: python
+
+    from django.urls import include, path
+    urlpatterns = [
+        path('admin_tools_stats/', include('admin_tools_stats.urls')),
+    ]
+
+Ensure, you have ``default`` cache set up: https://docs.djangoproject.com/en/3.2/topics/cache/#memcached
+
+Run migrations:
+
+.. code:: sh
+
+    $ python manage.py migrate
+
+Open Django admin root and add your ``Dashboard Stats`` configuration:
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-29-58.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-31-16.png
+
+Then the charts will appear on the root of Django admin page as well as on analytics page (``/admin_tools_stats/analytics/``).
+
+======================
+Special configurations
+======================
+
+Update from ``django-admin-tools-stats``
+----------------------------------------
+
+Uninstall ``django-admin-tools-stats``.
+
+Follow ``django-admin-charts`` installation according to previous section. Especially pay attention to these steps:
+- Move ``admin_tools_stats`` in ``INSTALLED_APPS`` before ``admin_tools`` and ``django.contrib.admin``.
+- Configure ``urls.py``.
+
+Change ``DashboardCharts`` to ``DashboardChart`` in dashboard definition (this is recomended even if dummy class is left for compatibility reasons).
+
+Check any overridden template from ``admin_tools_stats`` or ``DashboardChart(s)`` class that might interfere with the changes.
+
+Configure javascript libraries
+----------------------------------------------------------
+
+By default the nvd3/d3 libraries are taken from unpkg.
+If you want to install those libraries on your own, you can set their path by following settings:
+
+.. code:: python
+
+   ADMIN_CHARTS_NVD3_JS_PATH = 'bow/nvd3/build/nv.d3.js'
+   ADMIN_CHARTS_NVD3_CSS_PATH = 'bow/nvd3/build/nv.d3.css'
+   ADMIN_CHARTS_D3_JS_PATH = 'bow/d3/d3.js'
+
+The settings can accept either full path (with http...) or there can be static file path.
+Note that versions ``nvd3==1.8.6`` and ``d3==3.3.13`` are the only tested to be working.
+
+
+Installation of javascript libraries with ``django-bower``
+----------------------------------------------------------
+
+Add ``django-bower`` to INSTALLED_APPS in settings.py:
+
+.. code:: python
+
+    INSTALLED_APPS = (
+        ...
+        'djangobower'
+    )
+
+Add the following properties to you settings.py file:
+
+.. code:: python
+
+    # Specifie path to components root (you need to use absolute path)
+    BOWER_COMPONENTS_ROOT = os.path.join(PROJECT_ROOT, 'components')
+
+
+    BOWER_INSTALLED_APPS = (
+        'd3#3.3.13',
+        'nvd3#1.8.6',
+    )
+
+Add django-bower finder to your static file finders:
+
+.. code:: python
+
+    STATICFILES_FINDERS = (
+        ...
+        'djangobower.finders.BowerFinder',
+    )
+
+Run the following commands. These will download nvd3.js and its dependencies using bower and throw them in to you static folder for access by your application:
+
+.. code:: sh
+
+    $ python manage.py bower_install
+    $ python manage.py collectstatic
+
+
+
+Usage with ``django-admin-tools``
+----------------------------------
+
+Configure ``admin_tools``
+
+Add following code to dashboard.py:
+
+.. code:: python
+
+    from admin_tools_stats.modules import DashboardChart, get_active_graph
+
+    # append an app list module
+    self.children.append(modules.AppList(
+        _('Dashboard Stats Settings'),
+        models=('admin_tools_stats.*', ),
+    ))
+
+    # Copy following code into your custom dashboard
+    # append following code after recent actions module or
+    # a link list module for "quick links"
+    if context['request'].user.has_perm('admin_tools_stats.view_dashboardstats'):
+            graph_list = get_active_graph()
+        else:
+            graph_list = []
+
+    for i in graph_list:
+        kwargs = {}
+        kwargs['require_chart_jscss'] = True
+        kwargs['graph_key'] = i.graph_key
+
+        for key in context['request'].POST:
+            if key.startswith('select_box_'):
+                kwargs[key] = context['request'].POST[key]
+
+        self.children.append(DashboardChart(**kwargs))
+
+
+You may also need to add some includes to your template admin base, see an example on the demo project::
+
+    demoproject/demoproject/templates/admin/base_site.html
+
+
+Usage on DB that doesn't support JSONFields
+-------------------------------------------
+
+You can add following line to your settings in order to use JSONField from `django-jsonfield` instead of native Django JSONField:
+
+.. code:: python
+
+   ADMIN_CHARTS_USE_JSONFIELD = False
+
+This can become handy, when deploying on MySQL<5.7 (Like AWS RDS Aurora)
+
+
+============
+Running demo
+============
+
+Run following commands:
+
+.. code:: sh
+
+   export DB_ENGINE='sqlite'
+   pip install -r requirements.txt
+   python manage.py migrate
+   python manage.py loaddata demoproject/fixtures/auth_user.json
+   python manage.py loaddata demoproject/fixtures/test_data.json
+   python manage.py bower install
+   python manage.py runserver
+
+And log in with username `admin` and password `admin` to the `localhost:8000/admin` site.
+
+===========
+Development
+===========
+
+Dependencies
+------------
+
+django-admin-charts is a django based application, the major requirements are:
+
+- django-jsonfield
+- django-nvd3
+- django-bower
+
+
+Running tests
+-------------
+
+Test can be run with:
+
+.. code:: sh
+
+    DB_ENGINE="postgres" coverage run ./manage.py test --keepdb
+
+
+Contributing
+------------
+
+If you've found a bug, add a feature or improve django-admin-charts and
+think it is useful then please consider contributing.
+Patches, pull requests or just suggestions are always welcome!
+
+Source code: http://github.com/PetrDlouhy/django-admin-charts
+
+Bug tracker: https://github.com/PetrDlouhy/django-admin-charts/issues
+
+
+Debugging charts
+----------------
+
+For chart data view (/admin_tools_stats/chart_data/payments/) the URL query
+parameter `&debug=True` can be added, in order to get Django debug page or
+Django debug toolbar.
+
+
+Documentation
+-------------
+
+Documentation is available on 'Read the Docs':
+http://readthedocs.org/docs/django-admin-charts/
+
+
+License
+-------
+
+django-admin-charts is licensed under MIT, see ``MIT-LICENSE.txt``.
```

### Comparing `django-admin-charts-1.3.0/README.rst` & `django-admin-charts-1.3.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ===================
 Django admin charts
 ===================
 
 :Description: Easily configurable charts statistics for ``django-admin`` and ``django-admin-tools``.
 :Documentation: http://django-admin-charts.readthedocs.org/en/latest/
 
-.. image:: https://travis-ci.org/PetrDlouhy/django-admin-charts.svg?branch=master
-    :target: https://travis-ci.org/PetrDlouhy/django-admin-charts
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml/badge.svg?branch=master
+    :target: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml
 
 .. image:: https://img.shields.io/pypi/v/django-admin-charts.svg
   :target: https://pypi.python.org/pypi/django-admin-charts/
   :alt: Latest Version
 
 .. image:: https://img.shields.io/pypi/dm/django-admin-charts.svg
   :target: https://pypi.python.org/pypi/django-admin-charts/
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/__init__.py` & `django-admin-charts-1.3.1/admin_tools_stats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # Copyright (C) 2011-2014 Star2Billing S.L.
 #
 # The Initial Developer of the Original Code is
 # Arezqui Belaid <info@star2billing.com>
 #
 
 # edit also docs/source/conf.py and update requirements.txt
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 __author__ = "Petr Dlouhy"
 __contact__ = "petr.dlouhy@emai.cz"
 __homepage__ = "https://github.com/PetrDlouhy"
 __docformat__ = "restructuredtext"
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/admin.py` & `django-admin-charts-1.3.1/admin_tools_stats/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,17 +82,20 @@
     def criteria__criteria_dynamic_mapping_preview(self, obj):
         return obj.criteria.criteria_dynamic_mapping_preview()
 
 
 class DashboardStatsForm(forms.ModelForm):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.fields["default_multiseries_criteria"].queryset = CriteriaToStatsM2M.objects.filter(
-            stats=self.instance,
-        )
+        if self.instance.pk:
+            self.fields["default_multiseries_criteria"].queryset = (
+                CriteriaToStatsM2M.objects.filter(
+                    stats=self.instance,
+                )
+            )
 
 
 @admin.register(DashboardStats)
 class DashboardStatsAdmin(admin.ModelAdmin):
     """
     Allows the administrator to view and modify certain attributes
     of a DashboardStats.
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/app_label_renamer.py` & `django-admin-charts-1.3.1/admin_tools_stats/app_label_renamer.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/fixtures/20_dashboardstatscriteria_call_type.json` & `django-admin-charts-1.3.1/admin_tools_stats/fixtures/20_dashboardstatscriteria_call_type.json`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/fixtures/initial_data.json` & `django-admin-charts-1.3.1/admin_tools_stats/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/forms.py` & `django-admin-charts-1.3.1/admin_tools_stats/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,19 @@
                 multiple_series.select_related("stats__default_multiseries_criteria", "criteria")
                 .order_by("order")
                 .values_list("id", "criteria__criteria_name")
             )
             self.fields["select_box_multiple_series"] = forms.ChoiceField(
                 label="Divide",
                 choices=[("", "-------")] + list(choices),
-                initial=stats.default_multiseries_criteria.id
-                if stats.default_multiseries_criteria
-                else None,
+                initial=(
+                    stats.default_multiseries_criteria.id
+                    if stats.default_multiseries_criteria
+                    else None
+                ),
             )
             self.fields["select_box_multiple_series"].widget.attrs[
                 "class"
             ] = "chart-input select_box_multiple_series"
 
         if len(stats.allowed_type_operation_field_name) > 1:
             self.fields["select_box_operation"] = forms.ChoiceField(
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/management/commands/recalculate_charts.py` & `django-admin-charts-1.3.1/admin_tools_stats/management/commands/recalculate_charts.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0001_initial.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0002_auto_20190920_1058.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0002_auto_20190920_1058.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0003_auto_20191007_0950.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0003_auto_20191007_0950.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0004_dashboardstats_y_tick_format.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0004_dashboardstats_y_tick_format.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0005_auto_20200203_1537.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0005_auto_20200203_1537.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0006_auto_20200205_0944.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0006_auto_20200205_0944.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0007_auto_20200205_1054.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0007_auto_20200205_1054.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0008_auto_20200911_1400.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0008_auto_20200911_1400.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0009_auto_20200928_1003.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0009_auto_20200928_1003.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0010_dashboardstats_show_to_users.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0010_dashboardstats_show_to_users.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0011_auto_20210204_1206.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0011_auto_20210204_1206.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0012_auto_20210207_0859.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0012_auto_20210207_0859.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0013_auto_20210221_1247.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0013_auto_20210221_1247.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0014_auto_20211122_1511.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0014_auto_20211122_1511.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0015_auto_20211209_0822.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0015_auto_20211209_0822.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0017_alter_dashboardstats_options_and_more.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0017_alter_dashboardstats_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0019_criteriatostatsm2m_recalculate.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0019_criteriatostatsm2m_recalculate.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0020_alter_dashboardstats_graph_key.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0020_alter_dashboardstats_graph_key.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/migrations/0021_auto_20230210_1102.py` & `django-admin-charts-1.3.1/admin_tools_stats/migrations/0021_auto_20230210_1102.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/models.py` & `django-admin-charts-1.3.1/admin_tools_stats/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,15 +399,15 @@
             "See description of possible values"
             "</a>.",
         ),
         null=True,
         blank=True,
         default=None,
     )
-    criteria = models.ManyToManyField(
+    criteria: models.ManyToManyField = models.ManyToManyField(
         DashboardStatsCriteria, blank=True, through="CriteriaToStatsM2M"
     )
     default_multiseries_criteria = models.ForeignKey(
         "CriteriaToStatsM2M",
         blank=True,
         null=True,
         on_delete=models.SET_NULL,
@@ -433,20 +433,24 @@
 
     def allowed_chart_types_choices(self):
         return (cht for cht in chart_types if cht[0] in self.allowed_chart_types)
 
     def get_model(self):
         return apps.get_model(self.model_app_name, self.model_name)
 
+    def get_queryset(self):
+        qs = self.get_model().objects
+        return qs
+
     def get_operation_field(self, operation):
-        query = self.get_model().objects.all().query
+        query = self.get_queryset().all().query
         return query.resolve_ref(operation).field
 
     def get_date_field(self):
-        query = self.get_model().objects.all().query
+        query = self.get_queryset().all().query
         return query.resolve_ref(self.date_field_name).field
 
     def clean(self, *args, **kwargs):
         errors = {}
         model = None
         try:
             apps.get_app_config(self.model_app_name)
@@ -522,15 +526,14 @@
         time_since: datetime.datetime,
         time_until: datetime.datetime,
         operation_choice: Optional[str],
         operation_field_choice: Optional[str],
         interval: Interval,
     ):
         """Get the stats time series"""
-        model_name = apps.get_model(self.model_app_name, self.model_name)
         kwargs = {}
         dynamic_kwargs: List[Optional[Q]] = []
         if not user.has_perm("admin_tools_stats.view_dashboardstats") and self.user_field_name:
             kwargs[self.user_field_name] = user
         for m2m in all_criteria:
             criteria = m2m.criteria
             # fixed mapping value passed info kwargs
@@ -592,15 +595,15 @@
                 i += 1
                 aggregate_dict["agg_%i" % i] = self.get_operation(
                     operation_choice, operation_field_choice, dkwargs
                 )
 
         # TODO: maybe backport values_list support back to django-qsstats-magic and use it again for the query
         time_range = {"%s__range" % self.date_field_name: (time_since, time_until)}
-        qs = model_name.objects
+        qs = self.get_queryset()
         qs = qs.filter(**time_range)
         qs = qs.filter(**kwargs)
         if isinstance(self.get_date_field(), DateTimeField):
             tzinfo_kwargs = {"tzinfo": get_charts_timezone()}
         else:
             tzinfo_kwargs = {}
         qs = qs.annotate(d=Trunc(self.date_field_name, interval.val(), **tzinfo_kwargs))
@@ -877,43 +880,42 @@
     )
 
     def get_dynamic_criteria_field_name(self):
         if self.prefix:
             return self.prefix + self.criteria.dynamic_criteria_field_name
         return self.criteria.dynamic_criteria_field_name
 
-    def get_dynamic_field(self, model):
+    def get_dynamic_field(self):
         field_name = self.get_dynamic_criteria_field_name()
-        query = model.objects.all().query
+        query = self.stats.get_queryset().all().query
         return query.resolve_ref(field_name).field
 
     @memoize(60 * 60 * 24 * 7)
     def _get_dynamic_choices(
         self,
         time_since: datetime.datetime,
         time_until: datetime.datetime,
         count_limit: Optional[int] = None,
         operation_choice=None,
         operation_field_choice=None,
         user=None,
     ) -> "Optional[OrderedDict[str, Tuple[Union[str, bool, List[str]], str]]]":
-        model = self.stats.get_model()
         field_name = self.get_dynamic_criteria_field_name()
         if self.criteria.criteria_dynamic_mapping:
             return OrderedDict(self.criteria.criteria_dynamic_mapping)
         if field_name:
             if field_name.endswith("__isnull"):
                 return OrderedDict(
                     (
                         ("", ("", "All")),
                         ("True", (True, "Blank")),
                         ("False", (False, "Non blank")),
                     )
                 )
-            field = self.get_dynamic_field(model)
+            field = self.get_dynamic_field()
             if field.__class__ == models.BooleanField:
                 return OrderedDict(
                     (
                         ("", ("", "All")),
                         ("True", (True, "True")),
                         ("False", (False, "False")),
                     )
@@ -936,15 +938,15 @@
                             or time_until.tzinfo.utcoffset(time_until) is None
                         ):
                             time_until = time_until.astimezone(get_charts_timezone()).replace(
                                 hour=23, minute=59
                             )
                         end_time = time_until
                         date_filters["%s__lte" % self.stats.date_field_name] = end_time
-                choices_queryset = model.objects.filter(
+                choices_queryset = self.stats.get_queryset().filter(
                     **date_filters,
                 )
                 if user and not user.has_perm("admin_tools_stats.view_dashboardstats"):
                     if not self.stats.user_field_name:
                         raise Exception(
                             "User field must be defined to enable charts for non-superusers"
                         )
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/modules.py` & `django-admin-charts-1.3.1/admin_tools_stats/modules.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0001_initial_migration.py` & `django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0001_initial_migration.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0002_add_sum_field_name.py` & `django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0002_add_sum_field_name.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/south_migrations/0003_add_operation_field_name.py` & `django-admin-charts-1.3.1/admin_tools_stats/south_migrations/0003_add_operation_field_name.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/templates/admin/index.html` & `django-admin-charts-1.3.1/admin_tools_stats/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/admin_charts.js` & `django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/admin_charts.js`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/analytics.html` & `django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/analytics.html`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/templates/admin_tools_stats/chart_form.html` & `django-admin-charts-1.3.1/admin_tools_stats/templates/admin_tools_stats/chart_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/templatetags/admin_chart_tags.py` & `django-admin-charts-1.3.1/admin_tools_stats/templatetags/admin_chart_tags.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/tests/test_admin.py` & `django-admin-charts-1.3.1/admin_tools_stats/tests/test_admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,22 @@
         self.assertEqual(response.status_code, 200)
 
     def test_admin_tools_stats_dashboardstatscriteria(self):
         """Test function to check dashboardstatscriteria admin pages"""
         response = self.client.get("/admin/admin_tools_stats/dashboardstatscriteria/")
         self.assertEqual(response.status_code, 200)
 
+    def test_add_view(self):
+        url = reverse("admin:admin_tools_stats_dashboardstats_add")
+        response = self.client.get(url)
+        self.assertEqual(response.status_code, 200)
+        url = reverse("admin:admin_tools_stats_dashboardstatscriteria_add")
+        response = self.client.get(url)
+        self.assertEqual(response.status_code, 200)
+
 
 class AdminToolsStatsAdminCharts(BaseSuperuserAuthenticatedClient):
     def test_admin_dashboard_page(self):
         """Test function to check dashboardstatscriteria admin pages"""
         stats = baker.make(
             "DashboardStats",
             date_field_name="date_joined",
```

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/tests/test_forms.py` & `django-admin-charts-1.3.1/admin_tools_stats/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/tests/test_models.py` & `django-admin-charts-1.3.1/admin_tools_stats/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/tests/test_views.py` & `django-admin-charts-1.3.1/admin_tools_stats/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/tests/utils.py` & `django-admin-charts-1.3.1/admin_tools_stats/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/urls.py` & `django-admin-charts-1.3.1/admin_tools_stats/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/utils.py` & `django-admin-charts-1.3.1/admin_tools_stats/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/admin_tools_stats/views.py` & `django-admin-charts-1.3.1/admin_tools_stats/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/dashboard.py` & `django-admin-charts-1.3.1/demoproject/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/fixtures/auth_user.json` & `django-admin-charts-1.3.1/demoproject/demoproject/fixtures/auth_user.json`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/fixtures/test_data.json` & `django-admin-charts-1.3.1/demoproject/demoproject/fixtures/test_data.json`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/migrations/0001_initial.py` & `django-admin-charts-1.3.1/demoproject/demoproject/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/migrations/0002_auto_20210221_0541.py` & `django-admin-charts-1.3.1/demoproject/demoproject/migrations/0002_auto_20210221_0541.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/migrations/0003_testkid_author.py` & `django-admin-charts-1.3.1/demoproject/demoproject/migrations/0003_testkid_author.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/models.py` & `django-admin-charts-1.3.1/demoproject/demoproject/models.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/settings.py` & `django-admin-charts-1.3.1/demoproject/demoproject/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/templates/admin/base_site.html` & `django-admin-charts-1.3.1/demoproject/demoproject/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/urls.py` & `django-admin-charts-1.3.1/demoproject/demoproject/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/demoproject/demoproject/wsgi.py` & `django-admin-charts-1.3.1/demoproject/demoproject/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Usually you will have the standard Django WSGI application here, but it also
 might make sense to replace the whole Django WSGI application with a custom one
 that later delegates to the Django one. For example, you could introduce WSGI
 middleware here, or combine a Django application with an application of another
 framework.
 
 """
+
 import os
 
 from django.core.wsgi import get_wsgi_application
 
 
 # We defer to a DJANGO_SETTINGS_MODULE already in the environment. This breaks
 # if running multiple sites in the same mod_wsgi process. To fix this, use
```

### Comparing `django-admin-charts-1.3.0/demoproject/menu.py` & `django-admin-charts-1.3.1/demoproject/menu.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/django_admin_charts.egg-info/PKG-INFO` & `django-admin-charts-1.3.1/django_admin_charts.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,321 +1,320 @@
 Metadata-Version: 2.1
 Name: django-admin-charts
-Version: 1.3.0
+Version: 1.3.1
 Summary: django-admin-charts - Easily configurable charts statistics for `django-admin` and `django-admin-tools`
 Home-page: https://github.com/PetrDlouhy/django-admin-charts
 Author: Petr Dlouhy
 Author-email: petr.dlouhy@email.cz
 License: MIT License
-Description: ===================
-        Django admin charts
-        ===================
-        
-        :Description: Easily configurable charts statistics for ``django-admin`` and ``django-admin-tools``.
-        :Documentation: http://django-admin-charts.readthedocs.org/en/latest/
-        
-        .. image:: https://travis-ci.org/PetrDlouhy/django-admin-charts.svg?branch=master
-            :target: https://travis-ci.org/PetrDlouhy/django-admin-charts
-        
-        .. image:: https://img.shields.io/pypi/v/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Latest Version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/pyversions/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/pypi/l/django-admin-charts.svg
-          :target: https://pypi.python.org/pypi/django-admin-charts/
-          :alt: License
-        
-        .. inclusion-marker-do-not-remove
-        
-        Create beautiful configurable charts from your models and display them on the ``django-admin`` index page or on ``django-admin-tools`` dashboard.
-        The charts are based on models and criterias defined through admin interface and some chart parameters are configurable in live view.
-        
-        This is application is fork of `django-admin-tools-stats <https://github.com/areski/django-admin-tools-stats/>`_ which has been reworked to display all charts through Ajax and made work with plain ``django-admin``. The ``django-admin-tools`` are supported but not needed.
-        
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/stacked_area_chart.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/bar_chart.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/aoe_chart.png
-        
-        ============
-        Requirements
-        ============
-        
-        * ``Django>=2.0``
-        * ``Python>3.6``
-        * PostgreSQL (MySQL is experimental, other databases probably not working but PRs are welcome)
-        * ``simplejson`` for charts based on ``DecimalField`` values
-        
-        ============
-        Installation
-        ============
-        
-        Install django-admin-charts with these commands:
-        
-            $ pip install django-admin-charts
-        
-        
-        
-        Basic setup for ``django-admin``
-        --------------------------------
-        
-        Add ``admin_tools_stats`` (the Django admin charts application) & ``django_nvd3`` into INSTALLED_APPS in settings.py:
-        
-        .. code:: python
-        
-            INSTALLED_APPS = (
-                'admin_tools_stats',  # this must be BEFORE 'admin_tools' and 'django.contrib.admin'
-                'django_nvd3',
-                ...
-                'django.contrib.admin',
-            )
-        
-        Register chart views in your ``urls.py``:
-        
-        .. code:: python
-        
-            from django.urls import include, path
-            urlpatterns = [
-                path('admin_tools_stats/', include('admin_tools_stats.urls')),
-            ]
-        
-        Ensure, you have ``default`` cache set up: https://docs.djangoproject.com/en/3.2/topics/cache/#memcached
-        
-        Run migrations:
-        
-        .. code:: sh
-        
-            $ python manage.py migrate
-        
-        Open Django admin root and add your ``Dashboard Stats`` configuration:
-        
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-29-58.png
-        .. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-31-16.png
-        
-        Then the charts will appear on the root of Django admin page as well as on analytics page (``/admin_tools_stats/analytics/``).
-        
-        ======================
-        Special configurations
-        ======================
-        
-        Update from ``django-admin-tools-stats``
-        ----------------------------------------
-        
-        Uninstall ``django-admin-tools-stats``.
-        
-        Follow ``django-admin-charts`` installation according to previous section. Especially pay attention to these steps:
-        - Move ``admin_tools_stats`` in ``INSTALLED_APPS`` before ``admin_tools`` and ``django.contrib.admin``.
-        - Configure ``urls.py``.
-        
-        Change ``DashboardCharts`` to ``DashboardChart`` in dashboard definition (this is recomended even if dummy class is left for compatibility reasons).
-        
-        Check any overridden template from ``admin_tools_stats`` or ``DashboardChart(s)`` class that might interfere with the changes.
-        
-        Configure javascript libraries
-        ----------------------------------------------------------
-        
-        By default the nvd3/d3 libraries are taken from unpkg.
-        If you want to install those libraries on your own, you can set their path by following settings:
-        
-        .. code:: python
-        
-           ADMIN_CHARTS_NVD3_JS_PATH = 'bow/nvd3/build/nv.d3.js'
-           ADMIN_CHARTS_NVD3_CSS_PATH = 'bow/nvd3/build/nv.d3.css'
-           ADMIN_CHARTS_D3_JS_PATH = 'bow/d3/d3.js'
-        
-        The settings can accept either full path (with http...) or there can be static file path.
-        Note that versions ``nvd3==1.8.6`` and ``d3==3.3.13`` are the only tested to be working.
-        
-        
-        Installation of javascript libraries with ``django-bower``
-        ----------------------------------------------------------
-        
-        Add ``django-bower`` to INSTALLED_APPS in settings.py:
-        
-        .. code:: python
-        
-            INSTALLED_APPS = (
-                ...
-                'djangobower'
-            )
-        
-        Add the following properties to you settings.py file:
-        
-        .. code:: python
-        
-            # Specifie path to components root (you need to use absolute path)
-            BOWER_COMPONENTS_ROOT = os.path.join(PROJECT_ROOT, 'components')
-        
-        
-            BOWER_INSTALLED_APPS = (
-                'd3#3.3.13',
-                'nvd3#1.8.6',
-            )
-        
-        Add django-bower finder to your static file finders:
-        
-        .. code:: python
-        
-            STATICFILES_FINDERS = (
-                ...
-                'djangobower.finders.BowerFinder',
-            )
-        
-        Run the following commands. These will download nvd3.js and its dependencies using bower and throw them in to you static folder for access by your application:
-        
-        .. code:: sh
-        
-            $ python manage.py bower_install
-            $ python manage.py collectstatic
-        
-        
-        
-        Usage with ``django-admin-tools``
-        ----------------------------------
-        
-        Configure ``admin_tools``
-        
-        Add following code to dashboard.py:
-        
-        .. code:: python
-        
-            from admin_tools_stats.modules import DashboardChart, get_active_graph
-        
-            # append an app list module
-            self.children.append(modules.AppList(
-                _('Dashboard Stats Settings'),
-                models=('admin_tools_stats.*', ),
-            ))
-        
-            # Copy following code into your custom dashboard
-            # append following code after recent actions module or
-            # a link list module for "quick links"
-            if context['request'].user.has_perm('admin_tools_stats.view_dashboardstats'):
-                    graph_list = get_active_graph()
-                else:
-                    graph_list = []
-        
-            for i in graph_list:
-                kwargs = {}
-                kwargs['require_chart_jscss'] = True
-                kwargs['graph_key'] = i.graph_key
-        
-                for key in context['request'].POST:
-                    if key.startswith('select_box_'):
-                        kwargs[key] = context['request'].POST[key]
-        
-                self.children.append(DashboardChart(**kwargs))
-        
-        
-        You may also need to add some includes to your template admin base, see an example on the demo project::
-        
-            demoproject/demoproject/templates/admin/base_site.html
-        
-        
-        Usage on DB that doesn't support JSONFields
-        -------------------------------------------
-        
-        You can add following line to your settings in order to use JSONField from `django-jsonfield` instead of native Django JSONField:
-        
-        .. code:: python
-        
-           ADMIN_CHARTS_USE_JSONFIELD = False
-        
-        This can become handy, when deploying on MySQL<5.7 (Like AWS RDS Aurora)
-        
-        
-        ============
-        Running demo
-        ============
-        
-        Run following commands:
-        
-        .. code:: sh
-        
-           export DB_ENGINE='sqlite'
-           pip install -r requirements.txt
-           python manage.py migrate
-           python manage.py loaddata demoproject/fixtures/auth_user.json
-           python manage.py loaddata demoproject/fixtures/test_data.json
-           python manage.py bower install
-           python manage.py runserver
-        
-        And log in with username `admin` and password `admin` to the `localhost:8000/admin` site.
-        
-        ===========
-        Development
-        ===========
-        
-        Dependencies
-        ------------
-        
-        django-admin-charts is a django based application, the major requirements are:
-        
-        - django-jsonfield
-        - django-nvd3
-        - django-bower
-        
-        
-        Running tests
-        -------------
-        
-        Test can be run with:
-        
-        .. code:: sh
-        
-            DB_ENGINE="postgres" coverage run ./manage.py test --keepdb
-        
-        
-        Contributing
-        ------------
-        
-        If you've found a bug, add a feature or improve django-admin-charts and
-        think it is useful then please consider contributing.
-        Patches, pull requests or just suggestions are always welcome!
-        
-        Source code: http://github.com/PetrDlouhy/django-admin-charts
-        
-        Bug tracker: https://github.com/PetrDlouhy/django-admin-charts/issues
-        
-        
-        Debugging charts
-        ----------------
-        
-        For chart data view (/admin_tools_stats/chart_data/payments/) the URL query
-        parameter `&debug=True` can be added, in order to get Django debug page or
-        Django debug toolbar.
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is available on 'Read the Docs':
-        http://readthedocs.org/docs/django-admin-charts/
-        
-        
-        License
-        -------
-        
-        django-admin-charts is licensed under MIT, see ``MIT-LICENSE.txt``.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+
+===================
+Django admin charts
+===================
+
+:Description: Easily configurable charts statistics for ``django-admin`` and ``django-admin-tools``.
+:Documentation: http://django-admin-charts.readthedocs.org/en/latest/
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml/badge.svg?branch=master
+    :target: https://github.com/PetrDlouhy/django-admin-charts/actions/workflows/main.yml
+
+.. image:: https://img.shields.io/pypi/v/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Latest Version
+
+.. image:: https://img.shields.io/pypi/dm/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/pyversions/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/l/django-admin-charts.svg
+  :target: https://pypi.python.org/pypi/django-admin-charts/
+  :alt: License
+
+.. inclusion-marker-do-not-remove
+
+Create beautiful configurable charts from your models and display them on the ``django-admin`` index page or on ``django-admin-tools`` dashboard.
+The charts are based on models and criterias defined through admin interface and some chart parameters are configurable in live view.
+
+This is application is fork of `django-admin-tools-stats <https://github.com/areski/django-admin-tools-stats/>`_ which has been reworked to display all charts through Ajax and made work with plain ``django-admin``. The ``django-admin-tools`` are supported but not needed.
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/stacked_area_chart.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/bar_chart.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/aoe_chart.png
+
+============
+Requirements
+============
+
+* ``Django>=2.0``
+* ``Python>3.6``
+* PostgreSQL (MySQL is experimental, other databases probably not working but PRs are welcome)
+* ``simplejson`` for charts based on ``DecimalField`` values
+
+============
+Installation
+============
+
+Install django-admin-charts with these commands:
+
+    $ pip install django-admin-charts
+
+
+
+Basic setup for ``django-admin``
+--------------------------------
+
+Add ``admin_tools_stats`` (the Django admin charts application) & ``django_nvd3`` into INSTALLED_APPS in settings.py:
+
+.. code:: python
+
+    INSTALLED_APPS = (
+        'admin_tools_stats',  # this must be BEFORE 'admin_tools' and 'django.contrib.admin'
+        'django_nvd3',
+        ...
+        'django.contrib.admin',
+    )
+
+Register chart views in your ``urls.py``:
+
+.. code:: python
+
+    from django.urls import include, path
+    urlpatterns = [
+        path('admin_tools_stats/', include('admin_tools_stats.urls')),
+    ]
+
+Ensure, you have ``default`` cache set up: https://docs.djangoproject.com/en/3.2/topics/cache/#memcached
+
+Run migrations:
+
+.. code:: sh
+
+    $ python manage.py migrate
+
+Open Django admin root and add your ``Dashboard Stats`` configuration:
+
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-29-58.png
+.. image:: https://github.com/PetrDlouhy/django-admin-charts/raw/master/docs/source/_static/Sn%C3%ADmek%20obrazovky_2022-03-04_17-31-16.png
+
+Then the charts will appear on the root of Django admin page as well as on analytics page (``/admin_tools_stats/analytics/``).
+
+======================
+Special configurations
+======================
+
+Update from ``django-admin-tools-stats``
+----------------------------------------
+
+Uninstall ``django-admin-tools-stats``.
+
+Follow ``django-admin-charts`` installation according to previous section. Especially pay attention to these steps:
+- Move ``admin_tools_stats`` in ``INSTALLED_APPS`` before ``admin_tools`` and ``django.contrib.admin``.
+- Configure ``urls.py``.
+
+Change ``DashboardCharts`` to ``DashboardChart`` in dashboard definition (this is recomended even if dummy class is left for compatibility reasons).
+
+Check any overridden template from ``admin_tools_stats`` or ``DashboardChart(s)`` class that might interfere with the changes.
+
+Configure javascript libraries
+----------------------------------------------------------
+
+By default the nvd3/d3 libraries are taken from unpkg.
+If you want to install those libraries on your own, you can set their path by following settings:
+
+.. code:: python
+
+   ADMIN_CHARTS_NVD3_JS_PATH = 'bow/nvd3/build/nv.d3.js'
+   ADMIN_CHARTS_NVD3_CSS_PATH = 'bow/nvd3/build/nv.d3.css'
+   ADMIN_CHARTS_D3_JS_PATH = 'bow/d3/d3.js'
+
+The settings can accept either full path (with http...) or there can be static file path.
+Note that versions ``nvd3==1.8.6`` and ``d3==3.3.13`` are the only tested to be working.
+
+
+Installation of javascript libraries with ``django-bower``
+----------------------------------------------------------
+
+Add ``django-bower`` to INSTALLED_APPS in settings.py:
+
+.. code:: python
+
+    INSTALLED_APPS = (
+        ...
+        'djangobower'
+    )
+
+Add the following properties to you settings.py file:
+
+.. code:: python
+
+    # Specifie path to components root (you need to use absolute path)
+    BOWER_COMPONENTS_ROOT = os.path.join(PROJECT_ROOT, 'components')
+
+
+    BOWER_INSTALLED_APPS = (
+        'd3#3.3.13',
+        'nvd3#1.8.6',
+    )
+
+Add django-bower finder to your static file finders:
+
+.. code:: python
+
+    STATICFILES_FINDERS = (
+        ...
+        'djangobower.finders.BowerFinder',
+    )
+
+Run the following commands. These will download nvd3.js and its dependencies using bower and throw them in to you static folder for access by your application:
+
+.. code:: sh
+
+    $ python manage.py bower_install
+    $ python manage.py collectstatic
+
+
+
+Usage with ``django-admin-tools``
+----------------------------------
+
+Configure ``admin_tools``
+
+Add following code to dashboard.py:
+
+.. code:: python
+
+    from admin_tools_stats.modules import DashboardChart, get_active_graph
+
+    # append an app list module
+    self.children.append(modules.AppList(
+        _('Dashboard Stats Settings'),
+        models=('admin_tools_stats.*', ),
+    ))
+
+    # Copy following code into your custom dashboard
+    # append following code after recent actions module or
+    # a link list module for "quick links"
+    if context['request'].user.has_perm('admin_tools_stats.view_dashboardstats'):
+            graph_list = get_active_graph()
+        else:
+            graph_list = []
+
+    for i in graph_list:
+        kwargs = {}
+        kwargs['require_chart_jscss'] = True
+        kwargs['graph_key'] = i.graph_key
+
+        for key in context['request'].POST:
+            if key.startswith('select_box_'):
+                kwargs[key] = context['request'].POST[key]
+
+        self.children.append(DashboardChart(**kwargs))
+
+
+You may also need to add some includes to your template admin base, see an example on the demo project::
+
+    demoproject/demoproject/templates/admin/base_site.html
+
+
+Usage on DB that doesn't support JSONFields
+-------------------------------------------
+
+You can add following line to your settings in order to use JSONField from `django-jsonfield` instead of native Django JSONField:
+
+.. code:: python
+
+   ADMIN_CHARTS_USE_JSONFIELD = False
+
+This can become handy, when deploying on MySQL<5.7 (Like AWS RDS Aurora)
+
+
+============
+Running demo
+============
+
+Run following commands:
+
+.. code:: sh
+
+   export DB_ENGINE='sqlite'
+   pip install -r requirements.txt
+   python manage.py migrate
+   python manage.py loaddata demoproject/fixtures/auth_user.json
+   python manage.py loaddata demoproject/fixtures/test_data.json
+   python manage.py bower install
+   python manage.py runserver
+
+And log in with username `admin` and password `admin` to the `localhost:8000/admin` site.
+
+===========
+Development
+===========
+
+Dependencies
+------------
+
+django-admin-charts is a django based application, the major requirements are:
+
+- django-jsonfield
+- django-nvd3
+- django-bower
+
+
+Running tests
+-------------
+
+Test can be run with:
+
+.. code:: sh
+
+    DB_ENGINE="postgres" coverage run ./manage.py test --keepdb
+
+
+Contributing
+------------
+
+If you've found a bug, add a feature or improve django-admin-charts and
+think it is useful then please consider contributing.
+Patches, pull requests or just suggestions are always welcome!
+
+Source code: http://github.com/PetrDlouhy/django-admin-charts
+
+Bug tracker: https://github.com/PetrDlouhy/django-admin-charts/issues
+
+
+Debugging charts
+----------------
+
+For chart data view (/admin_tools_stats/chart_data/payments/) the URL query
+parameter `&debug=True` can be added, in order to get Django debug page or
+Django debug toolbar.
+
+
+Documentation
+-------------
+
+Documentation is available on 'Read the Docs':
+http://readthedocs.org/docs/django-admin-charts/
+
+
+License
+-------
+
+django-admin-charts is licensed under MIT, see ``MIT-LICENSE.txt``.
```

### Comparing `django-admin-charts-1.3.0/django_admin_charts.egg-info/SOURCES.txt` & `django-admin-charts-1.3.1/django_admin_charts.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 admin_tools_stats/charts.py
 admin_tools_stats/forms.py
 admin_tools_stats/models.py
 admin_tools_stats/modules.py
 admin_tools_stats/urls.py
 admin_tools_stats/utils.py
 admin_tools_stats/views.py
-admin_tools_stats/__pycache__/__init__.cpython-310.pyc
+admin_tools_stats/__pycache__/__init__.cpython-311.pyc
 admin_tools_stats/fixtures/10_dashboardstatscriteria_status.json
 admin_tools_stats/fixtures/20_dashboardstatscriteria_call_type.json
 admin_tools_stats/fixtures/initial_data.json
 admin_tools_stats/management/commands/recalculate_charts.py
 admin_tools_stats/migrations/0001_initial.py
 admin_tools_stats/migrations/0002_auto_20190920_1058.py
 admin_tools_stats/migrations/0003_auto_20191007_0950.py
```

### Comparing `django-admin-charts-1.3.0/docs/Makefile` & `django-admin-charts-1.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/Snímek obrazovky_2022-03-04_17-29-58.png` & `django-admin-charts-1.3.1/docs/source/_static/Snímek obrazovky_2022-03-04_17-29-58.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/Snímek obrazovky_2022-03-04_17-31-16.png` & `django-admin-charts-1.3.1/docs/source/_static/Snímek obrazovky_2022-03-04_17-31-16.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/admin_dashboard.png` & `django-admin-charts-1.3.1/docs/source/_static/admin_dashboard.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/aoe_chart.png` & `django-admin-charts-1.3.1/docs/source/_static/aoe_chart.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/bar_chart.png` & `django-admin-charts-1.3.1/docs/source/_static/bar_chart.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/images/admin_screenshot.png` & `django-admin-charts-1.3.1/docs/source/_static/images/admin_screenshot.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/_static/stacked_area_chart.png` & `django-admin-charts-1.3.1/docs/source/_static/stacked_area_chart.png`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/conf.py` & `django-admin-charts-1.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/developer-doc/objects-description.rst` & `django-admin-charts-1.3.1/docs/source/developer-doc/objects-description.rst`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/developer-doc/testing.rst` & `django-admin-charts-1.3.1/docs/source/developer-doc/testing.rst`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/docs/source/index.rst` & `django-admin-charts-1.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/setup.py` & `django-admin-charts-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-admin-charts-1.3.0/update_version.sh` & `django-admin-charts-1.3.1/update_version.sh`

 * *Files identical despite different names*

