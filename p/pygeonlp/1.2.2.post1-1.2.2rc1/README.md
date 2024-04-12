# Comparing `tmp/pygeonlp-1.2.2.post1.tar.gz` & `tmp/pygeonlp-1.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeonlp-1.2.2.post1.tar", last modified: Fri Apr 12 04:32:12 2024, max compression
+gzip compressed data, was "pygeonlp-1.2.2rc1.tar", last modified: Thu Dec  7 01:55:31 2023, max compression
```

## Comparing `pygeonlp-1.2.2.post1.tar` & `pygeonlp-1.2.2rc1.tar`

### file list

```diff
@@ -1,112 +1,103 @@
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      404 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/INSTALL-Ubuntu22.md
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1343 2023-07-11 06:20:04.000000 pygeonlp-1.2.2.post1/LICENSE
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      174 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/MANIFEST.in
--rw-r--r--   0 sagara    (1000) sagara    (1000)     6593 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/PKG-INFO
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     5992 2024-01-04 01:09:16.000000 pygeonlp-1.2.2.post1/README.md
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     7076 2024-01-04 01:09:16.000000 pygeonlp-1.2.2.post1/README_ja.md
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.727822 pygeonlp-1.2.2.post1/base_data/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)  1032184 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/edo-kiriezu-owariya.csv
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1591 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/edo-kiriezu-owariya.json
--rw-rw-r--   0 sagara    (1000) sagara    (1000)  4599959 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/geoshape-city.csv
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1444 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/geoshape-city.json
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    10411 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/geoshape-pref.csv
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1390 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/geoshape-pref.json
--rw-rw-r--   0 sagara    (1000) sagara    (1000)  1594207 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/ksj-station-N02-2020.csv
--rw-rw-r--   0 sagara    (1000) sagara    (1000)  1388771 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/ksj-station-N02.csv
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1427 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/base_data/ksj-station-N02.json
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.727822 pygeonlp-1.2.2.post1/libgeonlp/
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/libgeonlp/include/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2489 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Address.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3287 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/CSVReader.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8142 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/DBAccessor.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      488 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/DartsException.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1642 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Dictionary.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2051 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Exception.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      802 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/FileAccessor.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      531 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/FormatException.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8107 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/GeonlpMA.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8812 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/GeonlpMAImplSq3.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     7001 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Geoword.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1892 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/GeowordFormatter.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1180 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/MeCabAdapter.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6001 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Node.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3786 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/NodeExt.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1868 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/PHBSDefs.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3849 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Profile.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      587 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/SqliteErrException.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      487 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/SqliteNotInitializedException.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1701 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Suffix.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1634 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Util.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2891 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/Wordlist.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2972 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/config.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    14376 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/darts.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    22050 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/picojson.h
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6482 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/include/picojsonExt.h
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/libgeonlp/lib/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1693 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Address.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3851 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/CSVReader.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    48756 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/DBAccessor.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2424 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Dictionary.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     4969 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/FileAccessor.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2563 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/GeonlpMA.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    40116 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/GeonlpMAImplSq3.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6819 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Geoword.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3552 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/GeowordFormatter.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2449 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/MeCabAdapter.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2930 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Node.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6462 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/NodeExt.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3586 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/PHBSDefs.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     9933 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Profile.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6077 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/Util.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    14075 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/lib/picojsonExt.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     4889 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/py2pico.cpp
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    14335 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/libgeonlp/pygeonlp.cpp
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.723822 pygeonlp-1.2.2.post1/pygeonlp/
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp/api/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    36666 2024-04-12 04:31:19.000000 pygeonlp-1.2.2.post1/pygeonlp/api/__init__.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     9691 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/__main__.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    10491 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/devtool.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    18445 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/dict_manager.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8138 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/api/dictionary.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    19166 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/api/filter.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    14057 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/linker.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8575 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/metadata.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    12127 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/api/node.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    31822 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/api/parser.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     7618 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/api/scoring.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    26615 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/api/service.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    12857 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/api/spatial_filter.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    20968 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/api/temporal_filter.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    12880 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/api/workflow.py
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp/samples/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    11834 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/samples/context.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1774 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/samples/sample_myscore.py
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp/tests/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)        0 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/__init__.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1050 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/conftest.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     3521 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_api.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     6026 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_api_geocoder.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     8499 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_api_geocoder_neologd.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2341 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_doctest.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      149 2024-01-04 01:04:59.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_issue1.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2444 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pygeonlp/tests/test_multiprocess.py
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp/webapi/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1068 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/__init__.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    16637 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/app.py
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp/webapi/tests/
--rw-rw-r--   0 sagara    (1000) sagara    (1000)        0 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/tests/__init__.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     1426 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/tests/conftest.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     2914 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/tests/helpers.py
--rw-rw-r--   0 sagara    (1000) sagara    (1000)    37627 2024-01-04 01:07:47.000000 pygeonlp-1.2.2.post1/pygeonlp/webapi/tests/test_webapi.py
-drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/pygeonlp.egg-info/
--rw-r--r--   0 sagara    (1000) sagara    (1000)     6593 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/PKG-INFO
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     4332 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/SOURCES.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)        1 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/dependency_links.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)       56 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/entry_points.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      122 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/requires.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)        9 2024-04-12 04:32:12.000000 pygeonlp-1.2.2.post1/pygeonlp.egg-info/top_level.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      100 2023-07-11 04:45:08.000000 pygeonlp-1.2.2.post1/pyproject.toml
--rw-rw-r--   0 sagara    (1000) sagara    (1000)      206 2024-04-12 04:31:19.000000 pygeonlp-1.2.2.post1/requirements.txt
--rw-rw-r--   0 sagara    (1000) sagara    (1000)       38 2024-04-12 04:32:12.731822 pygeonlp-1.2.2.post1/setup.cfg
--rw-rw-r--   0 sagara    (1000) sagara    (1000)     5126 2024-04-12 04:31:19.000000 pygeonlp-1.2.2.post1/setup.py
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      404 2023-07-11 06:19:05.000000 pygeonlp-1.2.2rc1/INSTALL-Ubuntu22.md
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1343 2023-07-11 06:20:04.000000 pygeonlp-1.2.2rc1/LICENSE
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      174 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/MANIFEST.in
+-rw-r--r--   0 sagara    (1000) sagara    (1000)     6579 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/PKG-INFO
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     5981 2023-07-11 06:20:04.000000 pygeonlp-1.2.2rc1/README.md
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     7066 2023-10-05 00:30:14.000000 pygeonlp-1.2.2rc1/README_ja.md
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:30.991073 pygeonlp-1.2.2rc1/base_data/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)  1032184 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/edo-kiriezu-owariya.csv
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1591 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/edo-kiriezu-owariya.json
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)  4599959 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/geoshape-city.csv
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1444 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/geoshape-city.json
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    10411 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/geoshape-pref.csv
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1390 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/geoshape-pref.json
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)  1594207 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/ksj-station-N02-2020.csv
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)  1388771 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/ksj-station-N02.csv
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1427 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/base_data/ksj-station-N02.json
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:30.991073 pygeonlp-1.2.2rc1/libgeonlp/
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:30.999073 pygeonlp-1.2.2rc1/libgeonlp/include/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2489 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Address.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3287 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/CSVReader.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8142 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/DBAccessor.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      488 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/DartsException.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1642 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Dictionary.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2051 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Exception.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      802 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/FileAccessor.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      531 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/FormatException.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8107 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/GeonlpMA.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8812 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/GeonlpMAImplSq3.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     7001 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Geoword.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1892 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/GeowordFormatter.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1180 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/MeCabAdapter.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6001 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Node.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3786 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/NodeExt.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1868 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/PHBSDefs.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3849 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Profile.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      587 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/SqliteErrException.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      487 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/SqliteNotInitializedException.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1701 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Suffix.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1634 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Util.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2891 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/Wordlist.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2972 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/config.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    14376 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/darts.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    22050 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/picojson.h
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6482 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/include/picojsonExt.h
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.003073 pygeonlp-1.2.2rc1/libgeonlp/lib/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1693 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Address.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3851 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/CSVReader.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    48756 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/DBAccessor.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2376 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Dictionary.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     4969 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/FileAccessor.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2563 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/GeonlpMA.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    40116 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/GeonlpMAImplSq3.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6819 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Geoword.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3552 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/GeowordFormatter.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2449 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/MeCabAdapter.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2930 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Node.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6462 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/NodeExt.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3586 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/PHBSDefs.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     9933 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Profile.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6077 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/Util.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    14075 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/lib/picojsonExt.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     4889 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/py2pico.cpp
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    14335 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/libgeonlp/pygeonlp.cpp
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:30.955072 pygeonlp-1.2.2rc1/pygeonlp/
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/pygeonlp/api/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    36660 2023-12-05 04:28:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/__init__.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     9279 2023-12-05 07:29:45.000000 pygeonlp-1.2.2rc1/pygeonlp/api/__main__.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    10658 2023-12-07 01:29:32.000000 pygeonlp-1.2.2rc1/pygeonlp/api/devtool.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    18982 2023-12-05 05:29:11.000000 pygeonlp-1.2.2rc1/pygeonlp/api/dict_manager.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8138 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/dictionary.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    19166 2023-07-11 06:20:04.000000 pygeonlp-1.2.2rc1/pygeonlp/api/filter.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    14057 2023-12-07 01:29:32.000000 pygeonlp-1.2.2rc1/pygeonlp/api/linker.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8553 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/metadata.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    12127 2023-07-14 05:37:44.000000 pygeonlp-1.2.2rc1/pygeonlp/api/node.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    31822 2023-07-14 05:37:44.000000 pygeonlp-1.2.2rc1/pygeonlp/api/parser.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     7618 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/scoring.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    26614 2023-12-07 01:29:32.000000 pygeonlp-1.2.2rc1/pygeonlp/api/service.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    12857 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/spatial_filter.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    20968 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/temporal_filter.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    12880 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/api/workflow.py
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/pygeonlp/samples/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)    11834 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/samples/context.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     1774 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/samples/sample_myscore.py
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/pygeonlp/tests/
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)        0 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/__init__.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     3521 2023-07-14 05:37:44.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_api.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     6026 2023-07-11 06:10:43.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_api_geocoder.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     8499 2023-07-11 06:10:43.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_api_geocoder_neologd.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2341 2023-07-11 06:10:43.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_doctest.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      149 2023-07-11 06:20:04.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_issue1.py
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     2444 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pygeonlp/tests/test_multiprocess.py
+drwxrwxr-x   0 sagara    (1000) sagara    (1000)        0 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/pygeonlp.egg-info/
+-rw-r--r--   0 sagara    (1000) sagara    (1000)     6579 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/PKG-INFO
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     4116 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)        1 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)       56 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/entry_points.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      122 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/requires.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)        9 2023-12-07 01:55:30.000000 pygeonlp-1.2.2rc1/pygeonlp.egg-info/top_level.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      100 2023-07-11 04:45:08.000000 pygeonlp-1.2.2rc1/pyproject.toml
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)      531 2023-10-05 00:43:02.000000 pygeonlp-1.2.2rc1/requirements.txt
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)       38 2023-12-07 01:55:31.007073 pygeonlp-1.2.2rc1/setup.cfg
+-rw-rw-r--   0 sagara    (1000) sagara    (1000)     5122 2023-12-03 04:53:22.000000 pygeonlp-1.2.2rc1/setup.py
```

### Comparing `pygeonlp-1.2.2.post1/LICENSE` & `pygeonlp-1.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/PKG-INFO` & `pygeonlp-1.2.2rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeonlp
-Version: 1.2.2.post1
+Version: 1.2.2rc1
 Summary: A Python module for geotagging Japanese texts.
 Home-page: https://github.com/geonlp-platform/pygeonlp
 Author: GeoNLP Project Team
 Author-email: geonlp@nii.ac.jp
 License: 2-Clause "Simplified" BSD License
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
@@ -20,17 +20,17 @@
 
 # pygeonlp, A python module for geotagging Japanese texts
 
 `pygeonlp` is an open source software for geotagging/geoparsing 
 Japanese natural language text to extract place names.
 
 More detailed Japanese documentation and API references are available
-in the [/docs/source](./docs/source) directory.
+in the [/doc](./doc/) directory.
 You can also find the latest online documentation at
-[PyGeoNLP Reference](https://pygeonlp.readthedocs.io/latest/).
+[GeoNLP Documentation](https://geonlp.ex.nii.ac.jp/doc/pygeonlp/).
 
 ## How To Use
 
 Import `pygeonlp.api` and initialize it by specifying the directory
 where the place-name database is placed.
 
 ```python
```

### Comparing `pygeonlp-1.2.2.post1/README.md` & `pygeonlp-1.2.2rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # pygeonlp, A python module for geotagging Japanese texts
 
 `pygeonlp` is an open source software for geotagging/geoparsing 
 Japanese natural language text to extract place names.
 
 More detailed Japanese documentation and API references are available
-in the [/docs/source](./docs/source) directory.
+in the [/doc](./doc/) directory.
 You can also find the latest online documentation at
-[PyGeoNLP Reference](https://pygeonlp.readthedocs.io/latest/).
+[GeoNLP Documentation](https://geonlp.ex.nii.ac.jp/doc/pygeonlp/).
 
 ## How To Use
 
 Import `pygeonlp.api` and initialize it by specifying the directory
 where the place-name database is placed.
 
 ```python
```

### Comparing `pygeonlp-1.2.2.post1/README_ja.md` & `pygeonlp-1.2.2rc1/README_ja.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # pygeonlp, A python module for geotagging Japanese texts
 
 `pygeonlp` は、自然言語テキストを解析して地名を抽出する
 ジオタギング (geo-tagging) またはジオパージング (geo-parsing) と呼ばれる処理を行なうオープンソースソフトウェアです。
 
-より詳細なドキュメントと API リファレンスが[/docs/source](./docs/source)
-ディレクトリの下にあります。
+より詳細なドキュメントと API リファレンスが [/doc](./doc/) ディレクトリの下にあります。
 また、最新のオンラインドキュメントは
-[PyGeoNLP Reference](https://pygeonlp.readthedocs.io/latest/)
+[GeoNLP Documentation](https://geonlp.ex.nii.ac.jp/doc/pygeonlp/)
 からも参照できます。
 
 ## 使い方
 
 `pygeonlp.api` をインポートし、地名語解析辞書を登録したデータベースが
 置かれているディレクトリを指定して初期化します。
```

### Comparing `pygeonlp-1.2.2.post1/base_data/edo-kiriezu-owariya.csv` & `pygeonlp-1.2.2rc1/base_data/edo-kiriezu-owariya.csv`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/edo-kiriezu-owariya.json` & `pygeonlp-1.2.2rc1/base_data/edo-kiriezu-owariya.json`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/geoshape-city.csv` & `pygeonlp-1.2.2rc1/base_data/geoshape-city.csv`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/geoshape-city.json` & `pygeonlp-1.2.2rc1/base_data/geoshape-city.json`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/geoshape-pref.csv` & `pygeonlp-1.2.2rc1/base_data/geoshape-pref.csv`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/geoshape-pref.json` & `pygeonlp-1.2.2rc1/base_data/geoshape-pref.json`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/ksj-station-N02-2020.csv` & `pygeonlp-1.2.2rc1/base_data/ksj-station-N02-2020.csv`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/ksj-station-N02.csv` & `pygeonlp-1.2.2rc1/base_data/ksj-station-N02.csv`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/base_data/ksj-station-N02.json` & `pygeonlp-1.2.2rc1/base_data/ksj-station-N02.json`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Address.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Address.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/CSVReader.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/CSVReader.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/DBAccessor.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/DBAccessor.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Dictionary.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Dictionary.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Exception.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Exception.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/FileAccessor.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/FileAccessor.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/FormatException.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/FormatException.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/GeonlpMA.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/GeonlpMA.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/GeonlpMAImplSq3.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/GeonlpMAImplSq3.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Geoword.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Geoword.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/GeowordFormatter.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/GeowordFormatter.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/MeCabAdapter.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/MeCabAdapter.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Node.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Node.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/NodeExt.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/NodeExt.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/PHBSDefs.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/PHBSDefs.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Profile.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Profile.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/SqliteErrException.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/SqliteErrException.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Suffix.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Suffix.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Util.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Util.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/Wordlist.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/Wordlist.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/config.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/config.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/darts.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/darts.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/picojson.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/picojson.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/include/picojsonExt.h` & `pygeonlp-1.2.2rc1/libgeonlp/include/picojsonExt.h`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Address.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Address.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/CSVReader.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/CSVReader.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/DBAccessor.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/DBAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Dictionary.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Dictionary.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     return dic;
   }
 
   // 必須項目が揃っていることを確認する
   bool Dictionary::isValid(std::string& err) const {
     if (this->get_identifier().length() == 0) return false;
     if (this->get_name().length() == 0) return false;
-    // if (this->get_content_url().length() == 0) return false;
+    if (this->get_content_url().length() == 0) return false;
     return true;
   }
 
   bool Dictionary::isValid(void) const {
     std::string err("");
     return this->isValid(err);
   }
@@ -53,16 +53,15 @@
   }
 
   // CSV の置かれている場所を指す URL を取得する
   // "/distribution[0]/contentUrl"
   const std::string Dictionary::get_content_url(void) const {
     picojson::value v = this->get_value("distribution");
     if (!v.is<picojson::array>()) {
-      return "";  // No distribution url.
-      // throw std::runtime_error("'distribution' element must be an array.");
+      throw std::runtime_error("'distribution' element must be an array.");
     }
     picojson::array dist_list = v.get<picojson::array>();
     for (picojson::array::iterator it = dist_list.begin(); it != dist_list.end(); it++) {
       if (!(*it).is<picojson::object>()) continue;
       picojson::value v2 = (*it).get("contentUrl");
       if (v2.is<std::string>()) {
         return v2.get<std::string>();
```

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/FileAccessor.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/FileAccessor.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/GeonlpMA.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/GeonlpMA.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/GeonlpMAImplSq3.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/GeonlpMAImplSq3.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Geoword.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Geoword.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/GeowordFormatter.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/GeowordFormatter.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/MeCabAdapter.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/MeCabAdapter.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Node.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Node.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/NodeExt.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/NodeExt.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/PHBSDefs.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/PHBSDefs.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Profile.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Profile.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/Util.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/Util.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/lib/picojsonExt.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/lib/picojsonExt.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/py2pico.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/py2pico.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/libgeonlp/pygeonlp.cpp` & `pygeonlp-1.2.2rc1/libgeonlp/pygeonlp.cpp`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/__init__.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pygeonlp.api.dict_manager import DictManager
 from pygeonlp.api.workflow import Workflow, WorkflowError
 
 logger = getLogger(__name__)
 _default_workflow = None
 _default_manager = None
 
-__version__ = '1.2.2.post1'
+__version__ = '1.2.2rc1'
 
 
 def get_db_dir():
     """
     データベースディレクトリを取得します。
     データベースディレクトリは次の優先順位に従って決定します。
 
@@ -27,15 +27,15 @@
     終了します。
 
     Return
     ------
     str
         ディレクトリの絶対パス。
     """
-    # 環境変数 GEONLP_DB_DIR をチェック
+    # 環境変数 GEONLP_DIR をチェック
     db_dir = os.environ.get('GEONLP_DB_DIR')
     if db_dir:
         db_dir = os.path.abspath(db_dir)
 
     # 環境変数 HOME が利用できれば $HOME/geonlp/db
     home = os.environ.get('HOME')
     if not db_dir and home:
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/__main__.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 HELP = """
 'pygeonlp' は、自然言語テキストを解析して地名を抽出する
 ジオタギング (geo-tagging) またはジオパージング (geo-parsing) と呼ばれる
 処理を行なうオープンソースソフトウェアです。
 
 Usage:
   {p} -h
-  {p} --version
   {p} geoparse [--db-dir=<dir>] [--json] [<file>]
-  {p} search [--db-dir=<dir>] <word>
   {p} list-dictionaries [--db-dir=<dir>]
   {p} show-dictionary [--db-dir=<dir>] <id>
   {p} clear-dictionaries [--db-dir=<dir>]
   {p} add-dictionary [--db-dir=<dir>] (<json-path> <csv-path> | <url>)
   {p} remove-dictionary [--db-dir=<dir>] <id>
   {p} download-dictionary [--db-dir=<dir>] <url> <json-path> <csv-path>
   {p} setup [--db-dir=<dir>] [<dict-src-dir>]
@@ -32,18 +30,15 @@
 Options:
   -h --help           このヘルプを表示します。
   --json              JSON で出力します。
   --db-dir=<dir>      データベースディレクトリを指定します。
 
 Examples:
 - "test.txt" のテキストをジオパーズした結果を出力します
-  {p} geoparse test.txt
-
-- "神保町" をデータベースから検索します
-  {p} search 神保町
+  {p} geoparse test.txt    
 
 - パッケージに同梱されている辞書ファイルから初期データベースを設定します
   {p} setup
 
 - インストールされている辞書情報一覧を表示します
   {p} list-dictionaries
 
@@ -62,15 +57,15 @@
 
 - ウェブから辞書をダウンロードし、JSONおよびCSVファイルに保存します
   {p} download-dictionary https://geonlp.ex.nii.ac.jp/dictionary/geoshape-city/ geoshape.json geoshape.csv
 
 - JSONおよびCSVファイルから辞書をインストールします
   {p} add-dictionary base_data/geoshape-city.json base_data/geoshape-city.csv
 
-""".format(p='pygeonlp')
+""".format(p='pygeonlp.api')
 
 
 def setup_basic_database(db_dir=None, src_dir=None):
     """
     基本的な地名解析辞書を登録したデータベースを作成します。
 
     Parameters
@@ -147,18 +142,14 @@
     if updated:
         manager.updateIndex()
 
 
 def main():
     args = docopt(HELP)
 
-    if args['--version']:
-        print(pygeonlp.api.__version__)
-        exit(0)
-
     if args['--db-dir']:
         db_dir = args['--db-dir']
     else:
         db_dir = pygeonlp.api.get_db_dir()
 
     manager = pygeonlp.api.dict_manager.DictManager(db_dir)
     if manager.capi_ma is None and args['setup'] is False:
@@ -200,20 +191,14 @@
                     if args['--json']:
                         print(json.dumps(geojson, ensure_ascii=False))
                     else:
                         pp_mecab(geojson)
 
         exit(0)
 
-    if args['search']:
-        pygeonlp.api.init(db_dir=db_dir)
-        word = pygeonlp.api.searchWord(args["<word>"])
-        print(json.dumps(word, ensure_ascii=False))
-        exit(0)
-
     if args['list-dictionaries']:
         for metadata in manager.getDictionaries():
             dic = json.loads(metadata.jsonld)
             print("{} : {}\n- {}\n{}\n".format(
                 metadata.get_identifier(),
                 metadata.get_name(),
                 dic["url"],
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/devtool.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/devtool.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,18 +231,25 @@
             morphemes["prononciation"],
         )
 
     if node_type == "NORMAL":
         geo = tuple()
     elif node_type == "GEOWORD":
         geoword_properties = geojson["properties"]["geoword_properties"]
-        prefix = geoword_properties["prefix"][0] \
-          if "prefix" in geoword_properties else ""
-        suffix = geoword_properties["suffix"][0] \
-          if "suffix" in geoword_properties else ""
+        prefix = ""
+        if "prefix" in geoword_properties:
+            for k in geoword_properties["prefix"]:
+                if len(k) > len(prefix):
+                    prefix = k
+
+        suffix = ""
+        if "suffix" in geoword_properties:
+            for k in geoword_properties["suffix"]:
+                if len(k) > len(suffix):
+                    suffix = k
 
         geo = (
             geoword_properties["ne_class"],
             geoword_properties["geolod_id"],
             prefix + geoword_properties["body"] + suffix,
             geoword_properties["longitude"],
             geoword_properties["latitude"],
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/dict_manager.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/dict_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,17 @@
         """
         指定したパスにある辞書メタデータ（JSONファイル）と
         地名解析辞書（CSVファイル）をデータベースに登録します。
 
         既に同じ identifier を持つ辞書データがデータベースに登録されている場合、
         削除してから新しい辞書データを登録します。
 
+        登録した辞書を利用可能にするには、 ``setActivateDictionaries()``
+        または ``activateDictionaires()`` で有効化する必要があります。
+
         Parameters
         ----------
         jsonfile : str
             辞書メタデータファイルのパス。
         csvfile : str
             地名解析辞書ファイルのパス。
 
@@ -182,14 +185,17 @@
         指定した URL にあるページに含まれる辞書メタデータ（JSON-LD）を取得し、
         メタデータに記載されている URL から地名解析辞書（CSVファイル）を取得し、
         データベースに登録します。
 
         既に同じ identifier を持つ辞書データがデータベースに登録されている場合、
         削除してから新しい辞書データを登録します。
 
+        登録した辞書を利用可能にするには、 ``setActivateDictionaries()``
+        または ``activateDictionaires()`` で有効化する必要があります。
+
         Parameters
         ----------
         url : str
             辞書メタデータを含むウェブページの URL。
         params : dict, optional
             requests.get に渡す params パラメータ。
         **kwargs : dict, optional
@@ -225,14 +231,17 @@
 
         辞書の name と identifier を省略した場合、
         CSV ファイル名から自動的に設定されます。
 
         既に同じ identifier を持つ辞書データがデータベースに登録されている場合、
         削除してから新しい辞書データを登録します。
 
+        登録した辞書を利用可能にするには、 ``setActivateDictionaries()``
+        または ``activateDictionaries()`` で有効化する必要があります。
+
         Parameters
         ----------
         csvfile : str
             地名解析辞書ファイルのパス。
         name : str, optional
             辞書名。省略した場合、 CSV ファイルの basename を利用します。
         identifier : str, optional
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/dictionary.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/filter.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/filter.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/linker.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/linker.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/metadata.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
             for identifier in identifiers:
                 if identifier.startswith('geonlp:'):
                     return identifier
 
         except (IndexError, TypeError):
             raise MetadataError(
-                ("json-ldから 'geonlp:' で始まる identifier を見つけられません。"
+                ("json-ld から identifier を見つけられません。"
                  "{}".format(self.jsonld)))
 
         raise MetadataError(
             ("json-ldから identifier を見つけられません。"
              "{}".format(self.jsonld)))
         return None
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/node.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/node.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/parser.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/parser.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/scoring.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/scoring.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/service.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         address_class : str
             住所要素とみなす固有名クラスを正規表現で指定します。
             たとえば固有名クラスが「都道府県」である地名語から始まる住所表記だけを
             住所として解析したい（市区町村から始まる場合は無視したい）場合は
             r"^都道府県" を指定します。
             デフォルト値は r"^(都道府県|市区町村|行政地域|居住地名)(/.+|)" です。
-            環境変数 GEONLP_ADRESS_CLASS でデフォルト値を設定できます。
+            環境変数 GEONLP_DRESS_CLASS でデフォルト値を設定できます。
 
         system_dic_dir : str
             MeCab システム辞書のディレクトリを指定します。
             省略した場合はデフォルトシステム辞書を利用します。
             環境変数 GEONLP_MECAB_DIC_DIR でデフォルト値を設定できます。
         """
         self._dict_cache = {}
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/spatial_filter.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/spatial_filter.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/temporal_filter.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/temporal_filter.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/api/workflow.py` & `pygeonlp-1.2.2rc1/pygeonlp/api/workflow.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/samples/context.py` & `pygeonlp-1.2.2rc1/pygeonlp/samples/context.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/samples/sample_myscore.py` & `pygeonlp-1.2.2rc1/pygeonlp/samples/sample_myscore.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/tests/test_api.py` & `pygeonlp-1.2.2rc1/pygeonlp/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.dictmanager = api.dict_manager.DictManager(db_dir=testdir)
         self.dictmanager.setupBasicDatabase()
         api.init(db_dir=testdir)
 
     def test_search_word(self):
         words = self.service.searchWord('神保町')
         self.assertIsInstance(words, dict)
-        self.assertIn('uN6ecI', words)  # 新宿線神保町駅
+        self.assertIn('AGGwyc', words)  # 新宿線神保町駅
 
     def test_set_dictionaries(self):
         # Set active dictionaries and check the results
         self.service.setActiveDictionaries(pattern=r'.*')
         words = self.service.searchWord('和歌山市')
         self.assertIsInstance(words, dict)
         self.assertEqual(len(words.keys()), 4)
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/tests/test_api_geocoder.py` & `pygeonlp-1.2.2rc1/pygeonlp/tests/test_api_geocoder.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/tests/test_api_geocoder_neologd.py` & `pygeonlp-1.2.2rc1/pygeonlp/tests/test_api_geocoder_neologd.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/tests/test_doctest.py` & `pygeonlp-1.2.2rc1/pygeonlp/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp/tests/test_multiprocess.py` & `pygeonlp-1.2.2rc1/pygeonlp/tests/test_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pygeonlp-1.2.2.post1/pygeonlp.egg-info/PKG-INFO` & `pygeonlp-1.2.2rc1/pygeonlp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeonlp
-Version: 1.2.2.post1
+Version: 1.2.2rc1
 Summary: A Python module for geotagging Japanese texts.
 Home-page: https://github.com/geonlp-platform/pygeonlp
 Author: GeoNLP Project Team
 Author-email: geonlp@nii.ac.jp
 License: 2-Clause "Simplified" BSD License
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
@@ -20,17 +20,17 @@
 
 # pygeonlp, A python module for geotagging Japanese texts
 
 `pygeonlp` is an open source software for geotagging/geoparsing 
 Japanese natural language text to extract place names.
 
 More detailed Japanese documentation and API references are available
-in the [/docs/source](./docs/source) directory.
+in the [/doc](./doc/) directory.
 You can also find the latest online documentation at
-[PyGeoNLP Reference](https://pygeonlp.readthedocs.io/latest/).
+[GeoNLP Documentation](https://geonlp.ex.nii.ac.jp/doc/pygeonlp/).
 
 ## How To Use
 
 Import `pygeonlp.api` and initialize it by specifying the directory
 where the place-name database is placed.
 
 ```python
```

### Comparing `pygeonlp-1.2.2.post1/pygeonlp.egg-info/SOURCES.txt` & `pygeonlp-1.2.2rc1/pygeonlp.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -106,20 +106,13 @@
 pygeonlp/api/service.py
 pygeonlp/api/spatial_filter.py
 pygeonlp/api/temporal_filter.py
 pygeonlp/api/workflow.py
 pygeonlp/samples/context.py
 pygeonlp/samples/sample_myscore.py
 pygeonlp/tests/__init__.py
-pygeonlp/tests/conftest.py
 pygeonlp/tests/test_api.py
 pygeonlp/tests/test_api_geocoder.py
 pygeonlp/tests/test_api_geocoder_neologd.py
 pygeonlp/tests/test_doctest.py
 pygeonlp/tests/test_issue1.py
-pygeonlp/tests/test_multiprocess.py
-pygeonlp/webapi/__init__.py
-pygeonlp/webapi/app.py
-pygeonlp/webapi/tests/__init__.py
-pygeonlp/webapi/tests/conftest.py
-pygeonlp/webapi/tests/helpers.py
-pygeonlp/webapi/tests/test_webapi.py
+pygeonlp/tests/test_multiprocess.py
```

### Comparing `pygeonlp-1.2.2.post1/setup.py` & `pygeonlp-1.2.2rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,23 +136,23 @@
     )
     return libgeonlp
 
 
 # Setup tools
 setup(
     name='pygeonlp',
-    version='1.2.2.post1',
+    version='1.2.2rc1',
     description='A Python module for geotagging Japanese texts.',
     author='GeoNLP Project Team',
     author_email='geonlp@nii.ac.jp',
     url='https://github.com/geonlp-platform/pygeonlp',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     ext_modules=[get_libgeonlp()],
-    packages=['pygeonlp.api', 'pygeonlp.webapi'],
+    packages=['pygeonlp.api', 'pygeonlp.tests'],
     entry_points={
         'console_scripts': [
             'pygeonlp = pygeonlp.api.__main__:main'
         ]
     },
     test_suite='pygeonlp.tests',
     python_requires='>=3.6.8',
```

