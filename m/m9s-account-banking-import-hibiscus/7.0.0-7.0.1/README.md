# Comparing `tmp/m9s_account_banking_import_hibiscus-7.0.0.tar.gz` & `tmp/m9s_account_banking_import_hibiscus-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_account_banking_import_hibiscus-7.0.0.tar", last modified: Tue Jan 16 16:57:21 2024, max compression
+gzip compressed data, was "m9s_account_banking_import_hibiscus-7.0.1.tar", last modified: Fri Apr 12 08:35:30 2024, max compression
```

## Comparing `m9s_account_banking_import_hibiscus-7.0.0.tar` & `m9s_account_banking_import_hibiscus-7.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      101 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:03:51.000000 m9s_account_banking_import_hibiscus-7.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2018-02-28 18:25:36.000000 m9s_account_banking_import_hibiscus-7.0.0/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3606 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1364 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       78 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      446 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8030 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/banking_import.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      522 2020-03-26 15:09:07.000000 m9s_account_banking_import_hibiscus-7.0.0/banking_import.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       78 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.681083 m9s_account_banking_import_hibiscus-7.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2311 2022-04-08 10:03:43.000000 m9s_account_banking_import_hibiscus-7.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3606 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1031 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      100 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-26 14:54:42.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-01-16 16:57:21.000000 m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1170 2022-02-13 18:00:08.000000 m9s_account_banking_import_hibiscus-7.0.0/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4627 2024-01-16 16:55:52.000000 m9s_account_banking_import_hibiscus-7.0.0/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      348 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      103 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-01-16 16:57:21.685083 m9s_account_banking_import_hibiscus-7.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      384 2018-02-28 18:25:36.000000 m9s_account_banking_import_hibiscus-7.0.0/view/bank_import_form.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.694570 m9s_account_banking_import_hibiscus-7.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      101 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:03:51.000000 m9s_account_banking_import_hibiscus-7.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.690570 m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2018-02-28 18:25:36.000000 m9s_account_banking_import_hibiscus-7.0.1/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3606 2024-04-12 08:35:30.694570 m9s_account_banking_import_hibiscus-7.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1364 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       78 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      446 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/__init__.py
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     8040 2024-04-12 08:35:25.000000 m9s_account_banking_import_hibiscus-7.0.1/banking_import.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      522 2020-03-26 15:09:07.000000 m9s_account_banking_import_hibiscus-7.0.1/banking_import.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.690570 m9s_account_banking_import_hibiscus-7.0.1/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.690570 m9s_account_banking_import_hibiscus-7.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       78 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.686570 m9s_account_banking_import_hibiscus-7.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2311 2022-04-08 10:03:43.000000 m9s_account_banking_import_hibiscus-7.0.1/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.694570 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3606 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1031 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      100 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-26 14:54:42.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-04-12 08:35:30.000000 m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1170 2022-02-13 18:00:08.000000 m9s_account_banking_import_hibiscus-7.0.1/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-04-12 08:35:30.694570 m9s_account_banking_import_hibiscus-7.0.1/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4627 2024-01-16 16:55:52.000000 m9s_account_banking_import_hibiscus-7.0.1/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.690570 m9s_account_banking_import_hibiscus-7.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      348 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:56.000000 m9s_account_banking_import_hibiscus-7.0.1/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      103 2024-01-16 16:57:27.000000 m9s_account_banking_import_hibiscus-7.0.1/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-04-12 08:35:30.690570 m9s_account_banking_import_hibiscus-7.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      384 2018-02-28 18:25:36.000000 m9s_account_banking_import_hibiscus-7.0.1/view/bank_import_form.xml
```

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/.drone.yml` & `m9s_account_banking_import_hibiscus-7.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/.gitlab-ci.yml` & `m9s_account_banking_import_hibiscus-7.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/mail_curl.sh` & `m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/report.yml` & `m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/.woodpecker/test.yml` & `m9s_account_banking_import_hibiscus-7.0.1/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/COPYRIGHT` & `m9s_account_banking_import_hibiscus-7.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/INSTALL` & `m9s_account_banking_import_hibiscus-7.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/LICENSE` & `m9s_account_banking_import_hibiscus-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/PKG-INFO` & `m9s_account_banking_import_hibiscus-7.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_account_banking_import_hibiscus
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Account Banking Import Hibiscus Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_banking_import_hibiscus.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/README.md` & `m9s_account_banking_import_hibiscus-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/banking_import.py` & `m9s_account_banking_import_hibiscus-7.0.1/banking_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                     'amount': Decimal(transaction['betrag']),
                     'purpose': purpose,
                     # The PayPal plugin provides sometimes weird balances
                     # exceeding the digits of the field
                     'balance': self.journal.currency.round(
                         Decimal(transaction['saldo'])),
                     'kind': transaction['art'],
-                    'customer_ref': transaction['customerref'],
+                    'customer_ref': transaction.get('customerref', None),
                     'code': transaction.get('gvcode', None),
                     'addkey': transaction.get('addkey', None),
                     'primanota': transaction.get('primanota', None),
                     'hibiscus_id': transaction['id'],
                     }
                 lines.append(line)
         if lines:
```

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/banking_import.xml` & `m9s_account_banking_import_hibiscus-7.0.1/banking_import.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/locale/de.po` & `m9s_account_banking_import_hibiscus-7.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/PKG-INFO` & `m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-account-banking-import-hibiscus
-Version: 7.0.0
+Version: 7.0.1
 Summary: Tryton Account Banking Import Hibiscus Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/account_banking_import_hibiscus.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/m9s_account_banking_import_hibiscus.egg-info/SOURCES.txt` & `m9s_account_banking_import_hibiscus-7.0.1/m9s_account_banking_import_hibiscus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/message.xml` & `m9s_account_banking_import_hibiscus-7.0.1/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/setup.py` & `m9s_account_banking_import_hibiscus-7.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_account_banking_import_hibiscus-7.0.0/tox.ini` & `m9s_account_banking_import_hibiscus-7.0.1/tox.ini`

 * *Files identical despite different names*

