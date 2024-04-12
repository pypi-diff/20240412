# Comparing `tmp/TikTokApi-6.2.2.tar.gz` & `tmp/tiktokapi-6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TikTokApi-6.2.2.tar", last modified: Mon Mar 11 17:57:52 2024, max compression
+gzip compressed data, was "tiktokapi-6.3.tar", last modified: Fri Apr 12 17:24:16 2024, max compression
```

## Comparing `TikTokApi-6.2.2.tar` & `tiktokapi-6.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.647176 TikTokApi-6.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-03-11 17:57:52.647176 TikTokApi-6.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.643176 TikTokApi-6.2.2/TikTokApi/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.643176 TikTokApi-6.2.2/TikTokApi/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/hashtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/trending.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/api/video.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.643176 TikTokApi-6.2.2/TikTokApi/stealth/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.647176 TikTokApi-6.2.2/TikTokApi/stealth/js/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_csi.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_hairline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_load_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/generate_magic_arrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/iframe_contentWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/media_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_hardwareConcurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_userAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17591 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/webgl_vendor.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/js/window_outerdimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/stealth/stealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    17122 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/TikTokApi/tiktok.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.647176 TikTokApi-6.2.2/TikTokApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-03-11 17:57:52.000000 TikTokApi-6.2.2/TikTokApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-11 17:57:52.000000 TikTokApi-6.2.2/TikTokApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 17:57:52.000000 TikTokApi-6.2.2/TikTokApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 17:57:52.000000 TikTokApi-6.2.2/TikTokApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 17:57:52.000000 TikTokApi-6.2.2/TikTokApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-11 17:57:52.651176 TikTokApi-6.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:52.647176 TikTokApi-6.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_hashtag.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_sound.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_trending.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-11 17:57:43.000000 TikTokApi-6.2.2/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.190836 tiktokapi-6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 17:24:06.000000 tiktokapi-6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-12 17:24:06.000000 tiktokapi-6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-12 17:24:16.190836 tiktokapi-6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-12 17:24:06.000000 tiktokapi-6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.182836 tiktokapi-6.3/TikTokApi/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.182836 tiktokapi-6.3/TikTokApi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/trending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/api/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.182836 tiktokapi-6.3/TikTokApi/stealth/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.186836 tiktokapi-6.3/TikTokApi/stealth/js/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/chrome_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/chrome_csi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/chrome_hairline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/chrome_load_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/chrome_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/generate_magic_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/iframe_contentWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/media_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_hardwareConcurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_userAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/navigator_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17591 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/webgl_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/js/window_outerdimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/stealth/stealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-12 17:24:06.000000 tiktokapi-6.3/TikTokApi/tiktok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.190836 tiktokapi-6.3/TikTokApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-04-12 17:24:16.000000 tiktokapi-6.3/TikTokApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-12 17:24:16.000000 tiktokapi-6.3/TikTokApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:24:16.000000 tiktokapi-6.3/TikTokApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 17:24:16.000000 tiktokapi-6.3/TikTokApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 17:24:16.000000 tiktokapi-6.3/TikTokApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 17:24:16.190836 tiktokapi-6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 17:24:06.000000 tiktokapi-6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:16.190836 tiktokapi-6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_hashtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_trending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-12 17:24:06.000000 tiktokapi-6.3/tests/test_video.py
```

### Comparing `TikTokApi-6.2.2/LICENSE` & `tiktokapi-6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/LICENSE.txt` & `tiktokapi-6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/PKG-INFO` & `tiktokapi-6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 6.2.2
+Version: 6.3.0
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
 Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 6.2.2 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.3.0 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
 tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
 main Author: David Teather Author-email: contact.davidteather@gmail.com
 License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `TikTokApi-6.2.2/README.md` & `tiktokapi-6.3/README.md`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/comment.py` & `tiktokapi-6.3/TikTokApi/api/comment.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/hashtag.py` & `tiktokapi-6.3/TikTokApi/api/hashtag.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         if id is None:
             await self.info(**kwargs)
 
         found = 0
         while found < count:
             params = {
                 "challengeID": self.id,
-                "count": count,
+                "count": 35,
                 "cursor": cursor,
             }
 
             resp = await self.parent.make_request(
                 url="https://www.tiktok.com/api/challenge/item_list/",
                 params=params,
                 headers=kwargs.get("headers"),
```

### Comparing `TikTokApi-6.2.2/TikTokApi/api/search.py` & `tiktokapi-6.3/TikTokApi/api/search.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/sound.py` & `tiktokapi-6.3/TikTokApi/api/sound.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/trending.py` & `tiktokapi-6.3/TikTokApi/api/trending.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/user.py` & `tiktokapi-6.3/TikTokApi/api/user.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/api/video.py` & `tiktokapi-6.3/TikTokApi/api/video.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/exceptions.py` & `tiktokapi-6.3/TikTokApi/exceptions.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/helpers.py` & `tiktokapi-6.3/TikTokApi/helpers.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_app.py` & `tiktokapi-6.3/TikTokApi/stealth/js/chrome_app.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_csi.py` & `tiktokapi-6.3/TikTokApi/stealth/js/chrome_csi.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_load_times.py` & `tiktokapi-6.3/TikTokApi/stealth/js/chrome_load_times.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/chrome_runtime.py` & `tiktokapi-6.3/TikTokApi/stealth/js/chrome_runtime.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/generate_magic_arrays.py` & `tiktokapi-6.3/TikTokApi/stealth/js/generate_magic_arrays.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/iframe_contentWindow.py` & `tiktokapi-6.3/TikTokApi/stealth/js/iframe_contentWindow.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/media_codecs.py` & `tiktokapi-6.3/TikTokApi/stealth/js/media_codecs.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_permissions.py` & `tiktokapi-6.3/TikTokApi/stealth/js/navigator_permissions.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/navigator_plugins.py` & `tiktokapi-6.3/TikTokApi/stealth/js/navigator_plugins.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/utils.py` & `tiktokapi-6.3/TikTokApi/stealth/js/utils.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/js/webgl_vendor.py` & `tiktokapi-6.3/TikTokApi/stealth/js/webgl_vendor.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/stealth/stealth.py` & `tiktokapi-6.3/TikTokApi/stealth/stealth.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/TikTokApi/tiktok.py` & `tiktokapi-6.3/TikTokApi/tiktok.py`

 * *Files 9% similar despite different names*

```diff
@@ -208,14 +208,16 @@
         proxies: list = None,
         sleep_after=1,
         starting_url="https://www.tiktok.com",
         context_options: dict = {},
         override_browser_args: list[dict] = None,
         cookies: list[dict] = None,
         suppress_resource_load_types: list[str] = None,
+        browser: str = "chromium",
+        executable_path: str = None
     ):
         """
         Create sessions for use within the TikTokApi class.
 
         These sessions are what will carry out requesting your data from TikTok.
 
         Args:
@@ -226,29 +228,38 @@
             proxies (list): A list of proxies to use for the sessions
             sleep_after (int): The amount of time to sleep after creating a session, this is to allow the msToken to be generated.
             starting_url (str): The url to start the sessions on, this is usually https://www.tiktok.com.
             context_options (dict): Options to pass to the playwright context.
             override_browser_args (list[dict]): A list of dictionaries containing arguments to pass to the browser.
             cookies (list[dict]): A list of cookies to use for the sessions, you can get these from your cookies after visiting TikTok.
             suppress_resource_load_types (list[str]): Types of resources to suppress playwright from loading, excluding more types will make playwright faster.. Types: document, stylesheet, image, media, font, script, textrack, xhr, fetch, eventsource, websocket, manifest, other.
+            browser (str): specify either firefox or chromium, default is chromium
+            executable_path (str): Path to the browser executable
 
         Example Usage:
             .. code-block:: python
 
                 from TikTokApi import TikTokApi
                 with TikTokApi() as api:
                     await api.create_sessions(num_sessions=5, ms_tokens=['msToken1', 'msToken2'])
         """
         self.playwright = await async_playwright().start()
-        if headless and override_browser_args is None:
-            override_browser_args = ["--headless=new"]
-            headless = False  # managed by the arg
-        self.browser = await self.playwright.chromium.launch(
-            headless=headless, args=override_browser_args, proxy=random_choice(proxies)
-        )
+        if browser == "chromium":
+            if headless and override_browser_args is None:
+                override_browser_args = ["--headless=new"]
+                headless = False  # managed by the arg
+            self.browser = await self.playwright.chromium.launch(
+                headless=headless, args=override_browser_args, proxy=random_choice(proxies), executable_path=executable_path
+            )
+        elif browser == "firefox":
+            self.browser = await self.playwright.firefox.launch(
+                headless=headless, args=override_browser_args, proxy=random_choice(proxies), executable_path=executable_path
+            )
+        else:
+            raise ValueError("Invalid browser argument passed")
 
         await asyncio.gather(
             *(
                 self.__create_session(
                     proxy=random_choice(proxies),
                     ms_token=random_choice(ms_tokens),
                     url=starting_url,
@@ -413,15 +424,15 @@
                     )
                 params["msToken"] = ms_token
 
         encoded_params = f"{url}?{urlencode(params, safe='=', quote_via=quote)}"
         signed_url = await self.sign_url(encoded_params, session_index=i)
 
         retry_count = 0
-        while i < retries:
+        while retry_count < retries:
             retry_count += 1
             result = await self.run_fetch_script(
                 signed_url, headers=headers, session_index=i
             )
 
             if result is None:
                 raise Exception("TikTokApi.run_fetch_script returned None")
```

### Comparing `TikTokApi-6.2.2/TikTokApi.egg-info/PKG-INFO` & `tiktokapi-6.3/TikTokApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TikTokApi
-Version: 6.2.2
+Version: 6.3.0
 Summary: The Unofficial TikTok API Wrapper in Python 3.
 Home-page: https://github.com/davidteather/tiktok-api
 Download-URL: https://github.com/davidteather/TikTok-Api/tarball/main
 Author: David Teather
 Author-email: contact.davidteather@gmail.com
 License: MIT
 Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TikTokApi Version: 6.2.2 Summary: The Unofficial
+Metadata-Version: 2.1 Name: TikTokApi Version: 6.3.0 Summary: The Unofficial
 TikTok API Wrapper in Python 3. Home-page: https://github.com/davidteather/
 tiktok-api Download-URL: https://github.com/davidteather/TikTok-Api/tarball/
 main Author: David Teather Author-email: contact.davidteather@gmail.com
 License: MIT Keywords: tiktok,python3,api,unofficial,tiktok-api,tiktok api
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `TikTokApi-6.2.2/TikTokApi.egg-info/SOURCES.txt` & `tiktokapi-6.3/TikTokApi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/setup.py` & `tiktokapi-6.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TikTokApi",
     packages=setuptools.find_packages(),
-    version="6.2.2",
+    version="6.3.0",
     license="MIT",
     description="The Unofficial TikTok API Wrapper in Python 3.",
     author="David Teather",
     author_email="contact.davidteather@gmail.com",
     url="https://github.com/davidteather/tiktok-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `TikTokApi-6.2.2/tests/test_hashtag.py` & `tiktokapi-6.3/tests/test_hashtag.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/tests/test_integration.py` & `tiktokapi-6.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/tests/test_search.py` & `tiktokapi-6.3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/tests/test_sound.py` & `tiktokapi-6.3/tests/test_sound.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/tests/test_user.py` & `tiktokapi-6.3/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `TikTokApi-6.2.2/tests/test_video.py` & `tiktokapi-6.3/tests/test_video.py`

 * *Files identical despite different names*

