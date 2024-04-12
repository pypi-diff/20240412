# Comparing `tmp/souschef-1.4.1.tar.gz` & `tmp/souschef-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/souschef-1.4.1.tar", last modified: Fri Mar  8 17:37:53 2024, max compression
+gzip compressed data, was "dist/souschef-1.4.2.tar", last modified: Fri Apr 12 15:59:24 2024, max compression
```

## Comparing `souschef-1.4.1.tar` & `souschef-1.4.2.tar`

### file list

```diff
@@ -1,433 +1,381 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/
--rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.1/INSTALL.md
--rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2261 2024-03-08 17:37:53.000000 souschef-1.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.1/UPDATE.md
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       78 2024-03-08 17:37:53.000000 souschef-1.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1787 2024-03-08 17:35:35.000000 souschef-1.4.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/
--rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/admin.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/billing/apps.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/billing/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/billing/migrations/
--rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/migrations/0002_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/migrations/0003_auto_20161122_0515.py
--rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/migrations/0004_auto_20201030_1540.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/billing/templates/
--rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/base_billing.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/billing/templates/billing/
--rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/add.html
--rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/billing_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/billing/templates/billing/partials/
--rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/partials/statistics.html
--rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.1/souschef/billing/templates/billing/partials/summary.html
--rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/print_summary.html
--rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/billing/templates/billing/view.html
--rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.1/souschef/billing/templates/billing/view_orders.html
--rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/tests.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/billing/urls.py
--rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/billing/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/configsamples/
--rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.1/souschef/configsamples/nginx.conf
--rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.1/souschef/configsamples/souschef.service
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/cronscripts/
--rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.1/souschef/cronscripts/souschef_daily.sh
--rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/dataexec.py
--rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/dataload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/datamigration/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/datamigration/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/datamigration/admin.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/datamigration/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/datamigration/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.1/souschef/datamigration/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/datamigration/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.1/souschef/datamigration/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importaddresses.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importclients.py
--rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importcontactaddresses.py
--rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importmeals.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importorders.py
--rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/management/commands/importrelationships.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/datamigration/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/datamigration/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/datamigration/models.py
--rw-r--r--   0 root         (0) root         (0)     6840 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/datamigration/tests.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/datamigration/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/delivery/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/delivery/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/delivery/admin.py
--rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/delivery/apps.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/delivery/filters.py
--rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.1/souschef/delivery/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/delivery/migrations/
--rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/delivery/migrations/0001_fix004a.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/delivery/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/delivery/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/delivery/templates/
--rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/templates/edit_delivery_route.html
--rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.1/souschef/delivery/templates/ingredients.html
--rw-r--r--   0 root         (0) root         (0)     4323 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/templates/kitchen_count.html
--rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.1/souschef/delivery/templates/kitchen_count_steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/delivery/templates/partials/
--rw-r--r--   0 root         (0) root         (0)     2622 2021-03-20 15:32:41.000000 souschef-1.4.1/souschef/delivery/templates/partials/generated_orders.html
--rw-r--r--   0 root         (0) root         (0)     1737 2021-03-19 19:57:48.000000 souschef-1.4.1/souschef/delivery/templates/partials/generated_orders_order_row_content.html
--rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.1/souschef/delivery/templates/partials/generated_orders_table_head.html
--rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.1/souschef/delivery/templates/review_orders.html
--rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/templates/route_sheet.html
--rw-r--r--   0 root         (0) root         (0)     5297 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/templates/routes.html
--rwxr-xr-x   0 root         (0) root         (0)    52469 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/tests.py
--rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/delivery/tsp.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/delivery/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    82370 2024-03-08 17:35:22.000000 souschef-1.4.1/souschef/delivery/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/frontend/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/frontend/images/
--rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/frontend/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/frontend/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/frontend/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/frontend/images/katrina.jpg
--rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/meal/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/meal/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3537 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/meal/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/meal/apps.py
--rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/meal/migrations/
--rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0002_ingredient_ingredient_group.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0003_fix224a.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0004_fix004d.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0006_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0007_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/migrations/0008_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/meal/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/models.py
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/meal/settings.py
--rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/meal/tests.py
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/meal/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/meal/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/admin.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/apps.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/factories.py
--rw-r--r--   0 root         (0) root         (0)    20434 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/forms.py
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/formsets.py
--rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/formsfield.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.1/souschef/member/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.1/souschef/member/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/management/commands/createclients.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/management/commands/createnotes.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/management/commands/processscheduledstatuschange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/migrations/
--rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0002_auto_20160605_1609.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0003_auto_20160615_2100.py
--rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0005_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0006_client_meal_default_week.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0007_auto_20160726_1703.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0008_auto_20160727_2251.py
--rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0009_auto_20160728_1443.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0010_auto_20160803_2052.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0011_client_delivery_note.py
--rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0012_clientscheduledstatus.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0013_auto_20160820_2322.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0014_auto_20160826_0007.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0015_route_client_id_sequence.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0016_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0017_auto_20161020_2039.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0018_auto_20161110_2352.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0019_auto_20161111_1750.py
--rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0020_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0021_auto_20161125_2055.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0022_auto_20161215_1936.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0023_auto_20161220_1401.py
--rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0024_auto_20161227_1819.py
--rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0025_route_vehicle.py
--rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0026_change_to_emergency_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0027_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0029_member_address_fk_to_1to1.py
--rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0030_route_deliveryhistory.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0032_relationship.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0033_auto_20170801_1607.py
--rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0034_auto_20170816_0850.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0035_auto_20210115_1155.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0036_member_addresses.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0037_one_address_per_member.py
--rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/migrations/0038_member_verbose_names.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28788 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/signals/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/signals/__init__.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/signals/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/
--rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/create/
--rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/create/form.html
--rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/create/steps.html
--rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/partials/
--rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/birthdays.html
--rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/filters.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/
--rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/address_information.html
--rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/basic_information.html
--rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/dietary_restriction.html
--rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/meal_defaults.html
--rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/payment_information.html
--rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/relationship_form.html
--rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/forms/relationships.html
--rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/partials/menu.html
--rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.1/souschef/member/templates/client/partials/order_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/update/
--rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.1/souschef/member/templates/client/update/base.html
--rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.1/souschef/member/templates/client/update/status.html
--rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/update/step.html
--rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/update/steps.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/member/templates/client/view/
--rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/address.html
--rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/allergies.html
--rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/delete_status_confirmation.html
--rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/information.html
--rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.1/souschef/member/templates/client/view/notes.html
--rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.1/souschef/member/templates/client/view/orders.html
--rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/payment.html
--rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/referent.html
--rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/status.html
--rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/client/view/summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/member/templates/route/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/route/delivered_route_detail.html
--rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/route/delivery_history_detail.html
--rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/route/detail.html
--rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/route/edit.html
--rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/member/templates/route/list.html
--rw-r--r--   0 root         (0) root         (0)   160926 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/member/tests.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/member/urls.py
--rw-r--r--   0 root         (0) root         (0)    54834 2024-02-24 23:48:36.000000 souschef-1.4.1/souschef/member/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/note/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/note/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/note/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/note/apps.py
--rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/factories.py
--rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/note/migrations/
--rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0002_auto_20160818_2104.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0003_auto_20160819_2037.py
--rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0004_notepriority.py
--rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0005_note_priority_old_data_migration.py
--rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0006_change_priority_field.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0007_notecategory.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0008_auto_20170116_1441.py
--rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0009_auto_20170116_1543.py
--rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0010_auto_20170313_1442.py
--rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0011_auto_20170419_1109.py
--rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0012_note_is_deleted.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0013_date_modified.py
--rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/migrations/0014_date_created.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/note/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/note/templates/
--rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.1/souschef/note/templates/note_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.1/souschef/note/templates/note_edit.html
--rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.1/souschef/note/templates/notes_add.html
--rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.1/souschef/note/templates/notes_client_list.html
--rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.1/souschef/note/templates/notes_list.html
--rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/tests.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/note/urls.py
--rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/note/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/notification/admin.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/notification/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/notification/migrations/
--rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/notification/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/notification/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.1/souschef/notification/models.py
--rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/notification/tests.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/notification/urls.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/notification/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/order/admin.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/order/apps.py
--rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/factories.py
--rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/management/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.1/souschef/order/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.1/souschef/order/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/management/commands/createorders.py
--rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/management/commands/generateorders.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/management/commands/setordersdelivered.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/migrations/
--rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0001_fix161f.py
--rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0002_auto_20160614_1736.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0003_auto_20160615_1504.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0004_fix004a.py
--rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0005_fix241b.py
--rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0006_auto_20160803_2217.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0007_remove_order_item_component.py
--rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0008_auto_20160912_1509.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0009_auto_20161012_1919.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0010_auto_20161012_1921.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0011_auto_20161014_1901.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0012_auto_20161122_0458.py
--rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0013_orderstatuschange.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0014_auto_20161209_2045.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0015_auto_20170410_1029.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0016_auto_20180704_1613.py
--rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/migrations/0017_total_quantity_not_nullable.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/order/mixins.py
--rw-r--r--   0 root         (0) root         (0)    45942 2024-02-24 23:48:36.000000 souschef-1.4.1/souschef/order/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/templates/
--rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/_form.html
--rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/_order_info.html
--rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/base_order.html
--rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/create.html
--rw-r--r--   0 root         (0) root         (0)     4421 2021-03-26 14:22:55.000000 souschef-1.4.1/souschef/order/templates/list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/templates/order/
--rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/order/create_batch.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/order/templates/order/partials/
--rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/order/templates/order/partials/filters.html
--rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.1/souschef/order/templates/order_confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.1/souschef/order/templates/order_update_status.html
--rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.1/souschef/order/templates/update.html
--rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.1/souschef/order/templates/view.html
--rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.1/souschef/order/tests.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/order/urls.py
--rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.1/souschef/order/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/page/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/page/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/page/admin.py
--rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/page/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/page/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/page/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/page/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/page/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/page/templates/pages/
--rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/page/templates/pages/card.html
--rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/page/templates/pages/home.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/page/templates/registration/
--rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/page/templates/registration/login.html
--rw-r--r--   0 root         (0) root         (0)    10123 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/page/tests.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/page/urls.py
--rw-r--r--   0 root         (0) root         (0)     4830 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/page/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/pycrons/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.1/souschef/pycrons/__init__.py
--rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/pycrons/cleaning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef/sous_chef/assets/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/assets/css/
--rw-r--r--   0 root         (0) root         (0)   655527 2024-03-08 17:37:35.000000 souschef-1.4.1/souschef/sous_chef/assets/css/main.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/
--rw-r--r--   0 root         (0) root         (0)    98640 2024-03-08 17:37:28.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/brand-icons.eot
--rw-r--r--   0 root         (0) root         (0)   507628 2024-03-08 17:37:28.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/brand-icons.svg
--rw-r--r--   0 root         (0) root         (0)    98404 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/brand-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    63728 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/brand-icons.woff
--rw-r--r--   0 root         (0) root         (0)    54488 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/brand-icons.woff2
--rw-r--r--   0 root         (0) root         (0)   106004 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.eot
--rw-r--r--   0 root         (0) root         (0)    93888 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.otf
--rw-r--r--   0 root         (0) root         (0)   390837 2024-03-08 17:37:33.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.svg
--rw-r--r--   0 root         (0) root         (0)   105784 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.ttf
--rw-r--r--   0 root         (0) root         (0)    50524 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.woff
--rw-r--r--   0 root         (0) root         (0)    40148 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/icons.woff2
--rw-r--r--   0 root         (0) root         (0)    31156 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/outline-icons.eot
--rw-r--r--   0 root         (0) root         (0)   107201 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/outline-icons.svg
--rw-r--r--   0 root         (0) root         (0)    30928 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/outline-icons.ttf
--rw-r--r--   0 root         (0) root         (0)    14712 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/outline-icons.woff
--rw-r--r--   0 root         (0) root         (0)    12240 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/assets/images/
--rw-r--r--   0 root         (0) root         (0)   258972 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/bg1.jpg
--rw-r--r--   0 root         (0) root         (0)    11449 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/demo.png
--rw-r--r--   0 root         (0) root         (0)      608 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/favicon.png
--rw-r--r--   0 root         (0) root         (0)    28123 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/images/flags.png
--rw-r--r--   0 root         (0) root         (0)      490 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/images/geocoder.png
--rw-r--r--   0 root         (0) root         (0)     1374 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/glyph-marker-icon.png
--rw-r--r--   0 root         (0) root         (0)     1287 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/glyph-marker-icon.svg
--rw-r--r--   0 root         (0) root         (0)    21977 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/jenny.jpg
--rw-r--r--   0 root         (0) root         (0)    26952 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/joe.jpg
--rw-r--r--   0 root         (0) root         (0)    23839 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/katrina.jpg
--rw-r--r--   0 root         (0) root         (0)     2306 2024-03-08 17:37:33.000000 souschef-1.4.1/souschef/sous_chef/assets/images/leaflet.routing.icons.png
--rw-r--r--   0 root         (0) root         (0)     4060 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/images/leaflet.routing.icons.svg
--rw-r--r--   0 root         (0) root         (0)     6363 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/logo-souschef-coul.png
--rw-r--r--   0 root         (0) root         (0)     6033 2024-03-08 17:37:46.000000 souschef-1.4.1/souschef/sous_chef/assets/images/logo-souschef-nb.png
--rw-r--r--   0 root         (0) root         (0)      891 2024-03-08 17:37:46.000000 souschef-1.4.1/souschef/sous_chef/assets/images/logo.png
--rw-r--r--   0 root         (0) root         (0)    14323 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-matte.png
--rw-r--r--   0 root         (0) root         (0)    30194 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-matte@2x.png
--rw-r--r--   0 root         (0) root         (0)     7946 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-plain.png
--rw-r--r--   0 root         (0) root         (0)      535 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-shadow.png
--rw-r--r--   0 root         (0) root         (0)     1134 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-shadow@2x.png
--rw-r--r--   0 root         (0) root         (0)    36367 2024-03-08 17:37:43.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-soft.png
--rw-r--r--   0 root         (0) root         (0)   146362 2024-03-08 17:37:45.000000 souschef-1.4.1/souschef/sous_chef/assets/images/markers-soft@2x.png
--rw-r--r--   0 root         (0) root         (0)      454 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/images/routing-icon.png
--rw-r--r--   0 root         (0) root         (0)     4831 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/images/throbber.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/assets/js/
--rw-r--r--   0 root         (0) root         (0)  1031323 2024-03-08 17:37:29.000000 souschef-1.4.1/souschef/sous_chef/assets/js/leaflet.js
--rw-r--r--   0 root         (0) root         (0)   627692 2024-03-08 17:37:33.000000 souschef-1.4.1/souschef/sous_chef/assets/js/leaflet.min.js
--rw-r--r--   0 root         (0) root         (0)    22295 2024-03-08 17:37:28.000000 souschef-1.4.1/souschef/sous_chef/assets/js/multidatespicker.js
--rw-r--r--   0 root         (0) root         (0)    10453 2024-03-08 17:37:28.000000 souschef-1.4.1/souschef/sous_chef/assets/js/multidatespicker.min.js
--rw-r--r--   0 root         (0) root         (0)  1111829 2024-03-08 17:37:36.000000 souschef-1.4.1/souschef/sous_chef/assets/js/sous-chef.js
--rw-r--r--   0 root         (0) root         (0)   399694 2024-03-08 17:37:42.000000 souschef-1.4.1/souschef/sous_chef/assets/js/sous-chef.min.js
--rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/formats/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/formats/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/formats/en/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/formats/en/__init__.py
--rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/formats/en/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/formats/fr/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/formats/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/formats/fr/formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/management/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/management/commands/makemessages.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/rules.py
--rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/settings.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/sous_chef/settings_test.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/sous_chef/settings_test_fr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/templates/
--rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/templates/avatar/
--rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/avatar/change.html
--rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/avatar/confirm_delete.html
--rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.1/souschef/sous_chef/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/templates/dashboard/
--rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/dashboard/statistics.html
--rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/splash.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/templates/system/
--rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/system/_button_export.html
--rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templates/system/breadcrumb.html
--rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.1/souschef/sous_chef/templates/system/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:53.000000 souschef-1.4.1/souschef/sous_chef/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/sous_chef/templatetags/sous_chef_extras.py
--rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.1/souschef/sous_chef/tests.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.1/souschef/sous_chef/urls.py
--rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.1/souschef/sous_chef/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2261 2024-03-08 17:37:51.000000 souschef-1.4.1/souschef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15624 2024-03-08 17:37:52.000000 souschef-1.4.1/souschef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 17:37:51.000000 souschef-1.4.1/souschef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      462 2024-03-08 17:37:51.000000 souschef-1.4.1/souschef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-08 17:37:51.000000 souschef-1.4.1/souschef.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/
+-rw-r--r--   0 root         (0) root         (0)     5731 2024-02-17 22:37:08.000000 souschef-1.4.2/INSTALL.md
+-rw-r--r--   0 root         (0) root         (0)    33893 2020-11-20 01:08:04.000000 souschef-1.4.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      230 2021-01-23 15:51:37.000000 souschef-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-04-12 15:59:24.000000 souschef-1.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1366 2021-01-22 18:52:15.000000 souschef-1.4.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1409 2021-01-23 16:03:53.000000 souschef-1.4.2/UPDATE.md
+-rw-r--r--   0 root         (0) root         (0)      249 2024-02-18 19:41:03.000000 souschef-1.4.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-12 15:59:24.000000 souschef-1.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-04-12 15:59:04.000000 souschef-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/
+-rw-r--r--   0 root         (0) root         (0)    32621 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      314 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/admin.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/billing/apps.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/billing/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/billing/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      459 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/migrations/0002_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      370 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/migrations/0003_auto_20161122_0515.py
+-rw-r--r--   0 root         (0) root         (0)      374 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/migrations/0004_auto_20201030_1540.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5211 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/billing/templates/
+-rw-r--r--   0 root         (0) root         (0)       42 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/base_billing.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/billing/templates/billing/
+-rw-r--r--   0 root         (0) root         (0)     4897 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/add.html
+-rw-r--r--   0 root         (0) root         (0)      863 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/billing_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3310 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/billing/templates/billing/partials/
+-rw-r--r--   0 root         (0) root         (0)      531 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/partials/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     5508 2021-07-16 15:48:25.000000 souschef-1.4.2/souschef/billing/templates/billing/partials/summary.html
+-rw-r--r--   0 root         (0) root         (0)      864 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/print_summary.html
+-rw-r--r--   0 root         (0) root         (0)      822 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/billing/templates/billing/view.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2021-03-19 15:14:11.000000 souschef-1.4.2/souschef/billing/templates/billing/view_orders.html
+-rw-r--r--   0 root         (0) root         (0)     8556 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/tests.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/billing/urls.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/billing/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/configsamples/
+-rw-r--r--   0 root         (0) root         (0)      809 2021-03-02 23:43:41.000000 souschef-1.4.2/souschef/configsamples/nginx.conf
+-rw-r--r--   0 root         (0) root         (0)      409 2020-12-19 18:25:21.000000 souschef-1.4.2/souschef/configsamples/souschef.service
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/cronscripts/
+-rwxr-xr-x   0 root         (0) root         (0)      469 2021-01-23 16:08:34.000000 souschef-1.4.2/souschef/cronscripts/souschef_daily.sh
+-rw-r--r--   0 root         (0) root         (0)      350 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/dataexec.py
+-rw-r--r--   0 root         (0) root         (0)    76889 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/dataload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/datamigration/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/datamigration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/datamigration/admin.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/datamigration/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/datamigration/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:34.000000 souschef-1.4.2/souschef/datamigration/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/datamigration/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:11.000000 souschef-1.4.2/souschef/datamigration/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importclients.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importcontactaddresses.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importmeals.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importorders.py
+-rw-r--r--   0 root         (0) root         (0)     3299 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/datamigration/management/commands/importrelationships.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/datamigration/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/datamigration/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/datamigration/models.py
+-rw-r--r--   0 root         (0) root         (0)     6840 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/datamigration/tests.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/datamigration/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/delivery/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/delivery/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/delivery/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)       91 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/delivery/apps.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/delivery/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2024-02-17 22:36:40.000000 souschef-1.4.2/souschef/delivery/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/delivery/migrations/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/delivery/migrations/0001_fix004a.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/delivery/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      232 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/delivery/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/delivery/templates/
+-rw-r--r--   0 root         (0) root         (0)    12210 2024-02-19 02:15:16.000000 souschef-1.4.2/souschef/delivery/templates/edit_delivery_route.html
+-rw-r--r--   0 root         (0) root         (0)     3686 2024-03-06 02:24:13.000000 souschef-1.4.2/souschef/delivery/templates/ingredients.html
+-rw-r--r--   0 root         (0) root         (0)     4380 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/delivery/templates/kitchen_count.html
+-rw-r--r--   0 root         (0) root         (0)     1360 2024-03-06 02:24:13.000000 souschef-1.4.2/souschef/delivery/templates/kitchen_count_steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/delivery/templates/partials/
+-rw-r--r--   0 root         (0) root         (0)     2622 2021-03-20 15:32:41.000000 souschef-1.4.2/souschef/delivery/templates/partials/generated_orders.html
+-rw-r--r--   0 root         (0) root         (0)     1737 2021-03-19 19:57:48.000000 souschef-1.4.2/souschef/delivery/templates/partials/generated_orders_order_row_content.html
+-rw-r--r--   0 root         (0) root         (0)     1085 2021-03-19 15:56:24.000000 souschef-1.4.2/souschef/delivery/templates/partials/generated_orders_table_head.html
+-rw-r--r--   0 root         (0) root         (0)     5472 2024-03-06 02:24:13.000000 souschef-1.4.2/souschef/delivery/templates/review_orders.html
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-02-19 02:15:16.000000 souschef-1.4.2/souschef/delivery/templates/route_sheet.html
+-rw-r--r--   0 root         (0) root         (0)     5284 2024-04-09 15:26:23.000000 souschef-1.4.2/souschef/delivery/templates/routes.html
+-rwxr-xr-x   0 root         (0) root         (0)    53637 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/delivery/tests.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/delivery/tsp.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-09 15:26:23.000000 souschef-1.4.2/souschef/delivery/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)    80902 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/delivery/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/frontend/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/frontend/images/
+-rw-r--r--   0 root         (0) root         (0)   292180 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/frontend/images/bg1.jpg
+-rw-r--r--   0 root         (0) root         (0)    21988 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/frontend/images/jenny.jpg
+-rw-r--r--   0 root         (0) root         (0)    28209 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/frontend/images/joe.jpg
+-rw-r--r--   0 root         (0) root         (0)    23839 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/frontend/images/katrina.jpg
+-rwxr-xr-x   0 root         (0) root         (0)      284 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/manage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/meal/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/meal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-04-01 00:23:07.000000 souschef-1.4.2/souschef/meal/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/meal/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/meal/migrations/
+-rw-r--r--   0 root         (0) root         (0)     7348 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0002_ingredient_ingredient_group.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0003_fix224a.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0004_fix004d.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0006_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0007_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/migrations/0008_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/meal/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8100 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/meal/models.py
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/meal/settings.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/meal/tests.py
+-rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/meal/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/meal/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/admin.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/apps.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/factories.py
+-rw-r--r--   0 root         (0) root         (0)    20434 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/member/forms.py
+-rw-r--r--   0 root         (0) root         (0)      294 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/formsets.py
+-rw-r--r--   0 root         (0) root         (0)      964 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/formsfield.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:20:56.000000 souschef-1.4.2/souschef/member/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:35:45.000000 souschef-1.4.2/souschef/member/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      578 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/management/commands/createclients.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/management/commands/createnotes.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/member/management/commands/processscheduledstatuschange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/migrations/
+-rw-r--r--   0 root         (0) root         (0)    15890 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0002_auto_20160605_1609.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0003_auto_20160615_2100.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      595 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0005_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0006_client_meal_default_week.py
+-rw-r--r--   0 root         (0) root         (0)      908 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0007_auto_20160726_1703.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0008_auto_20160727_2251.py
+-rw-r--r--   0 root         (0) root         (0)      918 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0009_auto_20160728_1443.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0010_auto_20160803_2052.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0011_client_delivery_note.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0012_clientscheduledstatus.py
+-rw-r--r--   0 root         (0) root         (0)      754 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0013_auto_20160820_2322.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0014_auto_20160826_0007.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0015_route_client_id_sequence.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0016_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      575 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0017_auto_20161020_2039.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0018_auto_20161110_2352.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0019_auto_20161111_1750.py
+-rw-r--r--   0 root         (0) root         (0)      438 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0020_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0021_auto_20161125_2055.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0022_auto_20161215_1936.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0023_auto_20161220_1401.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0024_auto_20161227_1819.py
+-rw-r--r--   0 root         (0) root         (0)      672 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0025_route_vehicle.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0026_change_to_emergency_contacts.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0027_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py
+-rw-r--r--   0 root         (0) root         (0)     1716 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/member/migrations/0029_member_address_fk_to_1to1.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0030_route_deliveryhistory.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0031_client_option_allow_reverse_relation.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0032_relationship.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0033_auto_20170801_1607.py
+-rw-r--r--   0 root         (0) root         (0)      554 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0034_auto_20170816_0850.py
+-rw-r--r--   0 root         (0) root         (0)      866 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0035_auto_20210115_1155.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0036_member_addresses.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0037_one_address_per_member.py
+-rw-r--r--   0 root         (0) root         (0)      601 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/member/migrations/0038_member_verbose_names.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28565 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/member/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/signals/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/signals/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/signals/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/member/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/
+-rw-r--r--   0 root         (0) root         (0)     3988 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/create/
+-rw-r--r--   0 root         (0) root         (0)     3868 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/create/form.html
+-rw-r--r--   0 root         (0) root         (0)     1038 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/create/steps.html
+-rw-r--r--   0 root         (0) root         (0)     5918 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/partials/
+-rw-r--r--   0 root         (0) root         (0)     1030 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/birthdays.html
+-rw-r--r--   0 root         (0) root         (0)     1391 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/filters.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/
+-rw-r--r--   0 root         (0) root         (0)     2386 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/address_information.html
+-rw-r--r--   0 root         (0) root         (0)     2100 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/basic_information.html
+-rw-r--r--   0 root         (0) root         (0)     1467 2021-03-12 15:24:10.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/dietary_restriction.html
+-rw-r--r--   0 root         (0) root         (0)     1293 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/meal_defaults.html
+-rw-r--r--   0 root         (0) root         (0)     2480 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/payment_information.html
+-rw-r--r--   0 root         (0) root         (0)     4373 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/relationship_form.html
+-rw-r--r--   0 root         (0) root         (0)      549 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/forms/relationships.html
+-rw-r--r--   0 root         (0) root         (0)     1386 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/partials/menu.html
+-rw-r--r--   0 root         (0) root         (0)     2017 2021-06-18 20:11:28.000000 souschef-1.4.2/souschef/member/templates/client/partials/order_list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/update/
+-rw-r--r--   0 root         (0) root         (0)     3033 2021-03-12 15:24:10.000000 souschef-1.4.2/souschef/member/templates/client/update/base.html
+-rw-r--r--   0 root         (0) root         (0)     2153 2021-03-12 21:55:40.000000 souschef-1.4.2/souschef/member/templates/client/update/status.html
+-rw-r--r--   0 root         (0) root         (0)      291 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/update/step.html
+-rw-r--r--   0 root         (0) root         (0)      149 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/update/steps.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/client/view/
+-rw-r--r--   0 root         (0) root         (0)      188 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/address.html
+-rw-r--r--   0 root         (0) root         (0)     4633 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/allergies.html
+-rw-r--r--   0 root         (0) root         (0)     1731 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/delete_status_confirmation.html
+-rw-r--r--   0 root         (0) root         (0)     4471 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/information.html
+-rw-r--r--   0 root         (0) root         (0)     2716 2021-06-11 15:40:13.000000 souschef-1.4.2/souschef/member/templates/client/view/notes.html
+-rw-r--r--   0 root         (0) root         (0)      637 2021-03-05 21:39:33.000000 souschef-1.4.2/souschef/member/templates/client/view/orders.html
+-rw-r--r--   0 root         (0) root         (0)     1825 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/payment.html
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/referent.html
+-rw-r--r--   0 root         (0) root         (0)     2204 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/status.html
+-rw-r--r--   0 root         (0) root         (0)     1622 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/client/view/summary.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/member/templates/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/route/delivered_route_detail.html
+-rw-r--r--   0 root         (0) root         (0)     5832 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/route/delivery_history_detail.html
+-rw-r--r--   0 root         (0) root         (0)     6159 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/route/detail.html
+-rw-r--r--   0 root         (0) root         (0)     9150 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/route/edit.html
+-rw-r--r--   0 root         (0) root         (0)     1875 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/member/templates/route/list.html
+-rw-r--r--   0 root         (0) root         (0)   160818 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/member/tests.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/member/urls.py
+-rw-r--r--   0 root         (0) root         (0)    54776 2024-04-11 01:19:40.000000 souschef-1.4.2/souschef/member/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/note/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/note/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/note/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/note/apps.py
+-rw-r--r--   0 root         (0) root         (0)      775 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/factories.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/note/migrations/
+-rw-r--r--   0 root         (0) root         (0)     2230 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)      607 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0002_auto_20160818_2104.py
+-rw-r--r--   0 root         (0) root         (0)      481 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0003_auto_20160819_2037.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0004_notepriority.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0005_note_priority_old_data_migration.py
+-rw-r--r--   0 root         (0) root         (0)      482 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0006_change_priority_field.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0007_notecategory.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0008_auto_20170116_1441.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0009_auto_20170116_1543.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0010_auto_20170313_1442.py
+-rw-r--r--   0 root         (0) root         (0)      987 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0011_auto_20170419_1109.py
+-rw-r--r--   0 root         (0) root         (0)      414 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0012_note_is_deleted.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0013_date_modified.py
+-rw-r--r--   0 root         (0) root         (0)      495 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/migrations/0014_date_created.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/note/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/note/templates/
+-rw-r--r--   0 root         (0) root         (0)      909 2021-07-09 19:21:52.000000 souschef-1.4.2/souschef/note/templates/note_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     1720 2021-07-09 19:00:25.000000 souschef-1.4.2/souschef/note/templates/note_edit.html
+-rw-r--r--   0 root         (0) root         (0)     2186 2021-07-09 19:00:30.000000 souschef-1.4.2/souschef/note/templates/notes_add.html
+-rw-r--r--   0 root         (0) root         (0)     4080 2021-06-11 15:41:01.000000 souschef-1.4.2/souschef/note/templates/notes_client_list.html
+-rw-r--r--   0 root         (0) root         (0)     5780 2021-07-23 15:17:48.000000 souschef-1.4.2/souschef/note/templates/notes_list.html
+-rw-r--r--   0 root         (0) root         (0)     9225 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/tests.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/note/urls.py
+-rw-r--r--   0 root         (0) root         (0)     5709 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/note/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/notification/admin.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/notification/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/notification/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/notification/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/notification/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-02-11 21:15:42.000000 souschef-1.4.2/souschef/notification/models.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/notification/tests.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/notification/urls.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/notification/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/order/admin.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/order/apps.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/factories.py
+-rw-r--r--   0 root         (0) root         (0)     5183 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:21:15.000000 souschef-1.4.2/souschef/order/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-01-23 15:36:52.000000 souschef-1.4.2/souschef/order/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/management/commands/createorders.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/management/commands/generateorders.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/management/commands/setordersdelivered.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/migrations/
+-rw-r--r--   0 root         (0) root         (0)     4735 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0001_fix161f.py
+-rw-r--r--   0 root         (0) root         (0)      581 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0002_auto_20160614_1736.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0003_auto_20160615_1504.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0004_fix004a.py
+-rw-r--r--   0 root         (0) root         (0)      873 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0005_fix241b.py
+-rw-r--r--   0 root         (0) root         (0)      681 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0006_auto_20160803_2217.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0007_remove_order_item_component.py
+-rw-r--r--   0 root         (0) root         (0)      633 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0008_auto_20160912_1509.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0009_auto_20161012_1919.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0010_auto_20161012_1921.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0011_auto_20161014_1901.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0012_auto_20161122_0458.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0013_orderstatuschange.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0014_auto_20161209_2045.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0015_auto_20170410_1029.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0016_auto_20180704_1613.py
+-rw-r--r--   0 root         (0) root         (0)      463 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/migrations/0017_total_quantity_not_nullable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/order/mixins.py
+-rw-r--r--   0 root         (0) root         (0)    46300 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/order/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/templates/
+-rw-r--r--   0 root         (0) root         (0)     5283 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/_form.html
+-rw-r--r--   0 root         (0) root         (0)     1098 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/_order_info.html
+-rw-r--r--   0 root         (0) root         (0)       92 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/base_order.html
+-rw-r--r--   0 root         (0) root         (0)     1227 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/create.html
+-rw-r--r--   0 root         (0) root         (0)     4421 2021-03-26 14:22:55.000000 souschef-1.4.2/souschef/order/templates/list.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/templates/order/
+-rw-r--r--   0 root         (0) root         (0)     9056 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/order/create_batch.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/order/templates/order/partials/
+-rw-r--r--   0 root         (0) root         (0)     1308 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/order/templates/order/partials/filters.html
+-rw-r--r--   0 root         (0) root         (0)     1070 2021-07-09 19:21:52.000000 souschef-1.4.2/souschef/order/templates/order_confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     2315 2021-03-26 15:05:24.000000 souschef-1.4.2/souschef/order/templates/order_update_status.html
+-rw-r--r--   0 root         (0) root         (0)     2023 2021-03-26 14:34:44.000000 souschef-1.4.2/souschef/order/templates/update.html
+-rw-r--r--   0 root         (0) root         (0)     3240 2021-04-02 19:14:01.000000 souschef-1.4.2/souschef/order/templates/view.html
+-rw-r--r--   0 root         (0) root         (0)    66186 2024-02-24 23:48:36.000000 souschef-1.4.2/souschef/order/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/order/urls.py
+-rw-r--r--   0 root         (0) root         (0)    14652 2024-02-19 02:15:16.000000 souschef-1.4.2/souschef/order/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/page/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/page/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/page/admin.py
+-rw-r--r--   0 root         (0) root         (0)       83 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/page/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/page/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/page/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/page/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef/page/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/page/templates/pages/
+-rw-r--r--   0 root         (0) root         (0)      487 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/page/templates/pages/card.html
+-rw-r--r--   0 root         (0) root         (0)     7007 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/page/templates/pages/home.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/page/templates/registration/
+-rw-r--r--   0 root         (0) root         (0)     1634 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/page/templates/registration/login.html
+-rw-r--r--   0 root         (0) root         (0)    10123 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/page/tests.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/page/urls.py
+-rw-r--r--   0 root         (0) root         (0)     4830 2024-04-12 15:39:37.000000 souschef-1.4.2/souschef/page/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/pycrons/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-02-12 02:23:19.000000 souschef-1.4.2/souschef/pycrons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      461 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/pycrons/cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/formats/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/formats/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/formats/en/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/formats/en/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      145 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/formats/en/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/formats/fr/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/formats/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/formats/fr/formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/management/commands/makemessages.py
+-rw-r--r--   0 root         (0) root         (0)      471 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/rules.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/settings.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/sous_chef/settings_test.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/sous_chef/settings_test_fr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/templates/
+-rw-r--r--   0 root         (0) root         (0)      611 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/templates/avatar/
+-rw-r--r--   0 root         (0) root         (0)     1870 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/avatar/change.html
+-rw-r--r--   0 root         (0) root         (0)     1125 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/avatar/confirm_delete.html
+-rw-r--r--   0 root         (0) root         (0)     3656 2021-07-23 15:25:58.000000 souschef-1.4.2/souschef/sous_chef/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/templates/dashboard/
+-rw-r--r--   0 root         (0) root         (0)      771 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/dashboard/statistics.html
+-rw-r--r--   0 root         (0) root         (0)     1271 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/splash.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/templates/system/
+-rw-r--r--   0 root         (0) root         (0)      219 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/system/_button_export.html
+-rw-r--r--   0 root         (0) root         (0)      209 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templates/system/breadcrumb.html
+-rw-r--r--   0 root         (0) root         (0)     2878 2021-07-09 19:03:35.000000 souschef-1.4.2/souschef/sous_chef/templates/system/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:24.000000 souschef-1.4.2/souschef/sous_chef/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/sous_chef/templatetags/sous_chef_extras.py
+-rw-r--r--   0 root         (0) root         (0)     3420 2024-02-18 19:41:03.000000 souschef-1.4.2/souschef/sous_chef/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-05-26 21:47:13.000000 souschef-1.4.2/souschef/sous_chef/urls.py
+-rw-r--r--   0 root         (0) root         (0)      395 2020-11-06 14:25:57.000000 souschef-1.4.2/souschef/sous_chef/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2261 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13368 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 15:59:23.000000 souschef-1.4.2/souschef.egg-info/top_level.txt
```

### Comparing `souschef-1.4.1/INSTALL.md` & `souschef-1.4.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/LICENSE.txt` & `souschef-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/PKG-INFO` & `souschef-1.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.1
+Version: 1.4.2
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.1/README.md` & `souschef-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/UPDATE.md` & `souschef-1.4.2/UPDATE.md`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/setup.py` & `souschef-1.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="souschef",
-    version="1.4.1",
+    version="1.4.2",
     license="AGPL-3.0",
     author="Santropol Roulant and Savoir Faire Linux",
     author_email="info@santropolroulant.org",
     description="Webapp used to manage orders for meals-on-wheel delivery",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/santropolroulant/sous-chef",
@@ -37,13 +37,14 @@
         "django-formtools>=2.0,<2.0.999",
         "django-leaflet>=0.22,<0.22.999",
         "django-localflavor>=1.5,<1.5.999",
         "django-template-i18n-lint>=1.2,<1.2.999",
         "django>=1.11,<1.11.999",
         "factory_boy>=2.8,<2.8.999",
         "mysqlclient>=1.3,<1.3.999",
+        "pypdf>=4.2,<5",
         "pylabels>=1.2,<1.2.999",
         "reportlab>=3.4,<3.4.999",
         "rules>=1.2,<1.2.999",
         "transifex-client>=0.12,<0.12.999",
     ],
 )
```

### Comparing `souschef-1.4.1/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg` & `souschef-1.4.2/souschef/160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/migrations/0001_initial.py` & `souschef-1.4.2/souschef/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/models.py` & `souschef-1.4.2/souschef/billing/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/add.html` & `souschef-1.4.2/souschef/billing/templates/billing/add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/billing_confirm_delete.html` & `souschef-1.4.2/souschef/billing/templates/billing/billing_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/list.html` & `souschef-1.4.2/souschef/billing/templates/billing/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/partials/statistics.html` & `souschef-1.4.2/souschef/billing/templates/billing/partials/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/partials/summary.html` & `souschef-1.4.2/souschef/billing/templates/billing/partials/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/print_summary.html` & `souschef-1.4.2/souschef/billing/templates/billing/print_summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/view.html` & `souschef-1.4.2/souschef/billing/templates/billing/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/templates/billing/view_orders.html` & `souschef-1.4.2/souschef/billing/templates/billing/view_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/tests.py` & `souschef-1.4.2/souschef/billing/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/urls.py` & `souschef-1.4.2/souschef/billing/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/billing/views.py` & `souschef-1.4.2/souschef/billing/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/configsamples/nginx.conf` & `souschef-1.4.2/souschef/configsamples/nginx.conf`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/dataload.py` & `souschef-1.4.2/souschef/dataload.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importaddresses.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importclients.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importcontactaddresses.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importcontactaddresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importmeals.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importmeals.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importorders.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/management/commands/importrelationships.py` & `souschef-1.4.2/souschef/datamigration/management/commands/importrelationships.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/datamigration/tests.py` & `souschef-1.4.2/souschef/datamigration/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/filters.py` & `souschef-1.4.2/souschef/delivery/filters.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/forms.py` & `souschef-1.4.2/souschef/delivery/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/migrations/0001_fix004a.py` & `souschef-1.4.2/souschef/delivery/migrations/0001_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/edit_delivery_route.html` & `souschef-1.4.2/souschef/delivery/templates/edit_delivery_route.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/ingredients.html` & `souschef-1.4.2/souschef/delivery/templates/ingredients.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/kitchen_count.html` & `souschef-1.4.2/souschef/delivery/templates/kitchen_count.html`

 * *Files 11% similar despite different names*

```diff
@@ -13,37 +13,35 @@
 <div class="ui secondary pointing fluid menu">
     <h1 class="ui header">{% trans "Kitchen Count Report" %}</h1>
     <div class="right menu">
       <div class="ui item"><h3><i class="calendar icon"></i>{{ delivery_date }}</h3></div>
     </div>
 </div>
 
-
 <div class="ui basic segment no-print">
-    {% if num_pages > 0 %}
-      <a href="{% url 'delivery:downloadKitchenCount' %}?delivery_date={{ delivery_date.isoformat }}" class="ui labeled icon right pink basic big button" title="{% trans 'Download the kitchen count report' %}">
+    {% if has_data %}
+      <a href="{% url 'delivery:kitchen_count' %}?delivery_date={{ delivery_date.isoformat }}&download=kitchen_count" class="ui labeled icon right pink basic big button" title="{% trans 'Download the kitchen count report' %}">
         <i class="download icon"></i>{% trans "Kitchen Count" %}
       </a>
     {% else %}
-      <a href="{% url 'delivery:downloadKitchenCount' %}?delivery_date={{ delivery_date.isoformat }}" class="ui disabled labeled icon right pink basic big button" title="{% trans 'No kitchen count report available' %}">
+      <a href="{% url 'delivery:kitchen_count' %}?delivery_date={{ delivery_date.isoformat }}&download=kitchen_count" class="ui disabled labeled icon right pink basic big button" title="{% trans 'No kitchen count report available' %}">
         <i class="download icon"></i>{% trans "Kitchen Count" %}
       </a>
     {% endif %}
-    {% if num_labels > 0 %}
-      <a href="{% url 'delivery:mealLabels' %}?delivery_date={{ delivery_date.isoformat }}" class="ui labeled icon right pink basic big button" title="{% trans 'Download the labels' %}">
+    {% if has_data %}
+      <a href="{% url 'delivery:kitchen_count' %}?delivery_date={{ delivery_date.isoformat }}&download=labels" class="ui labeled icon right pink basic big button" title="{% trans 'Download the labels' %}">
          <i class="download icon"></i>{% trans "Labels" %}
       </a>
     {% else %}
-        <a href="{% url 'delivery:mealLabels' %}?delivery_date={{ delivery_date.isoformat }}" class="ui disabled labeled icon right pink basic big button" title="{% trans 'No labels available' %}">
+        <a href="{% url 'delivery:kitchen_count' %}?delivery_date={{ delivery_date.isoformat }}&download=labels" class="ui disabled labeled icon right pink basic big button" title="{% trans 'No labels available' %}">
            <i class="download icon"></i>{% trans "Labels" %}
         </a>
     {% endif %}
 </div>
 
-
 <table class="ui very basic celled table">
   <thead>
    <tr class="top aligned">
     <th class="">{% trans 'Component' %}</th>
     <th class="">{% trans "TOTAL" %}<br>{% trans 'Regular' %}</th>
     <th class="">{% trans "TOTAL" %}<br>{% trans 'Large' %}</th>
     <th class="">{% trans 'Dish today' %}</th>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 {% extends "base.html" %} {% load i18n %} {% load rules %} {% block title %}{%
 trans 'Kitchen Count report' %} {% endblock %} {% block content %} {% has_perm
 'sous_chef.edit' request.user as can_edit_data %} {% include
 'kitchen_count_steps.html' with step='kitchen_count' %}
 ************ {{%% ttrraannss ""KKiittcchheenn CCoouunntt RReeppoorrtt"" %%}} ************
 {{{{ ddeelliivveerryy__ddaattee }}}}
-{% if num_pages > 0 %}
+{% if has_data %}
 _{_%_ _t_r_a_n_s_ _"_K_i_t_c_h_e_n_ _C_o_u_n_t_"_ _%_}
 {% else %}
 _{_%_ _t_r_a_n_s_ _"_K_i_t_c_h_e_n_ _C_o_u_n_t_"_ _%_}
-{% endif %} {% if num_labels > 0 %}
+{% endif %} {% if has_data %}
 _{_%_ _t_r_a_n_s_ _"_L_a_b_e_l_s_"_ _%_}
 {% else %}
 _{_%_ _t_r_a_n_s_ _"_L_a_b_e_l_s_"_ _%_}
 {% endif %}
                        {{%% ttrraannss    {{%% ttrraannss
 {{%% ttrraannss ''CCoommppoonneenntt''   ""TTOOTTAALL"" %%}}  ""TTOOTTAALL"" %%}}   {{%% ttrraannss     {{%% ttrraannss
 %%}}                     {{%% ttrraannss    {{%% ttrraannss     ''DDiisshh ttooddaayy'' ''IInnggrreeddiieennttss
```

### Comparing `souschef-1.4.1/souschef/delivery/templates/kitchen_count_steps.html` & `souschef-1.4.2/souschef/delivery/templates/kitchen_count_steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/partials/generated_orders.html` & `souschef-1.4.2/souschef/delivery/templates/partials/generated_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/partials/generated_orders_order_row_content.html` & `souschef-1.4.2/souschef/delivery/templates/partials/generated_orders_order_row_content.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/partials/generated_orders_table_head.html` & `souschef-1.4.2/souschef/delivery/templates/partials/generated_orders_table_head.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/review_orders.html` & `souschef-1.4.2/souschef/delivery/templates/review_orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/route_sheet.html` & `souschef-1.4.2/souschef/delivery/templates/route_sheet.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/templates/routes.html` & `souschef-1.4.2/souschef/delivery/templates/routes.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     <div class="right menu">
       <div class="ui item"><h3><i class="calendar icon"></i>{{ delivery_date }}</h3></div>
     </div>
 </div>
 
 <div class="row">
     <div class="column">
-        <a href="?print=yes&delivery_date={{ delivery_date.isoformat }}" class="ui big labeled icon right basic pink button {% if not all_configured %}disabled{% endif %}" title="{% trans 'Download the route sheets report' %}" target="_blank">
+        <a href="?delivery_date={{ delivery_date.isoformat }}&download=yes" class="ui big labeled icon right basic pink button {% if not all_configured %}disabled{% endif %}" title="{% trans 'Download the route sheets report' %}">
             <i class="download icon"></i>{% trans 'Route Sheets' %}
         </a>
         <i class="help-text question pink icon link" data-content="{% trans 'This is activated after organising all deliverable routes.' %}"></i>
     </div>
 </div>
 
 <div class="row">
```

### Comparing `souschef-1.4.1/souschef/delivery/tests.py` & `souschef-1.4.2/souschef/delivery/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import datetime
 import json
+from io import BytesIO
 
 from django.contrib.auth.models import User
 from django.db.models import Q
 from django.test import (
     RequestFactory,
     TestCase,
 )
 from django.urls import (
     reverse,
     reverse_lazy,
 )
 from django.utils import timezone as tz
-from django.utils.translation import (
-    ugettext,
-    ugettext_lazy,
-)
+from django.utils.translation import ugettext, ugettext_lazy
+from pypdf import PdfReader
 
 from souschef.meal.factories import (
     ComponentFactory,
     ComponentIngredientFactory,
     IncompatibilityFactory,
     IngredientFactory,
     RestrictedItemFactory,
@@ -55,168 +54,191 @@
 
 class KitchenCountReportTestCase(SousChefTestMixin, TestCase):
     # This data set includes 'Ground porc' clashing ingredient
     # This data set includes 'Tracy' client lastname
     #   and his side dish is 'compote'
     fixtures = ["sample_data"]
 
-    @classmethod
-    def setUpTestData(cls):
-        Menu.create_menu_and_components(
-            datetime.date(2016, 5, 21),
-            [
-                "Ginger pork",
-                "Green Salad",
-                "Fruit Salad",
-                "Day s Dessert",
-                "Day s Diabetic Dessert",
-                "Day s Pudding",
-                "Day s Compote",
-            ],
-        )
-
     def setUp(self):
         self.force_login()
 
     def test_clashing_ingredient(self):
         """An ingredient we know will clash must be in the page"""
-        self.today = datetime.date.today()
+        today = datetime.date.today()
         # create orders today
         clients = Client.active.all()
-        Order.objects.auto_create_orders(self.today, clients)
+        Order.objects.auto_create_orders(today, clients)
         # main dish and its ingredients today
         main_dishes = Component.objects.filter(name="Ginger pork")
         main_dish = main_dishes[0]
         dish_ingredients = Component.get_recipe_ingredients(main_dish.id)
         for ing in dish_ingredients:
-            ci = Component_ingredient(
-                component=main_dish, ingredient=ing, date=self.today
-            )
+            ci = Component_ingredient(component=main_dish, ingredient=ing, date=today)
             ci.save()
         # Add extra ingredient so that more clashing clients will
         #  require two pages on the PDF kitchen count report
         extra = Ingredient.objects.get(name="Walnuts")
-        ci = Component_ingredient(
-            component=main_dish, ingredient=extra, date=self.today
-        )
+        ci = Component_ingredient(component=main_dish, ingredient=extra, date=today)
         ci.save()
         # add sides ingredient
         sides_component = Component.objects.get(
             component_group=COMPONENT_GROUP_CHOICES_SIDES
         )
         extra = Ingredient.objects.get(name="Cabbage")
         ci = Component_ingredient(
-            component=sides_component, ingredient=extra, date=self.today
+            component=sides_component, ingredient=extra, date=today
         )
         ci.save()
         # menu today
         Menu.create_menu_and_components(
-            self.today,
+            today,
             [
                 "Ginger pork",
                 "Green Salad",
                 "Fruit Salad",
                 "Day s Dessert",
                 "Day s Diabetic Dessert",
                 "Day s Pudding",
                 "Day s Compote",
             ],
         )
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today()},
+            {"delivery_date": datetime.date.today(), "download": "kitchen_count"},
         )
-        self.assertTrue(b"Ground porc" in response.content)
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Ground porc" in pdf_content)
 
     def test_no_components(self):
-        """No orders on this day therefore no component summary"""
+        """No orders on this day therefore no documents to download."""
+        menu_day = datetime.date(1999, 1, 1)
+        Menu.create_menu_and_components(
+            menu_day,
+            [
+                "Ginger pork",
+                "Green Salad",
+                "Fruit Salad",
+                "Day s Dessert",
+                "Day s Diabetic Dessert",
+                "Day s Pudding",
+                "Day s Compote",
+            ],
+        )
+        # main dish and its ingredients today
+        main_dishes = Component.objects.filter(name="Ginger pork")
+        main_dish = main_dishes[0]
+        dish_ingredients = Component.get_recipe_ingredients(main_dish.id)
+        for ing in dish_ingredients:
+            ci = Component_ingredient(
+                component=main_dish, ingredient=ing, date=menu_day
+            )
+            ci.save()
+        # add sides ingredient
+        sides_component = Component.objects.get(
+            component_group=COMPONENT_GROUP_CHOICES_SIDES
+        )
+        extra = Ingredient.objects.get(name="Cabbage")
+        ci = Component_ingredient(
+            component=sides_component, ingredient=extra, date=menu_day
+        )
+        ci.save()
+
         response = self.client.get(
             reverse("delivery:kitchen_count"),
-            {"delivery_date": "2015-05-21"},
+            {"delivery_date": menu_day.isoformat()},
         )
-        self.assertTrue(b"SUBTOTAL" not in response.content)
+        self.assertEqual(response.status_code, 200)
+        self.assertTrue(b"No kitchen count report available" in response.content)
 
-    def test_labels_show_restrictions(self):
-        """An ingredient we know will clash must be in the labels"""
+    def test_pdf_kitchen_count_and_labels_reports(self):
         # generate orders today
-        self.today = datetime.date.today()
+        today = datetime.date.today()
         clients = Client.active.all()
-        Order.objects.auto_create_orders(self.today, clients)
+        Order.objects.auto_create_orders(today, clients)
         # main dish and its ingredients today
         main_dishes = Component.objects.filter(name="Ginger pork")
         main_dish = main_dishes[0]
         dish_ingredients = Component.get_recipe_ingredients(main_dish.id)
         for ing in dish_ingredients:
-            ci = Component_ingredient(
-                component=main_dish, ingredient=ing, date=self.today
-            )
+            ci = Component_ingredient(component=main_dish, ingredient=ing, date=today)
             ci.save()
         # Add sides ingredient
         sides_component = Component.objects.get(
             component_group=COMPONENT_GROUP_CHOICES_SIDES
         )
         # This ingredient is in the restrictions of some clients in the data
         sides_ingredient = Ingredient.objects.get(name="Brussel sprouts")
         ci = Component_ingredient(
-            component=sides_component, ingredient=sides_ingredient, date=self.today
+            component=sides_component, ingredient=sides_ingredient, date=today
         )
         ci.save()
         # menu today
         Menu.create_menu_and_components(
-            self.today,
+            today,
             [
                 "Ginger pork",
                 "Green Salad",
                 "Fruit Salad",
                 "Day s Dessert",
                 "Day s Diabetic Dessert",
                 "Day s Pudding",
                 "Day s Compote",
                 "Days Sides",
             ],
         )
 
-        self.client.get(
+        response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
+        self.assertEqual(response.status_code, 200)
+        self.assertTrue("ReportLab" in repr(response.content))
+
         response = self.client.get(
-            reverse_lazy("delivery:mealLabels"),
-            {"delivery_date": datetime.date.today().isoformat()},
+            reverse_lazy("delivery:kitchen_count"),
+            {"delivery_date": datetime.date.today().isoformat(), "download": "labels"},
         )
+        self.assertEqual(response.status_code, 200)
         self.assertTrue("ReportLab" in repr(response.content))
 
-    def test_pdf_report_show_restrictions(self):
-        """An ingredient we know will clash must be in the pdf report"""
-        # generate orders today
-        self.today = datetime.date.today()
+    def test_ingredients_not_defined_redirect(self):
+        # generate orders
+        today = datetime.date.today()
         clients = Client.active.all()
-        Order.objects.auto_create_orders(self.today, clients)
-        Menu.create_menu_and_components(
-            self.today,
+        created_orders = Order.objects.auto_create_orders(today, clients)
+        self.assertTrue(created_orders)
+
+        num_menu_comp_created = Menu.create_menu_and_components(
+            today,
             [
                 "Ginger pork",
                 "Green Salad",
                 "Fruit Salad",
                 "Day s Dessert",
                 "Day s Diabetic Dessert",
                 "Day s Pudding",
                 "Day s Compote",
             ],
         )
+        self.assertEqual(num_menu_comp_created, 7)
 
-        self.client.get(
-            "/delivery/kitchen_count/",
-            {"delivery_date": datetime.date.today().isoformat()},
-        )
         response = self.client.get(
-            "/delivery/viewDownloadKitchenCount/",
-            {"delivery_date": datetime.date.today().isoformat()},
+            reverse_lazy("delivery:kitchen_count"),
+            {
+                "delivery_date": today.isoformat(),
+            },
         )
-        self.assertTrue("ReportLab" in repr(response.content))
+        # Ingredients were not defined; kitchen count page will redirect to the
+        # ingredients page.
+        self.assertEqual(response.status_code, 302)
 
 
 class ChooseDayMainDishIngredientsTestCase(SousChefTestMixin, TestCase):
     fixtures = ["sample_data"]
 
     @classmethod
     def setUpTestData(cls):
@@ -254,17 +276,23 @@
         req["sides_ingredients"] = [
             Ingredient.objects.filter(name="zucchini").first().id
         ]
         req["delivery_date"] = datetime.date.today().isoformat()
         response = self.client.post(reverse_lazy("delivery:meal"), req)
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
-        self.assertTrue(b"Ginger pork" in response.content)
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Ginger pork" in pdf_content)
 
     def test_remember_day_ingredients(self):
         """After Kitchen Count Report we remember chosen ingredients."""
         response = self.client.get(reverse_lazy("delivery:meal"))
         maindish = Component.objects.get(name="Ginger pork")
         cis = Component_ingredient.objects.filter(date=None, component=maindish)
         ing_ids = [ci.ingredient.id for ci in cis]
@@ -273,17 +301,23 @@
         req["maindish"] = str(maindish.id)
         req["ingredients"] = ing_ids
         req["sides_ingredients"] = [Ingredient.objects.filter(name="Onions").first().id]
         req["delivery_date"] = datetime.date.today().isoformat()
         response = self.client.post(reverse_lazy("delivery:meal"), req)
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
-        self.assertTrue(b"Ginger pork" in response.content)
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Ginger pork" in pdf_content)
         response = self.client.get(
             reverse_lazy("delivery:meal"),
             {"delivery_date": datetime.date.today().isoformat()},
         )
         self.assertTrue(b"Ginger pork" in response.content)
 
     def test_restore_dish_recipe(self):
@@ -299,19 +333,24 @@
         req["maindish"] = str(maindish.id)
         req["ingredients"] = ing_ids + [Ingredient.objects.get(name="Pepper").id]
         req["sides_ingredients"] = [Ingredient.objects.all().first().id]
         req["delivery_date"] = datetime.date.today().isoformat()
         response = self.client.post(reverse_lazy("delivery:meal"), req)
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
-        )
-        self.assertTrue(
-            b"Ginger pork" in response.content and b"Pepper" in response.content
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Ginger pork" in pdf_content)
+        self.assertTrue("Pepper" in pdf_content)
         # restore recipe
         response = self.client.post(
             reverse_lazy("delivery:meal"),
             {
                 "_restore": "Restore recipe",
                 "delivery_date": datetime.date.today().isoformat(),
             },
@@ -323,19 +362,24 @@
         req["ingredients"] = ing_ids
         req["sides_ingredients"] = [Ingredient.objects.all().first().id]
         req["delivery_date"] = datetime.date.today().isoformat()
         response = self.client.post(reverse_lazy("delivery:meal"), req)
         # check that we have Ginger pork with no Pepper in Kitchen count
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
-        )
-        self.assertTrue(
-            b"Ginger pork" in response.content and b"Pepper" not in response.content
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Ginger pork" in pdf_content)
+        self.assertTrue("Pepper" not in pdf_content)
 
     def test_change_main_dish(self):
         """Change dish then go directly to Kitchen Count Report."""
         maindish = Component.objects.get(name="Coq au vin")
         cis = Component_ingredient.objects.filter(date=None, component=maindish)
         ing_ids = [ci.ingredient.id for ci in cis]
 
@@ -345,17 +389,23 @@
         req["maindish"] = str(maindish.id)
         req["ingredients"] = ing_ids
         req["sides_ingredients"] = [Ingredient.objects.all().first().id]
         req["delivery_date"] = datetime.date.today().isoformat()
         response = self.client.post(reverse_lazy("delivery:meal"), req)
         response = self.client.get(
             reverse_lazy("delivery:kitchen_count"),
-            {"delivery_date": datetime.date.today().isoformat()},
+            {
+                "delivery_date": datetime.date.today().isoformat(),
+                "download": "kitchen_count",
+            },
         )
-        self.assertTrue(b"Coq au vin" in response.content)
+        self.assertEqual(response.status_code, 200)
+        pdf_data = PdfReader(BytesIO(response.content))
+        pdf_content = pdf_data.pages[0].extract_text()
+        self.assertTrue("Coq au vin" in pdf_content)
 
     def test_post_invalid_form(self):
         """Invalid form."""
         response = self.client.get(reverse_lazy("delivery:meal"))
         req = {}
         req["_update"] = "Next: Print Kitchen Count"
         req["maindish"] = "wrong"
@@ -570,15 +620,14 @@
         check(reverse("delivery:order"))
         check(reverse("delivery:meal"))
         meal = Component.objects.first()
         meal_id = meal.id
         check(reverse("delivery:meal_id", kwargs={"id": meal_id}))
         check(reverse("delivery:routes"))
         check(reverse("delivery:kitchen_count"))
-        check(reverse("delivery:mealLabels"))
         check(reverse("delivery:route_sheet", kwargs={"pk": 1}))
         check(reverse("delivery:refresh_orders"))
 
 
 class OrderlistViewTestCase(SousChefTestMixin, TestCase):
     fixtures = ["sample_data"]
 
@@ -672,15 +721,15 @@
         # Run
         response_1 = self.client.get(
             url,
             {"delivery_date": datetime.date.today().isoformat()},
         )
         response_2 = self.client.get(
             url,
-            {"print": "yes", "delivery_date": datetime.date.today().isoformat()},
+            {"download": "yes", "delivery_date": datetime.date.today().isoformat()},
         )
         # Check
         self.assertNotIn("routes_dict", response_1)
         self.assertIn("routes_dict", response_2)
 
     def test_redirects_users_who_do_not_have_read_permission(self):
         # Setup
@@ -759,45 +808,14 @@
             url,
             {"delivery_date": datetime.date.today().isoformat()},
         )
         # Check
         self.assertEqual(response.status_code, 200)
 
 
-class MealLabelsViewTestCase(SousChefTestMixin, TestCase):
-    fixtures = ["sample_data"]
-
-    def test_redirects_users_who_do_not_have_read_permission(self):
-        # Setup
-        User.objects.create_user(
-            username="foo", email="foo@example.com", password="secure"
-        )
-        self.client.login(username="foo", password="secure")
-        url = reverse("delivery:mealLabels")
-        # Run & check
-        self.assertRedirectsWithAllMethods(url)
-
-    def test_allow_access_to_users_with_read_permission(self):
-        # Setup
-        user = User.objects.create_user(
-            username="foo", email="foo@example.com", password="secure"
-        )
-        user.is_staff = True
-        user.save()
-        self.client.login(username="foo", password="secure")
-        url = reverse("delivery:mealLabels")
-        # Run
-        response = self.client.get(
-            url,
-            {"delivery_date": datetime.date.today().isoformat()},
-        )
-        # Check
-        self.assertEqual(response.status_code, 200)
-
-
 class RefreshOrderViewTestCase(SousChefTestMixin, TestCase):
     def test_redirects_users_who_do_not_have_edit_permission(self):
         # Setup
         user = User.objects.create_user(
             username="foo", email="foo@example.com", password="secure"
         )
         user.is_staff = True
@@ -1153,16 +1171,15 @@
             reverse("delivery:meal")
             + f"?delivery_date={datetime.date.today().isoformat()}",
         )
         response = self.client.get(
             reverse("delivery:kitchen_count"),
             {"delivery_date": datetime.date.today().isoformat()},
         )
-        num_labels = response.context["num_labels"]
-        self.assertEqual(num_labels, 1)  # only c_valid
+        self.assertEqual(response.context["has_data"], True)
 
     def test_step_4__routes_before_organizing(self):
         """
         Should ignore route==None and non geolocalized clients.
         When the delivery history doesn't exist or it's invalid,
         don't let route sheet and route sheets work.
         """
@@ -1189,15 +1206,15 @@
             DeliveryHistory.objects.filter(
                 route=self.route2, date=tz.datetime.today()
             ).exists()
         )
         # Assert print doesn't work
         response = self.client.get(
             reverse("delivery:routes"),
-            {"print": "yes", "delivery_date": datetime.date.today().isoformat()},
+            {"download": "yes", "delivery_date": datetime.date.today().isoformat()},
         )
         self.assertEqual(response.status_code, 404)
         # Assert route sheets don't exist
         response = self.client.get(
             reverse("delivery:route_sheet", args=[self.route1.pk]),
             {"delivery_date": datetime.date.today().isoformat()},
         )
@@ -1215,15 +1232,15 @@
             # As long as this sequence is not exactly same as the clients',
             # it's always invalid, even if it contains all the clients.
             client_id_sequence=[999999, 888888, self.c_valid.pk],
         )
         # Assert print doesn't work
         response = self.client.get(
             reverse("delivery:routes"),
-            {"print": "yes", "delivery_date": datetime.date.today().isoformat()},
+            {"download": "yes", "delivery_date": datetime.date.today().isoformat()},
         )
         self.assertEqual(response.status_code, 404)
 
     def test_step_4__routes_after_organizing(self):
         """
         Should ignore route==None and not geolocalized
         """
@@ -1292,15 +1309,15 @@
             {"delivery_date": datetime.date.today().isoformat()},
         )
         self.assertEqual(response.status_code, 404)
 
         # Assert print works
         response = self.client.get(
             reverse("delivery:routes"),
-            {"delivery_date": datetime.date.today().isoformat(), "print": "yes"},
+            {"delivery_date": datetime.date.today().isoformat(), "download": "yes"},
         )
         self.assertEqual(response.status_code, 200)
         # Check print result
         routes_dict = json.loads(response["routes_dict"])
         # only route1 has one client
         route1 = routes_dict[str(self.route1.id)]
         self.assertEqual(len(route1["detail_lines"]), 1)
@@ -1405,13 +1422,13 @@
                     + f"?delivery_date={datetime.date.today().isoformat()}",
                 )
 
         # generate the PDF route sheets of all the routes
         response = self.client.get(
             reverse("delivery:routes"),
             {
-                "print": "yes",
+                "download": "yes",
                 "delivery_date": datetime.date.today().isoformat(),
             },
         )
         self.assertEqual(response.status_code, 200)
         self.assertTrue("ReportLab" in repr(response.content))
```

### Comparing `souschef-1.4.1/souschef/delivery/tsp.py` & `souschef-1.4.2/souschef/delivery/tsp.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/delivery/urls.py` & `souschef-1.4.2/souschef/delivery/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from django.utils.translation import ugettext_lazy as _
 
 from souschef.delivery.views import (
     CreateDelivery,
     DeliveryRouteSheet,
     EditDeliveryRoute,
     KitchenCount,
-    KitchenCountDownload,
     MealInformation,
-    MealLabels,
     RefreshOrderView,
     ReviewOrders,
     RoutesInformation,
 )
 
 app_name = "delivery"
 
@@ -29,19 +27,13 @@
     url(
         _(r"^route/(?P<pk>\d+)/create/$"),
         CreateDelivery.as_view(),
         name="create_delivery",
     ),
     url(_(r"^kitchen_count/$"), KitchenCount.as_view(), name="kitchen_count"),
     url(
-        _(r"^viewDownloadKitchenCount/$"),
-        KitchenCountDownload.as_view(),
-        name="downloadKitchenCount",
-    ),
-    url(_(r"^viewMealLabels/$"), MealLabels.as_view(), name="mealLabels"),
-    url(
         _(r"^route_sheet/(?P<pk>\d+)/$"),
         DeliveryRouteSheet.as_view(),
         name="route_sheet",
     ),
     url(_(r"^refresh_orders/$"), RefreshOrderView.as_view(), name="refresh_orders"),
 ]
```

### Comparing `souschef-1.4.1/souschef/delivery/views.py` & `souschef-1.4.2/souschef/delivery/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import collections
 import json
 import os
 import textwrap
+from copy import deepcopy
 from dataclasses import dataclass
 from datetime import date, datetime
+from pathlib import Path
 from typing import List
 
 import labels  # package pylabels
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin.models import LogEntry
 from django.contrib.auth.mixins import (
@@ -77,28 +79,32 @@
 LOGO_IMAGE = os.path.join(
     settings.BASE_DIR,
     "160widthSR-Logo-Screen-PurpleGreen-HI-RGB1.jpg",
 )
 DELIVERY_STARTING_POINT_LAT_LONG = (45.516564, -73.575145)  # Santropol Roulant
 
 
-def _get_pdf_filename(base_filename, delivery_date):
-    return f"{base_filename.rstrip('.pdf')}_{delivery_date.strftime('%Y%m%d')}.pdf"
+def _get_pdf_file_path(filename, delivery_date):
+    delivery = delivery_date.strftime("%Y-%m-%d")
+    today = datetime.now().replace(microsecond=0).isoformat()
+    filepath = Path(filename)
+    new_name = f"{filepath.name.rstrip('.pdf')}_{delivery}__{today}.pdf"
+    return filepath.parent / delivery / new_name
 
 
-def get_meals_label_filename(delivery_date):
-    return _get_pdf_filename(settings.MEAL_LABELS_FILE, delivery_date)
+def get_meals_label_file_path(delivery_date):
+    return _get_pdf_file_path(settings.MEAL_LABELS_FILE, delivery_date)
 
 
-def get_kitchen_count_filename(delivery_date):
-    return _get_pdf_filename(settings.KITCHEN_COUNT_FILE, delivery_date)
+def get_kitchen_count_file_path(delivery_date):
+    return _get_pdf_file_path(settings.KITCHEN_COUNT_FILE, delivery_date)
 
 
-def get_route_sheets_filename(delivery_date):
-    return _get_pdf_filename(settings.ROUTE_SHEETS_FILE, delivery_date)
+def get_route_sheets_file_path(delivery_date):
+    return _get_pdf_file_path(settings.ROUTE_SHEETS_FILE, delivery_date)
 
 
 def get_orders_for_kitchen_count(order_statuses, delivery_date=None):
     return (
         Order.objects.get_orders(
             delivery_date=delivery_date, order_statuses=order_statuses
         )
@@ -363,25 +369,25 @@
     The view must first determine whether each of the routes with orders
     has been "organized by the user".
 
     By default the view displays a list of all the known routes
     indicating for each route the number of orders and its organize state.
     The view then creates the context to be rendered on the page.
 
-    If the request includes argument "print=yes", the view obtains
+    If the request includes argument "download=yes", the view obtains
     for each route the detailed orders to be delivered, sorts them in the
     chosen sequence and combines all the routes in a PDF report that
     is stored in the BASE_DIR and then downloaded by the browser.
     """
 
     permission_required = "sous_chef.read"
 
     @property
-    def doprint(self):
-        return self.request.GET.get("print", False)
+    def download(self):
+        return self.request.GET.get("download", False)
 
     def get(self, request, *args, **kwargs):
         delivery_date = date.fromisoformat(request.GET["delivery_date"])
         routes = Route.objects.all()
         route_details = []
         all_configured = True
         for route in routes:
@@ -403,15 +409,15 @@
                 # `client_id_sequence` is not iterable.
                 has_organised = "invalid"
 
             route_details.append((route, order_count, has_organised, delivery_history))
             if order_count > 0 and has_organised != "yes":
                 all_configured = False
 
-        if not self.doprint:
+        if not self.download:
             # display list of delivery routes on web page
             return render(
                 request,
                 "routes.html",
                 {
                     "all_configured": all_configured,
                     "delivery_date": delivery_date,
@@ -433,39 +439,26 @@
                 summary_lines, detail_lines = drs_make_lines(route_list)
                 routes_dict[delivery_history.route_id] = {
                     "route": delivery_history.route,
                     "summary_lines": summary_lines,
                     "detail_lines": detail_lines,
                 }
             # generate PDF report
-            MultiRouteReport.routes_make_pages(routes_dict, delivery_date)
-            filename = get_route_sheets_filename(delivery_date)
-            try:
-                f = open(filename, "rb")  # noqa: SIM115
-            except Exception as e:
-                raise Http404(f"File {filename} does not exist.") from e
-            response = HttpResponse(content_type="application/pdf")
-            response[
-                "Content-Disposition"
-            ] = 'attachment; filename="routesheets{}.pdf"'.format(
-                delivery_date.strftime("%Y%m%d")
-            )
+            file_path = MultiRouteReport.routes_make_pages(routes_dict, delivery_date)
+            response = download_pdf(file_path)
             # add serializable data in response header to be used in unit tests
             routes_dict_fortest = {}
             for key, item in routes_dict.items():
                 routes_dict_fortest[key] = {
                     "route": item["route"].name,
                     "detail_lines": [
                         client.lastname for client in item["detail_lines"]
                     ],
                 }
             response["routes_dict"] = json.dumps(routes_dict_fortest)
-            #
-            response.write(f.read())
-            f.close()
             return response
 
 
 class CreateDelivery(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     permission_required = "sous_chef.edit"
 
     def post(self, request, pk, *args, **kwargs):
@@ -862,16 +855,18 @@
 
         def go():
             """Generate the pages.
 
             Returns:
                 An integer : The number of pages generated.
             """
+            file_path = get_route_sheets_file_path(delivery_date)
+            file_path.parent.mkdir(parents=True, exist_ok=True)
             doc = MultiRouteReport.RLMultiRouteDocTemplate(
-                get_route_sheets_filename(delivery_date),
+                str(file_path),
                 leftMargin=0.5 * rl_inch,
                 rightMargin=0.5 * rl_inch,
                 bottomMargin=0.5 * rl_inch,
                 footerFunc=drawFooter,
             )
             # initialize
             MultiRouteReport.table_split = 0
@@ -1015,144 +1010,157 @@
             # build full document
             doc.build(
                 story,
                 onFirstPage=drawHeader,
                 onLaterPages=drawHeader,
             )
 
-            return doc.page  # number of last page
+            return file_path
 
         # END def
-        return go()  # returns number of pages generated
+        return go()  # returns the file path
 
 
 # END Route sheet report.
 
 
 # Kitchen count report view, helper classes and functions
 
 
-class KitchenCountDownload(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
-    permission_required = "sous_chef.read"
+class IngredientsMissingError(Exception):
+    pass
 
-    def get(self, request, *args, **kwargs):
-        delivery_date = date.fromisoformat(request.GET["delivery_date"])
-        # download kitchen count report as PDF
-        filename = get_kitchen_count_filename(delivery_date)
-        try:
-            f = open(filename, "rb")  # noqa: SIM115
-        except Exception as e:
-            raise Http404(f"File {filename} does not exist.") from e
+
+def get_kitchen_list(delivery_date):
+    # Display kitchen count report for given delivery date
+    # and generate meal labels.
+    #  get sides component
+    try:
+        sides_component = Component.objects.get(
+            component_group=COMPONENT_GROUP_CHOICES_SIDES
+        )
+    except Component.DoesNotExist as e:
+        raise Exception(
+            "The database must contain exactly one component "
+            + "having 'Component group' = 'Sides' "
+        ) from e
+    # check if main dish ingredients were confirmed
+    main_ingredients = Component_ingredient.objects.filter(date=delivery_date).exclude(
+        component=sides_component
+    )
+    # check if sides ingredients were confirmed
+    sides_ingredients = Component_ingredient.objects.filter(
+        component=sides_component, date=delivery_date
+    )
+    if len(main_ingredients) == 0 or len(sides_ingredients) == 0:
+        raise IngredientsMissingError
+
+    kitchen_list_unfiltered = Order.get_kitchen_items(delivery_date)
+
+    # filter out route=None clients and not geolocalized clients
+    kitchen_list = {}
+    geolocalized_client_ids = list(
+        Client.objects.filter(
+            pk__in=kitchen_list_unfiltered.keys(),
+            member__address__latitude__isnull=False,
+            member__address__longitude__isnull=False,
+        ).values_list("pk", flat=True)
+    )
+
+    for client_id, kitchen_item in kitchen_list_unfiltered.items():
+        if kitchen_item.routename is not None and client_id in geolocalized_client_ids:
+            kitchen_list[client_id] = kitchen_item
+
+    return kitchen_list
+
+
+def make_kitchen_count(kitchen_list, component_lines, meal_lines, delivery_date):
+    if not component_lines:
+        # we have no orders on that date
+        return
+    preperation_lines_with_incompatible_ingr = kcr_make_preparation_lines(
+        kitchen_list, "only_clients_with_incompatible_ingredients"
+    )
+    preperation_lines_without_incompatible_ingr = kcr_make_preparation_lines(
+        kitchen_list, "only_clients_without_incompatible_ingredients"
+    )
+    return kcr_make_pages(  # kitchen count as PDF
+        delivery_date,
+        component_lines,
+        meal_lines,  # summary
+        preperation_lines_with_incompatible_ingr,
+        preperation_lines_without_incompatible_ingr,
+    )  # detail
+
+
+def make_labels(kitchen_list, component_lines, delivery_date):
+    if not component_lines:
+        return
+    return kcr_make_labels(  # meal labels as PDF
+        delivery_date,
+        kitchen_list,  # KitchenItems
+        component_lines[0].name,  # main dish name
+        component_lines[0].ingredients,
+    )  # main dish ingredients
+
+
+def download_pdf(file_path):
+    with open(file_path, "rb") as f:
         response = HttpResponse(content_type="application/pdf")
-        response[
-            "Content-Disposition"
-        ] = 'attachment; filename="kitchencount{}.pdf"'.format(
-            delivery_date.strftime("%Y%m%d")
-        )
+        response["Content-Disposition"] = f'attachment; filename="{file_path.name}"'
         response.write(f.read())
-        f.close()
         return response
 
 
 class KitchenCount(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     permission_required = "sous_chef.read"
 
     def get(self, request, *args, **kwargs):
         delivery_date = date.fromisoformat(request.GET["delivery_date"])
+        download = request.GET.get("download")
 
-        # Display kitchen count report for given delivery date
-        # and generate meal labels.
-        #  get sides component
         try:
-            sides_component = Component.objects.get(
-                component_group=COMPONENT_GROUP_CHOICES_SIDES
-            )
-        except Component.DoesNotExist as e:
-            raise Exception(
-                "The database must contain exactly one component "
-                + "having 'Component group' = 'Sides' "
-            ) from e
-        # check if main dish ingredients were confirmed
-        main_ingredients = Component_ingredient.objects.filter(
-            date=delivery_date
-        ).exclude(component=sides_component)
-        # check if sides ingredients were confirmed
-        sides_ingredients = Component_ingredient.objects.filter(
-            component=sides_component, date=delivery_date
-        )
-        if len(main_ingredients) == 0 or len(sides_ingredients) == 0:
+            kitchen_list = get_kitchen_list(delivery_date)
+        except IngredientsMissingError:
             # some ingredients not confirmed, must go back one step
             messages.add_message(
                 self.request,
                 messages.WARNING,
                 _(
                     "Please check main dish and confirm "
                     "all ingredients before proceeding to kitchen count."
                 ),
             )
             return HttpResponseRedirect(
                 reverse_lazy("delivery:meal")
                 + f"?delivery_date={request.GET['delivery_date']}"
             )
 
-        kitchen_list_unfiltered = Order.get_kitchen_items(delivery_date)
+        component_lines = kcr_make_component_lines(kitchen_list, delivery_date)
+        meal_lines = kcr_make_meal_lines(kitchen_list)
 
-        # filter out route=None clients and not geolocalized clients
-        kitchen_list = {}
-        geolocalized_client_ids = list(
-            Client.objects.filter(
-                pk__in=kitchen_list_unfiltered.keys(),
-                member__address__latitude__isnull=False,
-                member__address__longitude__isnull=False,
-            ).values_list("pk", flat=True)
-        )
+        file_path = None
+        if download == "kitchen_count":
+            file_path = make_kitchen_count(
+                kitchen_list, component_lines, meal_lines, delivery_date
+            )
+        elif download == "labels":
+            file_path = make_labels(kitchen_list, component_lines, delivery_date)
 
-        for client_id, kitchen_item in kitchen_list_unfiltered.items():
-            if (
-                kitchen_item.routename is not None
-                and client_id in geolocalized_client_ids
-            ):
-                kitchen_list[client_id] = kitchen_item
+        if file_path:
+            return download_pdf(file_path)
 
-        component_lines = kcr_make_component_lines(kitchen_list, delivery_date)
-        meal_lines = kcr_make_meal_lines(kitchen_list)
-        preperation_lines_with_incompatible_ingr = kcr_make_preparation_lines(
-            kitchen_list, "only_clients_with_incompatible_ingredients"
-        )
-        preperation_lines_without_incompatible_ingr = kcr_make_preparation_lines(
-            kitchen_list, "only_clients_without_incompatible_ingredients"
-        )
-        if component_lines:
-            # we have orders on that date
-            num_pages = kcr_make_pages(  # kitchen count as PDF
-                delivery_date,
-                component_lines,
-                meal_lines,  # summary
-                preperation_lines_with_incompatible_ingr,
-                preperation_lines_without_incompatible_ingr,
-            )  # detail
-            num_labels = kcr_make_labels(  # meal labels as PDF
-                delivery_date,
-                kitchen_list,  # KitchenItems
-                component_lines[0].name,  # main dish name
-                component_lines[0].ingredients,
-            )  # main dish ingredients
-        else:
-            # no orders on that date
-            num_pages = 0
-            num_labels = 0
         return render(
             request,
             "kitchen_count.html",
             {
                 "component_lines": component_lines,
                 "delivery_date": delivery_date,
+                "has_data": bool(kitchen_list),
                 "meal_lines": meal_lines,
-                "num_pages": num_pages,
-                "num_labels": num_labels,
             },
         )
 
 
 component_line_fields = [  # Component summary Line on Kitchen Count.
     # field name       default value
     "component_group",
@@ -1269,27 +1277,31 @@
     line_start = 0
     rsubtotal, lsubtotal = (0, 0)
     client_id, kitchen_item = next(clients, (0, 0))  # has end sentinel
     while client_id > 0:
         if rsubtotal == 0 and lsubtotal == 0:
             # add line for subtotal at top of combination
             meal_lines.append(MealLine(*meal_line_fields[1::2]))
-        combination = kitchen_item.incompatible_ingredients
+        ingredients_clashing = kitchen_item.incompatible_ingredients
         meal_lines.append(meal_line(kitchen_item))
         rsubtotal, lsubtotal = kcr_cumulate(rsubtotal, lsubtotal, kitchen_item)
         client_id, kitchen_item = next(clients, (0, 0))
-        if client_id == 0 or combination != kitchen_item.incompatible_ingredients:
-            # last line of this combination of ingredients
+        if (
+            client_id == 0
+            or ingredients_clashing != kitchen_item.incompatible_ingredients
+        ):
+            # last line of this combination of clashing ingredients
             line_end = len(meal_lines)
-            # set rowspan to total number of lines for this combination
+            # set rowspan to total number of lines for this combination of clashing
+            # ingredients
             meal_lines[line_start] = meal_lines[line_start]._replace(
                 client="SUBTOTAL",
                 rqty=str(rsubtotal),
                 lqty=str(lsubtotal),
-                ingr_clash=", ".join(combination),
+                ingr_clash=", ".join(ingredients_clashing),
                 span=str(line_end - line_start),
             )
             rtotal, ltotal = (rtotal + rsubtotal, ltotal + lsubtotal)
             rsubtotal, lsubtotal = (0, 0)
             # hide ingredients for lines following the first
             for j in range(line_start + 1, line_end):
                 meal_lines[j] = meal_lines[j]._replace(span="-1")
@@ -1565,59 +1577,71 @@
 
     def go():
         """Generate the pages.
 
         Returns:
             An integer : The number of pages generated.
         """
-        doc = RLSimpleDocTemplate(get_kitchen_count_filename(kcr_date))
+        file_path = get_kitchen_count_file_path(kcr_date)
+        file_path.parent.mkdir(parents=True, exist_ok=True)
+        doc = RLSimpleDocTemplate(str(file_path))
         story = []
 
         # begin Summary section
-        story.append(RLSpacer(1, 0.25 * rl_inch))
         rows = []
+
+        # Menu name
+        menu = component_lines[0].name if component_lines else ""
+        title_style = deepcopy(styles["NormalLeftBold"])
+        title_style.spaceBefore = 0
+        title_style.leftIndent = 60
+        title_style.fontSize = 14
+        story.append(RLParagraph(menu, title_style))
+        story.append(RLSpacer(1, 0.5 * rl_inch))
+
+        # Component table
+        small_left = deepcopy(styles["SmallRight"])
+        small_left.alignment = 0
+
         rows.append(
             [
+                RLParagraph("Component", styles["NormalLeft"]),
+                RLParagraph("Total", styles["NormalLeft"]),
                 "",
-                RLParagraph("TOTAL", styles["NormalCenter"]),
-                "",
-                RLParagraph("Menu", styles["NormalLeft"]),
                 RLParagraph("Ingredients", styles["NormalLeft"]),
             ]
         )
         rows.append(
             [
                 "",
-                RLParagraph("Regular", styles["SmallRight"]),
-                RLParagraph("Large", styles["SmallRight"]),
-                "",
+                RLParagraph("Regular", small_left),
+                RLParagraph("Large", small_left),
                 "",
             ]
         )
         for cl in component_lines:
             rows.append(
                 [
                     cl.component_group,
                     cl.rqty,
                     cl.lqty,
-                    cl.name,
                     RLParagraph(cl.ingredients, styles["NormalLeft"]),
                 ]
             )
         tab = RLTable(
             rows,
-            colWidths=(100, 40, 40, 120, 220),
+            colWidths=(100, 40, 40, 340),
             style=[
-                ("VALIGN", (0, 0), (-1, 1), "TOP"),
-                ("VALIGN", (0, 2), (-1, -1), "BOTTOM"),
-                ("GRID", (1, 0), (-1, 1), 1, rl_colors.black),
+                # style, start cell, end cell, params
+                ("VALIGN", (0, 2), (-1, -1), "TOP"),
+                ("LINEABOVE", (0, 0), (-1, 0), 1, rl_colors.black),
+                ("LINEBELOW", (0, 0), (-1, 0), 1, rl_colors.black),
+                ("LINEBEFORE", (0, 0), (0, 0), 1, rl_colors.black),
+                ("LINEAFTER", (-1, 0), (-1, 0), 1, rl_colors.black),
                 ("SPAN", (1, 0), (2, 0)),
-                ("ALIGN", (1, 2), (2, -1), "RIGHT"),
-                ("SPAN", (3, 0), (3, 1)),
-                ("SPAN", (4, 0), (4, 1)),
             ],
         )
         story.append(tab)
         story.append(RLSpacer(1, 0.25 * rl_inch))
         # end Summary section
 
         # begin Detail section
@@ -1728,17 +1752,17 @@
                 preperation_lines_without_incompatible_ingr, "without restrictions"
             )
         )
         story.append(RLSpacer(1, 1 * rl_inch))
 
         # build full document
         doc.build(story, onFirstPage=myFirstPage, onLaterPages=myLaterPages)
-        return doc.page
+        return file_path
 
-    return go()  # returns number of pages generated
+    return go()  # returns the file path
 
 
 # END Kitchen count report view, helper classes and functions
 
 
 # Meal labels generation data structures and functions.
 
@@ -1780,14 +1804,17 @@
         width : Single label width in font points.
         height : Single label height in font points.
         data : A MealLabel namedtuple.
     """
     # dimensions are in font points (72 points = 1 inch)
     # Line 1
     vertic_pos = height * 0.85
+    # Leave a margin on top of the label to make it easier to read in actual usage,
+    # as the top of the label can be hidden by the rim of the container.
+    vertic_pos -= 25
     horiz_margin = 9  # distance from edge of label 9/72 = 1/8 inch
     if data.name:
         label.add(
             rl_shapes.String(
                 horiz_margin,
                 vertic_pos,
                 data.name,
@@ -2027,49 +2054,14 @@
                 break_on_hyphens=False,
             )
             # remove prefix from first line
             sides_clashes_list[0] = sides_clashes_list[0][len(prefix) :]
             meal_label = meal_label._replace(
                 sides_clashes=[prefix] + sides_clashes_list
             )
-        other_restrictions = []
-        if kititm.sides_clashes:
-            other_restrictions.extend(
-                sorted(list(set(kititm.avoid_ingredients) - set(kititm.sides_clashes)))
-            )
-            other_restrictions.extend(
-                sorted(list(set(kititm.restricted_items) - set(kititm.sides_clashes)))
-            )
-        else:
-            other_restrictions.extend(
-                sorted(
-                    list(
-                        set(kititm.avoid_ingredients)
-                        - set(kititm.incompatible_ingredients)
-                    )
-                )
-            )
-            other_restrictions.extend(
-                sorted(
-                    list(
-                        set(kititm.restricted_items)
-                        - set(kititm.incompatible_ingredients)
-                    )
-                )
-            )
-        if other_restrictions:
-            meal_label = meal_label._replace(
-                other_restrictions=textwrap.wrap(
-                    ugettext("Other restrictions")
-                    + " : {}".format(" , ".join(other_restrictions)),
-                    width=65,
-                    break_long_words=False,
-                    break_on_hyphens=False,
-                )
-            )
         for _j in range(1, kititm.meal_qty + 1):
             meal_labels.append(meal_label)
 
     # find max lengths of fields to sort on
     routew = 0
     namew = 0
     for label in meal_labels:
@@ -2092,44 +2084,28 @@
                 grp=group, rou=route, rouw=routew, nam=meal_labels[j].name, namw=namew
             )
         )
     # generate labels into PDF
     for label in sorted(meal_labels, key=lambda x: x.sortkey):
         sheet.add_label(label)
 
+    file_path = None
     if sheet.label_count > 0:
-        sheet.save(get_meals_label_filename(kcr_date))
-    return sheet.label_count
+        file_path = get_meals_label_file_path(kcr_date)
+        file_path.parent.mkdir(parents=True, exist_ok=True)
+        sheet.save(str(file_path))
+    return file_path
 
 
 # END Meal labels
 
 
 # Delivery route sheet view, helper classes and functions.
 
 
-class MealLabels(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
-    permission_required = "sous_chef.read"
-
-    def get(self, request, **kwargs):
-        delivery_date = date.fromisoformat(request.GET["delivery_date"])
-        filename = get_meals_label_filename(delivery_date)
-        try:
-            f = open(filename, "rb")  # noqa: SIM115
-        except Exception as e:
-            raise Http404(f"File {filename} does not exist.") from e
-        response = HttpResponse(content_type="application/pdf")
-        response["Content-Disposition"] = 'attachment; filename="labels{}.pdf"'.format(
-            delivery_date.strftime("%Y%m%d")
-        )
-        response.write(f.read())
-        f.close()
-        return response
-
-
 class DeliveryRouteSheet(LoginRequiredMixin, PermissionRequiredMixin, generic.View):
     permission_required = "sous_chef.read"
 
     def get(self, request, **kwargs):
         delivery_date = date.fromisoformat(request.GET["delivery_date"])
         delivery_history = get_object_or_404(
             DeliveryHistory, route__pk=kwargs["pk"], date=delivery_date
```

### Comparing `souschef-1.4.1/souschef/frontend/images/bg1.jpg` & `souschef-1.4.2/souschef/frontend/images/bg1.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/frontend/images/jenny.jpg` & `souschef-1.4.2/souschef/frontend/images/jenny.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/frontend/images/joe.jpg` & `souschef-1.4.2/souschef/frontend/images/joe.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/frontend/images/katrina.jpg` & `souschef-1.4.2/souschef/frontend/images/katrina.jpg`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/admin.py` & `souschef-1.4.2/souschef/meal/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/factories.py` & `souschef-1.4.2/souschef/meal/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0001_fix161f.py` & `souschef-1.4.2/souschef/meal/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0002_ingredient_ingredient_group.py` & `souschef-1.4.2/souschef/meal/migrations/0002_ingredient_ingredient_group.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0003_fix224a.py` & `souschef-1.4.2/souschef/meal/migrations/0003_fix224a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0005_fix241b.py` & `souschef-1.4.2/souschef/meal/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0006_auto_20160826_0007.py` & `souschef-1.4.2/souschef/meal/migrations/0006_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0007_auto_20170313_1442.py` & `souschef-1.4.2/souschef/meal/migrations/0007_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/migrations/0008_auto_20180704_1613.py` & `souschef-1.4.2/souschef/meal/migrations/0008_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/meal/models.py` & `souschef-1.4.2/souschef/meal/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,17 @@
         verbose_name=_("date"),
         blank=True,
         null=True,
     )
 
     def __str__(self):
         if self.date:
-            return "<{}> includes <{}> on <{}>".format(
-                self.component.name, self.ingredient.name, self.date
+            return (
+                f"<{self.component.name}> includes <{self.ingredient.name}> on "
+                f"<{self.date}>"
             )
         else:
             return f"<{self.component.name}> contains <{self.ingredient.name}>"
 
 
 class Restricted_item(models.Model):
     class Meta:
```

### Comparing `souschef-1.4.1/souschef/meal/tests.py` & `souschef-1.4.2/souschef/meal/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/admin.py` & `souschef-1.4.2/souschef/member/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/factories.py` & `souschef-1.4.2/souschef/member/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/forms.py` & `souschef-1.4.2/souschef/member/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/formsfield.py` & `souschef-1.4.2/souschef/member/formsfield.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/management/commands/createclients.py` & `souschef-1.4.2/souschef/member/management/commands/createclients.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/management/commands/processscheduledstatuschange.py` & `souschef-1.4.2/souschef/member/management/commands/processscheduledstatuschange.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,24 @@
         changes = ClientScheduledStatus.objects.filter(
             operation_status=ClientScheduledStatus.TOBEPROCESSED
         ).filter(change_date__lte=date.today())
 
         # For each change to be processed,
         for scheduled_change in changes:
             if scheduled_change.process():
-                suc_msg = ": client «{}» status updated from {} to {}.".format(
-                    scheduled_change.client.member,
-                    scheduled_change.get_status_from_display(),
-                    scheduled_change.get_status_to_display(),
+                suc_msg = (
+                    f": client «{scheduled_change.client.member}» status updated "
+                    f"from {scheduled_change.get_status_from_display()} to "
+                    f"{scheduled_change.get_status_to_display()}."
                 )
                 self.stdout.write(self.style.SUCCESS(str(datetime.now()) + suc_msg))
             # If not, mark change as processed with error
             else:
-                err_msg = ": client «{}» status not updated.".format(
-                    scheduled_change.client.member
+                err_msg = (
+                    f": client «{scheduled_change.client.member}» status not updated."
                 )
-                err_msg += " Current status is «{}», should be «{}».".format(
-                    scheduled_change.client.get_status_display(),
-                    scheduled_change.get_status_from_display(),
+                err_msg += (
+                    " Current status is "
+                    f"«{scheduled_change.client.get_status_display()}», should be "
+                    f"«{scheduled_change.get_status_from_display()}»."
                 )
                 self.stdout.write(self.style.ERROR(str(datetime.now()) + err_msg))
```

### Comparing `souschef-1.4.1/souschef/member/migrations/0001_fix161f.py` & `souschef-1.4.2/souschef/member/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0002_auto_20160605_1609.py` & `souschef-1.4.2/souschef/member/migrations/0002_auto_20160605_1609.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0003_auto_20160615_2100.py` & `souschef-1.4.2/souschef/member/migrations/0003_auto_20160615_2100.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0004_fix004a.py` & `souschef-1.4.2/souschef/member/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0005_fix004a.py` & `souschef-1.4.2/souschef/member/migrations/0005_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0007_auto_20160726_1703.py` & `souschef-1.4.2/souschef/member/migrations/0007_auto_20160726_1703.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0009_auto_20160728_1443.py` & `souschef-1.4.2/souschef/member/migrations/0009_auto_20160728_1443.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0012_clientscheduledstatus.py` & `souschef-1.4.2/souschef/member/migrations/0012_clientscheduledstatus.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0013_auto_20160820_2322.py` & `souschef-1.4.2/souschef/member/migrations/0013_auto_20160820_2322.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0014_auto_20160826_0007.py` & `souschef-1.4.2/souschef/member/migrations/0014_auto_20160826_0007.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0016_auto_20160912_1509.py` & `souschef-1.4.2/souschef/member/migrations/0016_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0017_auto_20161020_2039.py` & `souschef-1.4.2/souschef/member/migrations/0017_auto_20161020_2039.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0018_auto_20161110_2352.py` & `souschef-1.4.2/souschef/member/migrations/0018_auto_20161110_2352.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0019_auto_20161111_1750.py` & `souschef-1.4.2/souschef/member/migrations/0019_auto_20161111_1750.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0022_auto_20161215_1936.py` & `souschef-1.4.2/souschef/member/migrations/0022_auto_20161215_1936.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0023_auto_20161220_1401.py` & `souschef-1.4.2/souschef/member/migrations/0023_auto_20161220_1401.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0024_auto_20161227_1819.py` & `souschef-1.4.2/souschef/member/migrations/0024_auto_20161227_1819.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0025_route_vehicle.py` & `souschef-1.4.2/souschef/member/migrations/0025_route_vehicle.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0026_change_to_emergency_contacts.py` & `souschef-1.4.2/souschef/member/migrations/0026_change_to_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0027_auto_20170313_1442.py` & `souschef-1.4.2/souschef/member/migrations/0027_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py` & `souschef-1.4.2/souschef/member/migrations/0028_change_linked_scheduled_status_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0029_member_address_fk_to_1to1.py` & `souschef-1.4.2/souschef/member/migrations/0029_member_address_fk_to_1to1.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,17 @@
         if a is None:
             continue
         if a.pk not in address_ids:
             address_ids.add(a.pk)
             continue
         else:  # a.pk in address_ids
             print(
-                "Member #{} ({} {}) shares the Address #{}. I'm copying this "
-                "Address instance and relinking the member to it...".format(
-                    m.pk, m.firstname, m.lastname, a.pk
-                )
+                f"Member #{m.pk} ({m.firstname} {m.lastname}) shares the Address "
+                f"#{a.pk}. I'm copying this Address instance and relinking the member "
+                "to it..."
             )
             # Copy this object in DB
             a.pk = None
             a.save()
             assert a.pk not in address_ids
             address_ids.add(a.pk)
             m.address = a
```

### Comparing `souschef-1.4.1/souschef/member/migrations/0030_route_deliveryhistory.py` & `souschef-1.4.2/souschef/member/migrations/0030_route_deliveryhistory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0031_client_option_allow_reverse_relation.py` & `souschef-1.4.2/souschef/member/migrations/0031_client_option_allow_reverse_relation.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0032_relationship.py` & `souschef-1.4.2/souschef/member/migrations/0032_relationship.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0033_auto_20170801_1607.py` & `souschef-1.4.2/souschef/member/migrations/0033_auto_20170801_1607.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0034_auto_20170816_0850.py` & `souschef-1.4.2/souschef/member/migrations/0034_auto_20170816_0850.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0035_auto_20210115_1155.py` & `souschef-1.4.2/souschef/member/migrations/0035_auto_20210115_1155.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0036_member_addresses.py` & `souschef-1.4.2/souschef/member/migrations/0036_member_addresses.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0037_one_address_per_member.py` & `souschef-1.4.2/souschef/member/migrations/0037_one_address_per_member.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/migrations/0038_member_verbose_names.py` & `souschef-1.4.2/souschef/member/migrations/0038_member_verbose_names.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/models.py` & `souschef-1.4.2/souschef/member/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -386,35 +386,25 @@
             client.age_to_celebrate = today.year - client.birthdate.year
 
         return clients
 
 
 class ActiveClientManager(ClientManager):
     def get_queryset(self):
-        return (
-            super().get_queryset().filter(status=Client.ACTIVE)
-        )
+        return super().get_queryset().filter(status=Client.ACTIVE)
 
 
 class OngoingClientManager(ClientManager):
     def get_queryset(self):
-        return (
-            super()
-            .get_queryset()
-            .filter(status=Client.ACTIVE, delivery_type="O")
-        )
+        return super().get_queryset().filter(status=Client.ACTIVE, delivery_type="O")
 
 
 class PendingClientManager(ClientManager):
     def get_queryset(self):
-        return (
-            super()
-            .get_queryset()
-            .filter(status=Client.PENDING)
-        )
+        return super().get_queryset().filter(status=Client.PENDING)
 
 
 class ContactClientManager(ClientManager):
     def get_queryset(self):
         return (
             super()
             .get_queryset()
@@ -778,19 +768,18 @@
         max_length=3, choices=OPERATION_STATUS, default=TOBEPROCESSED
     )
 
     class Meta:
         ordering = ["change_date"]
 
     def __str__(self):
-        return "Update {} status: from {} to {}, on {}".format(
-            self.client.member,
-            self.get_status_from_display(),
-            self.get_status_to_display(),
-            self.change_date,
+        return (
+            f"Update {self.client.member} status: from "
+            f"{self.get_status_from_display()} to {self.get_status_to_display()}, "
+            f"on {self.change_date}"
         )
 
     @property
     def get_pair(self):
         """
         Returns the pair relationship. If the pair relationship does
         not exists, None value will be returned.
@@ -891,20 +880,18 @@
     nature = models.CharField(max_length=100)
     # Relationship.type is linked with a forms.MultipleChoiceField
     type = JSONField(default=[], blank=True)
     extra_fields = JSONField(default={}, blank=True)
     remark = models.TextField(blank=True)
 
     def __str__(self):
-        return "{} {} is {} member of {} {}".format(
-            self.member.firstname,
-            self.member.lastname,
-            self.get_type_display(),
-            self.client.member.firstname,
-            self.client.member.lastname,
+        return (
+            f"{self.member.firstname} {self.member.lastname} is "
+            f"{self.get_type_display()} member of {self.client.member.firstname} "
+            f"{self.client.member.lastname}"
         )
 
     def get_type_display(self):
         return "+".join(
             map(
                 force_text,
                 list(map(lambda t: self.TYPE_CHOICES_DICT[t], self.type))
@@ -957,16 +944,17 @@
     #  value contents depends on option_group of option occurence pointed to:
     #    if option_group = main_dish_size : 'Regular' or 'Large'
     #    if option_group = dish : qty Monday to Sunday ex. '1110120'
     #    if option_group = preparation : Null
     #    if option_group = other_order_item : No occurrence of Client_option
 
     def __str__(self):
-        return "{} {} <has> {}".format(
-            self.client.member.firstname, self.client.member.lastname, self.option.name
+        return (
+            f"{self.client.member.firstname} {self.client.member.lastname} <has> "
+            f"{self.option.name}"
         )
 
 
 class Restriction(models.Model):
     client = models.ForeignKey(
         "member.Client",
         verbose_name=_("client"),
@@ -978,18 +966,17 @@
         "meal.Restricted_item",
         verbose_name=_("restricted item"),
         related_name="+",
         on_delete=models.CASCADE,
     )
 
     def __str__(self):
-        return "{} {} <restricts> {}".format(
-            self.client.member.firstname,
-            self.client.member.lastname,
-            self.restricted_item.name,
+        return (
+            f"{self.client.member.firstname} {self.client.member.lastname} "
+            f"<restricts> {self.restricted_item.name}"
         )
 
 
 class Client_avoid_ingredient(models.Model):
     client = models.ForeignKey(
         "member.Client",
         verbose_name=_("client"),
@@ -1001,18 +988,17 @@
         "meal.Ingredient",
         verbose_name=_("ingredient"),
         related_name="+",
         on_delete=models.CASCADE,
     )
 
     def __str__(self):
-        return "{} {} <has> {}".format(
-            self.client.member.firstname,
-            self.client.member.lastname,
-            self.ingredient.name,
+        return (
+            f"{self.client.member.firstname} {self.client.member.lastname} "
+            f"<has> {self.ingredient.name}"
         )
 
 
 class Client_avoid_component(models.Model):
     client = models.ForeignKey(
         "member.Client",
         verbose_name=_("client"),
@@ -1024,12 +1010,11 @@
         "meal.Component",
         verbose_name=_("component"),
         related_name="+",
         on_delete=models.CASCADE,
     )
 
     def __str__(self):
-        return "{} {} <has> {}".format(
-            self.client.member.firstname,
-            self.client.member.lastname,
-            self.component.name,
+        return (
+            f"{self.client.member.firstname} {self.client.member.lastname} "
+            f"<has> {self.component.name}"
         )
```

### Comparing `souschef-1.4.1/souschef/member/templates/client/base.html` & `souschef-1.4.2/souschef/member/templates/client/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/create/form.html` & `souschef-1.4.2/souschef/member/templates/client/create/form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/create/steps.html` & `souschef-1.4.2/souschef/member/templates/client/create/steps.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/list.html` & `souschef-1.4.2/souschef/member/templates/client/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/birthdays.html` & `souschef-1.4.2/souschef/member/templates/client/partials/birthdays.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/filters.html` & `souschef-1.4.2/souschef/member/templates/client/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/address_information.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/address_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/basic_information.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/basic_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/dietary_restriction.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/dietary_restriction.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/meal_defaults.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/meal_defaults.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/payment_information.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/payment_information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/relationship_form.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/relationship_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/forms/relationships.html` & `souschef-1.4.2/souschef/member/templates/client/partials/forms/relationships.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/menu.html` & `souschef-1.4.2/souschef/member/templates/client/partials/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/partials/order_list.html` & `souschef-1.4.2/souschef/member/templates/client/partials/order_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/update/base.html` & `souschef-1.4.2/souschef/member/templates/client/update/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/update/status.html` & `souschef-1.4.2/souschef/member/templates/client/update/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/allergies.html` & `souschef-1.4.2/souschef/member/templates/client/view/allergies.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/delete_status_confirmation.html` & `souschef-1.4.2/souschef/member/templates/client/view/delete_status_confirmation.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/information.html` & `souschef-1.4.2/souschef/member/templates/client/view/information.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/notes.html` & `souschef-1.4.2/souschef/member/templates/client/view/notes.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/orders.html` & `souschef-1.4.2/souschef/member/templates/client/view/orders.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/payment.html` & `souschef-1.4.2/souschef/member/templates/client/view/payment.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/referent.html` & `souschef-1.4.2/souschef/member/templates/client/view/referent.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/status.html` & `souschef-1.4.2/souschef/member/templates/client/view/status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/client/view/summary.html` & `souschef-1.4.2/souschef/member/templates/client/view/summary.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/route/delivery_history_detail.html` & `souschef-1.4.2/souschef/member/templates/route/delivery_history_detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/route/detail.html` & `souschef-1.4.2/souschef/member/templates/route/detail.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/route/edit.html` & `souschef-1.4.2/souschef/member/templates/route/edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/templates/route/list.html` & `souschef-1.4.2/souschef/member/templates/route/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/tests.py` & `souschef-1.4.2/souschef/member/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         "facturation": "",
         "billing_payment_type": "",
     }
     return initial
 
 
 class MemberContact(TestCase):
-
     """
     Contact information data should be attached to members.
     Three types of data: EMAIL, CELL and HOME.
     """
 
     @classmethod
     def setUpTestData(cls):
@@ -739,17 +738,15 @@
             ],
             "dietary_restriction-food_preparation": self.food_preparation.id,
             "dietary_restriction-ingredient_to_avoid": self.ingredient.id,
             "dietary_restriction-dish_to_avoid": self.component.id,
             "wizard_goto_step": "",
         }
         for day in restriction_information_data["dietary_restriction-meals_schedule"]:
-            restriction_information_data[
-                f"dietary_restriction-size_{day}"
-            ] = "R"
+            restriction_information_data[f"dietary_restriction-size_{day}"] = "R"
             for component, _ in COMPONENT_GROUP_CHOICES:
                 name = f"dietary_restriction-{component}_{day}_quantity"
                 restriction_information_data[name] = 1
 
         relationships_data = {
             "client_wizard-current_step": "relationships",
             "relationships-TOTAL_FORMS": "1",
@@ -1401,17 +1398,15 @@
             "dietary_restriction-status": "on",
             "dietary_restriction-delivery_type": "O",
             "dietary_restriction-meals_schedule": "monday",
             "dietary_restriction-meal_default": "1",
             "wizard_goto_step": "",
         }
         for day in [restriction_information_data["dietary_restriction-meals_schedule"]]:
-            restriction_information_data[
-                f"dietary_restriction-size_{day}"
-            ] = "R"
+            restriction_information_data[f"dietary_restriction-size_{day}"] = "R"
             for component, _ in COMPONENT_GROUP_CHOICES:
                 name = f"dietary_restriction-{component}_{day}_quantity"
                 restriction_information_data[name] = 1
 
         # Send the data to the form.
         response = self.client.post(
             reverse_lazy(
@@ -1578,19 +1573,17 @@
             status_from=Client.ACTIVE,
             status_to=Client.PAUSED,
         )
         out = StringIO()
         call_command("processscheduledstatuschange", stdout=out)
         with translation.override("en"):
             self.assertIn(
-                "client «{}» status updated from {} to {}".format(
-                    self.active_client.member,
-                    scheduled_change.get_status_from_display(),
-                    scheduled_change.get_status_to_display(),
-                ),
+                f"client «{self.active_client.member}» status updated from "
+                f"{scheduled_change.get_status_from_display()} to "
+                f"{scheduled_change.get_status_to_display()}",
                 out.getvalue(),
             )
         # Reload
         scheduled_change = ClientScheduledStatus.objects.get(id=scheduled_change.id)
         self.assertEqual(
             scheduled_change.operation_status, ClientScheduledStatus.PROCESSED
         )
@@ -2207,16 +2200,17 @@
             {
                 "firstname": None,
                 "lastname": None,
                 "street": None,
                 "city": None,
                 "apartment": None,
                 "postal_code": None,
-                "member": "[{}] {} {}".format(
-                    client.member.id, client.member.firstname, client.member.lastname
+                "member": (
+                    f"[{client.member.id}] {client.member.firstname} "
+                    f"{client.member.lastname}"
                 ),
                 "same_as_client": True,
                 "billing_payment_type": "eft",
                 "facturation": "default",
             }
         )
         form = ClientPaymentInformation(data=data)
@@ -2514,16 +2508,16 @@
             {
                 "relationships-TOTAL_FORMS": "1",
                 "relationships-INITIAL_FORMS": "1",
                 "relationships-MIN_NUM_FORMS": "0",
                 "relationships-MAX_NUM_FORMS": "1000",
                 "relationships-0-firstname": None,
                 "relationships-0-lastname": None,
-                "relationships-0-member": "[{}] {} {}".format(
-                    member.id, member.firstname, member.lastname
+                "relationships-0-member": (
+                    f"[{member.id}] {member.firstname} {member.lastname}"
                 ),
                 "relationships-0-type": [],
                 "relationships-0-nature": "friend",
             }
         )
 
         # Login as admin
```

### Comparing `souschef-1.4.1/souschef/member/urls.py` & `souschef-1.4.2/souschef/member/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/member/views.py` & `souschef-1.4.2/souschef/member/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,18 +805,17 @@
             {
                 "firstname": None,
                 "lastname": None,
                 "street": None,
                 "city": None,
                 "apartment": None,
                 "postal_code": None,
-                "member": "[{}] {} {}".format(
-                    client.billing_member.id,
-                    client.billing_member.firstname,
-                    client.billing_member.lastname,
+                "member": (
+                    f"[{client.billing_member.id}] {client.billing_member.firstname} "
+                    f"{client.billing_member.lastname}"
                 ),
                 "same_as_client": client.member == client.billing_member,
                 "facturation": client.rate_type,
                 "billing_payment_type": client.billing_payment_type,
             }
         )
 
@@ -969,18 +968,17 @@
                 else:
                     contact_type = None
                     contact_value = None
 
                 initial[i] = {
                     "firstname": None,
                     "lastname": None,
-                    "member": "[{}] {} {}".format(
-                        relationship.member.id,
-                        relationship.member.firstname,
-                        relationship.member.lastname,
+                    "member": (
+                        f"[{relationship.member.id}] {relationship.member.firstname} "
+                        f"{relationship.member.lastname}"
                     ),
                     "contact_type": contact_type,
                     "contact_value": contact_value,
                     "nature": relationship.nature,
                     "type": relationship.type,
                     "remark": relationship.remark,
                 }
```

### Comparing `souschef-1.4.1/souschef/note/admin.py` & `souschef-1.4.2/souschef/note/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/factories.py` & `souschef-1.4.2/souschef/note/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/forms.py` & `souschef-1.4.2/souschef/note/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0001_initial.py` & `souschef-1.4.2/souschef/note/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0002_auto_20160818_2104.py` & `souschef-1.4.2/souschef/note/migrations/0002_auto_20160818_2104.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0004_notepriority.py` & `souschef-1.4.2/souschef/note/migrations/0004_notepriority.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0005_note_priority_old_data_migration.py` & `souschef-1.4.2/souschef/note/migrations/0005_note_priority_old_data_migration.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0007_notecategory.py` & `souschef-1.4.2/souschef/note/migrations/0007_notecategory.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0008_auto_20170116_1441.py` & `souschef-1.4.2/souschef/note/migrations/0008_auto_20170116_1441.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0009_auto_20170116_1543.py` & `souschef-1.4.2/souschef/note/migrations/0009_auto_20170116_1543.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0010_auto_20170313_1442.py` & `souschef-1.4.2/souschef/note/migrations/0010_auto_20170313_1442.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0011_auto_20170419_1109.py` & `souschef-1.4.2/souschef/note/migrations/0011_auto_20170419_1109.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/migrations/0013_date_modified.py` & `souschef-1.4.2/souschef/note/migrations/0013_date_modified.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/models.py` & `souschef-1.4.2/souschef/note/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/templates/note_confirm_delete.html` & `souschef-1.4.2/souschef/note/templates/note_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/templates/note_edit.html` & `souschef-1.4.2/souschef/note/templates/note_edit.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/templates/notes_add.html` & `souschef-1.4.2/souschef/note/templates/notes_add.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/templates/notes_client_list.html` & `souschef-1.4.2/souschef/note/templates/notes_client_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/templates/notes_list.html` & `souschef-1.4.2/souschef/note/templates/notes_list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/tests.py` & `souschef-1.4.2/souschef/note/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/urls.py` & `souschef-1.4.2/souschef/note/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/note/views.py` & `souschef-1.4.2/souschef/note/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/notification/migrations/0001_fix161f.py` & `souschef-1.4.2/souschef/notification/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/notification/models.py` & `souschef-1.4.2/souschef/notification/models.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/admin.py` & `souschef-1.4.2/souschef/order/admin.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/factories.py` & `souschef-1.4.2/souschef/order/factories.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/forms.py` & `souschef-1.4.2/souschef/order/forms.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/management/commands/generateorders.py` & `souschef-1.4.2/souschef/order/management/commands/generateorders.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/management/commands/setordersdelivered.py` & `souschef-1.4.2/souschef/order/management/commands/setordersdelivered.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0001_fix161f.py` & `souschef-1.4.2/souschef/order/migrations/0001_fix161f.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0002_auto_20160614_1736.py` & `souschef-1.4.2/souschef/order/migrations/0002_auto_20160614_1736.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0003_auto_20160615_1504.py` & `souschef-1.4.2/souschef/order/migrations/0003_auto_20160615_1504.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0004_fix004a.py` & `souschef-1.4.2/souschef/order/migrations/0004_fix004a.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0005_fix241b.py` & `souschef-1.4.2/souschef/order/migrations/0005_fix241b.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0006_auto_20160803_2217.py` & `souschef-1.4.2/souschef/order/migrations/0006_auto_20160803_2217.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0008_auto_20160912_1509.py` & `souschef-1.4.2/souschef/order/migrations/0008_auto_20160912_1509.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0009_auto_20161012_1919.py` & `souschef-1.4.2/souschef/order/migrations/0009_auto_20161012_1919.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0011_auto_20161014_1901.py` & `souschef-1.4.2/souschef/order/migrations/0011_auto_20161014_1901.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0013_orderstatuschange.py` & `souschef-1.4.2/souschef/order/migrations/0013_orderstatuschange.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0014_auto_20161209_2045.py` & `souschef-1.4.2/souschef/order/migrations/0014_auto_20161209_2045.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0015_auto_20170410_1029.py` & `souschef-1.4.2/souschef/order/migrations/0015_auto_20170410_1029.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/migrations/0016_auto_20180704_1613.py` & `souschef-1.4.2/souschef/order/migrations/0016_auto_20180704_1613.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/mixins.py` & `souschef-1.4.2/souschef/order/mixins.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/models.py` & `souschef-1.4.2/souschef/order/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,14 +438,21 @@
                 row.oiorderid
                 and row.menucompid
                 and row.component_group == COMPONENT_GROUP_CHOICES_SIDES
                 and row.ingredient not in kitchen_list[row.cid].sides_clashes
             ):
                 # found new avoid ingredient clash in sides
                 kitchen_list[row.cid].sides_clashes.append(row.ingredient)
+
+                # This might be reactivated shortly:
+                # # we also add side clash ingredients into main ingredient clashes
+                # # so they can be grouped and displayed together
+                # kitchen_list[row.cid].incompatible_ingredients.append(
+                #     f"{row.ingredient} (sides)"
+                # )
             if row.ingredient not in kitchen_list[row.cid].avoid_ingredients:
                 # remember ingredient to avoid
                 kitchen_list[row.cid].avoid_ingredients.append(row.ingredient)
 
         # Day's restrictions.
         for row in day_restrictions(delivery_date):
             check_for_new_client(kitchen_list, row)
@@ -485,27 +492,27 @@
                     meal_size=row.size,
                 )
             old_component = kitchen_list[row.cid].meal_components.get(
                 row.component_group
             )
             if old_component:
                 # component group already exists in the order
-                kitchen_list[row.cid].meal_components[
-                    row.component_group
-                ] = old_component._replace(
-                    qty=old_component.qty + (row.total_quantity or 0)
+                kitchen_list[row.cid].meal_components[row.component_group] = (
+                    old_component._replace(
+                        qty=old_component.qty + (row.total_quantity or 0)
+                    )
                 )
             else:
                 # new component group for this order
-                kitchen_list[row.cid].meal_components[
-                    row.component_group
-                ] = MealComponent(
-                    id=row.component_id,
-                    name=row.component_name,
-                    qty=row.total_quantity or 0,
+                kitchen_list[row.cid].meal_components[row.component_group] = (
+                    MealComponent(
+                        id=row.component_id,
+                        name=row.component_name,
+                        qty=row.total_quantity or 0,
+                    )
                 )
             kitchen_list[row.cid] = kitchen_list[row.cid]._replace(
                 routename=row.routename
             )
 
         # Sort requirements list in each value.
         for value in kitchen_list.values():
@@ -1227,19 +1234,18 @@
     status_to = models.CharField(max_length=1, choices=ORDER_STATUS)
 
     reason = models.CharField(max_length=200, blank=True, default="")
 
     change_time = models.DateTimeField(auto_now_add=True)
 
     def __str__(self):
-        return "Order #{} status update: from {} to {}, on {}".format(
-            self.order.pk,
-            self.get_status_from_display(),
-            self.get_status_to_display(),
-            self.change_time,
+        return (
+            f"Order #{self.order.pk} status update: from "
+            f"{self.get_status_from_display()} to {self.get_status_to_display()}, on "
+            f"{self.change_time}"
         )
 
     def clean(self):
         """
         Make sure this is valid in regards to Order.
         """
         if self.order.status != self.status_from:
```

### Comparing `souschef-1.4.1/souschef/order/templates/_form.html` & `souschef-1.4.2/souschef/order/templates/_form.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/_order_info.html` & `souschef-1.4.2/souschef/order/templates/_order_info.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/create.html` & `souschef-1.4.2/souschef/order/templates/create.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/list.html` & `souschef-1.4.2/souschef/order/templates/list.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/order/create_batch.html` & `souschef-1.4.2/souschef/order/templates/order/create_batch.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/order/partials/filters.html` & `souschef-1.4.2/souschef/order/templates/order/partials/filters.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/order_confirm_delete.html` & `souschef-1.4.2/souschef/order/templates/order_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/order_update_status.html` & `souschef-1.4.2/souschef/order/templates/order_update_status.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/update.html` & `souschef-1.4.2/souschef/order/templates/update.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/templates/view.html` & `souschef-1.4.2/souschef/order/templates/view.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/tests.py` & `souschef-1.4.2/souschef/order/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/urls.py` & `souschef-1.4.2/souschef/order/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/order/views.py` & `souschef-1.4.2/souschef/order/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/page/templates/pages/home.html` & `souschef-1.4.2/souschef/page/templates/pages/home.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/page/templates/registration/login.html` & `souschef-1.4.2/souschef/page/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/page/tests.py` & `souschef-1.4.2/souschef/page/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/page/views.py` & `souschef-1.4.2/souschef/page/views.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/context_processors.py` & `souschef-1.4.2/souschef/sous_chef/context_processors.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/management/commands/makemessages.py` & `souschef-1.4.2/souschef/sous_chef/management/commands/makemessages.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/settings.py` & `souschef-1.4.2/souschef/sous_chef/settings.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/404.html` & `souschef-1.4.2/souschef/sous_chef/templates/404.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/avatar/change.html` & `souschef-1.4.2/souschef/sous_chef/templates/avatar/change.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/avatar/confirm_delete.html` & `souschef-1.4.2/souschef/sous_chef/templates/avatar/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/base.html` & `souschef-1.4.2/souschef/sous_chef/templates/base.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/dashboard/statistics.html` & `souschef-1.4.2/souschef/sous_chef/templates/dashboard/statistics.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/splash.html` & `souschef-1.4.2/souschef/sous_chef/templates/splash.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/templates/system/menu.html` & `souschef-1.4.2/souschef/sous_chef/templates/system/menu.html`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/tests.py` & `souschef-1.4.2/souschef/sous_chef/tests.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef/sous_chef/urls.py` & `souschef-1.4.2/souschef/sous_chef/urls.py`

 * *Files identical despite different names*

### Comparing `souschef-1.4.1/souschef.egg-info/PKG-INFO` & `souschef-1.4.2/souschef.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souschef
-Version: 1.4.1
+Version: 1.4.2
 Summary: Webapp used to manage orders for meals-on-wheel delivery
 Home-page: https://github.com/santropolroulant/sous-chef
 Author: Santropol Roulant and Savoir Faire Linux
 Author-email: info@santropolroulant.org
 License: AGPL-3.0
 Keywords: meals-on-wheel
 Platform: UNKNOWN
```

### Comparing `souschef-1.4.1/souschef.egg-info/SOURCES.txt` & `souschef-1.4.2/souschef.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -291,61 +291,14 @@
 souschef/sous_chef/rules.py
 souschef/sous_chef/settings.py
 souschef/sous_chef/settings_test.py
 souschef/sous_chef/settings_test_fr.py
 souschef/sous_chef/tests.py
 souschef/sous_chef/urls.py
 souschef/sous_chef/wsgi.py
-souschef/sous_chef/assets/css/main.min.css
-souschef/sous_chef/assets/fonts/brand-icons.eot
-souschef/sous_chef/assets/fonts/brand-icons.svg
-souschef/sous_chef/assets/fonts/brand-icons.ttf
-souschef/sous_chef/assets/fonts/brand-icons.woff
-souschef/sous_chef/assets/fonts/brand-icons.woff2
-souschef/sous_chef/assets/fonts/icons.eot
-souschef/sous_chef/assets/fonts/icons.otf
-souschef/sous_chef/assets/fonts/icons.svg
-souschef/sous_chef/assets/fonts/icons.ttf
-souschef/sous_chef/assets/fonts/icons.woff
-souschef/sous_chef/assets/fonts/icons.woff2
-souschef/sous_chef/assets/fonts/outline-icons.eot
-souschef/sous_chef/assets/fonts/outline-icons.svg
-souschef/sous_chef/assets/fonts/outline-icons.ttf
-souschef/sous_chef/assets/fonts/outline-icons.woff
-souschef/sous_chef/assets/fonts/outline-icons.woff2
-souschef/sous_chef/assets/images/bg1.jpg
-souschef/sous_chef/assets/images/demo.png
-souschef/sous_chef/assets/images/favicon.png
-souschef/sous_chef/assets/images/flags.png
-souschef/sous_chef/assets/images/geocoder.png
-souschef/sous_chef/assets/images/glyph-marker-icon.png
-souschef/sous_chef/assets/images/glyph-marker-icon.svg
-souschef/sous_chef/assets/images/jenny.jpg
-souschef/sous_chef/assets/images/joe.jpg
-souschef/sous_chef/assets/images/katrina.jpg
-souschef/sous_chef/assets/images/leaflet.routing.icons.png
-souschef/sous_chef/assets/images/leaflet.routing.icons.svg
-souschef/sous_chef/assets/images/logo-souschef-coul.png
-souschef/sous_chef/assets/images/logo-souschef-nb.png
-souschef/sous_chef/assets/images/logo.png
-souschef/sous_chef/assets/images/markers-matte.png
-souschef/sous_chef/assets/images/markers-matte@2x.png
-souschef/sous_chef/assets/images/markers-plain.png
-souschef/sous_chef/assets/images/markers-shadow.png
-souschef/sous_chef/assets/images/markers-shadow@2x.png
-souschef/sous_chef/assets/images/markers-soft.png
-souschef/sous_chef/assets/images/markers-soft@2x.png
-souschef/sous_chef/assets/images/routing-icon.png
-souschef/sous_chef/assets/images/throbber.gif
-souschef/sous_chef/assets/js/leaflet.js
-souschef/sous_chef/assets/js/leaflet.min.js
-souschef/sous_chef/assets/js/multidatespicker.js
-souschef/sous_chef/assets/js/multidatespicker.min.js
-souschef/sous_chef/assets/js/sous-chef.js
-souschef/sous_chef/assets/js/sous-chef.min.js
 souschef/sous_chef/formats/__init__.py
 souschef/sous_chef/formats/en/__init__.py
 souschef/sous_chef/formats/en/formats.py
 souschef/sous_chef/formats/fr/__init__.py
 souschef/sous_chef/formats/fr/formats.py
 souschef/sous_chef/management/__init__.py
 souschef/sous_chef/management/commands/__init__.py
```

