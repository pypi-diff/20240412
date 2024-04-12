# Comparing `tmp/bibtexautocomplete-1.3.1.tar.gz` & `tmp/bibtexautocomplete-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtexautocomplete-1.3.1.tar", last modified: Tue Feb 20 19:42:21 2024, max compression
+gzip compressed data, was "bibtexautocomplete-1.3.2.tar", last modified: Fri Apr 12 21:41:37 2024, max compression
```

## Comparing `bibtexautocomplete-1.3.1.tar` & `bibtexautocomplete-1.3.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.378606 bibtexautocomplete-1.3.1/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1075 2024-01-23 21:45:51.000000 bibtexautocomplete-1.3.1/LICENSE
--rw-r--r--   0 dorian    (1000) dorian    (1000)    20680 2024-02-20 19:42:21.378606 bibtexautocomplete-1.3.1/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    17497 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/README.md
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.366607 bibtexautocomplete-1.3.1/bibtexautocomplete/
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.370607 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4178 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/arxiv.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4571 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/crossref.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2977 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/dblp.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3736 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/doi.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4471 2024-02-05 21:40:22.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/inspire_hep.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     5050 2024-02-05 21:40:22.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/openalex.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3466 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/researchr.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     6415 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/semantic_scholar.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3897 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/unpaywall.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      184 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       67 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/__main__.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.370607 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2794 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/author.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    11346 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/base_field.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2686 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/constants.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     6266 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/entry.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    13896 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/fields.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2500 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/io.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3395 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/normalize.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.374606 bibtexautocomplete-1.3.1/bibtexautocomplete/core/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      121 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      730 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/apis.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    14292 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/autocomplete.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1100 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/data_dump.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     5406 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/main.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    11359 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/parser.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2192 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/core/threads.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.374606 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3991 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/abstract_base.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1854 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/abstract_entry_lookup.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     9440 2024-02-17 10:26:47.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/https.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      699 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/lookups.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2764 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/multiple_mixin.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4060 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/search_mixin.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.374606 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2709 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/ansi.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1533 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/constants.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1144 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/functions.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     7892 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/logger.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2591 2024-02-05 21:40:22.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/only_exclude.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     4857 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/bibtexautocomplete/utils/safe_json.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.374606 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/
--rw-r--r--   0 dorian    (1000) dorian    (1000)    20680 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1943 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/SOURCES.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/dependency_links.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       54 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/entry_points.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       96 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/requires.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       19 2024-02-20 19:42:21.000000 bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/top_level.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     2325 2024-02-20 19:42:16.000000 bibtexautocomplete-1.3.1/pyproject.toml
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       38 2024-02-20 19:42:21.378606 bibtexautocomplete-1.3.1/setup.cfg
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-02-20 19:42:21.374606 bibtexautocomplete-1.3.1/tests/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     3175 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/tests/test_1_utils.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    14998 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/tests/test_2_bibtex.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     7577 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.1/tests/test_3_lookup.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1330 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/tests/test_4_parser.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      372 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.1/tests/test_5_options.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     5504 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.1/tests/test_9_APIs.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.355454 bibtexautocomplete-1.3.2/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1075 2024-01-23 21:45:51.000000 bibtexautocomplete-1.3.2/LICENSE
+-rw-r--r--   0 dorian    (1000) dorian    (1000)    21229 2024-04-12 21:41:37.355454 bibtexautocomplete-1.3.2/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    18051 2024-04-12 21:41:10.000000 bibtexautocomplete-1.3.2/README.md
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.343454 bibtexautocomplete-1.3.2/bibtexautocomplete/
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.347453 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4193 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/arxiv.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4589 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/crossref.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2992 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/dblp.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3736 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/doi.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4486 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/inspire_hep.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5065 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/openalex.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3481 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/researchr.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     6430 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/semantic_scholar.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3912 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/unpaywall.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      184 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       67 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/__main__.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.347453 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2794 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/author.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    11469 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/base_field.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2686 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/constants.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     9793 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/entry.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    13946 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/fields.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2500 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/io.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3395 2024-02-20 19:39:06.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/normalize.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.351453 bibtexautocomplete-1.3.2/bibtexautocomplete/core/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      121 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      730 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/apis.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    15985 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/autocomplete.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1100 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/data_dump.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5176 2024-04-12 21:41:10.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/main.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    11864 2024-04-12 21:41:10.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/parser.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2782 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/core/threads.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.351453 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3991 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/abstract_base.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      801 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/abstract_entry_lookup.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     9440 2024-02-17 10:26:47.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/https.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      594 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/lookups.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2764 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/multiple_mixin.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4060 2024-02-05 21:38:43.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/search_mixin.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.351453 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2709 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/ansi.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1533 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/constants.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1144 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/functions.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     7892 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/logger.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2591 2024-02-05 21:40:22.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/only_exclude.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     4857 2024-02-16 21:24:19.000000 bibtexautocomplete-1.3.2/bibtexautocomplete/utils/safe_json.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.355454 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/
+-rw-r--r--   0 dorian    (1000) dorian    (1000)    21229 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1943 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       54 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/entry_points.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       96 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/requires.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       19 2024-04-12 21:41:37.000000 bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/top_level.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     2320 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/pyproject.toml
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       38 2024-04-12 21:41:37.355454 bibtexautocomplete-1.3.2/setup.cfg
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2024-04-12 21:41:37.355454 bibtexautocomplete-1.3.2/tests/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3175 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/tests/test_1_utils.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    14922 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/tests/test_2_bibtex.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5066 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/tests/test_3_lookup.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1330 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/tests/test_4_parser.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      372 2024-01-23 21:44:38.000000 bibtexautocomplete-1.3.2/tests/test_5_options.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5444 2024-04-12 18:34:08.000000 bibtexautocomplete-1.3.2/tests/test_9_APIs.py
```

### Comparing `bibtexautocomplete-1.3.1/LICENSE` & `bibtexautocomplete-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/PKG-INFO` & `bibtexautocomplete-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtexautocomplete
-Version: 1.3.1
+Version: 1.3.2
 Summary: Script to autocomplete bibtex files by polling online databases
 Author-email: Dorian Lesbre <dorian.lesbre@gmail.com>
 Maintainer-email: Dorian Lesbre <dorian.lesbre@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2024 Dorian Lesbre
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dlesbre/bibtex-autocomplete
-Project-URL: Repository, https://github.com/dlesbre/bibtex-autocomplete/spam.git
+Project-URL: Repository, https://github.com/dlesbre/bibtex-autocomplete.git
 Project-URL: Issues, https://github.com/dlesbre/bibtex-autocomplete/issues
 Project-URL: Changelog, https://github.com/dlesbre/bibtex-autocomplete/blob/master/CHANGELOG.md
 Keywords: bibtex,biblatex,latex,autocomplete,btac
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -313,22 +313,29 @@
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
+- `-b --filter-fields-by-entrytype <required|optional|all>` only add fields that correspond to
+  the given entry type in bibtex's data model. Disabled by default. `required`
+  only adds required fields, `optional` adds required and optional fields, and
+  `all` adds required, optional and non-standard fields (doi, issn and isbn).
+  A list of required/optional fields by entry type can be found
+  [on the tex stackexchange](https://tex.stackexchange.com/questions/239042/where-can-we-find-a-list-of-all-available-bibtex-entries-and-the-available-fiel)
+
 - `-w --overwrite <field>` or `-W --dont-overwrite <field>`
 
   Force overwriting of the selected fields. If using `-W author -W journal`
   your force overwrite of all fields except `author` and `journal`. The
   default is to override nothing (only complete absent and blank fields).
 
   For a more complex example `btac -C doi -w author` means complete all fields
-  save DOI, and only overwrite author fields
+  save DOI, and only overwrite author fields.
 
   You can also use the `-f` flag to overwrite everything or the `-p` flag to add
   a prefix to new fields, thus avoiding overwrites.
 
 - `-m --mark` and `-M --ignore-mark`
 
   This is useful to avoid repeated queries if you want to run `btac` many times
```

### Comparing `bibtexautocomplete-1.3.1/README.md` & `bibtexautocomplete-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -248,22 +248,29 @@
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
+- `-b --filter-fields-by-entrytype <required|optional|all>` only add fields that correspond to
+  the given entry type in bibtex's data model. Disabled by default. `required`
+  only adds required fields, `optional` adds required and optional fields, and
+  `all` adds required, optional and non-standard fields (doi, issn and isbn).
+  A list of required/optional fields by entry type can be found
+  [on the tex stackexchange](https://tex.stackexchange.com/questions/239042/where-can-we-find-a-list-of-all-available-bibtex-entries-and-the-available-fiel)
+
 - `-w --overwrite <field>` or `-W --dont-overwrite <field>`
 
   Force overwriting of the selected fields. If using `-W author -W journal`
   your force overwrite of all fields except `author` and `journal`. The
   default is to override nothing (only complete absent and blank fields).
 
   For a more complex example `btac -C doi -w author` means complete all fields
-  save DOI, and only overwrite author fields
+  save DOI, and only overwrite author fields.
 
   You can also use the `-f` flag to overwrite everything or the `-p` flag to add
   a prefix to new fields, thus avoiding overwrites.
 
 - `-m --mark` and `-M --ignore-mark`
 
   This is useful to avoid repeated queries if you want to run `btac` many times
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/arxiv.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/arxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
             if link.attrib.get("title") == "pdf" and link.text:
                 return link.text
         return None
 
     def get_value(self, result: Element) -> BibtexEntry:
         """Extract bibtex data from JSON output"""
         year, month = self.get_date(result)
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.author.set(self.get_authors(result))
         values.doi.set(self.get_doi(result))
         values.month.set(month)
         values.title.set(self.get_title(result))
         values.url.set(self.get_link(result))
         values.year.set(year)
         return values
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/crossref.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/crossref.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,27 +96,30 @@
         return None, None
 
     def get_value(self, result: SafeJSON) -> BibtexEntry:
         """Extract bibtex data from JSON output"""
         year, month = self.get_date(result)
         title = result["container-title"][0].to_str()
         is_journal = result["type"].to_str() == "journal-article"
-        values = BibtexEntry(self.name)
+
+        values = BibtexEntry(self.name, self.entry.id)
+
         values.author.set(self.get_authors(result["author"]))
         values.booktitle.set(None if is_journal else title)
         values.doi.set(result["DOI"].to_str())
         values.issn.set_str(result["ISSN"][0].to_str())
         values.isbn.set(result["ISBN"][0].to_str())
         values.journal.set(title if is_journal else None)
         values.month.set(month)
         values.pages.set_str(result["page"].to_str())
         values.publisher.set(result["publisher"].to_str())
         values.title.set(result["title"][0].to_str())
         values.volume.set(result["volume"].to_str())
         values.year.set(year)
+
         return values
 
     # Set of fields we can get from a query.
     # If all are already present on an entry, the query can be skipped.
     fields = {
         FieldNames.AUTHOR,
         FieldNames.BOOKTITLE,
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/dblp.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/dblp.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             aut = Author.from_name(name)
             if aut is not None:
                 formatted.append(aut)
         return formatted
 
     def get_value(self, result: SafeJSON) -> BibtexEntry:
         info = result["info"]
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.author.set(self.get_authors(info))
         values.doi.set(info["doi"].to_str())
         values.pages.set_str(info["pages"].to_str())
         values.title.set(info["title"].to_str())
         values.volume.set(info["volume"].to_str())
         values.url.set(info["ee"].to_str() if info["access"].to_str() == "open" else None)
         values.year.set(info["year"].to_str())
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/doi.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/doi.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/inspire_hep.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/inspire_hep.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         metadata = result["metadata"]
         journal = metadata["publication_info"][0]
         year, month = self.get_date(metadata)
 
         first_page = journal["page_start"].force_str()
         last_page = journal["page_end"].force_str()
 
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.author.set(self.get_authors(metadata["authors"]))
         values.doi.set(metadata["dois"][0]["value"].to_str())
         values.isbn.set(metadata["isbns"][0]["value"].force_str())
         values.journal.set(journal["journal_title"].to_str())
         values.month.set(month)
         values.number.set(journal["journal_issue"].force_str())
         values.pages.from_pair(first_page, last_page)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/openalex.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/openalex.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         is_book = result["type"].to_str() in ["book", "book-chapter"]
         journal = location["source"]["display_name"].to_str()
 
         first_page = result["biblio"]["first_page"].to_str()
         last_page = result["biblio"]["last_page"].to_str()
 
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.author.set(self.get_authors(result["authorships"]))
         values.doi.set(result["doi"].to_str())
         values.issn.set_str(location["source"]["issn_l"].to_str())
         values.journal.set(journal if not is_book else None)
         values.month.set(month)
         values.number.set(result["biblio"]["issue"].to_str())
         values.pages.from_pair(first_page, last_page)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/researchr.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/researchr.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             if aut is not None:
                 formatted.append(aut)
         return formatted
 
     def get_value(self, result: SafeJSON) -> BibtexEntry:
         page_1 = result["firstpage"].to_str()
         page_n = result["lastpage"].to_str()
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.address.set(result["address"].to_str())
         values.author.set(self.get_authors(result["authors"]))
         values.booktitle.set(result["booktitle"].to_str())
         values.doi.set(result["doi"].to_str())
         values.editor.set(self.get_authors(result["editors"]))
         values.month.set(result["month"].to_str())
         values.number.set(result["number"].to_str())
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/semantic_scholar.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/semantic_scholar.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
         venue = result["venue"].to_str()
         if venue is None:
             venue = result["publicationVenue"]["name"].to_str()
         if venue is None:
             venue = result["journal"]["name"].to_str()
 
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
         values.author.set(self.get_authors(result["authors"]))
         values.booktitle.set(None if is_journal else venue)
         values.doi.set(result["externalIds"]["DOI"].to_str())
         values.issn.set_str(result["publicationVenue"]["issn"].to_str())
         values.journal.set(venue if is_journal else None)
         values.month.set(month)
         values.pages.set_str(result["journal"]["pages"].to_str())
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/APIs/unpaywall.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/APIs/unpaywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 month = None
         if year is None:
             year = result["year"].force_str()
 
         title = result["journal_name"].to_str()
         is_journal = result["genre"].to_str() == "journal-article"
 
-        values = BibtexEntry(self.name)
+        values = BibtexEntry(self.name, self.entry.id)
 
         values.author.set(self.get_authors(result["z_authors"]))
         values.booktitle.set(None if is_journal else title)
         values.doi.set(result["doi"].to_str())
         values.issn.set_str(result["journal_issn_l"].to_str())
         values.journal.set(title if is_journal else None)
         values.month.set(month)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/author.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/author.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/base_field.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/base_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,18 @@
     @classmethod
     def normalize(cls, value: T) -> Optional[T]:
         """Return a normal representation of the entry
         Can return None if invalid format"""
         return value
 
     @classmethod
-    def slow_check(cls, value: T) -> bool:
+    def slow_check(cls, value: T, entry_name: str) -> bool:
         """Performs a slow check (e.g. query URL to ensure it resolves)
-        Only done if we want to use this in our field"""
+        Only done if we want to use this in our field
+        entry_name is the name of the current entry, used for error printing"""
         return True
 
     @classmethod
     def match_values(cls, a: T, b: T) -> int:
         """returns a match score: 0 <= score <= FIELD_FULL_MATCH"""
         if a == b:
             return FIELD_FULL_MATCH
@@ -228,16 +229,16 @@
             if norm is not None:
                 normalized.append(norm)
         if normalized:
             return normalized
         return None
 
     @classmethod
-    def slow_check(cls, value: List[T]) -> bool:
-        return all(cls.base_class.slow_check(x) for x in value)
+    def slow_check(cls, value: List[T], entry_name: str) -> bool:
+        return all(cls.base_class.slow_check(x, entry_name) for x in value)
 
     @classmethod
     def match_values(cls, a: List[T], b: List[T]) -> int:
         if len(a) * len(b) <= LONG_LIST_DELIMITER:
             return cls.match_values_slow(a, b)
         return cls.match_values_fast(a, b)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/constants.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/constants.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/fields.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,23 +97,23 @@
         """Returns doi to canonical form (i.e. removing url)"""
         match = search(DOIField.DOI_REGEX, doi)
         if match is not None:
             return match.group(1).lower()  # DOI's are case insensitive
         return None
 
     @classmethod
-    def slow_check(cls, doi: str) -> bool:
+    def slow_check(cls, doi: str, entry_name: str) -> bool:
         """Query doi.org API to check DOI exists"""
         try:
             doi_checker = DOICheck(doi)
             return doi_checker.query() is True
         except Exception as err:
             logger.traceback(
                 f"Uncaught exception when checking DOI resolution\n"
-                f"Entry = {id}\n"
+                f"Entry = {entry_name}\n"
                 f"DOI = {doi}\n\n"
                 "As a result, this DOI will NOT be added to the entry",
                 err,
             )
             return False
 
 
@@ -126,22 +126,22 @@
     def normalize(cls, value: str) -> Optional[str]:
         url = normalize_url(value)
         if url is not None:
             return "https://" + url[0] + url[1]
         return None
 
     @classmethod
-    def slow_check(cls, value: str) -> bool:
+    def slow_check(cls, value: str, entry_name: str) -> bool:
         try:
             checker = URLCheck(value)
             return checker.query() is not None
         except Exception as err:
             logger.traceback(
                 f"Uncaught exception when checking URL resolution\n"
-                f"Entry = {id}\n"
+                f"Entry = {entry_name}\n"
                 f"URL = {value}\n\n"
                 "As a result, this URL will NOT be added to the entry",
                 err,
             )
         return False
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/io.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/io.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/bibtex/normalize.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/bibtex/normalize.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/apis.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/apis.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/autocomplete.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/autocomplete.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 from typing import (
     Any,
     Callable,
     Container,
     Iterable,
     Iterator,
     List,
+    Literal,
     NamedTuple,
     Optional,
     Set,
     Tuple,
     TypeVar,
     cast,
 )
 
 from alive_progress import alive_bar  # type: ignore
 from bibtexparser.bibdatabase import BibDatabase
 from bibtexparser.latexenc import string_to_latex
 
 from ..bibtex.base_field import BibtexField
 from ..bibtex.constants import FIELD_NO_MATCH, FieldType
-from ..bibtex.entry import BibtexEntry
+from ..bibtex.entry import ENTRY_TYPES, BibtexEntry
 from ..bibtex.io import file_read, file_write, get_entries
 from ..bibtex.normalize import has_field
 from ..lookups.abstract_entry_lookup import LookupType
 from ..utils.constants import (
     BULLET,
     FIELD_PREFIX,
     MARKED_FIELD,
@@ -73,47 +74,49 @@
 
 
 class BibtexAutocomplete(Iterable[EntryType]):
     """Main class used to dispatch calls to the relevant lookups"""
 
     bibdatabases: List[BibDatabase]
     lookups: List[LookupType]
-    fields: Container[str]
+    fields: Set[FieldType]  # Set of fields to complete
     entries: OnlyExclude[str]
     force_overwrite: Container[str]
     force_overwrite_all: bool
     escape_unicode: bool
     fields_to_protect_uppercase: Container[str]
     prefix: str
     mark: bool
     filter: Callable[[EntryType], bool]
     dumps: List[DataDump]
     diff_mode: bool
+    filter_by_entrytype: Literal["no", "required", "optional", "all"]
 
     changed_fields: int
     changed_entries: int
 
     # Ordered list of (entry, changes) where
     # changes is a list of (field, new_value, source)
     changes: List[Tuple[str, List[Changes]]]
 
     def __init__(
         self,
         bibdatabases: List[BibDatabase],
         lookups: Iterable[LookupType],
-        fields: Container[str],
+        fields: Set[FieldType],
         entries: OnlyExclude[str],
         force_overwrite: Container[str] = [],
         force_overwrite_all: bool = False,
         mark: bool = False,
         ignore_mark: bool = False,
         prefix: bool = False,
         escape_unicode: bool = False,
         diff_mode: bool = False,
         fields_to_protect_uppercase: Container[str] = set(),
+        filter_by_entrytype: Literal["no", "required", "optional", "all"] = "no",
     ):
         self.bibdatabases = bibdatabases
         self.lookups = list(lookups)
         self.fields = fields
         self.entries = entries
         self.force_overwrite = force_overwrite
         self.force_overwrite_all = force_overwrite_all
@@ -126,14 +129,15 @@
         if ignore_mark:
             self.filter = lambda x: x["ID"] in self.entries
         else:
             self.filter = lambda x: x["ID"] in self.entries and MARKED_FIELD.lower() not in x
         self.escape_unicode = escape_unicode
         self.fields_to_protect_uppercase = fields_to_protect_uppercase
         self.diff_mode = diff_mode
+        self.filter_by_entrytype = filter_by_entrytype
 
     def __iter__(self) -> Iterator[EntryType]:
         """Iterate through entries"""
         for db in self.bibdatabases:
             yield from filter(self.filter, get_entries(db))
 
     @memoize
@@ -165,18 +169,19 @@
     def autocomplete(self, no_progressbar: bool = False) -> None:
         """Main function that does all the work
         Iterate through entries, performing all lookups"""
         logger.header("Completing entries")
         total = self.count_entries() * len(self.lookups)
         entries = list(self)
         bib_entries: List[BibtexEntry] = []
+        to_complete: List[Set[FieldType]] = []
         for x in entries:
-            bib = BibtexEntry("input")
-            bib.from_entry(x)
+            bib = BibtexEntry.from_entry("input", x)
             bib_entries.append(bib)
+            to_complete.append(self.get_fields_to_complete(x))
         condition = Condition()
         assert len(self.lookups) < MAX_THREAD_NB
         threads: List[LookupThread] = []
         is_verbose = logger.get_level() < INFO
         with alive_bar(
             total,
             title="Querying databases:",
@@ -186,15 +191,15 @@
             monitor_end="[{percent:.0%}]",
             stats="(eta: {eta})",
             stats_end="",
             dual_line=True,
         ) as bar:
             # Create all threads
             for lookup in self.lookups:
-                threads.append(LookupThread(lookup, bib_entries, condition, bar))
+                threads.append(LookupThread(lookup, bib_entries, to_complete, condition, bar))
             condition.acquire()
             # Start all threads
             for thread in threads:
                 thread.start()
             position = 0
             nb_entries = self.count_entries()
             while position < nb_entries:
@@ -208,27 +213,55 @@
                 if is_verbose:
                     bar.text = " ".join(thread_positions)
                 else:
                     bar.text = f"Processed {position}/{nb_entries} entries, " f"found {self.changed_fields} new fields"
                 if not step:  # Some threads have not found data for current entry
                     condition.wait()
                 else:  # update data for current entry
-                    self.update_entry(entries[position], threads, position)
+                    self.update_entry(entries[position], to_complete[position], threads, position)
                     position += 1
         logger.info(
             "Modified {changed_entries} / {count_entries} entries" ", added {changed_fields} fields",
             changed_entries=self.changed_entries,
             count_entries=self.count_entries(),
             changed_fields=self.changed_fields,
         )
         # Delete empty entries (in diff mode)
         for db in self.bibdatabases:
             db.entries = filter(None, db.entries)
 
-    def update_entry(self, entry: EntryType, threads: List[LookupThread], position: int) -> None:
+    def get_fields_to_complete_by_entrytype(self, entry: EntryType) -> Set[FieldType]:
+        """Set of fields that can be accepted by the current entry,
+        Only looking at the given entry type"""
+        field_set = self.fields.copy()
+        if self.filter_by_entrytype == "no":
+            return field_set
+        entry_type = entry.get("ENTRYTYPE", "misc")
+        if entry_type not in ENTRY_TYPES:
+            entry_type = "misc"
+        entry_fields = ENTRY_TYPES[entry_type]
+        if self.filter_by_entrytype == "all":
+            return field_set & (entry_fields.required | entry_fields.optional | entry_fields.non_standard)
+        if self.filter_by_entrytype == "optional":
+            return field_set & (entry_fields.required | entry_fields.optional)
+        return field_set & entry_fields.required
+
+    def get_fields_to_complete(self, entry: EntryType) -> Set[FieldType]:
+        """Set of fields that can be accepted by the current entry,
+        looking at the entrytype and list of present fields"""
+        fields = self.get_fields_to_complete_by_entrytype(entry)
+        return set(
+            field
+            for field in fields
+            if (not has_field(entry, field)) or self.force_overwrite_all or field in self.force_overwrite
+        )
+
+    def update_entry(
+        self, entry: EntryType, to_complete: Set[FieldType], threads: List[LookupThread], position: int
+    ) -> None:
         """Reads all data the threads have found on a new entry,
         and uses it to update the entry with new fields"""
         changes: List[Changes] = []
         results: List[BibtexEntry] = []
         entry_id = entry.get("ID", "unnamed")
         new_fields: Set[FieldType] = set()
 
@@ -239,17 +272,17 @@
             if result is not None:
                 results.append(result)
                 new_fields = new_fields.union(result.fields())
 
         new_entry: EntryType = dict()
         for field in new_fields:
             # Filter which fields to add
-            if not (self.force_overwrite_all or (field in self.force_overwrite) or (not has_field(entry, field))):
+            if field not in to_complete:
                 continue
-            bib_field = self.combine_field(results, field)
+            bib_field = self.combine_field(results, field, entry_id)
             if bib_field is None:
                 continue
             value = bib_field.to_str()
             if value is None:
                 continue
             if self.escape_unicode:
                 value = string_to_latex(value)
@@ -277,15 +310,17 @@
                 new_entry["ID"] = entry_id
                 new_entry["ENTRYTYPE"] = entry.get("ENTRYTYPE", "unknown")
             else:
                 new_entry = dict()
             entry.clear()
         entry.update(new_entry)
 
-    def combine_field(self, results: List[BibtexEntry], fieldname: FieldType) -> Optional[BibtexField[Any]]:
+    def combine_field(
+        self, results: List[BibtexEntry], fieldname: FieldType, entry_name: str
+    ) -> Optional[BibtexField[Any]]:
         """Combine the values of a single field"""
         fields = [entry.get_field(fieldname) for entry in results if fieldname in entry]
         groups: List[Tuple[int, BibtexField[Any]]] = []
         for field in fields:
             for i, (count, combined_field) in enumerate(groups):
                 score = combined_field.matches(field)
                 if score is not None and score > FIELD_NO_MATCH:
@@ -294,15 +329,15 @@
             else:
                 groups.append((1, field))
         # Return the first maximal element that passes the test
         # We use reverse sort to have elements with biggest counts at the front
         # While retaining order on elements with equal counts
         groups.sort(key=lambda x: x[0], reverse=True)
         for _, elt in groups:
-            if elt.value is not None and elt.slow_check(elt.value):
+            if elt.value is not None and elt.slow_check(elt.value, entry_name):
                 return elt
         return None
 
     def print_changes(self) -> None:
         """prints a pretty list of changes"""
         logger.header("New fields", VERBOSE_INFO)
         if self.changes == []:
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/data_dump.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/data_dump.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/main.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from pathlib import Path
 from sys import stdout
 from typing import Container, List, Optional
 
 from ..bibtex.constants import FieldNamesSet, SearchedFields
 from ..bibtex.io import writer
-from ..lookups.abstract_entry_lookup import FieldConditionMixin
 from ..lookups.https import HTTPSLookup
 from ..utils.ansi import ANSICodes, ansi_format
 from ..utils.constants import (
     CONNECTION_TIMEOUT,
     FIELD_PREFIX,
     LICENSE,
     MARKED_FIELD,
@@ -109,44 +108,39 @@
         fields_to_protect_proto = OnlyExclude[str].from_nonempty(args.protect_uppercase, args.dont_protect_uppercase)
         fields_to_protect_proto.default = False
         fields_to_protect_uppercase = fields_to_protect_proto
 
     overwrite = OnlyExclude[str].from_nonempty(args.overwrite, args.dont_overwrite)
     overwrite.default = False
 
-    FieldConditionMixin.fields_to_complete = set(fields.filter(SearchedFields, lambda x: x))
-    FieldConditionMixin.overwrites = set(overwrite.filter(SearchedFields, lambda x: x))
-
-    if args.force_overwrite:
-        FieldConditionMixin.overwrites = SearchedFields
-
     if args.diff and args.inplace:
         logger.error(
             "Cannot use {FgYellow}-D/--diff{Reset} flag and {FgYellow}-i/--inplace{Reset} flag "
             "simultaneously, as there\n"
             "       is a big risk of deleting data.\n"
             "       If that is truly what you want to do, specify the output file explictly\n"
             "       with {FgYellow}-o / --output {FgGreen}<filename>{Reset}."
         )
         exit(5)
 
     databases = BibtexAutocomplete.read(args.input)
     completer = BibtexAutocomplete(
         databases,
         lookups,
-        fields,
+        set(fields.filter(SearchedFields, lambda x: x)),
         entries,
         force_overwrite=overwrite,
         force_overwrite_all=args.force_overwrite,
         mark=args.mark,
         ignore_mark=args.ignore_mark,
         prefix=args.prefix,
         fields_to_protect_uppercase=fields_to_protect_uppercase,
         escape_unicode=args.escape_unicode,
         diff_mode=args.diff,
+        filter_by_entrytype=args.filter_fields_by_entrytype,
     )
     completer.print_filters()
     try:
         completer.autocomplete(args.verbose < 0)
         completer.print_changes()
         if args.dump_data is not None:
             completer.write_dumps(args.dump_data)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/parser.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 parser.add_argument("--dont-query", "-Q", action="append", default=[], choices=LOOKUP_NAMES)
 parser.add_argument("--only-query", "-q", action="append", default=[], choices=LOOKUP_NAMES)
 parser.add_argument("--dont-complete", "-C", action="append", default=[], choices=FIELD_NAMES)
 parser.add_argument("--only-complete", "-c", action="append", default=[], choices=FIELD_NAMES)
 parser.add_argument("--dont-overwrite", "-W", action="append", default=[], choices=FIELD_NAMES)
 parser.add_argument("--overwrite", "-w", action="append", default=[], choices=FIELD_NAMES)
+parser.add_argument("--filter-fields-by-entrytype", "-b", default="no", choices=["required", "optional", "all"])
 
 parser.add_argument("--exclude-entry", "-E", action="append", default=[])
 parser.add_argument("--only-entry", "-e", action="append", default=[])
 
 parser.add_argument("--escape-unicode", "--fu", action="store_true")
 parser.add_argument("--protect-all-uppercase", "--fpa", action="store_true")
 parser.add_argument("--protect-uppercase", "--fp", action="append", default=[], choices=FIELD_NAMES)
@@ -187,14 +188,19 @@
   {FgYellow}-e --only-entry{Reset}    {FgGreen}<id>{Reset}     Only perform lookup these entries
   {FgYellow}-E --exclude-entry{Reset} {FgGreen}<id>{Reset}     Don't perform lookup these entries
         ID is the identifier in bibtex (e.g. @inproceedings{{<id> ... }})
 
   {FgYellow}-c --only-complete{Reset} {FgGreen}<field>{Reset}  Only complete the given fields
   {FgYellow}-C --dont-complete{Reset} {FgGreen}<field>{Reset}  Don't complete the given fields
         Field is a bibtex field (e.g. 'author', 'doi',...)
+  {FgYellow}-b --filter-fields-by-entrytype{Reset} {FgGreen}required|optional|all{Reset} Disabled by default
+        Only add fields defined as part of given entry type by bibtex (e.g. no
+        'publisher' on '@article'). 'required' only adds required fields,
+        'optional' adds required and optional, 'all' adds required, optional and
+        non-standard ('doi', 'issn' and 'isbn').
 
   {FgYellow}-w --overwrite{Reset} {FgGreen}<field>{Reset}       Overwrite the given fields,
         even if already present. Default is to overwrite nothing. See also "-f" flag
   {FgYellow}-W --dont-overwrite{Reset} {FgGreen}<field>{Reset}  Don't overwrite the given field
         Implicitly forces overwrite of all others.
         Field is a bibtex field (e.g. 'author', 'doi',...)
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/core/threads.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/core/threads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from threading import Condition, Thread
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Optional, Set, Tuple
 
+from ..bibtex.constants import FieldType
 from ..bibtex.entry import BibtexEntry
 from ..lookups.abstract_entry_lookup import LookupType
 from ..utils.logger import logger
 from ..utils.safe_json import JSONType
 
 
 class LookupThread(Thread):
     """As we our I/O limited,
     we can use threads to perform queries
     We create one thread per lookup, to keep query rate polite for each domain"""
 
     lookup: LookupType
     entries: List[BibtexEntry] = []  # Read only
+    to_complete: List[Set[FieldType]] = []  # Read only
     condition: Condition
     entry_name: Optional[str]
     result: List[
         Tuple[
             Optional[BibtexEntry],
             Dict[str, JSONType],
         ]
@@ -26,18 +28,20 @@
     position: int
     nb_entries: int
 
     def __init__(
         self,
         lookup: LookupType,
         entries: List[BibtexEntry],
+        to_complete: List[Set[FieldType]],
         condition: Condition,
         bar: Callable[[], None],
     ):
         self.entries = entries
+        self.to_complete = to_complete
         self.lookup = lookup
         self.condition = condition
         self.position = 0
         self.nb_entries = len(entries)
         self.result = []
 
         self.bar = bar
@@ -49,25 +53,33 @@
         self.condition.acquire()
         while self.position < self.nb_entries:
             entry = self.entries[self.position]
             self.entry_name = entry.id
             lookup = self.lookup(entry)
             self.condition.release()
 
-            try:
-                result = lookup.query()
-            except Exception as err:
+            if lookup.fields.isdisjoint(self.to_complete[self.position]):
+                # Skip query as no fields need to be completed
                 result = None
-                logger.traceback(
-                    "Uncaught exception when trying to autocomplete entry\n"
-                    f"Entry = {self.entry_name}\n"
-                    f"Website = {self.name}",
-                    err,
-                )
+                info = dict()
+                logger.debug("Skipping query, no data to add")
+            else:
+                try:
+                    result = lookup.query()
+                    info = lookup.get_last_query_info()
+                except Exception as err:
+                    result = None
+                    info = lookup.get_last_query_info()
+                    logger.traceback(
+                        "Uncaught exception when trying to autocomplete entry\n"
+                        f"Entry = {self.entry_name}\n"
+                        f"Website = {self.name}",
+                        err,
+                    )
 
             self.condition.acquire()
-            self.result.append((result, lookup.get_last_query_info()))
+            self.result.append((result, info))
             self.position += 1
             self.bar()
             self.condition.notify()
         self.condition.release()
         return None
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/abstract_base.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/abstract_base.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/https.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/https.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/lookups.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/lookups.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,29 +2,26 @@
 Combine all the mixins into full fledge classes
 """
 
 from xml.etree.ElementTree import Element
 
 from ..bibtex.entry import BibtexEntry
 from ..utils.safe_json import SafeJSON
-from .abstract_entry_lookup import FieldConditionMixin
 from .https import HTTPSRateCapedLookup
 from .multiple_mixin import DAT_Query_Mixin
 from .search_mixin import EntryMatchSearchMixin
 
 
 class JSON_Lookup(
-    FieldConditionMixin,
     DAT_Query_Mixin,
     EntryMatchSearchMixin[SafeJSON],
     HTTPSRateCapedLookup[BibtexEntry, BibtexEntry],
 ):
     pass
 
 
 class XML_Lookup(
-    FieldConditionMixin,
     DAT_Query_Mixin,
     EntryMatchSearchMixin[Element],
     HTTPSRateCapedLookup[BibtexEntry, BibtexEntry],
 ):
     pass
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/multiple_mixin.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/multiple_mixin.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/lookups/search_mixin.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/lookups/search_mixin.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/ansi.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/constants.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 URL = "https://github.com/dlesbre/bibtex-autocomplete"
 ISSUES_URL = URL + "/issues"
 LICENSE = "MIT"
 DESCRIPTION = "Script to autocomplete bibtex files by polling online databases"
 
 VERSION_MAJOR = 1
 VERSION_MINOR = 3
-VERSION_PATCH = 1
+VERSION_PATCH = 2
 
-VERSION_DATE = "2024-02-20"
+VERSION_DATE = "2024-04-12"
 
 VERSION = (VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH)
 VERSION_STR = f"{VERSION_MAJOR}.{VERSION_MINOR}.{VERSION_PATCH}"
 
 EMAIL = "dorian.lesbre" + chr(64) + "gmail.com"
 
 # Minimum delay between queries to same host, to avoid surcharging server
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/functions.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/functions.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/logger.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/only_exclude.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/only_exclude.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete/utils/safe_json.py` & `bibtexautocomplete-1.3.2/bibtexautocomplete/utils/safe_json.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/PKG-INFO` & `bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibtexautocomplete
-Version: 1.3.1
+Version: 1.3.2
 Summary: Script to autocomplete bibtex files by polling online databases
 Author-email: Dorian Lesbre <dorian.lesbre@gmail.com>
 Maintainer-email: Dorian Lesbre <dorian.lesbre@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2024 Dorian Lesbre
         
@@ -23,15 +23,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dlesbre/bibtex-autocomplete
-Project-URL: Repository, https://github.com/dlesbre/bibtex-autocomplete/spam.git
+Project-URL: Repository, https://github.com/dlesbre/bibtex-autocomplete.git
 Project-URL: Issues, https://github.com/dlesbre/bibtex-autocomplete/issues
 Project-URL: Changelog, https://github.com/dlesbre/bibtex-autocomplete/blob/master/CHANGELOG.md
 Keywords: bibtex,biblatex,latex,autocomplete,btac
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -313,22 +313,29 @@
   be used multiple times to select only/exclude multiple entries
 
 - `-c --only-complete <field>` or `-C --dont-complete <field>`
 
   Restrict which fields you wish to autocomplete. Field is a BibTeX field (e.g.
   `author`, `doi`,...). So if you only wish to add missing DOIs use `-c doi`.
 
+- `-b --filter-fields-by-entrytype <required|optional|all>` only add fields that correspond to
+  the given entry type in bibtex's data model. Disabled by default. `required`
+  only adds required fields, `optional` adds required and optional fields, and
+  `all` adds required, optional and non-standard fields (doi, issn and isbn).
+  A list of required/optional fields by entry type can be found
+  [on the tex stackexchange](https://tex.stackexchange.com/questions/239042/where-can-we-find-a-list-of-all-available-bibtex-entries-and-the-available-fiel)
+
 - `-w --overwrite <field>` or `-W --dont-overwrite <field>`
 
   Force overwriting of the selected fields. If using `-W author -W journal`
   your force overwrite of all fields except `author` and `journal`. The
   default is to override nothing (only complete absent and blank fields).
 
   For a more complex example `btac -C doi -w author` means complete all fields
-  save DOI, and only overwrite author fields
+  save DOI, and only overwrite author fields.
 
   You can also use the `-f` flag to overwrite everything or the `-p` flag to add
   a prefix to new fields, thus avoiding overwrites.
 
 - `-m --mark` and `-M --ignore-mark`
 
   This is useful to avoid repeated queries if you want to run `btac` many times
```

### Comparing `bibtexautocomplete-1.3.1/bibtexautocomplete.egg-info/SOURCES.txt` & `bibtexautocomplete-1.3.2/bibtexautocomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/pyproject.toml` & `bibtexautocomplete-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "Topic :: Utilities",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dlesbre/bibtex-autocomplete"
-Repository = "https://github.com/dlesbre/bibtex-autocomplete/spam.git"
+Repository = "https://github.com/dlesbre/bibtex-autocomplete.git"
 Issues = "https://github.com/dlesbre/bibtex-autocomplete/issues"
 Changelog = "https://github.com/dlesbre/bibtex-autocomplete/blob/master/CHANGELOG.md"
 
 [project.scripts]
 btac = "bibtexautocomplete.core:main"
 
 [project.optional-dependencies]
```

### Comparing `bibtexautocomplete-1.3.1/tests/test_1_utils.py` & `bibtexautocomplete-1.3.2/tests/test_1_utils.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/tests/test_2_bibtex.py` & `bibtexautocomplete-1.3.2/tests/test_2_bibtex.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,106 +135,95 @@
     field = NameField("author", "test")
     field.set_str(author)
     assert field.value == (res if res != [] else None)
 
 
 @pytest.mark.parametrize(("author", "res"), authors)
 def test_BibtexEntry_author_get(author: str, res: List[Author]) -> None:
-    b = BibtexEntry("test")
-    b.from_entry({FieldNames.AUTHOR: author})
+    b = BibtexEntry.from_entry("test", {FieldNames.AUTHOR: author})
     assert b.author.value == (res if res != [] else None)
 
 
 @pytest.mark.parametrize(("author", "res"), authors)
 def test_BibtexEntry_editor_get(author: str, res: List[Author]) -> None:
-    b = BibtexEntry("test")
-    b.from_entry({FieldNames.EDITOR: author})
+    b = BibtexEntry.from_entry("test", {FieldNames.EDITOR: author})
     assert b.editor.value == (res if res != [] else None)
 
 
 @pytest.mark.parametrize(("author", "res"), authors)
 def test_BibtexEntry_author_set(author: str, res: List[Author]) -> None:
-    b = BibtexEntry("test")
+    b = BibtexEntry("test", "testentry")
     b.author.set(res)
     assert b.author.value == (res if res != [] else None)
 
 
 @pytest.mark.parametrize(("author", "res"), authors)
 def test_BibtexEntry_editor_set(author: str, res: List[Author]) -> None:
-    b = BibtexEntry("test")
+    b = BibtexEntry("test", "testentry")
     b.editor.set(res)
     assert b.editor.value == (res if res != [] else None)
 
 
 def iterate_nested(list: List[List[str]]) -> Iterator[Tuple[int, str]]:
     """Iterate over a nested list, returning (index of sublist, element)"""
     for i, sublist in enumerate(list):
         for x in sublist:
             yield (i, x)
 
 
 def test_matching() -> None:
-    assert BibtexEntry("test").matches(BibtexEntry("test")) <= ENTRY_NO_MATCH
-    doi1 = BibtexEntry("test")
-    doi1.from_entry({"doi": "10.1234/12345"})
-    doi2 = BibtexEntry("test")
-    doi2.from_entry({"doi": "10.1234/different.12345"})
+    assert BibtexEntry("test", "testentry").matches(BibtexEntry("test", "testentry")) <= ENTRY_NO_MATCH
+    doi1 = BibtexEntry.from_entry("test", {"doi": "10.1234/12345"})
+    doi2 = BibtexEntry.from_entry("test", {"doi": "10.1234/different.12345"})
     assert doi1.matches(doi1) >= ENTRY_CERTAIN_MATCH
     assert doi1.matches(doi2) <= ENTRY_NO_MATCH
     # in same sublist should match (weakly)
     # in different sublists => no match
     titles = [
         ["My\tawesome paper!", "my awesome paper", "My AwESoMe Paper..."],
         ["My book, volume 1", "my book volume 1"],
         ["My book, volume 2"],
     ]
     authors = [
         ["Doe, J. and Smith, T.", "Doe, John", "John Doe", "Patrick, H. and Doe, J."],
         ["Henry, F."],
     ]
     for id, title in iterate_nested(titles):
-        entry = BibtexEntry("test")
-        entry.from_entry({"title": title})
+        entry = BibtexEntry.from_entry("test", {"title": title})
         score_same = entry.matches(entry)
         assert score_same >= ENTRY_NO_MATCH
         for id2, title2 in iterate_nested(titles):
-            entry2 = BibtexEntry("test")
-            entry2.from_entry({"title": title2})
+            entry2 = BibtexEntry.from_entry("test", {"title": title2})
             score_diff = entry.matches(entry2)
             assert score_same >= score_diff
             assert score_diff == entry2.matches(entry)
             if id == id2:
                 assert score_diff > ENTRY_NO_MATCH
             else:
                 assert score_diff <= ENTRY_NO_MATCH
 
     title = "My Awesome paper"
     for id, author in iterate_nested(authors):
-        entry = BibtexEntry("test")
-        entry.from_entry({"title": title, "author": author})
+        entry = BibtexEntry.from_entry("test", {"title": title, "author": author})
         score_same = entry.matches(entry)
         assert score_same >= ENTRY_NO_MATCH
         for id2, author2 in iterate_nested(authors):
-            entry2 = BibtexEntry("test")
-            entry2.from_entry({"title": title, "author": author2})
+            entry2 = BibtexEntry.from_entry("test", {"title": title, "author": author2})
             score_diff = entry.matches(entry2)
             assert score_same >= score_diff
             assert score_diff == entry2.matches(entry)
             if id == id2:
                 print(author, author2)
                 assert score_diff > ENTRY_NO_MATCH
             else:
                 assert score_diff <= ENTRY_NO_MATCH
 
-    entry = BibtexEntry("test")
-    entry.from_entry({"title": title, "year": "2023"})
-    entry2 = BibtexEntry("test")
-    entry2.from_entry({"title": title, "year": "2024"})
-    entry3 = BibtexEntry("test")
-    entry3.from_entry({"title": title, "year": "Invalid"})
+    entry = BibtexEntry.from_entry("test", {"title": title, "year": "2023"})
+    entry2 = BibtexEntry.from_entry("test", {"title": title, "year": "2024"})
+    entry3 = BibtexEntry.from_entry("test", {"title": title, "year": "Invalid"})
     assert entry.matches(entry) > ENTRY_NO_MATCH
     assert entry.matches(entry2) <= ENTRY_NO_MATCH
     assert entry.matches(entry3) > ENTRY_NO_MATCH
 
 
 urls: List[Tuple[str, Optional[Tuple[str, str]]]] = [
     ("http://google.com", ("google.com", "")),
```

### Comparing `bibtexautocomplete-1.3.1/tests/test_4_parser.py` & `bibtexautocomplete-1.3.2/tests/test_4_parser.py`

 * *Files identical despite different names*

### Comparing `bibtexautocomplete-1.3.1/tests/test_9_APIs.py` & `bibtexautocomplete-1.3.2/tests/test_9_APIs.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,48 +62,43 @@
     @pytest.fixture(autouse=True)
     def incr_timeout(self) -> None:
         logger.set_verbosity(4)
         self.Lookup.connection_timeout = 120.0
         self.Lookup.query_delay = 20.0
 
     def test_valid(self) -> None:
-        bib = BibtexEntry("test")
-        bib.from_entry(self.entry[0])
+        bib = BibtexEntry.from_entry("test", self.entry[0])
         a = self.Lookup(bib)
         res = a.query()
         assert res is not None
         assert res.doi.to_str() == self.entry[1]
 
     def test_junk(self) -> None:
-        bib = BibtexEntry("test")
-        bib.from_entry(entry_junk)
+        bib = BibtexEntry.from_entry("test", entry_junk)
         a = self.Lookup(bib)
         assert a.query() is None
 
     def test_invalid(self) -> None:
-        bib = BibtexEntry("test")
-        bib.from_entry(entry_invalid)
+        bib = BibtexEntry.from_entry("test", entry_invalid)
         a = self.Lookup(bib)
         assert a.query() is None
 
     def test_no_author(self) -> None:
         entry = self.entry[0].copy()
         del entry["author"]
-        bib = BibtexEntry("test")
-        bib.from_entry(entry)
+        bib = BibtexEntry.from_entry("test", entry)
         a = self.Lookup(bib)
         res = a.query()
         assert res is not None
         assert res.doi.to_str() == self.entry[1]
 
     def test_no_title(self) -> None:
         entry = self.entry[0].copy()
         del entry["title"]
-        bib = BibtexEntry("test")
-        bib.from_entry(entry)
+        bib = BibtexEntry.from_entry("test", entry)
         a = self.Lookup(bib)
         assert a.query() is None
 
 
 class TestCrossref(Base):
     Lookup = CrossrefLookup
     entry = (entry1, doi1)
```

