# Comparing `tmp/m9s_account_batch-7.0.3.tar.gz` & `tmp/m9s_account_batch-7.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_account_batch-7.0.3.tar", last modified: Tue Jan 16 19:47:08 2024, max compression
+gzip compressed data, was "m9s_account_batch-7.0.4.tar", last modified: Fri Apr 12 08:33:54 2024, max compression
```

## Comparing `m9s_account_batch-7.0.3.tar` & `m9s_account_batch-7.0.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.348026 m9s_account_batch-7.0.3/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:03:52.000000 m9s_account_batch-7.0.3/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.344026 m9s_account_batch-7.0.3/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1803 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3408 2024-01-16 19:47:08.348026 m9s_account_batch-7.0.3/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1238 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       42 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      913 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1187 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/account.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    57808 2024-01-16 19:46:58.000000 m9s_account_batch-7.0.3/batch.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14883 2022-03-17 22:33:59.000000 m9s_account_batch-7.0.3/batch.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-16 16:32:23.000000 m9s_account_batch-7.0.3/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.344026 m9s_account_batch-7.0.3/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.344026 m9s_account_batch-7.0.3/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       41 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       42 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6836 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/doc/index_de.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/invoice.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2553 2024-01-16 19:46:58.000000 m9s_account_batch-7.0.3/journal.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3089 2022-02-13 17:27:21.000000 m9s_account_batch-7.0.3/journal.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.336026 m9s_account_batch-7.0.3/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14395 2022-03-10 16:54:42.000000 m9s_account_batch-7.0.3/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.344026 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3408 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2148 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       64 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-22 23:27:41.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      312 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-01-16 19:47:08.000000 m9s_account_batch-7.0.3/m9s_account_batch.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1939 2022-02-03 16:35:35.000000 m9s_account_batch-7.0.3/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3548 2024-01-16 16:32:25.000000 m9s_account_batch-7.0.3/move.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      394 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-16 19:47:08.348026 m9s_account_batch-7.0.3/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4575 2023-12-23 15:33:29.000000 m9s_account_batch-7.0.3/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.340026 m9s_account_batch-7.0.3/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    48332 2022-02-10 15:11:34.000000 m9s_account_batch-7.0.3/tests/scenario_account_batch.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15369 2024-01-16 16:32:25.000000 m9s_account_batch-7.0.3/tests/scenario_account_batch_line_update.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    37005 2022-02-07 10:42:22.000000 m9s_account_batch-7.0.3/tests/scenario_account_batch_tax_cash.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      266 2023-12-14 09:38:06.000000 m9s_account_batch-7.0.3/tests/test_scenario.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1500 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/tests/tools.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.3/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      274 2024-01-16 16:43:09.000000 m9s_account_batch-7.0.3/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 19:47:08.344026 m9s_account_batch-7.0.3/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      314 2020-03-22 22:40:26.000000 m9s_account_batch-7.0.3/view/batch_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      824 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/view/batch_form2.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      502 2021-09-17 06:24:45.000000 m9s_account_batch-7.0.3/view/batch_journal_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      274 2020-03-22 22:40:26.000000 m9s_account_batch-7.0.3/view/batch_journal_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1522 2020-03-22 23:41:19.000000 m9s_account_batch-7.0.3/view/batch_line_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      790 2024-01-16 16:42:55.000000 m9s_account_batch-7.0.3/view/batch_line_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      822 2024-01-16 16:42:55.000000 m9s_account_batch-7.0.3/view/batch_line_tree_editable.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2020-03-22 23:42:18.000000 m9s_account_batch-7.0.3/view/batch_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      696 2020-03-22 23:42:46.000000 m9s_account_batch-7.0.3/view/cancel_batch_lines_ask_problem_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      549 2020-03-22 23:44:31.000000 m9s_account_batch-7.0.3/view/cancel_batch_lines_ask_sure_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      298 2023-12-23 16:13:52.000000 m9s_account_batch-7.0.3/view/move_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      313 2023-12-23 16:12:21.000000 m9s_account_batch-7.0.3/view/move_line_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      260 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/view/move_line_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.3/view/move_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      589 2020-03-22 23:45:14.000000 m9s_account_batch-7.0.3/view/open_batch_journal_ask_form.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:03:52.000000 m9s_account_batch-7.0.4/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1803 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3408 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1238 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       42 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      913 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1187 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/account.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)    57792 2024-04-12 08:33:48.000000 m9s_account_batch-7.0.4/batch.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14883 2022-03-17 22:33:59.000000 m9s_account_batch-7.0.4/batch.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-01-16 16:32:23.000000 m9s_account_batch-7.0.4/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       41 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       42 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6836 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/doc/index_de.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/invoice.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2553 2024-01-16 19:46:58.000000 m9s_account_batch-7.0.4/journal.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3089 2022-02-13 17:27:21.000000 m9s_account_batch-7.0.4/journal.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.527223 m9s_account_batch-7.0.4/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14395 2022-03-10 16:54:42.000000 m9s_account_batch-7.0.4/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3408 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2148 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       64 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-22 23:27:41.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      312 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-12 08:33:54.000000 m9s_account_batch-7.0.4/m9s_account_batch.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1939 2022-02-03 16:35:35.000000 m9s_account_batch-7.0.4/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3548 2024-01-16 16:32:25.000000 m9s_account_batch-7.0.4/move.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      394 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-12 08:33:54.535223 m9s_account_batch-7.0.4/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4575 2023-12-23 15:33:29.000000 m9s_account_batch-7.0.4/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.527223 m9s_account_batch-7.0.4/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    48332 2022-02-10 15:11:34.000000 m9s_account_batch-7.0.4/tests/scenario_account_batch.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15369 2024-01-16 16:32:25.000000 m9s_account_batch-7.0.4/tests/scenario_account_batch_line_update.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    37005 2022-02-07 10:42:22.000000 m9s_account_batch-7.0.4/tests/scenario_account_batch_tax_cash.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      266 2023-12-14 09:38:06.000000 m9s_account_batch-7.0.4/tests/test_scenario.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1500 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/tests/tools.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:56.000000 m9s_account_batch-7.0.4/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      274 2024-01-16 19:47:14.000000 m9s_account_batch-7.0.4/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:33:54.531223 m9s_account_batch-7.0.4/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      314 2020-03-22 22:40:26.000000 m9s_account_batch-7.0.4/view/batch_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      824 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/view/batch_form2.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      502 2021-09-17 06:24:45.000000 m9s_account_batch-7.0.4/view/batch_journal_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      274 2020-03-22 22:40:26.000000 m9s_account_batch-7.0.4/view/batch_journal_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1522 2020-03-22 23:41:19.000000 m9s_account_batch-7.0.4/view/batch_line_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      790 2024-01-16 16:42:55.000000 m9s_account_batch-7.0.4/view/batch_line_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      822 2024-01-16 16:42:55.000000 m9s_account_batch-7.0.4/view/batch_line_tree_editable.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2020-03-22 23:42:18.000000 m9s_account_batch-7.0.4/view/batch_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      696 2020-03-22 23:42:46.000000 m9s_account_batch-7.0.4/view/cancel_batch_lines_ask_problem_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      549 2020-03-22 23:44:31.000000 m9s_account_batch-7.0.4/view/cancel_batch_lines_ask_sure_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      298 2023-12-23 16:13:52.000000 m9s_account_batch-7.0.4/view/move_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      313 2023-12-23 16:12:21.000000 m9s_account_batch-7.0.4/view/move_line_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      260 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/view/move_line_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2018-02-28 18:25:36.000000 m9s_account_batch-7.0.4/view/move_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      589 2020-03-22 23:45:14.000000 m9s_account_batch-7.0.4/view/open_batch_journal_ask_form.xml
```

### Comparing `m9s_account_batch-7.0.3/.drone.yml` & `m9s_account_batch-7.0.4/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/.gitlab-ci.yml` & `m9s_account_batch-7.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/.woodpecker/mail_curl.sh` & `m9s_account_batch-7.0.4/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/.woodpecker/report.yml` & `m9s_account_batch-7.0.4/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/.woodpecker/test.yml` & `m9s_account_batch-7.0.4/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/CHANGELOG` & `m9s_account_batch-7.0.4/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/COPYRIGHT` & `m9s_account_batch-7.0.4/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/INSTALL` & `m9s_account_batch-7.0.4/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/LICENSE` & `m9s_account_batch-7.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/PKG-INFO` & `m9s_account_batch-7.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_account_batch
-Version: 7.0.3
+Version: 7.0.4
 Summary: Tryton Account Batch Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_batch.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_batch-7.0.3/README.md` & `m9s_account_batch-7.0.4/README.md`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/__init__.py` & `m9s_account_batch-7.0.4/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/account.xml` & `m9s_account_batch-7.0.4/account.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/batch.py` & `m9s_account_batch-7.0.4/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,16 +568,16 @@
                 and self.journal):
             self.fiscalyear = fiscalyear_for_date
             self.account = self.batch.journal.account
             self.contra_account = None
         # check if date is valid for the period/fiscalyear
         if context.get('period'):
             period = Period(context['period'])
-            period_for_date = period.find(company_id, date=date,
-                exception=False, test_state=True)
+            period_for_date = period.find(
+                company_id, date=date, test_state=True)
             if period_for_date != period.id:
                 self.date = None
         elif context.get('fiscalyear'):
             if fiscalyear_for_date != context['fiscalyear']:
                 self.date = None
 
     @fields.depends(
```

### Comparing `m9s_account_batch-7.0.3/batch.xml` & `m9s_account_batch-7.0.4/batch.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/doc/index_de.rst` & `m9s_account_batch-7.0.4/doc/index_de.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/journal.py` & `m9s_account_batch-7.0.4/journal.py`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/journal.xml` & `m9s_account_batch-7.0.4/journal.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/locale/de.po` & `m9s_account_batch-7.0.4/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/m9s_account_batch.egg-info/PKG-INFO` & `m9s_account_batch-7.0.4/m9s_account_batch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-account-batch
-Version: 7.0.3
+Version: 7.0.4
 Summary: Tryton Account Batch Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_batch.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_batch-7.0.3/m9s_account_batch.egg-info/SOURCES.txt` & `m9s_account_batch-7.0.4/m9s_account_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/message.xml` & `m9s_account_batch-7.0.4/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/move.py` & `m9s_account_batch-7.0.4/move.py`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/setup.py` & `m9s_account_batch-7.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/tests/scenario_account_batch.rst` & `m9s_account_batch-7.0.4/tests/scenario_account_batch.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/tests/scenario_account_batch_line_update.rst` & `m9s_account_batch-7.0.4/tests/scenario_account_batch_line_update.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/tests/scenario_account_batch_tax_cash.rst` & `m9s_account_batch-7.0.4/tests/scenario_account_batch_tax_cash.rst`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/tests/tools.py` & `m9s_account_batch-7.0.4/tests/tools.py`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/tox.ini` & `m9s_account_batch-7.0.4/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/batch_form2.xml` & `m9s_account_batch-7.0.4/view/batch_form2.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/batch_line_form.xml` & `m9s_account_batch-7.0.4/view/batch_line_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/batch_line_tree.xml` & `m9s_account_batch-7.0.4/view/batch_line_tree.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/batch_line_tree_editable.xml` & `m9s_account_batch-7.0.4/view/batch_line_tree_editable.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/cancel_batch_lines_ask_problem_form.xml` & `m9s_account_batch-7.0.4/view/cancel_batch_lines_ask_problem_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/cancel_batch_lines_ask_sure_form.xml` & `m9s_account_batch-7.0.4/view/cancel_batch_lines_ask_sure_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_batch-7.0.3/view/open_batch_journal_ask_form.xml` & `m9s_account_batch-7.0.4/view/open_batch_journal_ask_form.xml`

 * *Files identical despite different names*

