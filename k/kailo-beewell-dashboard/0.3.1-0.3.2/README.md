# Comparing `tmp/kailo-beewell-dashboard-0.3.1.tar.gz` & `tmp/kailo-beewell-dashboard-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kailo-beewell-dashboard-0.3.1.tar", last modified: Tue Apr  9 15:53:17 2024, max compression
+gzip compressed data, was "kailo-beewell-dashboard-0.3.2.tar", last modified: Fri Apr 12 14:53:47 2024, max compression
```

## Comparing `kailo-beewell-dashboard-0.3.1.tar` & `kailo-beewell-dashboard-0.3.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.289265 kailo-beewell-dashboard-0.3.1/
--rw-rw-r--   0 amy       (1000) amy       (1000)     1070 2024-02-19 16:48:26.000000 kailo-beewell-dashboard-0.3.1/LICENSE
--rw-rw-r--   0 amy       (1000) amy       (1000)      158 2024-04-09 15:53:10.000000 kailo-beewell-dashboard-0.3.1/MANIFEST.in
--rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-09 15:53:17.289265 kailo-beewell-dashboard-0.3.1/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     1590 2024-04-09 15:49:07.000000 kailo-beewell-dashboard-0.3.1/README.md
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.273265 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/
--rw-rw-r--   0 amy       (1000) amy       (1000)      151 2024-04-09 15:48:43.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/__init__.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6619 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/about_page.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3939 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/authentication.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    15122 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/bar_charts.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6242 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/bar_charts_text.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.277265 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/css/
--rw-rw-r--   0 amy       (1000) amy       (1000)     1802 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/css/static_report_style.css
--rw-rw-r--   0 amy       (1000) amy       (1000)     3223 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/css/style.css
--rw-rw-r--   0 amy       (1000) amy       (1000)    25957 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/explore_results.py
--rw-rw-r--   0 amy       (1000) amy       (1000)      557 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/grammar.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.281265 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/
--rw-rw-r--   0 amy       (1000) amy       (1000)    61702 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/beewell_map.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   185745 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/canva_people.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    48221 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/circle_divider.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    72751 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/dashboard_home_section.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    31928 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/devices.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   550917 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)   258283 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/home_image_3_transparent.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    92545 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_beewell_logo.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    93979 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    88360 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_systems_adapted.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   564177 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/levelling-the-ground.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)    21040 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/northern_devon.png
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.289265 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/
--rw-rw-r--   0 amy       (1000) amy       (1000)   180897 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choice.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   155419 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    23923 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   131754 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/family.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   106617 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   127520 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/free_time.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   102391 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   129719 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/friends.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   104548 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   123168 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/future.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    98588 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    21352 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/happy.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   108174 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/health.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    82741 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   120585 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/home.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    95604 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   121744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/life.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    96996 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    16076 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/ok.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    19823 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/sad.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   121199 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/school.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    96276 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   156249 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/things.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   131030 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
--rw-rw-r--   0 amy       (1000) amy       (1000)    85100 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/thinking.png
--rw-rw-r--   0 amy       (1000) amy       (1000)   475730 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/young-person-journey.jpg
--rw-rw-r--   0 amy       (1000) amy       (1000)     1767 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     4418 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/import_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1843 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/map.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2503 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/page_setup.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     6853 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/reshape_data.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14456 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/response_labels.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    13118 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/reuse_text.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2723 2024-02-21 10:54:31.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/score_descriptions.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    13575 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/static_report.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     2297 2024-02-21 10:54:39.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/stylable_container.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    12744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/summary_rag.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/switch_page_button.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14229 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_aggregate.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3553 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_demographic.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    19646 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_responses.py
--rw-rw-r--   0 amy       (1000) amy       (1000)    14885 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_scores.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     3935 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/topic_labels.py
--rw-rw-r--   0 amy       (1000) amy       (1000)     7968 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/who_took_part.py
-drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-09 15:53:17.289265 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/
--rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-09 15:53:17.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 amy       (1000) amy       (1000)     3546 2024-04-09 15:53:17.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)        1 2024-04-09 15:53:17.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      275 2024-04-09 15:53:17.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/requires.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-04-09 15:53:17.000000 kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)      693 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.1/requirements.txt
--rw-rw-r--   0 amy       (1000) amy       (1000)       38 2024-04-09 15:53:17.289265 kailo-beewell-dashboard-0.3.1/setup.cfg
--rw-rw-r--   0 amy       (1000) amy       (1000)     1167 2024-04-09 15:51:48.000000 kailo-beewell-dashboard-0.3.1/setup.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1070 2024-02-19 16:48:26.000000 kailo-beewell-dashboard-0.3.2/LICENSE
+-rw-rw-r--   0 amy       (1000) amy       (1000)      158 2024-04-09 15:53:10.000000 kailo-beewell-dashboard-0.3.2/MANIFEST.in
+-rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/PKG-INFO
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1590 2024-04-12 14:51:29.000000 kailo-beewell-dashboard-0.3.2/README.md
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.633476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/
+-rw-rw-r--   0 amy       (1000) amy       (1000)      151 2024-04-12 14:50:52.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/__init__.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6619 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/about_page.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3939 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/authentication.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    15122 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6242 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts_text.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.637476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1802 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/static_report_style.css
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3223 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/style.css
+-rw-rw-r--   0 amy       (1000) amy       (1000)    25957 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/explore_results.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)      557 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/grammar.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.645476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/
+-rw-rw-r--   0 amy       (1000) amy       (1000)    61702 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/beewell_map.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   185745 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/canva_people.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    48221 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/circle_divider.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    72751 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/dashboard_home_section.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    31928 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/devices.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   550917 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/discovery-looking-researching.jpg
+-rw-rw-r--   0 amy       (1000) amy       (1000)   258283 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/home_image_3_transparent.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    92545 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    93979 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    88360 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_systems_adapted.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   564177 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/levelling-the-ground.jpg
+-rw-rw-r--   0 amy       (1000) amy       (1000)    21040 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/northern_devon.png
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/
+-rw-rw-r--   0 amy       (1000) amy       (1000)   180897 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   155419 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    23923 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choose_one.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   131754 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   106617 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   127520 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   102391 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   129719 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   104548 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   123168 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    98588 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    21352 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/happy.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   108174 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    82741 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   120585 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    95604 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   121744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    96996 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    16076 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/ok.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    19823 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/sad.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   121199 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    96276 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   156249 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   131030 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things_crop.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)    85100 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/thinking.png
+-rw-rw-r--   0 amy       (1000) amy       (1000)   475730 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/young-person-journey.jpg
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1767 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     4418 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/import_data.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1843 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/map.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2503 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/page_setup.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     6853 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reshape_data.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14456 2024-03-01 15:06:45.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/response_labels.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    13118 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reuse_text.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2723 2024-02-21 10:54:31.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/score_descriptions.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    13596 2024-04-12 14:37:13.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/static_report.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     2297 2024-02-21 10:54:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/stylable_container.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    12744 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/summary_rag.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1077 2024-02-19 14:53:39.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/switch_page_button.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14229 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_aggregate.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3553 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_demographic.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    19646 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_responses.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)    14885 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_scores.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3935 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/topic_labels.py
+-rw-rw-r--   0 amy       (1000) amy       (1000)     7968 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/who_took_part.py
+drwxrwxr-x   0 amy       (1000) amy       (1000)        0 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/
+-rw-r--r--   0 amy       (1000) amy       (1000)     2640 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 amy       (1000) amy       (1000)     3546 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)        1 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)      275 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)       24 2024-04-12 14:53:47.000000 kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)      693 2024-04-09 14:48:12.000000 kailo-beewell-dashboard-0.3.2/requirements.txt
+-rw-rw-r--   0 amy       (1000) amy       (1000)       38 2024-04-12 14:53:47.661476 kailo-beewell-dashboard-0.3.2/setup.cfg
+-rw-rw-r--   0 amy       (1000) amy       (1000)     1167 2024-04-09 15:51:48.000000 kailo-beewell-dashboard-0.3.2/setup.py
```

### Comparing `kailo-beewell-dashboard-0.3.1/LICENSE` & `kailo-beewell-dashboard-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/PKG-INFO` & `kailo-beewell-dashboard-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
 Requires-Dist: matplotlib==3.8.3
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.1-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.1/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +50,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.1). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-09},
-  version = {0.3.1},
+  date = {2024-04-12},
+  version = {0.3.2},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.1/README.md` & `kailo-beewell-dashboard-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.1-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.1/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -19,19 +19,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.1). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-09},
-  version = {0.3.1},
+  date = {2024-04-12},
+  version = {0.3.2},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/about_page.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/about_page.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/authentication.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/authentication.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/bar_charts.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/bar_charts_text.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/bar_charts_text.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/css/static_report_style.css` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/static_report_style.css`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/css/style.css` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/css/style.css`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/explore_results.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/explore_results.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/grammar.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/grammar.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/beewell_map.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/beewell_map.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/canva_people.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/canva_people.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/circle_divider.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/circle_divider.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/dashboard_home_section.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/dashboard_home_section.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/devices.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/devices.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/discovery-looking-researching.jpg` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/discovery-looking-researching.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/home_image_3_transparent.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/home_image_3_transparent.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_beewell_logo.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_beewell_logo_padded.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/kailo_systems_adapted.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/kailo_systems_adapted.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/levelling-the-ground.jpg` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/levelling-the-ground.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/northern_devon.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/northern_devon.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choice.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choice_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/choose_one.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/choose_one.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/family.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/family_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/family_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/free_time.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/free_time_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/friends.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/friends_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/future.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/future_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/future_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/happy.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/happy.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/health.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/health_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/health_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/home.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/home_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/home_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/life.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/life_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/life_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/ok.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/ok.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/sad.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/sad.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/school.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/school_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/school_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/things.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/symbol_survey/things_crop.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/symbol_survey/things_crop.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/thinking.png` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/thinking.png`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images/young-person-journey.jpg` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images/young-person-journey.jpg`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/images.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/images.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/import_data.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/import_data.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/map.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/map.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/page_setup.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/page_setup.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/reshape_data.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reshape_data.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/response_labels.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/response_labels.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/reuse_text.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/reuse_text.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/score_descriptions.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/score_descriptions.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/static_report.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/static_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 '''
 import base64
 from .images import get_image_path
 from importlib.resources import files
 from markdown import markdown
 import os
 from .reshape_data import get_school_size
-from .reuse_text import reuse_text
+from .reuse_text import reuse_text, caution_comparing
 from .summary_rag import summary_intro, summary_table
 from .explore_results import (
     create_bar_charts,
     create_explore_topic_page,
     create_topic_dict,
     get_chosen_result,
     write_page_title)
@@ -191,15 +191,15 @@
 
     # Using the report (duplicate text with About.py)
     content.append('<h2>How to use this report</h2>')
     content.append(markdown(reuse_text['how_to_use_results']))
 
     # Comparison warning (duplicate text with Explore results.py)
     content.append('<h2>Comparing between schools</h2>')
-    content.append(markdown(reuse_text['caution_comparing']))
+    content.append(markdown(caution_comparing(type='school')))
 
     #####################
     # Table of contents #
     #####################
 
     # Get all of the explore results pages as lines for the table of contents
     explore_results_pages = []
@@ -346,15 +346,15 @@
 
     # Heading
     content.append('''<h1 style='page-break-before:always;'>
                    Introduction</h1>''')
 
     # Using the report (duplicate text with About.py)
     content.append('<h2>How to use this report</h2>')
-    content.append(markdown(reuse_text['caution_comparing']))
+    content.append(markdown(caution_comparing(type='school')))
 
     #####################
     # Table of contents #
     #####################
 
     # Get all of the explore results pages as lines for the table of contents
     explore_results_pages = []
```

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/stylable_container.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/stylable_container.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/summary_rag.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/summary_rag.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/switch_page_button.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/switch_page_button.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_aggregate.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_aggregate.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_demographic.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_demographic.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_responses.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_responses.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/synthesise_scores.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/synthesise_scores.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/topic_labels.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/topic_labels.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard/who_took_part.py` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard/who_took_part.py`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/PKG-INFO` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kailo-beewell-dashboard
-Version: 0.3.1
+Version: 0.3.2
 Summary: Tools to support creation of #BeeWell survey dashboards for Kailo
 Home-page: https://github.com/kailo-beewell/kailo_beewell_dashboard_package
 Author: Amy Heather
 Author-email: a.heather2@exeter.ac.uk
 License: The MIT License (MIT)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 Requires-Dist: sphinx-rtd-theme==2.0.0
 Requires-Dist: myst-parser==2.0.0
 Requires-Dist: sphinx-autoapi==3.0.0
 Requires-Dist: matplotlib==3.8.3
 
 # `kailo-beewell-dashboard`: tools to support creation of #BeeWell survey dashboards for the Kailo project.
 
-[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.1-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.1/)
+[![PyPI package](https://img.shields.io/badge/PyPI_package-0.3.2-2596be.svg)](https://pypi.org/project/kailo-beewell-dashboard/0.3.2/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![ORCID: Amy Heather](https://img.shields.io/badge/ORCID_Amy_Heather-0000--0002--6596--3479-brightgreen)](https://orcid.org/0000-0002-6596-3479)
 
 This package contains functions that are used in the creation of the various #BeeWell survey dashboards for Kailo. They have been compiled into a single package to prevent code duplication between the different repositories.
 
 **Package on PyPI:** https://pypi.org/project/kailo-beewell-dashboard/
 
@@ -50,19 +50,19 @@
 
 `pip install kailo-beewell-dashboard`
 
 ## Citation
 
 If you use this package, please include the following citation
 
-> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.1). https://pypi.org/project/kailo-beewell-dashboard/.
+> Heather, Amy. (2024). kailo-beewell-dashboard: tools to support creation of #BeeWell survey dashboards for the Kailo project (0.3.2). https://pypi.org/project/kailo-beewell-dashboard/.
 
 ```tex
 @software{kailo-beewell-dashboard,
   author = {Heather, Amy},
   title = {kailo-beewell-dashboard},
-  date = {2024-04-09},
-  version = {0.3.1},
+  date = {2024-04-12},
+  version = {0.3.2},
   publisher = {PyPI},
   url = {https://pypi.org/project/kailo-beewell-dashboard/}
 }
 ```
```

### Comparing `kailo-beewell-dashboard-0.3.1/kailo_beewell_dashboard.egg-info/SOURCES.txt` & `kailo-beewell-dashboard-0.3.2/kailo_beewell_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/requirements.txt` & `kailo-beewell-dashboard-0.3.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `kailo-beewell-dashboard-0.3.1/setup.py` & `kailo-beewell-dashboard-0.3.2/setup.py`

 * *Files identical despite different names*

