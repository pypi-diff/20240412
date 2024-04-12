# Comparing `tmp/biorobot-0.1.6.tar.gz` & `tmp/biorobot-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biorobot-0.1.6.tar", last modified: Thu Apr 11 09:18:31 2024, max compression
+gzip compressed data, was "biorobot-0.1.7.tar", last modified: Fri Apr 12 11:53:19 2024, max compression
```

## Comparing `biorobot-0.1.6.tar` & `biorobot-0.1.7.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.947706 biorobot-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-11 09:18:27.000000 biorobot-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 09:18:27.000000 biorobot-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-11 09:18:31.947706 biorobot-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-11 09:18:27.000000 biorobot-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.935706 biorobot-0.1.6/biorobot/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.935706 biorobot-0.1.6/biorobot/brittle_star/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.935706 biorobot-0.1.6/biorobot/brittle_star/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.935706 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.935706 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/environment/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/shared/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/shared/mjc_observables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/shared/mjx_observables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/dual.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/arena/aquarium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.939706 biorobot-0.1.6/biorobot/brittle_star/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/usage_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/usage_examples/light_escape_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/environment/mjc_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/environment/mjx_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/mjcf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/mjcf/arena/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/arena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/arena/arena.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/arena/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/morphology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/torso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/usage_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.943706 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/example_usage_single.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.947706 biorobot-0.1.6/biorobot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/utils/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-11 09:18:27.000000 biorobot-0.1.6/biorobot/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:18:31.947706 biorobot-0.1.6/biorobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-11 09:18:31.000000 biorobot-0.1.6/biorobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-11 09:18:31.000000 biorobot-0.1.6/biorobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:18:31.000000 biorobot-0.1.6/biorobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 09:18:31.000000 biorobot-0.1.6/biorobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 09:18:31.000000 biorobot-0.1.6/biorobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-11 09:18:27.000000 biorobot-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 09:18:27.000000 biorobot-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:18:31.947706 biorobot-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-11 09:18:27.000000 biorobot-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.145481 biorobot-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 11:53:14.000000 biorobot-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 11:53:14.000000 biorobot-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-12 11:53:19.141481 biorobot-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-12 11:53:14.000000 biorobot-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/brittle_star/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.129481 biorobot-0.1.7/biorobot/brittle_star/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjc_observables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjx_observables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/dual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.133481 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/aquarium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/brittle_star/usage_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/directed_locomotion_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_vectorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/mjc_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/environment/mjx_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/mjcf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.137481 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/arena.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/arena/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/morphology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/torso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 11:53:14.000000 biorobot-0.1.7/biorobot/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:53:19.141481 biorobot-0.1.7/biorobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 11:53:19.000000 biorobot-0.1.7/biorobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 11:53:14.000000 biorobot-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 11:53:14.000000 biorobot-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:53:19.145481 biorobot-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 11:53:14.000000 biorobot-0.1.7/setup.py
```

### Comparing `biorobot-0.1.6/LICENSE` & `biorobot-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/PKG-INFO` & `biorobot-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.6 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.7 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.6/README.md` & `biorobot-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/dual.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/directed_locomotion/shared.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/directed_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/dual.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/mjc_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/mjx_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/light_escape/shared.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/light_escape/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/shared/base.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/shared/base.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/shared/mjc_observables.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjc_observables.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,24 +46,42 @@
             [
                 state.mj_data.sensordata[sensor.adr[0] : sensor.adr[0] + sensor.dim[0]]
                 for sensor in joint_vel_sensors
             ]
         ).flatten(),
     )
 
-    # All actuator torques
-    actuator_frc_sensors = [
+    # All joint actuator torques
+    joint_actuator_frc_sensors = [
         sensor
         for sensor in sensors
         if sensor.type[0] == mujoco.mjtSensor.mjSENS_JOINTACTFRC
     ]
-    actuator_force_observable = MJCObservable(
+    joint_actuator_force_observable = MJCObservable(
         name="joint_actuator_force",
-        low=-np.inf * np.ones(len(actuator_frc_sensors)),
-        high=np.inf * np.ones(len(actuator_frc_sensors)),
+        low=-np.inf * np.ones(len(joint_actuator_frc_sensors)),
+        high=np.inf * np.ones(len(joint_actuator_frc_sensors)),
+        retriever=lambda state: np.array(
+            [
+                state.mj_data.sensordata[sensor.adr[0] : sensor.adr[0] + sensor.dim[0]]
+                for sensor in joint_actuator_frc_sensors
+            ]
+        ).flatten(),
+    )
+
+    # All actuator forces
+    actuator_frc_sensors = [
+        sensor
+        for sensor in sensors
+        if sensor.type[0] == mujoco.mjtSensor.mjSENS_ACTUATORFRC
+    ]
+    actuator_force_observable = MJCObservable(
+        name="actuator_force",
+        low=np.array([limits[0] for limits in mj_model.actuator_forcerange]),
+        high=np.array([limits[1] for limits in mj_model.actuator_forcerange]),
         retriever=lambda state: np.array(
             [
                 state.mj_data.sensordata[sensor.adr[0] : sensor.adr[0] + sensor.dim[0]]
                 for sensor in actuator_frc_sensors
             ]
         ).flatten(),
     )
@@ -187,14 +205,15 @@
             ]
         ),
     )
 
     return [
         joint_position_observable,
         joint_velocity_observable,
+        joint_actuator_force_observable,
         actuator_force_observable,
         touch_observable,
         disk_position_observable,
         disk_rotation_observable,
         disk_linvel_observable,
         disk_angvel_observable,
     ]
```

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/shared/mjx_observables.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/shared/mjx_observables.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,21 +33,50 @@
     joint_velocity_observable = MJXObservable(
         name="joint_velocity",
         low=-jnp.inf * jnp.ones(len(joints)),
         high=jnp.inf * jnp.ones(len(joints)),
         retriever=lambda state: state.mjx_data.qvel[joint_dof_adr],
     )
 
-    actuator_force_observable = MJXObservable(
+    joint_actuator_force_observable = MJXObservable(
         name="joint_actuator_force",
         low=-jnp.inf * jnp.ones(len(joint_dof_adr)),
         high=jnp.inf * jnp.ones(len(joint_dof_adr)),
         retriever=lambda state: state.mjx_data.qfrc_actuator[joint_dof_adr].flatten(),
     )
 
+    low_actuator_force_limit = jnp.array(
+        [limits[0] for limits in mj_model.actuator_forcerange]
+    )
+    high_actuator_force_limit = jnp.array(
+        [limits[1] for limits in mj_model.actuator_forcerange]
+    )
+
+    def calculate_actuator_force(state: MJXEnvState) -> jnp.ndarray:
+        l = state.mjx_data.actuator_length
+        v = state.mjx_data.actuator_velocity
+        gain = state.mjx_model.actuator_gainprm[:, 0]
+        b0 = state.mjx_model.actuator_biasprm[:, 0]
+        b1 = state.mjx_model.actuator_biasprm[:, 1]
+        b2 = state.mjx_model.actuator_biasprm[:, 2]
+        ctrl = state.mjx_data.ctrl
+
+        return jnp.clip(
+            gain * ctrl + b0 + b1 * l + b2 * v,
+            low_actuator_force_limit,
+            high_actuator_force_limit,
+        )
+
+    actuator_force_observable = MJXObservable(
+        name="actuator_force",
+        low=low_actuator_force_limit,
+        high=high_actuator_force_limit,
+        retriever=calculate_actuator_force,
+    )
+
     segment_capsule_geom_ids = jnp.array(
         [
             geom_id
             for geom_id in range(mj_model.ngeom)
             if "segment" in mj_model.geom(geom_id).name
             and "capsule" in mj_model.geom(geom_id).name
         ]
@@ -121,14 +150,15 @@
             morphology_freejoint_adr + 3 : morphology_freejoint_adr + 6
         ],
     )
 
     return [
         joint_position_observable,
         joint_velocity_observable,
+        joint_actuator_force_observable,
         actuator_force_observable,
         touch_observable,
         disk_position_observable,
         disk_rotation_observable,
         disk_linvel_observable,
         disk_angvel_observable,
     ]
```

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/dual.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/dual.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/environment/undirected_locomotion/shared.py` & `biorobot-0.1.7/biorobot/brittle_star/environment/undirected_locomotion/shared.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/arena/aquarium.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/arena/aquarium.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/morphology.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/arm.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/arm_segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,48 +119,56 @@
     def _get_strength(self, joint: _ElementImpl) -> float:
         strength = (
             self._segment_specification.radius.value
             * self.morphology_specification.actuation_specification.radius_to_strength_factor.value
         )
         return strength
 
-    def _configure_p_control_actuator(self, joint: _ElementImpl) -> None:
-        self.mjcf_model.actuator.add(
+    def _configure_p_control_actuator(self, joint: _ElementImpl) -> _ElementImpl:
+        return self.mjcf_model.actuator.add(
             "position",
             name=f"{joint.name}_p_control",
             joint=joint,
             kp=50,
             ctrllimited=True,
             ctrlrange=joint.range,
             forcelimited=True,
             forcerange=[-self._get_strength(joint), self._get_strength(joint)],
         )
 
     def _configure_p_control_actuators(self) -> None:
         if self.morphology_specification.actuation_specification.use_p_control.value:
-            self._configure_p_control_actuator(self._in_plane_joint)
-            self._configure_p_control_actuator(self._out_of_plane_joint)
+            self._in_plane_actuator = self._configure_p_control_actuator(
+                self._in_plane_joint
+            )
+            self._out_of_plane_actuator = self._configure_p_control_actuator(
+                self._out_of_plane_joint
+            )
 
-    def _configure_torque_control_actuator(self, joint: _ElementImpl) -> None:
-        self.mjcf_model.actuator.add(
+    def _configure_torque_control_actuator(self, joint: _ElementImpl) -> _ElementImpl:
+        return self.mjcf_model.actuator.add(
             "motor",
             name=f"{joint.name}_torque_control",
             joint=joint,
             ctrllimited=True,
             ctrlrange=[-self._get_strength(joint), self._get_strength(joint)],
             forcelimited=True,
             forcerange=[-self._get_strength(joint), self._get_strength(joint)],
         )
 
     def _configure_torque_control_actuators(self) -> None:
         if (
             self.morphology_specification.actuation_specification.use_torque_control.value
         ):
-            self._configure_torque_control_actuator(self._in_plane_joint)
-            self._configure_torque_control_actuator(self._out_of_plane_joint)
+            self._in_plane_actuator = self._configure_torque_control_actuator(
+                self._in_plane_joint
+            )
+            self._out_of_plane_actuator = self._configure_torque_control_actuator(
+                self._out_of_plane_joint
+            )
 
     def _configure_actuators(self) -> None:
         self._configure_p_control_actuators()
         self._configure_torque_control_actuators()
 
     def _configure_position_sensor(self) -> None:
         self.mjcf_model.sensor.add(
@@ -181,10 +189,23 @@
             "jointactuatorfrc", joint=joint, name=f"{joint.name}_actuatorfrc_sensor"
         )
 
     def _configure_joints_sensors(self) -> None:
         self._configure_joint_sensors(joint=self._in_plane_joint)
         self._configure_joint_sensors(joint=self._out_of_plane_joint)
 
+    def _configure_actuator_sensors(self) -> None:
+        self.mjcf_model.sensor.add(
+            "actuatorfrc",
+            actuator=self._in_plane_actuator,
+            name=f"{self._in_plane_actuator.name}_actuatorfrc_sensor",
+        )
+        self.mjcf_model.sensor.add(
+            "actuatorfrc",
+            actuator=self._out_of_plane_actuator,
+            name=f"{self._out_of_plane_actuator.name}_actuatorfrc_sensor",
+        )
+
     def _configure_sensors(self) -> None:
         self._configure_position_sensor()
         self._configure_joints_sensors()
+        self._configure_actuator_sensors()
```

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/parts/disk.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/parts/disk.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/default.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/default.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/mjcf/morphology/specification/specification.py` & `biorobot-0.1.7/biorobot/brittle_star/mjcf/morphology/specification/specification.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/usage_examples/directed_locomotion_single.py` & `biorobot-0.1.7/biorobot/brittle_star/usage_examples/directed_locomotion_single.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,14 @@
             rng, sub_rng = jax.random.split(rng, 2)
             return env.action_space.sample(rng=sub_rng), rng
 
     state = reset_fn(env_rng, [-1.0, 0.0, 0.05])
     while True:
         action, action_rng = action_sample_fn(action_rng)
         state = step_fn(state=state, action=action)
-        print(state.observations["joint_position"])
-        print(state.observations["joint_velocity"])
         print(state.observations["joint_actuator_force"])
+        print(state.observations["actuator_force"])
         print()
         post_render(env.render(state=state), env.environment_configuration)
         if state.terminated | state.truncated:
             state = reset_fn(env_rng)
     env.close()
```

### Comparing `biorobot-0.1.6/biorobot/brittle_star/usage_examples/light_escape_single.py` & `biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/usage_examples/light_escape_vectorized.py` & `biorobot-0.1.7/biorobot/brittle_star/usage_examples/light_escape_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py` & `biorobot-0.1.7/biorobot/brittle_star/usage_examples/undirected_locomotion_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/environment/mjc_env.py` & `biorobot-0.1.7/biorobot/toy_example/environment/mjc_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/environment/mjx_env.py` & `biorobot-0.1.7/biorobot/toy_example/environment/mjx_env.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/arena/arena.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/arena/arena.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/morphology.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/morphology.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/arm.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/arm_segment.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/parts/torso.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/parts/torso.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/default.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/default.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/mjcf/morphology/specification/specification.py` & `biorobot-0.1.7/biorobot/toy_example/mjcf/morphology/specification/specification.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/example_usage_single.py` & `biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py` & `biorobot-0.1.7/biorobot/toy_example/usage_examples/mjc/example_usage_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/example_usage_single.py` & `biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_single.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py` & `biorobot-0.1.7/biorobot/toy_example/usage_examples/mjx/example_usage_vectorized.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/utils/colors.py` & `biorobot-0.1.7/biorobot/utils/colors.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/utils/noise.py` & `biorobot-0.1.7/biorobot/utils/noise.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot/utils/video.py` & `biorobot-0.1.7/biorobot/utils/video.py`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/biorobot.egg-info/PKG-INFO` & `biorobot-0.1.7/biorobot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorobot
-Version: 0.1.6
+Version: 0.1.7
 Summary: The Bio-inspired Robotics Testbed (BRT).
 Home-page: https://github.com/Co-Evolve/brb
 Author-email: Dries Marzougui <dries.marzougui@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biorobot Version: 0.1.6 Summary: The Bio-inspired
+Metadata-Version: 2.1 Name: biorobot Version: 0.1.7 Summary: The Bio-inspired
 Robotics Testbed (BRT). Home-page: https://github.com/Co-Evolve/brb Author-
 email: Dries Marzougui
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/Co-Evolve/brt
 Project-URL: Repository, https://github.com/Co-Evolve/brt Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
```

### Comparing `biorobot-0.1.6/biorobot.egg-info/SOURCES.txt` & `biorobot-0.1.7/biorobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biorobot-0.1.6/pyproject.toml` & `biorobot-0.1.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "biorobot"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name = "Dries Marzougui", email = "dries.marzougui@gmail.com" },
 ]
 description = "The Bio-inspired Robotics Testbed (BRT)."
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "MIT" }
 classifiers = [
```

### Comparing `biorobot-0.1.6/setup.py` & `biorobot-0.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     license = f.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
         name='biorobot',
-        version='0.1.6',
+        version='0.1.7',
         description='The Bio-inspired Robotics Testbed.',
         long_description=readme,
         url='https://github.com/Co-Evolve/brb',
         license=license,
         packages=find_packages(exclude=('tests', 'docs')),
         install_requires=required
         )
```

