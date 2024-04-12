# Comparing `tmp/nautobot_floor_plan-2.0.0rc1.tar.gz` & `tmp/nautobot_floor_plan-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_floor_plan-2.0.0rc1.tar", max compression
+gzip compressed data, was "nautobot_floor_plan-2.1.0.tar", max compression
```

## Comparing `nautobot_floor_plan-2.0.0rc1.tar` & `nautobot_floor_plan-2.1.0.tar`

### file list

```diff
@@ -1,38 +1,124 @@
--rw-r--r--   0        0        0      591 2023-09-11 12:20:53.273331 nautobot_floor_plan-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0     3995 2023-09-11 12:20:53.273331 nautobot_floor_plan-2.0.0rc1/README.md
--rw-r--r--   0        0        0      832 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/__init__.py
--rw-r--r--   0        0        0       54 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/__init__.py
--rw-r--r--   0        0        0      676 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/serializers.py
--rw-r--r--   0        0        0      449 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/urls.py
--rw-r--r--   0        0        0     1353 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/views.py
--rw-r--r--   0        0        0      415 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/choices.py
--rw-r--r--   0        0        0      622 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/filter_extensions.py
--rw-r--r--   0        0        0     1603 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/filters.py
--rw-r--r--   0        0        0     2656 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/forms.py
--rwxr-xr-x   0        0        0     5729 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0001_initial.py
--rw-r--r--   0        0        0      736 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0002_fixup_null.py
--rw-r--r--   0        0        0     1473 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0003_auto_20230908_1339.py
--rw-r--r--   0        0        0        0 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/__init__.py
--rw-r--r--   0        0        0     6714 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/models.py
--rw-r--r--   0        0        0     1190 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/navigation.py
--rw-r--r--   0        0        0      973 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/static/nautobot_floor_plan/css/svg.css
--rw-r--r--   0        0        0    16114 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/svg.py
--rw-r--r--   0        0        0     1217 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tables.py
--rw-r--r--   0        0        0     2545 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/template_content.py
--rw-r--r--   0        0        0     1385 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/floorplan_retrieve.html
--rw-r--r--   0        0        0     1935 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/floorplantile_retrieve.html
--rw-r--r--   0        0        0     5797 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/inc/floorplan_svg.html
--rw-r--r--   0        0        0      195 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/location_floor_plan.html
--rw-r--r--   0        0        0       49 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/__init__.py
--rw-r--r--   0        0        0     1838 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/fixtures.py
--rw-r--r--   0        0        0      985 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_api.py
--rw-r--r--   0        0        0     3390 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_api_views.py
--rw-r--r--   0        0        0     1524 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_basic.py
--rw-r--r--   0        0        0     5316 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_filters.py
--rw-r--r--   0        0        0     2429 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_forms.py
--rw-r--r--   0        0        0    10436 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_models.py
--rw-r--r--   0        0        0      920 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_views.py
--rw-r--r--   0        0        0     1095 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/urls.py
--rw-r--r--   0        0        0     1405 2023-09-11 12:20:53.277331 nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/views.py
--rw-r--r--   0        0        0     3467 2023-09-11 12:21:03.765989 nautobot_floor_plan-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 nautobot_floor_plan-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-12 20:05:27.915862 nautobot_floor_plan-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3972 2024-04-12 20:05:27.915862 nautobot_floor_plan-2.1.0/README.md
+-rw-r--r--   0        0        0     1986 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/__init__.py
+-rw-r--r--   0        0        0       51 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/__init__.py
+-rw-r--r--   0        0        0      666 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/serializers.py
+-rw-r--r--   0        0        0      446 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/urls.py
+-rw-r--r--   0        0        0     1383 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/views.py
+-rw-r--r--   0        0        0      581 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/app-config-schema.json
+-rw-r--r--   0        0        0      629 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/choices.py
+-rw-r--r--   0        0        0      623 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/filter_extensions.py
+-rw-r--r--   0        0        0     1601 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/filters.py
+-rw-r--r--   0        0        0     5808 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/forms.py
+-rwxr-xr-x   0        0        0     5729 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0001_initial.py
+-rw-r--r--   0        0        0      736 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0002_fixup_null.py
+-rw-r--r--   0        0        0     1473 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0003_auto_20230908_1339.py
+-rw-r--r--   0        0        0      605 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0004_auto_20240321_1438.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:05:27.919862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/__init__.py
+-rw-r--r--   0        0        0     7135 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/models.py
+-rw-r--r--   0        0        0     1188 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/navigation.py
+-rw-r--r--   0        0        0      973 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/css/svg.css
+-rw-r--r--   0        0        0    31533 2024-04-12 20:05:51.239828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/404.html
+-rw-r--r--   0        0        0    34287 2024-04-12 20:05:51.259828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    41083 2024-04-12 20:05:51.263828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/install.html
+-rw-r--r--   0        0        0    33836 2024-04-12 20:05:51.271828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    36243 2024-04-12 20:05:51.275828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    36479 2024-04-12 20:05:51.275828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    34269 2024-04-12 20:05:51.279828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/release_notes/version_2.1.html
+-rw-r--r--   0        0        0    36943 2024-04-12 20:05:51.267828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    35216 2024-04-12 20:05:51.271828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    17074 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-04-12 20:05:51.123828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0     9204 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   113505 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/stylesheets/main.26e3688c.min.css
+-rw-r--r--   0        0        0    38975 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/stylesheets/main.26e3688c.min.css.map
+-rw-r--r--   0        0        0    12245 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/stylesheets/palette.ecc896b0.min.css
+-rw-r--r--   0        0        0     3639 2024-04-12 20:05:51.127828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/assets/stylesheets/palette.ecc896b0.min.css.map
+-rw-r--r--   0        0        0    63071 2024-04-12 20:05:51.323828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    33701 2024-04-12 20:05:51.307828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0   109772 2024-04-12 20:05:51.367828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/code_reference/models.html
+-rw-r--r--   0        0        0    52009 2024-04-12 20:05:51.379828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0   178622 2024-04-12 20:05:51.467827 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/code_reference/svg.html
+-rw-r--r--   0        0        0    41398 2024-04-12 20:05:51.283828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/contributing.html
+-rw-r--r--   0        0        0   100205 2024-04-12 20:05:51.303828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    34169 2024-04-12 20:05:51.307828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/dev/extending.html
+-rw-r--r--   0        0        0    24289 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/add-floor-plan-button.png
+-rw-r--r--   0        0        0    42613 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/add-floor-plan-form.png
+-rw-r--r--   0        0        0    53213 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/add-tile-form.png
+-rw-r--r--   0        0        0    94630 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/floor-plan-empty.png
+-rw-r--r--   0        0        0   126846 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/floor-plan-populated.png
+-rw-r--r--   0        0        0     2117 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/icon-nautobot-floor-plan.png
+-rw-r--r--   0        0        0    32877 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/images/status-definition.png
+-rw-r--r--   0        0        0    40290 2024-04-12 20:05:51.259828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/index.html
+-rw-r--r--   0        0        0      489 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/objects.inv
+-rw-r--r--   0        0        0      120 2024-04-12 20:05:51.119828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/requirements.txt
+-rw-r--r--   0        0        0    84167 2024-04-12 20:05:51.479828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/search/search_index.json
+-rw-r--r--   0        0        0     4355 2024-04-12 20:05:51.131828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/sitemap.xml
+-rw-r--r--   0        0        0      415 2024-04-12 20:05:51.131828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    38855 2024-04-12 20:05:51.471827 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    40047 2024-04-12 20:05:51.475827 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/user/app_overview.html
+-rw-r--r--   0        0        0    35636 2024-04-12 20:05:51.475827 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    33818 2024-04-12 20:05:51.479828 nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/docs/user/faq.html
+-rw-r--r--   0        0        0    16674 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/svg.py
+-rw-r--r--   0        0        0     2560 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tables.py
+-rw-r--r--   0        0        0     2543 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/template_content.py
+-rw-r--r--   0        0        0     1853 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/floorplan_retrieve.html
+-rw-r--r--   0        0        0     1935 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/floorplantile_retrieve.html
+-rw-r--r--   0        0        0     5797 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/inc/floorplan_svg.html
+-rw-r--r--   0        0        0      195 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/location_floor_plan.html
+-rw-r--r--   0        0        0       46 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/__init__.py
+-rw-r--r--   0        0        0     1838 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/fixtures.py
+-rw-r--r--   0        0        0      986 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_api.py
+-rw-r--r--   0        0        0     3447 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_api_views.py
+-rw-r--r--   0        0        0     1042 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_basic.py
+-rw-r--r--   0        0        0     5317 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_filters.py
+-rw-r--r--   0        0        0     6111 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_forms.py
+-rw-r--r--   0        0        0    10436 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_models.py
+-rw-r--r--   0        0        0     1114 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_utils.py
+-rw-r--r--   0        0        0     1057 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_views.py
+-rw-r--r--   0        0        0      952 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/urls.py
+-rw-r--r--   0        0        0      672 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/utils.py
+-rw-r--r--   0        0        0     1715 2024-04-12 20:05:27.923862 nautobot_floor_plan-2.1.0/nautobot_floor_plan/views.py
+-rw-r--r--   0        0        0     5806 2024-04-12 20:05:35.823851 nautobot_floor_plan-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4968 1970-01-01 00:00:00.000000 nautobot_floor_plan-2.1.0/PKG-INFO
```

### Comparing `nautobot_floor_plan-2.0.0rc1/LICENSE` & `nautobot_floor_plan-2.1.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2023, Network to Code, LLC
+Copyright (c) 2024, Network to Code, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nautobot_floor_plan-2.0.0rc1/README.md` & `nautobot_floor_plan-2.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Nautobot Floor Plan
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/icon-nautobot-floor-plan.png" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/icon-nautobot-floor-plan.png" class="logo" height="200px">
   <br>
-  <a href="https://github.com/nautobot/nautobot-plugin-floor-plan/actions"><img src="https://github.com/nautobot/nautobot-plugin-floor-plan/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/floor-plan/en/latest"><img src="https://readthedocs.org/projects/nautobot-plugin-floor-plan/badge/"></a>
+  <a href="https://github.com/nautobot/nautobot-app-floor-plan/actions"><img src="https://github.com/nautobot/nautobot-app-floor-plan/actions/workflows/ci.yml/badge.svg?branch=main"></a>
+  <a href="https://docs.nautobot.com/projects/floor-plan/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-floor-plan/badge/"></a>
   <a href="https://pypi.org/project/nautobot-floor-plan/"><img src="https://img.shields.io/pypi/v/nautobot-floor-plan"></a>
   <a href="https://pypi.org/project/nautobot-floor-plan/"><img src="https://img.shields.io/pypi/dm/nautobot-floor-plan"></a>
   <br>
   An <a href="https://www.networktocode.com/nautobot/apps/">App</a> for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
 
 ## Overview
 
 This App aids in data center management by providing the ability to create a gridded representation of the floor plan of a Nautobot Location and indicate the relative location of each Nautobot Rack within that floor plan.
 
 ### Screenshots
 
-![A sample floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-populated.png)
+![A sample floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-populated.png)
 
-![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/add-floor-plan-button.png)
+![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/add-floor-plan-button.png)
 
-![Form to define a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/add-floor-plan-form.png)
+![Form to define a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/add-floor-plan-form.png)
 
-![A new blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-empty.png)
+![A new blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-empty.png)
 
 More screenshots can be found in the [Using the App](https://docs.nautobot.com/projects/floor-plan/en/latest/user/app_use_cases/) page in the documentation.
 
 ## Documentation
 
 Full documentation for this App can be found over on the [Nautobot Docs](https://docs.nautobot.com) website:
 
@@ -35,15 +35,15 @@
 - [Administrator Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the App.
 - [Developer Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution Guide.
 - [Release Notes / Changelog](https://docs.nautobot.com/projects/floor-plan/en/latest/admin/release_notes/).
 - [Frequently Asked Questions](https://docs.nautobot.com/projects/floor-plan/en/latest/user/faq/).
 
 ### Contributing to the Documentation
 
-You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-plugin-floor-plan/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
+You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-app-floor-plan/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
 
 If you need to view the fully-generated documentation site, you can build it with [MkDocs](https://www.mkdocs.org/). A container hosting the documentation can be started using the `invoke` commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). Using this container, as your changes to the documentation are saved, they will be automatically rebuilt and any pages currently being viewed will be reloaded in your browser.
 
 Any PRs with fixes or improvements are very welcome!
 
 ## Questions
```

#### html2text {}

```diff
@@ -1,41 +1,40 @@
 # Nautobot Floor Plan
-[https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/
+ [https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/
                    docs/images/icon-nautobot-floor-plan.png]
-  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_f_l_o_o_r_-_p_l_a_n_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
-_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-
-_f_l_o_o_r_-_p_l_a_n_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]_[_h_t_t_p_s_:_/_/
+_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_f_l_o_o_r_-_p_l_a_n_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/
+_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_f_l_o_o_r_-
+   _p_l_a_n_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]
                              An _A_p_p for _N_a_u_t_o_b_o_t.
 ## Overview This App aids in data center management by providing the ability to
 create a gridded representation of the floor plan of a Nautobot Location and
 indicate the relative location of each Nautobot Rack within that floor plan.
 ### Screenshots ![A sample floor plan](https://raw.githubusercontent.com/
-nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-
-populated.png) ![Button to add a new floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/add-floor-plan-button.png) ![Form to define a new floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/add-floor-plan-form.png) ![A new blank floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/floor-plan-empty.png) More screenshots can be found in the [Using the
-App](https://docs.nautobot.com/projects/floor-plan/en/latest/user/
-app_use_cases/) page in the documentation. ## Documentation Full documentation
-for this App can be found over on the [Nautobot Docs](https://
+nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-populated.png)
+![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/
+nautobot-app-floor-plan/develop/docs/images/add-floor-plan-button.png) ![Form
+to define a new floor plan](https://raw.githubusercontent.com/nautobot/
+nautobot-app-floor-plan/develop/docs/images/add-floor-plan-form.png) ![A new
+blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-
+floor-plan/develop/docs/images/floor-plan-empty.png) More screenshots can be
+found in the [Using the App](https://docs.nautobot.com/projects/floor-plan/en/
+latest/user/app_use_cases/) page in the documentation. ## Documentation Full
+documentation for this App can be found over on the [Nautobot Docs](https://
 docs.nautobot.com) website: - [User Guide](https://docs.nautobot.com/projects/
 floor-plan/en/latest/user/app_overview/) - Overview, Using the App, Getting
 Started. - [Administrator Guide](https://docs.nautobot.com/projects/floor-plan/
 en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall
 the App. - [Developer Guide](https://docs.nautobot.com/projects/floor-plan/en/
 latest/dev/contributing/) - Extending the App, Code Reference, Contribution
 Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/floor-
 plan/en/latest/admin/release_notes/). - [Frequently Asked Questions](https://
 docs.nautobot.com/projects/floor-plan/en/latest/user/faq/). ### Contributing to
 the Documentation You can find all the Markdown source for the App
-documentation under the [`docs`](https://github.com/nautobot/nautobot-plugin-
+documentation under the [`docs`](https://github.com/nautobot/nautobot-app-
 floor-plan/tree/develop/docs) folder in this repository. For simple edits, a
 Markdown capable editor is sufficient: clone the repository and edit away. If
 you need to view the fully-generated documentation site, you can build it with
 [MkDocs](https://www.mkdocs.org/). A container hosting the documentation can be
 started using the `invoke` commands (details in the [Development Environment
 Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/
 dev_environment/#docker-development-environment)) on [http://localhost:8001]
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/serializers.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """API serializers for nautobot_floor_plan."""
-from nautobot.core.api.serializers import NautobotModelSerializer
-from nautobot.extras.api.mixins import TaggedModelSerializerMixin
+
+from nautobot.apps.api import NautobotModelSerializer, TaggedModelSerializerMixin
+
 from nautobot_floor_plan import models
 
 
-class FloorPlanSerializer(NautobotModelSerializer, TaggedModelSerializerMixin):
+class FloorPlanSerializer(NautobotModelSerializer, TaggedModelSerializerMixin):  # pylint: disable=too-many-ancestors
     """FloorPlan Serializer."""
 
     class Meta:
         """Meta attributes."""
 
         model = models.FloorPlan
         fields = "__all__"
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/api/views.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/api/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 from django.http import HttpResponse
 from django.shortcuts import get_object_or_404
 from django.views.decorators.clickjacking import xframe_options_sameorigin
 from drf_spectacular.utils import extend_schema
 from rest_framework.decorators import action
 
-from nautobot.extras.api.views import NautobotModelViewSet
+from nautobot.apps.api import NautobotModelViewSet
 
 from nautobot_floor_plan import filters, models
 from nautobot_floor_plan.api import serializers
 
 
-class FloorPlanViewSet(NautobotModelViewSet):
+class FloorPlanViewSet(NautobotModelViewSet):  # pylint: disable=too-many-ancestors
     """FloorPlan viewset."""
 
     queryset = models.FloorPlan.objects.all()
     serializer_class = serializers.FloorPlanSerializer
     filterset_class = filters.FloorPlanFilterSet
 
     @extend_schema(exclude=True)
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/filter_extensions.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/filter_extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extensions to Nautobot core models' filtering functionality."""
+
 import django_filters
 
 from nautobot.extras.plugins import PluginFilterExtension
 
 from nautobot_floor_plan import models
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/filters.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Filtering for nautobot_floor_plan."""
 
 import django_filters
 
 from nautobot.dcim.models import Location, Rack
-from nautobot.extras.filters import NautobotFilterSet
+from nautobot.apps.filters import NautobotFilterSet
 from nautobot.apps.filters import NaturalKeyOrPKMultipleChoiceFilter, SearchFilter
 
 from nautobot_floor_plan import models
 
 
 class FloorPlanFilterSet(NautobotFilterSet):
     """Filter for FloorPlan."""
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/forms.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tables.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,93 @@
-# TBD: Remove after releasing pylint-nautobot v0.3.0
-# https://github.com/nautobot/pylint-nautobot/commit/48efc016fffa0b9df02f61bdaa9c4a0933351d29
-# pylint: disable=nb-incorrect-base-class
-
-"""Forms for nautobot_floor_plan."""
-from django import forms
-
-from nautobot.dcim.models import Location, Rack
-from nautobot.extras.forms import (
-    NautobotBulkEditForm,
-    NautobotFilterForm,
-    NautobotModelForm,
-    TagsBulkEditFormMixin,
-)
-from nautobot.apps.forms import (
-    DynamicModelChoiceField,
-    DynamicModelMultipleChoiceField,
-    TagFilterField,
-)
+"""Tables for nautobot_floor_plan."""
 
-from nautobot_floor_plan import models
+import django_tables2 as tables
+from nautobot.apps.tables import BaseTable, ButtonsColumn, TagColumn, ToggleColumn
+from nautobot.core.templatetags.helpers import hyperlinked_object
 
+from nautobot_floor_plan import models
 
-class FloorPlanForm(NautobotModelForm):
-    """FloorPlan creation/edit form."""
 
-    location = DynamicModelChoiceField(queryset=Location.objects.all())
+class FloorPlanTable(BaseTable):
+    # pylint: disable=too-few-public-methods
+    """Table for list view."""
+
+    pk = ToggleColumn()
+    floor_plan = tables.Column(empty_values=[])
+    location = tables.Column(linkify=True)
+    tags = TagColumn()
+    actions = ButtonsColumn(models.FloorPlan)
+
+    def render_floor_plan(self, record):
+        """Render a link to the detail view for the FloorPlan record itself."""
+        return hyperlinked_object(record)
 
-    class Meta:
+    class Meta(BaseTable.Meta):
         """Meta attributes."""
 
         model = models.FloorPlan
-        fields = [
+        # pylint: disable=nb-use-fields-all
+        fields = (
+            "pk",
+            "floor_plan",
             "location",
             "x_size",
             "y_size",
             "tile_width",
             "tile_depth",
             "tags",
-        ]
-
-
-class FloorPlanBulkEditForm(TagsBulkEditFormMixin, NautobotBulkEditForm):
-    """FloorPlan bulk edit form."""
-
-    pk = forms.ModelMultipleChoiceField(queryset=models.FloorPlan.objects.all(), widget=forms.MultipleHiddenInput)
-    x_size = forms.IntegerField(min_value=1, required=False)
-    y_size = forms.IntegerField(min_value=1, required=False)
-    tile_width = forms.IntegerField(min_value=1, required=False)
-    tile_depth = forms.IntegerField(min_value=1, required=False)
-
-    class Meta:
-        """Meta attributes."""
-
-        fields = ["pk", "x_size", "y_size", "tile_width", "tile_depth", "tags"]
-
-
-class FloorPlanFilterForm(NautobotFilterForm):
-    """Filter form to filter searches."""
-
-    model = models.FloorPlan
-    field_order = ["q", "location", "x_size", "y_size"]
-
-    q = forms.CharField(required=False, label="Search")
-    location = DynamicModelMultipleChoiceField(queryset=Location.objects.all(), to_field_name="pk", required=False)
-    tag = TagFilterField(model)
-
+            "actions",
+        )
+        default_columns = (
+            "pk",
+            "floor_plan",
+            "location",
+            "tags",
+            "actions",
+        )
 
-class FloorPlanTileForm(NautobotModelForm):
-    """FloorPlanTile creation/edit form."""
 
-    floor_plan = DynamicModelChoiceField(queryset=models.FloorPlan.objects.all())
-    rack = DynamicModelChoiceField(
-        queryset=Rack.objects.all(), required=False, query_params={"nautobot_floor_plan_floor_plan": "$floor_plan"}
-    )
+class FloorPlanTileTable(BaseTable):
+    # pylint: disable=too-few-public-methods
+    """Table for list view."""
+
+    floor_plan_tile = tables.Column(verbose_name="Tile", empty_values=[])
+    floor_plan = tables.Column(linkify=True)
+    location = tables.Column(accessor="floor_plan__location", linkify=True)
+    rack = tables.Column(linkify=True)
+    tags = TagColumn()
+    actions = ButtonsColumn(models.FloorPlanTile)
+
+    def render_floor_plan_tile(self, record):
+        """Render a link to the detail view for the FloorPlanTile record itself."""
+        return hyperlinked_object(record)
 
-    class Meta:
+    class Meta(BaseTable.Meta):
         """Meta attributes."""
 
         model = models.FloorPlanTile
-        fields = [
+        # pylint: disable=nb-use-fields-all
+        fields = (
+            "floor_plan_tile",
             "floor_plan",
+            "location",
             "x_origin",
             "y_origin",
             "x_size",
             "y_size",
-            "status",
             "rack",
             "rack_orientation",
             "tags",
-        ]
+            "actions",
+        )
+        default_columns = (
+            "floor_plan_tile",
+            "floor_plan",
+            "location",
+            "x_origin",
+            "y_origin",
+            "x_size",
+            "y_size",
+            "rack",
+            "tags",
+            "actions",
+        )
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0001_initial.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0002_fixup_null.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0002_fixup_null.py`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/migrations/0003_auto_20230908_1339.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/migrations/0003_auto_20230908_1339.py`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/models.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.core.validators import MinValueValidator
 from django.db import models
 
 from nautobot.apps.models import extras_features
 from nautobot.apps.models import PrimaryModel
 from nautobot.apps.models import StatusField
 
-from nautobot_floor_plan.choices import RackOrientationChoices
+from nautobot_floor_plan.choices import RackOrientationChoices, AxisLabelsChoices
 from nautobot_floor_plan.svg import FloorPlanSVG
 
 
 logger = logging.getLogger(__name__)
 
 
 @extras_features(
@@ -49,14 +49,26 @@
         help_text='Relative width of each "tile" in the floor plan (cm, inches, etc.)',
     )
     tile_depth = models.PositiveSmallIntegerField(
         validators=[MinValueValidator(1)],
         default=100,
         help_text='Relative depth of each "tile" in the floor plan (cm, inches, etc.)',
     )
+    x_axis_labels = models.CharField(
+        max_length=10,
+        choices=AxisLabelsChoices,
+        default=AxisLabelsChoices.NUMBERS,
+        help_text="Grid labels of X axis (horizontal).",
+    )
+    y_axis_labels = models.CharField(
+        max_length=10,
+        choices=AxisLabelsChoices,
+        default=AxisLabelsChoices.NUMBERS,
+        help_text="Grid labels of Y axis (vertical).",
+    )
 
     class Meta:
         """Metaclass attributes."""
 
         ordering = ["location___name"]
 
     def __str__(self):
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/navigation.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/navigation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Menu items."""
 
-from nautobot.core.apps import NavMenuGroup, NavMenuItem, NavMenuTab, NavMenuAddButton, NavMenuImportButton
+from nautobot.apps.ui import NavMenuGroup, NavMenuItem, NavMenuTab, NavMenuAddButton, NavMenuImportButton
 
 menu_items = (
     NavMenuTab(
         name="Organization",
         groups=(
             NavMenuGroup(
                 name="Locations",
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/static/nautobot_floor_plan/css/svg.css` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/static/nautobot_floor_plan/css/svg.css`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/svg.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/svg.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Render a FloorPlan as an SVG image."""
+
 import logging
 import os
 import svgwrite
 
 from django.urls import reverse
 from django.utils.functional import cached_property
 from django.utils.http import urlencode
 
 from nautobot.core.templatetags.helpers import fgcolor
 
-from nautobot_floor_plan.choices import RackOrientationChoices
+from nautobot_floor_plan.choices import RackOrientationChoices, AxisLabelsChoices
+from nautobot_floor_plan.utils import grid_number_to_letter
 
 
 logger = logging.getLogger(__name__)
 
 
 class FloorPlanSVG:
     """Use this class to render a FloorPlan as an SVG image."""
@@ -105,44 +107,48 @@
                         y * self.GRID_SIZE_Y + self.GRID_OFFSET,
                     ),
                     class_="grid",
                 )
             )
         # Axis labels
         for x in range(1, self.floor_plan.x_size + 1):
+            label = grid_number_to_letter(x) if self.floor_plan.x_axis_labels == AxisLabelsChoices.LETTERS else str(x)
             drawing.add(
                 drawing.text(
-                    str(x),
+                    label,
                     insert=(
                         (x - 0.5) * self.GRID_SIZE_X + self.GRID_OFFSET,
                         self.BORDER_WIDTH + self.TEXT_LINE_HEIGHT / 2,
                     ),
                     class_="grid-label",
                 )
             )
         for y in range(1, self.floor_plan.y_size + 1):
+            label = grid_number_to_letter(y) if self.floor_plan.y_axis_labels == AxisLabelsChoices.LETTERS else str(y)
             drawing.add(
                 drawing.text(
-                    str(y),
+                    label,
                     insert=(
                         self.BORDER_WIDTH + self.TEXT_LINE_HEIGHT / 2,
                         (y - 0.5) * self.GRID_SIZE_Y + self.GRID_OFFSET,
                     ),
                     class_="grid-label",
                 )
             )
 
         # Links to populate tiles
+        y_letters = self.floor_plan.y_axis_labels == AxisLabelsChoices.LETTERS
+        x_letters = self.floor_plan.x_axis_labels == AxisLabelsChoices.LETTERS
         for y in range(1, self.floor_plan.y_size + 1):
             for x in range(1, self.floor_plan.x_size + 1):
                 query_params = urlencode(
                     {
                         "floor_plan": self.floor_plan.pk,
-                        "x_origin": x,
-                        "y_origin": y,
+                        "x_origin": grid_number_to_letter(x) if x_letters else x,
+                        "y_origin": grid_number_to_letter(y) if y_letters else y,
                         "return_url": self.return_url,
                     }
                 )
                 add_url = f"{self.add_url}?{query_params}"
                 add_link = drawing.add(drawing.a(href=add_url, target="_top"))
                 # "add" button
                 add_link.add(
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/template_content.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/template_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Added content to the device model view for floor plan."""
+
 from django.core.exceptions import ObjectDoesNotExist
 from django.urls import reverse
 
 from nautobot.extras.plugins import PluginTemplateExtension
 
 
 class LocationFloorPlanTab(PluginTemplateExtension):  # pylint: disable=abstract-method
-    """Plugin extensions for Location model detail view."""
+    """App extensions for Location model detail view."""
 
     model = "dcim.location"
 
     def buttons(self):
         """Add "Add/Delete Floor Plan" button as appropriate to the Location detail view."""
         location = self.context["object"]
         user = self.context["request"].user
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/floorplan_retrieve.html` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/floorplan_retrieve.html`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,26 @@
                 <td>Tile Width (Relative Units)</td>
                 <td>{{ object.tile_width }}</td>
             </tr>
             <tr>
                 <td>Tile Depth (Relative Units)</td>
                 <td>{{ object.tile_depth }}</td>
             </tr>
+            <tr>
+                <td>X Axis Labels</td>
+                <td>{{ object.x_axis_labels }}</td>
+            </tr>
+            <tr>
+                <td>Y Axis Labels</td>
+                <td>{{ object.y_axis_labels }}</td>
+            </tr>
+            <tr>
+                <td>Tiles</td>
+                <td><a href="{% url 'plugins:nautobot_floor_plan:floorplantile_list' %}?floor_plan={{ object.pk }}">{{ object.tiles.count }}</a></td>
+            </tr>
         </table>
     </div>
 {% endblock content_left_page %}
 
 {% block content_full_width_page %}
     {% include 'nautobot_floor_plan/inc/floorplan_svg.html' with floor_plan=object %}
 {% endblock content_full_width_page %}
```

#### html2text {}

```diff
@@ -6,10 +6,13 @@
 {% endblock breadcrumbs %} {% block content_left_page %}
 FFlloooorr PPllaann
 Location                    {{ object.location | hyperlinked_object }}
 X Size (Tiles)              {{ object.x_size }}
 Y Size (Tiles)              {{ object.y_size }}
 Tile Width (Relative Units) {{ object.tile_width }}
 Tile Depth (Relative Units) {{ object.tile_depth }}
+X Axis Labels               {{ object.x_axis_labels }}
+Y Axis Labels               {{ object.y_axis_labels }}
+Tiles                       _{_{_ _o_b_j_e_c_t_._t_i_l_e_s_._c_o_u_n_t_ _}_}
 {% endblock content_left_page %} {% block content_full_width_page %} {% include
 'nautobot_floor_plan/inc/floorplan_svg.html' with floor_plan=object %} {%
 endblock content_full_width_page %}
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/floorplantile_retrieve.html` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/floorplantile_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/templates/nautobot_floor_plan/inc/floorplan_svg.html` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/templates/nautobot_floor_plan/inc/floorplan_svg.html`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/fixtures.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_api.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for nautobot_floor_plan."""
+
 from django.contrib.auth import get_user_model
 from django.test import TestCase
 from django.urls import reverse
 from rest_framework import status
 from rest_framework.test import APIClient
 
 from nautobot.users.models import Token
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_api_views.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_api_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Unit tests for nautobot_floor_plan."""
+
 from django.contrib.contenttypes.models import ContentType
 
 from nautobot.dcim.models import Rack
 from nautobot.extras.models import Tag
 from nautobot.apps.testing import APIViewTestCases
 
 from nautobot_floor_plan import choices, models
@@ -11,14 +12,15 @@
 
 class FloorPlanAPIViewTest(APIViewTestCases.APIViewTestCase):
     """Test the API viewsets for FloorPlan."""
 
     model = models.FloorPlan
     bulk_update_data = {"x_size": 10, "y_size": 1}
     brief_fields = ["display", "id", "url", "x_size", "y_size"]
+    choices_fields = ["x_axis_labels", "y_axis_labels"]
 
     @classmethod
     def setUpTestData(cls):
         data = fixtures.create_prerequisites(floor_count=6)
         fixtures.create_floor_plans(data["floors"][:3])
         cls.create_data = [
             {
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_filters.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test FloorPlan Filter."""
+
 from django.test import TestCase
 
 from nautobot.dcim.models import Rack
 from nautobot.extras.models import Tag
 
 from nautobot_floor_plan import filters
 from nautobot_floor_plan import models
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_models.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/tests/test_views.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/tests/test_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Unit tests for views."""
 
 from nautobot.apps.testing import ViewTestCases
 
-from nautobot_floor_plan import models
+from nautobot_floor_plan import models, choices
 from nautobot_floor_plan.tests import fixtures
 
 
 class FloorPlanViewTest(ViewTestCases.PrimaryObjectViewTestCase):
     """Test the FloorPlan views."""
 
     model = models.FloorPlan
@@ -24,8 +24,10 @@
         fixtures.create_floor_plans(data["floors"][:3])
         cls.form_data = {
             "location": data["floors"][3].pk,
             "tile_depth": 100,
             "tile_width": 100,
             "x_size": 1,
             "y_size": 2,
+            "x_axis_labels": choices.AxisLabelsChoices.NUMBERS,
+            "y_axis_labels": choices.AxisLabelsChoices.NUMBERS,
         }
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/urls.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-"""Django urlpatterns declaration for nautobot_floor_plan plugin."""
+"""Django urlpatterns declaration for nautobot_floor_plan app."""
 
 from django.urls import path
 
-# TODO: when minimum Nautobot version becomes 1.5.2 or later, we can use:
-# from nautobot.apps.urls import NautobotUIViewSetRouter
-from nautobot.core.views.routers import NautobotUIViewSetRouter
+from nautobot.apps.urls import NautobotUIViewSetRouter
 from nautobot.extras.views import ObjectChangeLogView, ObjectNotesView
 
 from nautobot_floor_plan import models, views
 
 
 app_name = "floor_plan"
 router = NautobotUIViewSetRouter()
```

### Comparing `nautobot_floor_plan-2.0.0rc1/nautobot_floor_plan/views.py` & `nautobot_floor_plan-2.1.0/nautobot_floor_plan/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 """Views for FloorPlan."""
 
-# TODO: when minimum Nautobot version becomes 1.5.2 or later, we can use:
-# from nautobot.apps import views
-from nautobot.core.views.generic import ObjectView
-from nautobot.core.views.viewsets import NautobotUIViewSet
+from nautobot.apps.views import (
+    NautobotUIViewSet,
+    ObjectListViewMixin,
+    ObjectDetailViewMixin,
+    ObjectEditViewMixin,
+    ObjectDestroyViewMixin,
+    ObjectChangeLogViewMixin,
+    ObjectNotesViewMixin,
+)
+from nautobot.apps.views import ObjectView
 from nautobot.dcim.models import Location
 
 from nautobot_floor_plan import filters, forms, models, tables
 from nautobot_floor_plan.api import serializers
 
 
 class FloorPlanUIViewSet(NautobotUIViewSet):  # TODO we only need a subset of views
@@ -26,14 +32,25 @@
 class LocationFloorPlanTab(ObjectView):
     """Add a "Floor Plan" tab to the Location detail view."""
 
     queryset = Location.objects.all()
     template_name = "nautobot_floor_plan/location_floor_plan.html"
 
 
-class FloorPlanTileUIViewSet(NautobotUIViewSet):  # TODO we only need a subset of views
+class FloorPlanTileUIViewSet(
+    ObjectDetailViewMixin,
+    ObjectListViewMixin,
+    ObjectEditViewMixin,
+    ObjectDestroyViewMixin,
+    ObjectChangeLogViewMixin,
+    ObjectNotesViewMixin,
+):
+    # pylint: disable=abstract-method
     """ViewSet for FloorPlanTile views."""
 
+    filterset_class = filters.FloorPlanTileFilterSet
     form_class = forms.FloorPlanTileForm
     lookup_field = "pk"
     queryset = models.FloorPlanTile.objects.all()
     serializer_class = serializers.FloorPlanTileSerializer
+    table_class = tables.FloorPlanTileTable
+    action_buttons = ()
```

### Comparing `nautobot_floor_plan-2.0.0rc1/PKG-INFO` & `nautobot_floor_plan-2.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: nautobot-floor-plan
-Version: 2.0.0rc1
+Version: 2.1.0
 Summary: Nautobot Floor Plan
-Home-page: https://github.com/nautobot/nautobot-plugin-floor-plan
+Home-page: https://github.com/nautobot/nautobot-app-floor-plan
 License: Apache-2.0
-Keywords: nautobot,nautobot-plugin
+Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: nautobot
-Requires-Dist: nautobot (>=2.0.0rc1,<2.0.0rc99) ; extra == "nautobot"
-Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-floor-plan
+Provides-Extra: all
+Requires-Dist: nautobot (>=2.0.0,<3.0.0)
+Project-URL: Documentation, https://docs.nautobot.com/projects/floor-plan/en/latest/
+Project-URL: Repository, https://github.com/nautobot/nautobot-app-floor-plan
 Description-Content-Type: text/markdown
 
 # Nautobot Floor Plan
 
 <p align="center">
-  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/icon-nautobot-floor-plan.png" class="logo" height="200px">
+  <img src="https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/icon-nautobot-floor-plan.png" class="logo" height="200px">
   <br>
-  <a href="https://github.com/nautobot/nautobot-plugin-floor-plan/actions"><img src="https://github.com/nautobot/nautobot-plugin-floor-plan/actions/workflows/ci.yml/badge.svg?branch=main"></a>
-  <a href="https://docs.nautobot.com/projects/floor-plan/en/latest"><img src="https://readthedocs.org/projects/nautobot-plugin-floor-plan/badge/"></a>
+  <a href="https://github.com/nautobot/nautobot-app-floor-plan/actions"><img src="https://github.com/nautobot/nautobot-app-floor-plan/actions/workflows/ci.yml/badge.svg?branch=main"></a>
+  <a href="https://docs.nautobot.com/projects/floor-plan/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-floor-plan/badge/"></a>
   <a href="https://pypi.org/project/nautobot-floor-plan/"><img src="https://img.shields.io/pypi/v/nautobot-floor-plan"></a>
   <a href="https://pypi.org/project/nautobot-floor-plan/"><img src="https://img.shields.io/pypi/dm/nautobot-floor-plan"></a>
   <br>
   An <a href="https://www.networktocode.com/nautobot/apps/">App</a> for <a href="https://nautobot.com/">Nautobot</a>.
 </p>
 
 ## Overview
 
 This App aids in data center management by providing the ability to create a gridded representation of the floor plan of a Nautobot Location and indicate the relative location of each Nautobot Rack within that floor plan.
 
 ### Screenshots
 
-![A sample floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-populated.png)
+![A sample floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-populated.png)
 
-![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/add-floor-plan-button.png)
+![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/add-floor-plan-button.png)
 
-![Form to define a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/add-floor-plan-form.png)
+![Form to define a new floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/add-floor-plan-form.png)
 
-![A new blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-empty.png)
+![A new blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-empty.png)
 
 More screenshots can be found in the [Using the App](https://docs.nautobot.com/projects/floor-plan/en/latest/user/app_use_cases/) page in the documentation.
 
 ## Documentation
 
 Full documentation for this App can be found over on the [Nautobot Docs](https://docs.nautobot.com) website:
 
@@ -56,15 +59,15 @@
 - [Administrator Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the App.
 - [Developer Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/contributing/) - Extending the App, Code Reference, Contribution Guide.
 - [Release Notes / Changelog](https://docs.nautobot.com/projects/floor-plan/en/latest/admin/release_notes/).
 - [Frequently Asked Questions](https://docs.nautobot.com/projects/floor-plan/en/latest/user/faq/).
 
 ### Contributing to the Documentation
 
-You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-plugin-floor-plan/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
+You can find all the Markdown source for the App documentation under the [`docs`](https://github.com/nautobot/nautobot-app-floor-plan/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient: clone the repository and edit away.
 
 If you need to view the fully-generated documentation site, you can build it with [MkDocs](https://www.mkdocs.org/). A container hosting the documentation can be started using the `invoke` commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). Using this container, as your changes to the documentation are saved, they will be automatically rebuilt and any pages currently being viewed will be reloaded in your browser.
 
 Any PRs with fixes or improvements are very welcome!
 
 ## Questions
```

#### html2text {}

```diff
@@ -1,52 +1,53 @@
-Metadata-Version: 2.1 Name: nautobot-floor-plan Version: 2.0.0rc1 Summary:
-Nautobot Floor Plan Home-page: https://github.com/nautobot/nautobot-plugin-
-floor-plan License: Apache-2.0 Keywords: nautobot,nautobot-plugin Author:
-Network to Code, LLC Author-email: info@networktocode.com Requires-Python:
->=3.8,<3.12 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Provides-Extra: nautobot Requires-Dist: nautobot
-(>=2.0.0rc1,<2.0.0rc99) ; extra == "nautobot" Project-URL: Repository, https://
-github.com/nautobot/nautobot-plugin-floor-plan Description-Content-Type: text/
-markdown # Nautobot Floor Plan
-[https://raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/
+Metadata-Version: 2.1 Name: nautobot-floor-plan Version: 2.1.0 Summary:
+Nautobot Floor Plan Home-page: https://github.com/nautobot/nautobot-app-floor-
+plan License: Apache-2.0 Keywords: nautobot,nautobot-app,nautobot-plugin
+Author: Network to Code, LLC Author-email: info@networktocode.com Requires-
+Python: >=3.8,<3.12 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
+Requires-Dist: nautobot (>=2.0.0,<3.0.0) Project-URL: Documentation, https://
+docs.nautobot.com/projects/floor-plan/en/latest/ Project-URL: Repository,
+https://github.com/nautobot/nautobot-app-floor-plan Description-Content-Type:
+text/markdown # Nautobot Floor Plan
+ [https://raw.githubusercontent.com/nautobot/nautobot-app-floor-plan/develop/
                    docs/images/icon-nautobot-floor-plan.png]
-  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_f_l_o_o_r_-_p_l_a_n_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/
-_c_i_._y_m_l_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-
-_f_l_o_o_r_-_p_l_a_n_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]_[_h_t_t_p_s_:_/_/
+_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_a_p_p_-_f_l_o_o_r_-_p_l_a_n_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/
+_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_f_l_o_o_r_-
+   _p_l_a_n_/_b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]_[_h_t_t_p_s_:_/_/
                   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_f_l_o_o_r_-_p_l_a_n_]
                              An _A_p_p for _N_a_u_t_o_b_o_t.
 ## Overview This App aids in data center management by providing the ability to
 create a gridded representation of the floor plan of a Nautobot Location and
 indicate the relative location of each Nautobot Rack within that floor plan.
 ### Screenshots ![A sample floor plan](https://raw.githubusercontent.com/
-nautobot/nautobot-plugin-floor-plan/develop/docs/images/floor-plan-
-populated.png) ![Button to add a new floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/add-floor-plan-button.png) ![Form to define a new floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/add-floor-plan-form.png) ![A new blank floor plan](https://
-raw.githubusercontent.com/nautobot/nautobot-plugin-floor-plan/develop/docs/
-images/floor-plan-empty.png) More screenshots can be found in the [Using the
-App](https://docs.nautobot.com/projects/floor-plan/en/latest/user/
-app_use_cases/) page in the documentation. ## Documentation Full documentation
-for this App can be found over on the [Nautobot Docs](https://
+nautobot/nautobot-app-floor-plan/develop/docs/images/floor-plan-populated.png)
+![Button to add a new floor plan](https://raw.githubusercontent.com/nautobot/
+nautobot-app-floor-plan/develop/docs/images/add-floor-plan-button.png) ![Form
+to define a new floor plan](https://raw.githubusercontent.com/nautobot/
+nautobot-app-floor-plan/develop/docs/images/add-floor-plan-form.png) ![A new
+blank floor plan](https://raw.githubusercontent.com/nautobot/nautobot-app-
+floor-plan/develop/docs/images/floor-plan-empty.png) More screenshots can be
+found in the [Using the App](https://docs.nautobot.com/projects/floor-plan/en/
+latest/user/app_use_cases/) page in the documentation. ## Documentation Full
+documentation for this App can be found over on the [Nautobot Docs](https://
 docs.nautobot.com) website: - [User Guide](https://docs.nautobot.com/projects/
 floor-plan/en/latest/user/app_overview/) - Overview, Using the App, Getting
 Started. - [Administrator Guide](https://docs.nautobot.com/projects/floor-plan/
 en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall
 the App. - [Developer Guide](https://docs.nautobot.com/projects/floor-plan/en/
 latest/dev/contributing/) - Extending the App, Code Reference, Contribution
 Guide. - [Release Notes / Changelog](https://docs.nautobot.com/projects/floor-
 plan/en/latest/admin/release_notes/). - [Frequently Asked Questions](https://
 docs.nautobot.com/projects/floor-plan/en/latest/user/faq/). ### Contributing to
 the Documentation You can find all the Markdown source for the App
-documentation under the [`docs`](https://github.com/nautobot/nautobot-plugin-
+documentation under the [`docs`](https://github.com/nautobot/nautobot-app-
 floor-plan/tree/develop/docs) folder in this repository. For simple edits, a
 Markdown capable editor is sufficient: clone the repository and edit away. If
 you need to view the fully-generated documentation site, you can build it with
 [MkDocs](https://www.mkdocs.org/). A container hosting the documentation can be
 started using the `invoke` commands (details in the [Development Environment
 Guide](https://docs.nautobot.com/projects/floor-plan/en/latest/dev/
 dev_environment/#docker-development-environment)) on [http://localhost:8001]
```

