# Comparing `tmp/djaodjin-pages-0.7.1.tar.gz` & `tmp/djaodjin-pages-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-pages-0.7.1.tar", last modified: Thu Jan 25 20:31:16 2024, max compression
+gzip compressed data, was "djaodjin-pages-0.8.0.tar", last modified: Fri Apr 12 01:22:33 2024, max compression
```

## Comparing `djaodjin-pages-0.7.1.tar` & `djaodjin-pages-0.8.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.941866 djaodjin-pages-0.7.1/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     2594 2024-01-25 20:31:16.941668 djaodjin-pages-0.7.1/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1503 2024-01-19 00:23:59.000000 djaodjin-pages-0.7.1/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.941429 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     2594 2024-01-25 20:31:16.000000 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1352 2024-01-25 20:31:16.000000 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2024-01-25 20:31:16.000000 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)      205 2024-01-25 20:31:16.000000 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        6 2024-01-25 20:31:16.000000 djaodjin-pages-0.7.1/djaodjin_pages.egg-info/top_level.txt
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.932841 djaodjin-pages-0.7.1/pages/
--rw-r--r--   0 smirolo    (501) staff       (20)     1434 2024-01-25 20:30:12.000000 djaodjin-pages-0.7.1/pages/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1520 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.934894 djaodjin-pages-0.7.1/pages/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)    10870 2024-01-15 20:54:10.000000 djaodjin-pages-0.7.1/pages/api/assets.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23538 2024-01-18 22:22:40.000000 djaodjin-pages-0.7.1/pages/api/elements.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8594 2024-01-18 23:53:36.000000 djaodjin-pages-0.7.1/pages/api/progress.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7465 2024-01-16 01:04:17.000000 djaodjin-pages-0.7.1/pages/api/reactions.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8239 2024-01-25 20:18:33.000000 djaodjin-pages-0.7.1/pages/api/relationship.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12276 2024-01-17 16:42:03.000000 djaodjin-pages-0.7.1/pages/api/sequences.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6909 2024-01-18 23:34:04.000000 djaodjin-pages-0.7.1/pages/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2196 2024-01-03 17:59:19.000000 djaodjin-pages-0.7.1/pages/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3040 2024-01-15 20:34:33.000000 djaodjin-pages-0.7.1/pages/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12680 2024-01-17 19:31:22.000000 djaodjin-pages-0.7.1/pages/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    28608 2024-01-17 19:31:15.000000 djaodjin-pages-0.7.1/pages/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)    13842 2024-01-18 23:36:59.000000 djaodjin-pages-0.7.1/pages/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4449 2024-01-18 22:04:24.000000 djaodjin-pages-0.7.1/pages/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1545 2022-08-20 02:39:53.000000 djaodjin-pages-0.7.1/pages/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.927963 djaodjin-pages-0.7.1/pages/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.935634 djaodjin-pages-0.7.1/pages/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    23744 2024-01-02 18:07:13.000000 djaodjin-pages-0.7.1/pages/static/js/djaodjin-pages-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)    52445 2023-08-03 00:38:17.000000 djaodjin-pages-0.7.1/pages/static/js/djaodjin-resources-vue.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.928079 djaodjin-pages-0.7.1/pages/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.937274 djaodjin-pages-0.7.1/pages/templates/pages/
--rw-r--r--   0 smirolo    (501) staff       (20)      705 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/templates/pages/_comments.html
--rw-r--r--   0 smirolo    (501) staff       (20)      600 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/templates/pages/_follow_vote.html
--rw-r--r--   0 smirolo    (501) staff       (20)      482 2024-01-02 18:07:13.000000 djaodjin-pages-0.7.1/pages/templates/pages/certificate.html
--rw-r--r--   0 smirolo    (501) staff       (20)       33 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/templates/pages/editables.html
--rw-r--r--   0 smirolo    (501) staff       (20)      612 2023-12-05 17:49:14.000000 djaodjin-pages-0.7.1/pages/templates/pages/element.html
--rw-r--r--   0 smirolo    (501) staff       (20)      378 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/templates/pages/index.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.937513 djaodjin-pages-0.7.1/pages/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3301 2023-12-05 17:49:14.000000 djaodjin-pages-0.7.1/pages/templatetags/pages_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.937749 djaodjin-pages-0.7.1/pages/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1489 2024-01-16 00:11:35.000000 djaodjin-pages-0.7.1/pages/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.939554 djaodjin-pages-0.7.1/pages/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     2069 2024-01-15 19:37:31.000000 djaodjin-pages-0.7.1/pages/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1664 2024-01-02 18:07:13.000000 djaodjin-pages-0.7.1/pages/urls/api/assets.py
--rw-r--r--   0 smirolo    (501) staff       (20)     3272 2024-01-25 18:50:00.000000 djaodjin-pages-0.7.1/pages/urls/api/editables.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1845 2024-01-17 19:18:04.000000 djaodjin-pages-0.7.1/pages/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1838 2024-01-19 00:06:00.000000 djaodjin-pages-0.7.1/pages/urls/api/progress.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2088 2024-01-16 20:13:53.000000 djaodjin-pages-0.7.1/pages/urls/api/readers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1787 2024-01-19 02:42:55.000000 djaodjin-pages-0.7.1/pages/urls/api/sequences.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.940509 djaodjin-pages-0.7.1/pages/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1577 2024-01-17 17:20:33.000000 djaodjin-pages-0.7.1/pages/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1689 2022-08-20 02:37:19.000000 djaodjin-pages-0.7.1/pages/urls/views/editables.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1587 2024-01-16 17:20:27.000000 djaodjin-pages-0.7.1/pages/urls/views/elements.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1911 2024-01-16 17:30:26.000000 djaodjin-pages-0.7.1/pages/urls/views/sequences.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2795 2022-08-20 02:26:11.000000 djaodjin-pages-0.7.1/pages/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-01-25 20:31:16.941129 djaodjin-pages-0.7.1/pages/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1776 2022-07-26 19:09:35.000000 djaodjin-pages-0.7.1/pages/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9086 2024-01-16 17:22:23.000000 djaodjin-pages-0.7.1/pages/views/elements.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6773 2024-01-18 23:35:55.000000 djaodjin-pages-0.7.1/pages/views/sequences.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1469 2024-01-18 21:35:11.000000 djaodjin-pages-0.7.1/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       38 2024-01-25 20:31:16.941901 djaodjin-pages-0.7.1/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-08-13 01:28:41.000000 djaodjin-pages-0.7.1/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.748432 djaodjin-pages-0.8.0/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     2709 2024-04-12 01:22:33.748223 djaodjin-pages-0.8.0/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1618 2024-04-12 00:18:40.000000 djaodjin-pages-0.8.0/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.747966 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2709 2024-04-12 01:22:33.000000 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1352 2024-04-12 01:22:33.000000 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2024-04-12 01:22:33.000000 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)      205 2024-04-12 01:22:33.000000 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        6 2024-04-12 01:22:33.000000 djaodjin-pages-0.8.0/djaodjin_pages.egg-info/top_level.txt
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.739574 djaodjin-pages-0.8.0/pages/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1434 2024-04-12 00:32:39.000000 djaodjin-pages-0.8.0/pages/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1520 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/pages/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.741260 djaodjin-pages-0.8.0/pages/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/pages/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11226 2024-02-28 04:45:05.000000 djaodjin-pages-0.8.0/pages/api/assets.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    24251 2024-04-12 00:14:04.000000 djaodjin-pages-0.8.0/pages/api/elements.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8594 2024-03-13 21:25:43.000000 djaodjin-pages-0.8.0/pages/api/progress.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8466 2024-04-11 23:47:40.000000 djaodjin-pages-0.8.0/pages/api/reactions.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8110 2024-04-11 23:47:02.000000 djaodjin-pages-0.8.0/pages/api/relationship.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12276 2024-02-28 04:33:08.000000 djaodjin-pages-0.8.0/pages/api/sequences.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6909 2024-01-18 23:34:04.000000 djaodjin-pages-0.8.0/pages/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2196 2024-01-03 17:59:19.000000 djaodjin-pages-0.8.0/pages/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3040 2024-01-15 20:34:33.000000 djaodjin-pages-0.8.0/pages/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12680 2024-02-28 04:33:08.000000 djaodjin-pages-0.8.0/pages/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    29274 2024-04-12 01:07:41.000000 djaodjin-pages-0.8.0/pages/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    15539 2024-04-12 00:56:27.000000 djaodjin-pages-0.8.0/pages/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4449 2024-01-18 22:04:24.000000 djaodjin-pages-0.8.0/pages/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1545 2022-08-20 02:39:53.000000 djaodjin-pages-0.8.0/pages/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.734834 djaodjin-pages-0.8.0/pages/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.741870 djaodjin-pages-0.8.0/pages/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    24175 2024-04-11 23:42:48.000000 djaodjin-pages-0.8.0/pages/static/js/djaodjin-pages-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    54992 2024-04-11 23:42:48.000000 djaodjin-pages-0.8.0/pages/static/js/djaodjin-resources-vue.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.734949 djaodjin-pages-0.8.0/pages/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.743552 djaodjin-pages-0.8.0/pages/templates/pages/
+-rw-r--r--   0 smirolo    (501) staff       (20)      741 2024-04-12 00:07:19.000000 djaodjin-pages-0.8.0/pages/templates/pages/_comments.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      680 2024-04-12 00:05:07.000000 djaodjin-pages-0.8.0/pages/templates/pages/_follow_vote.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      482 2024-01-02 18:07:13.000000 djaodjin-pages-0.8.0/pages/templates/pages/certificate.html
+-rw-r--r--   0 smirolo    (501) staff       (20)       33 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/pages/templates/pages/editables.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      618 2024-04-11 23:42:48.000000 djaodjin-pages-0.8.0/pages/templates/pages/element.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      551 2024-04-11 23:58:47.000000 djaodjin-pages-0.8.0/pages/templates/pages/index.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.743838 djaodjin-pages-0.8.0/pages/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-pages-0.8.0/pages/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3301 2023-12-05 17:49:14.000000 djaodjin-pages-0.8.0/pages/templatetags/pages_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.744073 djaodjin-pages-0.8.0/pages/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1489 2024-01-16 00:11:35.000000 djaodjin-pages-0.8.0/pages/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.745817 djaodjin-pages-0.8.0/pages/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     2069 2024-01-15 19:37:31.000000 djaodjin-pages-0.8.0/pages/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1664 2024-01-02 18:07:13.000000 djaodjin-pages-0.8.0/pages/urls/api/assets.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     3272 2024-02-28 04:33:08.000000 djaodjin-pages-0.8.0/pages/urls/api/editables.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1845 2024-01-17 19:18:04.000000 djaodjin-pages-0.8.0/pages/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1838 2024-01-19 00:06:00.000000 djaodjin-pages-0.8.0/pages/urls/api/progress.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2220 2024-04-11 23:46:28.000000 djaodjin-pages-0.8.0/pages/urls/api/readers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1787 2024-02-28 04:33:08.000000 djaodjin-pages-0.8.0/pages/urls/api/sequences.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.746832 djaodjin-pages-0.8.0/pages/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1577 2024-01-17 17:20:33.000000 djaodjin-pages-0.8.0/pages/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1689 2022-08-20 02:37:19.000000 djaodjin-pages-0.8.0/pages/urls/views/editables.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1587 2024-01-16 17:20:27.000000 djaodjin-pages-0.8.0/pages/urls/views/elements.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1911 2024-01-16 17:30:26.000000 djaodjin-pages-0.8.0/pages/urls/views/sequences.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2795 2022-08-20 02:26:11.000000 djaodjin-pages-0.8.0/pages/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2024-04-12 01:22:33.747582 djaodjin-pages-0.8.0/pages/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1775 2024-04-11 23:41:48.000000 djaodjin-pages-0.8.0/pages/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9086 2024-04-10 22:28:03.000000 djaodjin-pages-0.8.0/pages/views/elements.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6773 2024-02-28 04:33:08.000000 djaodjin-pages-0.8.0/pages/views/sequences.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1469 2024-01-18 21:35:11.000000 djaodjin-pages-0.8.0/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       38 2024-04-12 01:22:33.748472 djaodjin-pages-0.8.0/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-08-13 01:28:41.000000 djaodjin-pages-0.8.0/setup.py
```

### Comparing `djaodjin-pages-0.7.1/LICENSE.txt` & `djaodjin-pages-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/PKG-INFO` & `djaodjin-pages-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-pages
-Version: 0.7.1
+Version: 0.8.0
 Summary: Django application for practices-based content
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-pages
 Project-URL: documentation, https://djaodjin-pages.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-pages/changelog
@@ -66,18 +66,19 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.7.0
+0.7.2
 
-  * generates usable OpenAPI 3 schema
-  * adds sequences and user progress through a sequence
-  * imports content of PageElement as a .docx
+  * loads commenter picture/name from profile API
+  * makes API endpoint with or without account slug depending on URL pattern
+  * handles updates to django-storages>=1.14 properly
+  * newsfeed API for updates to PageElement a user follows (experimental)
 
 [previous release notes](changelog)
 
 Version 0.4.3 is the last version that contains the HTML templates
 online editor. This functionality was moved to [djaodjin-extended-templates](https://github.com/djaodjin/djaodjin-extended-templates/)
 as of version 0.5.0.
```

### Comparing `djaodjin-pages-0.7.1/README.md` & `djaodjin-pages-0.8.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -37,18 +37,19 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.7.0
+0.7.2
 
-  * generates usable OpenAPI 3 schema
-  * adds sequences and user progress through a sequence
-  * imports content of PageElement as a .docx
+  * loads commenter picture/name from profile API
+  * makes API endpoint with or without account slug depending on URL pattern
+  * handles updates to django-storages>=1.14 properly
+  * newsfeed API for updates to PageElement a user follows (experimental)
 
 [previous release notes](changelog)
 
 Version 0.4.3 is the last version that contains the HTML templates
 online editor. This functionality was moved to [djaodjin-extended-templates](https://github.com/djaodjin/djaodjin-extended-templates/)
 as of version 0.5.0.
```

### Comparing `djaodjin-pages-0.7.1/djaodjin_pages.egg-info/PKG-INFO` & `djaodjin-pages-0.8.0/djaodjin_pages.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-pages
-Version: 0.7.1
+Version: 0.8.0
 Summary: Django application for practices-based content
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-pages
 Project-URL: documentation, https://djaodjin-pages.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-pages/changelog
@@ -66,18 +66,19 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.7.0
+0.7.2
 
-  * generates usable OpenAPI 3 schema
-  * adds sequences and user progress through a sequence
-  * imports content of PageElement as a .docx
+  * loads commenter picture/name from profile API
+  * makes API endpoint with or without account slug depending on URL pattern
+  * handles updates to django-storages>=1.14 properly
+  * newsfeed API for updates to PageElement a user follows (experimental)
 
 [previous release notes](changelog)
 
 Version 0.4.3 is the last version that contains the HTML templates
 online editor. This functionality was moved to [djaodjin-extended-templates](https://github.com/djaodjin/djaodjin-extended-templates/)
 as of version 0.5.0.
```

### Comparing `djaodjin-pages-0.7.1/djaodjin_pages.egg-info/SOURCES.txt` & `djaodjin-pages-0.8.0/djaodjin_pages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/__init__.py` & `djaodjin-pages-0.8.0/pages/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the pages django app.
 """
 
-__version__ = '0.7.1'
+__version__ = '0.8.0'
```

### Comparing `djaodjin-pages-0.7.1/pages/admin.py` & `djaodjin-pages-0.8.0/pages/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/api/assets.py` & `djaodjin-pages-0.8.0/pages/api/assets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, Djaodjin Inc.
+# Copyright (c) 2024, Djaodjin Inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -32,15 +32,16 @@
 from django.utils.module_loading import import_string
 from rest_framework import parsers, status
 from rest_framework.exceptions import ValidationError
 from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response as HttpResponse
 
 from .. import settings
-from ..compat import force_str, gettext_lazy as _, reverse, urljoin, urlparse
+from ..compat import (NoReverseMatch, force_str, gettext_lazy as _, reverse,
+    urljoin, urlparse)
 from ..mixins import AccountMixin
 from ..serializers import AssetSerializer
 
 
 LOGGER = logging.getLogger(__name__)
 
 URL_PATH_SEP = '/'
@@ -168,15 +169,15 @@
 
         s3_client = boto3.client('s3')
         data = s3_client.get_object(Bucket=bucket_name, Key=src_key_name)
         uploaded_file = data['Body']
         if prefix.startswith(media_prefix):
             prefix = prefix[len(media_prefix) + 1:]
         storage_key_name = "%s%s%s" % (prefix,
-                                       hashlib.sha256(uploaded_file.read()).hexdigest(), ext)
+            hashlib.sha256(uploaded_file.read()).hexdigest(), ext)
 
         dst_key_name = "%s/%s" % (media_prefix, storage_key_name)
         LOGGER.info("S3 bucket %s: copy %s to %s",
                     bucket_name, src_key_name, dst_key_name)
         storage = get_default_storage(request)
         if is_public_asset:
             extra_args = {'ACL': "public-read"}
@@ -224,16 +225,20 @@
         raise ValidationError({'detail':
            _("Either 'location' or 'file' must be specified.")})
 
     if not is_public_asset:
         path = urlparse(location).path.lstrip(URL_PATH_SEP)
         if path.startswith(media_prefix):
             path = path[len(media_prefix):].lstrip(URL_PATH_SEP)
-        location = request.build_absolute_uri(
-            reverse('pages_api_asset', args=(path,)))
+        try:
+            location = request.build_absolute_uri(
+                reverse('pages_api_asset', args=(account, path,)))
+        except NoReverseMatch:
+            location = request.build_absolute_uri(
+                reverse('pages_api_asset', args=(path,)))
 
     return ({
         'location': location,
         'updated_at': datetime_or_now()},
         response_status)
 
 
@@ -247,15 +252,18 @@
         return storage
     return get_default_storage_base(request, **kwargs)
 
 
 def get_default_storage_base(request, public=False, **kwargs):
     # default implementation
     storage_class = get_storage_class()
-    if 's3boto' in storage_class.__name__.lower():
+    if storage_class.__name__.endswith('3Storage'):
+        # Hacky way to test for `storages.backends.s3.S3Storage`
+        # and `storages.backends.s3boto3.S3Boto3Storage` without importing
+        # the optional package 'django-storages'.
         storage_kwargs = {}
         storage_kwargs.update(**kwargs)
         if public:
             storage_kwargs.update({'default_acl': 'public-read'})
         bucket_name = _get_bucket_name()
         location = _get_media_prefix()
         LOGGER.debug("create %s(bucket_name='%s', location='%s', %s)",
```

### Comparing `djaodjin-pages-0.7.1/pages/api/elements.py` & `djaodjin-pages-0.8.0/pages/api/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import base64
 import logging
 import re
 from io import BytesIO
 
 import mammoth, requests
 from bs4 import BeautifulSoup
+from deployutils.helpers import datetime_or_now
 from django.core.files.uploadedfile import (SimpleUploadedFile,
     TemporaryUploadedFile)
 from django.db import transaction
 from django.db.models import Max, Q
 from django.http import Http404, QueryDict
 from markdownify import markdownify as md
 from rest_framework import (generics, response as api_response,
@@ -39,19 +40,19 @@
 from rest_framework.exceptions import ValidationError
 from rest_framework.filters import OrderingFilter, SearchFilter
 from rest_framework.mixins import CreateModelMixin
 from rest_framework.request import Request
 
 from .. import settings
 from ..docs import extend_schema
-from ..compat import reverse, gettext_lazy as _
+from ..compat import is_authenticated, reverse, gettext_lazy as _
 from ..helpers import ContentCut, get_extra
 from ..mixins import AccountMixin, PageElementMixin, TrailMixin
 from ..models import (PageElement, RelationShip, build_content_tree,
-    flatten_content_tree)
+    flatten_content_tree, Follow)
 from ..serializers import (AssetSerializer, NodeElementSerializer,
     NodeElementCreateSerializer, PageElementSerializer,
     PageElementTagSerializer)
 from ..utils import validate_title
 from .assets import process_upload
 
 LOGGER = logging.getLogger(__name__)
@@ -98,16 +99,27 @@
               "public",
               "scorecard"
             ]
           }
           ]
         }
     """
-    serializer_class = PageElementSerializer
     queryset = PageElement.objects.all()
+    serializer_class = PageElementSerializer
+
+    search_fields = (
+        'title',
+        'extra'
+    )
+    ordering_fields = (
+        ('title', 'title'),
+    )
+    ordering = ('title',)
+
+    filter_backends = (SearchFilter, OrderingFilter,)
 
     @property
     def visibility(self):
         return None
 
     @property
     def owners(self):
@@ -286,17 +298,32 @@
         }
     """
     serializer_class = PageElementSerializer
 
     def get_object(self):
         return self.element
 
+    def get(self, request, *args, **kwargs):
+        if is_authenticated(self.request):
+            # Marking the last time the PageElement was read by a user
+            # following it
+            try:
+                follow_obj = Follow.objects.get(
+                    user=self.request.user,
+                    element=self.element)
+                follow_obj.last_read_at = datetime_or_now()
+                follow_obj.save()
+            except Follow.DoesNotExist:
+                pass
+
+        return self.retrieve(request, *args, **kwargs)
 
-class PageElementEditableListAPIView(AccountMixin, TrailMixin,
-                                     generics.ListCreateAPIView):
+
+class PageElementEditableListAPIView(AccountMixin, CreateModelMixin,
+                                     PageElementAPIView):
     """
     Lists editable page elements
 
     This API endpoint lists page elements that are owned and thus editable
     by an account.
 
     **Tags**: editors
@@ -357,25 +384,14 @@
                     "avg_value": 2
                 }
             ]
         }
     """
     serializer_class = NodeElementSerializer
 
-    search_fields = (
-        'title',
-        'extra'
-    )
-    ordering_fields = (
-        ('title', 'title'),
-    )
-    ordering = ('title',)
-
-    filter_backends = (SearchFilter, OrderingFilter,)
-
     def get_serializer_class(self):
         if self.request.method.lower() == 'post':
             return NodeElementCreateSerializer
         return super(PageElementEditableListAPIView,
             self).get_serializer_class()
 
 
@@ -395,14 +411,17 @@
                 queryset = queryset.filter(
                     Q(extra__icontains=search_string)
                     | Q(title__icontains=search_string))
         except ValidationError:
             pass
         return queryset
 
+    def get(self, request, *args, **kwargs): # Overrides the overide in PageElementAPIView
+        return self.list(request, *args, **kwargs)
+
     @extend_schema(operation_id='editables_content_create')
     def post(self, request, *args, **kwargs):
         """
         Creates a page element
 
         **Tags: editors
 
@@ -425,16 +444,15 @@
             {
                 "slug": "boxes-enclosures",
                 "title": "Boxes enclosures"
             }
 
         """
         #pylint:disable=useless-super-delegation
-        return super(PageElementEditableListAPIView, self).create(
-            request, *args, **kwargs)
+        return self.create(request, *args, **kwargs)
 
     def perform_create(self, serializer):
         serializer.save(account=self.account)
 
 
 class PageElementEditableDetail(AccountMixin, TrailMixin, CreateModelMixin,
                                 generics.RetrieveUpdateDestroyAPIView):
```

### Comparing `djaodjin-pages-0.7.1/pages/api/progress.py` & `djaodjin-pages-0.8.0/pages/api/progress.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/api/reactions.py` & `djaodjin-pages-0.8.0/pages/api/reactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,23 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 from __future__ import unicode_literals
 
 from deployutils.helpers import datetime_or_now
 from django.core.exceptions import PermissionDenied
 from django.db import transaction
+from django.db.models import Subquery, OuterRef, F, Q, Count
 from rest_framework import generics
 
 from .. import signals
 from ..compat import is_authenticated
-from ..mixins import PageElementMixin
-from ..models import Comment, Follow, Vote
-from ..serializers import CommentSerializer, PageElementSerializer
+from ..mixins import PageElementMixin, UserMixin
+from ..models import Comment, Follow, PageElement, Vote
+from ..serializers import (CommentSerializer, PageElementSerializer,
+        PageElementUpdateSerializer)
 
 
 class FollowAPIView(PageElementMixin, generics.CreateAPIView):
     """
     Follows a page element
 
     The authenticated user making the request will receive notification
@@ -264,7 +266,34 @@
             serializer.save(created_at=datetime_or_now(),
                 element=self.element, user=self.request.user)
             # Subscribe the commenting user to this element
             Follow.objects.subscribe(self.element, user=self.request.user)
 
         signals.comment_was_posted.send(
             sender=__name__, comment=serializer.instance, request=self.request)
+
+
+class NewsFeedListAPIView(UserMixin, generics.ListAPIView):
+    serializer_class = PageElementUpdateSerializer
+
+    def get_queryset(self):
+        user = self.user
+
+        queryset = PageElement.objects.followed_by(user).annotate(
+            last_read_at=Subquery(
+                Follow.objects.filter(
+                    user=user,
+                    element=OuterRef("pk")
+                    ).values("last_read_at")[:1]),
+            nb_comments_since_last_read=Count(
+                "comments",
+                filter=Q(comments__created_at__gte=F("last_read_at")))
+            ).exclude(
+                (
+                    (Q(text_updated_at__isnull=True) |
+                     Q(text_updated_at__lte=F("last_read_at")))
+                    &
+                    Q(nb_comments_since_last_read__lte=0)
+                )
+            )
+
+        return queryset
```

### Comparing `djaodjin-pages-0.7.1/pages/api/relationship.py` & `djaodjin-pages-0.8.0/pages/api/relationship.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,22 +23,20 @@
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
 from copy import deepcopy
 
 from django.db import transaction
 from django.db.models import Max
-from rest_framework import generics, status
+from rest_framework import generics
 from rest_framework.exceptions import ValidationError
-from rest_framework.mixins import DestroyModelMixin
-from rest_framework.response import Response
 
 from ..mixins import TrailMixin
 from ..models import RelationShip
-from ..serializers import EdgeCreateSerializer, RelationShipSerializer
+from ..serializers import EdgeCreateSerializer
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class EdgesUpdateAPIView(TrailMixin, generics.CreateAPIView):
```

### Comparing `djaodjin-pages-0.7.1/pages/api/sequences.py` & `djaodjin-pages-0.8.0/pages/api/sequences.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/compat.py` & `djaodjin-pages-0.8.0/pages/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/docs.py` & `djaodjin-pages-0.8.0/pages/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/helpers.py` & `djaodjin-pages-0.8.0/pages/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/mixins.py` & `djaodjin-pages-0.8.0/pages/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/models.py` & `djaodjin-pages-0.8.0/pages/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import unicode_literals
 
 import datetime, json, logging, random
 from collections import OrderedDict
+from deployutils.helpers import datetime_or_now
 
 from django.contrib.auth import get_user_model
 from django.db import IntegrityError, models, transaction
 from django.db.models import Max, Q
 from django.template.defaultfilters import slugify
 from rest_framework.exceptions import ValidationError
 
@@ -158,14 +159,18 @@
 
     def get_leafs(self):
         return self.all().extra(where=[
             '(SELECT COUNT(*) FROM pages_relationship'\
             ' WHERE pages_relationship.orig_element_id = pages_pageelement.id)'\
             ' = 0'])
 
+    @staticmethod
+    def followed_by(user):
+        return PageElement.objects.filter(followers__user=user)
+
 
 @python_2_unicode_compatible
 class PageElement(models.Model):
     """
     Elements of an editable HTML page.
     """
     objects = PageElementManager()
@@ -189,14 +194,16 @@
     picture = models.URLField(_("URL to a icon picture"), max_length=2083,
         null=True, blank=True, help_text=_("Icon picture"))
     reading_time = models.DurationField(null=True,
         default=datetime.timedelta,  # stored in microseconds
         help_text=_("Reading time of the material (in hh:mm:ss)"))
     lang = models.CharField(default=settings.LANGUAGE_CODE, max_length=8,
         help_text=_("Language the material is written in"))
+    text_updated_at = models.DateTimeField(blank=True, null=True,
+        help_text=_("Last updated at date for the text field"))
     extra = get_extra_field_class()(null=True, blank=True)
     relationships = models.ManyToManyField("self",
         related_name='related_to', through='RelationShip', symmetrical=False)
 
     def __str__(self):
         return self.slug
 
@@ -273,16 +280,23 @@
             to_element__tag=tag, to_element__orig_element=self)
 
     def get_related_to(self, tag):
         return self.related_to.filter(
             from_element__tag=tag,
             from_element__dest_element=self)
 
+    def __init__(self, *args, **kwargs):
+        super(PageElement, self).__init__(*args, **kwargs)
+        self.__original_text = self.text
+
     def save(self, force_insert=False, force_update=False,
              using=None, update_fields=None):
+        if self.__original_text != self.text:
+            self.text_updated_at = datetime_or_now()
+
         if self.slug: # serializer will set created slug to '' instead of None.
             return super(PageElement, self).save(
                 force_insert=force_insert, force_update=force_update,
                 using=using, update_fields=update_fields)
         max_length = self._meta.get_field('slug').max_length
         slug_base = slugify(self.title)
         if not slug_base:
@@ -352,28 +366,29 @@
         """
         try:
             self.get(user=user, element=element).delete()
         except models.ObjectDoesNotExist:
             pass
 
 
-
 @python_2_unicode_compatible
 class Follow(models.Model):
     """
     A relationship intended for a User to follow comments on a Element.
     """
     objects = FollowManager()
 
     created_at = models.DateTimeField(editable=False, auto_now_add=True,
         help_text=_("Date/time the follow was created (in ISO format)"))
     user = models.ForeignKey(settings.AUTH_USER_MODEL, db_column='user_id',
          related_name='follows', on_delete=models.CASCADE)
     element = models.ForeignKey(PageElement,
         related_name='followers', on_delete=models.CASCADE)
+    last_read_at = models.DateTimeField(default=datetime_or_now,
+        help_text=_("Last date/time the element was read by the user"))
 
     class Meta:
         unique_together = (('user', 'element'),)
 
     def __str__(self):
         return '%s follows %s' % (self.user, self.element)
```

### Comparing `djaodjin-pages-0.7.1/pages/serializers.py` & `djaodjin-pages-0.8.0/pages/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -291,14 +291,56 @@
             # HTMLField
             html_field = HTMLField(html_tags=settings.ALLOWED_TAGS,
                                    html_attributes=settings.ALLOWED_ATTRIBUTES)
             data['text'] = html_field.to_internal_value(data['text'])
         return super(PageElementSerializer, self).to_internal_value(data)
 
 
+class PageElementUpdateSerializer(PageElementSerializer):
+    text_updated_at = serializers.DateTimeField(
+        required=False,
+        help_text=_("Datetime of last update on the page element's text"))
+    nb_comments_since_last_read = serializers.IntegerField(
+        help_text=_("Number of comments since last read"),
+        required=False)
+    last_read_at = serializers.DateTimeField(
+        required=False,
+        help_text=_("Last time the PageElement was read"),
+        read_only=True)
+
+    descr = serializers.SerializerMethodField()
+
+    class Meta(PageElementSerializer.Meta):
+        fields = PageElementSerializer.Meta.fields + (
+            'text_updated_at', 'nb_comments_since_last_read',
+            'last_read_at', 'descr')
+        read_only_fields = PageElementSerializer.Meta.read_only_fields + (
+            'text_updated_at', 'nb_comments_since_last_read',
+            'last_read_at', 'descr')
+
+    def get_descr(self, obj):
+        final_str_list = []
+
+        if obj.text_updated_at and obj.last_read_at:
+            final_str_list.append(
+                _("Text last updated on %(text_updated_at)s.") % {
+                    'text_updated_at': obj.text_updated_at.isoformat()})
+
+        if obj.nb_comments_since_last_read:
+            comment_or_comments = "comment" if obj.nb_comments_since_last_read \
+                == 1 else "comments"
+            final_str_list.append(_("%(nb_comments)s new "\
+                    "%(comment_or_comments)s since last visit.") % {
+                    'nb_comments': obj.nb_comments_since_last_read,
+                    'comment_or_comments': comment_or_comments
+                })
+
+        return ' '.join(final_str_list)
+
+
 class PageElementTagSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = PageElement
         fields = ('tag',)
```

### Comparing `djaodjin-pages-0.7.1/pages/settings.py` & `djaodjin-pages-0.8.0/pages/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/signals.py` & `djaodjin-pages-0.8.0/pages/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/static/js/djaodjin-pages-vue.js` & `djaodjin-pages-0.8.0/pages/static/js/djaodjin-pages-vue.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,16 @@
         this.get();
     }
 });
 
 
 Vue.component('editables-detail', {
     mixins: [
-        itemMixin
+        itemMixin,
+        accountDetailMixin
     ],
     data: function() {
         return {
             item: this.$element ? this.$element : {},
             url: this.$urls.api_content,
             tags: [],
             isFollowing: false,
@@ -130,14 +131,17 @@
                     vm.tags = resp.data.extra.tags;
                 }
             });
         }
         vm.reqGet(this.$urls.api_comments,
             function success(resp) {
                 vm.comments = resp;
+                // XXX If we are trying to load all user details at once,
+                //     we end up matching multiple profiles for a specific `slug`.
+                // vm.populateAccounts(resp, 'user');
             },
             function error() {
                 // We might be looking at the page anonymously and the comments
                 // will only load for authenticated users.
             });
     }
 });
@@ -658,8 +662,22 @@
         let hours = Math.floor(numericValue / 3600).toString().padStart(2, '0');
         let minutes = Math.floor((numericValue % 3600) / 60).toString().padStart(2, '0');
         let seconds = Math.floor(numericValue % 60).toString().padStart(2, '0');
         return `${hours}:${minutes}:${seconds}`;
     }
 
     return value || '00:00:00';
+});
+
+Vue.component('news-feed', {
+    mixins: [
+        itemListMixin
+    ],
+    data() {
+        return {
+            url: this.$urls.api_news_feed
+        };
+    },
+    mounted() {
+        this.get();
+    }
 });
```

### Comparing `djaodjin-pages-0.7.1/pages/static/js/djaodjin-resources-vue.js` & `djaodjin-pages-0.8.0/pages/static/js/djaodjin-resources-vue.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1046,19 +1046,19 @@
     }
 
 
     var sortableMixin = {
         data: function() {
             var defaultDir = this.$sortDirection || 'desc';
             var dir = (defaultDir === 'desc') ? DESC_SORT_PRE : '';
-            var o = this.$sortByField || 'created_at';
+            var params = this.$sortByField ? {
+                o: (dir + this.$sortByField)
+            } : {};
             return {
-                params: {
-                    o: dir + o,
-                },
+                params: params,
                 mixinSortCb: 'get'
             }
         },
         methods: {
             sortDir: function(field) {
                 return this.sortFields[field]
             },
@@ -1310,47 +1310,49 @@
                     vm.current--;
                 } else if (vm.current === -1) {
                     vm.current = vm.items.length - 1;
                 } else {
                     vm.current = -1;
                 }
             },
-            search: function() {
-                this.update();
-            },
-            update: function() {
+            reload: function() {
                 var vm = this;
-                vm.cancel();
-                if (!vm.query) {
-                    return vm.reset();
-                }
-                if (vm.minChars && vm.query.length < vm.minChars) {
-                    return;
-                }
                 vm.loading = true;
                 var params = {};
                 params[vm.queryParamName] = vm.query;
                 vm.reqGet(vm.url, params,
                     function(resp) {
-                        if (resp && vm.query) {
-                            var data = resp.results;
-                            data = vm.prepareResponseData ? vm.prepareResponseData(data) : data;
-                            vm.items = vm.limit ? data.slice(0, vm.limit) : data;
-                            vm.current = -1;
-                            vm.loading = false;
-                            if (vm.selectFirst) {
-                                vm.down();
-                            }
+                        const data = vm.prepareResponseData ?
+                            vm.prepareResponseData(resp.results) : resp.results;
+                        vm.items = vm.limit ? data.slice(0, vm.limit) : data;
+                        vm.current = -1;
+                        vm.loading = false;
+                        if (vm.selectFirst) {
+                            vm.down();
                         }
                     },
                     function() {
                         // on failure we just do nothing. - i.e. we don't want a bunch
                         // of error messages to pop up.
                     });
             },
+            search: function() {
+                this.update();
+            },
+            update: function() {
+                var vm = this;
+                vm.cancel();
+                if (!vm.query) {
+                    return vm.reset();
+                }
+                if (vm.minChars && vm.query.length < vm.minChars) {
+                    return;
+                }
+                vm.reload();
+            },
         },
         computed: {
             hasItems: function hasItems() {
                 return this.items.length > 0;
             },
             isEmpty: function isEmpty() {
                 return !this.query;
@@ -1362,16 +1364,92 @@
         mounted: function() {
             if (this.$el.dataset && this.$el.dataset.url) {
                 this.url = this.$el.dataset.url;
             }
         }
     };
 
+
+    /** Mixin to load user details from the profile APIs
+     */
+    var accountDetailMixin = {
+        data: function() {
+            return {
+                api_accounts_url: this.$urls.api_accounts,
+                accountsBySlug: {}
+            }
+        },
+        methods: {
+            getAccountField: function(user, fieldName) {
+                var vm = this;
+                if (user && user.hasOwnProperty(fieldName)) {
+                    return user[fieldName];
+                }
+                if (user) {
+                    const account = vm.accountsBySlug[user];
+                    if (account && account.hasOwnProperty(fieldName)) {
+                        return account[fieldName];
+                    }
+                    vm.accountsBySlug[user] = {
+                        picture: null,
+                        printable_name: user
+                    };
+                    if (vm.api_accounts_url) {
+                        vm.reqGet(vm._safeUrl(vm.api_accounts_url, user),
+                            function(resp) {
+                                vm.accountsBySlug[resp.slug] = resp;
+                            },
+                            function() {
+                                // discard errors (ex: "not found").
+                            });
+                    }
+                    return vm.accountsBySlug[user][fieldName];
+                }
+                return "";
+            },
+            getAccountPicture: function(user) {
+                return this.getAccountField(user, 'picture');
+            },
+            getAccountPrintableName: function(user) {
+                return this.getAccountField(user, 'printable_name');
+            },
+            populateAccounts: function(elements, fieldName) {
+                var vm = this;
+
+                if (!vm.api_accounts_url) return;
+
+                const accounts = new Set();
+                for (let idx = 0; idx < elements.length; ++idx) {
+                    const item = elements[idx];
+                    accounts.add((fieldName && item[fieldName]) ?
+                        item[fieldName] : item.slug);
+                }
+                let queryParams = "?q_f=slug&q=";
+                let sep = "";
+                for (const account of accounts) {
+                    queryParams += sep + account;
+                    sep = ",";
+                }
+                vm.reqGet(vm.api_accounts_url + queryParams,
+                    function(resp) {
+                        for (let idx = 0; idx < resp.results.length; ++idx) {
+                            vm.accountsBySlug[resp.results[idx].slug] =
+                                resp.results[idx];
+                        }
+                    },
+                    function() {
+                        // discard errors (ex: "not found").
+                    });
+            },
+        }
+    };
+
     // attach properties to the exports object to define
     // the exported module properties.
     exports.httpRequestMixin = httpRequestMixin;
     exports.itemListMixin = itemListMixin;
     exports.itemMixin = itemMixin;
     exports.messagesMixin = messagesMixin;
     exports.paramsMixin = paramsMixin;
     exports.typeAheadMixin = typeAheadMixin;
+    exports.accountDetailMixin = accountDetailMixin;
 }));
```

### Comparing `djaodjin-pages-0.7.1/pages/templates/pages/_comments.html` & `djaodjin-pages-0.8.0/pages/templates/pages/_comments.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div>
   <h4>[[comments.count]] Comments</h4>
   <table>
-    <tr v-for="comment in comments.results">
+    <tr :id="'comment_from_'+ comment.user" v-for="comment in comments.results">
       <td>
         [[comment.user]]<br />
         <small>[[comment.created_at]]</small>
       </td>
       <td >[[comment.text]]</td>
     </tr>
   </table>
```

#### html2text {}

```diff
@@ -1,8 +1,6 @@
 ****** [[[[ccoommmmeennttss..ccoouunntt]]]] CCoommmmeennttss ******
-[[comment.user]]       [[comment.text]]
-[[comment.created_at]]
 {% if user.is_authenticated %}
 [Submit]
 {% else %}
 Please _l_o_g_ _i_n to leave a comment.
 {% endif %}
```

### Comparing `djaodjin-pages-0.7.1/pages/templates/pages/element.html` & `djaodjin-pages-0.8.0/pages/templates/pages/element.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "base.html" %}
 
 {% block content %}
 <section  id="app">
   <editables-detail inline-template>
     <div :id="item.slug">
-        <h1 class="editable" data-key="title">[[item.title]]</h1>
+        <h1 class="title editable" data-key="title">[[item.title]]</h1>
         <div class="editable edit-formatted" data-key="text" v-html="item.html_formatted" v-if="item.text">
         </div>
         <div class="editable edit-formatted" data-key="text" v-if="!item.text">
             enter text here...
         </div>
         <hr />
         {% include "pages/_follow_vote.html" %}
```

### Comparing `djaodjin-pages-0.7.1/pages/templatetags/pages_tags.py` & `djaodjin-pages-0.8.0/pages/templatetags/pages_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/__init__.py` & `djaodjin-pages-0.8.0/pages/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/__init__.py` & `djaodjin-pages-0.8.0/pages/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/assets.py` & `djaodjin-pages-0.8.0/pages/urls/api/assets.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/editables.py` & `djaodjin-pages-0.8.0/pages/urls/api/editables.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/noauth.py` & `djaodjin-pages-0.8.0/pages/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/progress.py` & `djaodjin-pages-0.8.0/pages/urls/api/progress.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/readers.py` & `djaodjin-pages-0.8.0/pages/urls/api/readers.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,20 @@
 
 """
 API URLs for readers who must be authenticated
 """
 from ...compat import path
 
 from ...api.reactions import (FollowAPIView, UnfollowAPIView, UpvoteAPIView,
-  DownvoteAPIView, CommentListCreateAPIView)
+  DownvoteAPIView, CommentListCreateAPIView, NewsFeedListAPIView)
 
 urlpatterns = [
+    # NewsFeed
+    path('<slug:user>/newsfeed',
+         NewsFeedListAPIView.as_view(), name='api_news_feed'),
     # Following
     path('follow/<path:path>',
         FollowAPIView.as_view(), name='pages_api_follow'),
     path('unfollow/<path:path>',
         UnfollowAPIView.as_view(), name='pages_api_unfollow'),
     # Votes
     path('upvote/<path:path>',
```

### Comparing `djaodjin-pages-0.7.1/pages/urls/api/sequences.py` & `djaodjin-pages-0.8.0/pages/urls/api/sequences.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/views/__init__.py` & `djaodjin-pages-0.8.0/pages/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/views/editables.py` & `djaodjin-pages-0.8.0/pages/urls/views/editables.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/views/elements.py` & `djaodjin-pages-0.8.0/pages/urls/views/elements.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/urls/views/sequences.py` & `djaodjin-pages-0.8.0/pages/urls/views/sequences.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/utils.py` & `djaodjin-pages-0.8.0/pages/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/views/__init__.py` & `djaodjin-pages-0.8.0/pages/views/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from django.views.generic import RedirectView
 
 from ..utils import get_current_account
 
-
 class AccountRedirectView(RedirectView):
     """
     Redirects to the URL containing the app.
     """
     slug_url_kwarg = 'account'
 
     def get(self, request, *args, **kwargs):
```

### Comparing `djaodjin-pages-0.7.1/pages/views/elements.py` & `djaodjin-pages-0.8.0/pages/views/elements.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pages/views/sequences.py` & `djaodjin-pages-0.8.0/pages/views/sequences.py`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/pyproject.toml` & `djaodjin-pages-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-pages-0.7.1/setup.py` & `djaodjin-pages-0.8.0/setup.py`

 * *Files identical despite different names*

