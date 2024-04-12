# Comparing `tmp/turkish-profile-generator-0.1.0.tar.gz` & `tmp/turkish_profile_generator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turkish-profile-generator-0.1.0.tar", last modified: Fri Apr 12 19:58:34 2024, max compression
+gzip compressed data, was "turkish_profile_generator-0.1.6.tar", last modified: Fri Apr 12 21:06:53 2024, max compression
```

## Comparing `turkish-profile-generator-0.1.0.tar` & `turkish_profile_generator-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 19:58:34.275915 turkish-profile-generator-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-04-12 19:39:06.000000 turkish-profile-generator-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1055 2024-04-12 19:58:34.275915 turkish-profile-generator-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      506 2024-04-12 19:43:48.000000 turkish-profile-generator-0.1.0/README.md
--rw-rw-rw-   0        0        0      352 2024-04-12 19:45:32.000000 turkish-profile-generator-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 19:58:34.275915 turkish-profile-generator-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      748 2024-04-12 19:55:32.000000 turkish-profile-generator-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 19:58:34.275915 turkish-profile-generator-0.1.0/turkish_profile_generator.egg-info/
--rw-rw-rw-   0        0        0     1055 2024-04-12 19:58:34.000000 turkish-profile-generator-0.1.0/turkish_profile_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-04-12 19:58:34.000000 turkish-profile-generator-0.1.0/turkish_profile_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 19:58:34.000000 turkish-profile-generator-0.1.0/turkish_profile_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 19:58:34.000000 turkish-profile-generator-0.1.0/turkish_profile_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 21:06:53.080294 turkish_profile_generator-0.1.6/
+-rw-rw-rw-   0        0        0      298 2024-04-12 21:06:53.080294 turkish_profile_generator-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-12 21:06:53.080294 turkish_profile_generator-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-04-12 21:06:19.000000 turkish_profile_generator-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 21:06:53.080294 turkish_profile_generator-0.1.6/turkish_profile_generator.egg-info/
+-rw-rw-rw-   0        0        0      298 2024-04-12 21:06:52.000000 turkish_profile_generator-0.1.6/turkish_profile_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-04-12 21:06:52.000000 turkish_profile_generator-0.1.6/turkish_profile_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 21:06:52.000000 turkish_profile_generator-0.1.6/turkish_profile_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 21:06:52.000000 turkish_profile_generator-0.1.6/turkish_profile_generator.egg-info/top_level.txt
```

