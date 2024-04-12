# Comparing `tmp/MohuPy-0.2.8.tar.gz` & `tmp/mohupy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MohuPy-0.2.8.tar", last modified: Sat Apr  6 08:34:23 2024, max compression
+gzip compressed data, was "mohupy-0.3.0.tar", last modified: Fri Apr 12 16:02:30 2024, max compression
```

## Comparing `MohuPy-0.2.8.tar` & `mohupy-0.3.0.tar`

### file list

```diff
@@ -1,81 +1,131 @@
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.387270 MohuPy-0.2.8/
--rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 MohuPy-0.2.8/LICENSE
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386714 MohuPy-0.2.8/MohuPy.egg-info/
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     1613 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/SOURCES.txt
--rw-r--r--   0 yibow      (501) staff       (20)        1 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/dependency_links.txt
--rw-r--r--   0 yibow      (501) staff       (20)       39 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/requires.txt
--rw-r--r--   0 yibow      (501) staff       (20)        7 2024-04-06 08:34:23.000000 MohuPy-0.2.8/MohuPy.egg-info/top_level.txt
--rw-r--r--   0 yibow      (501) staff       (20)     4175 2024-04-06 08:34:23.387029 MohuPy-0.2.8/PKG-INFO
--rw-r--r--   0 yibow      (501) staff       (20)     3581 2023-11-29 10:30:24.000000 MohuPy-0.2.8/README.md
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.377083 MohuPy-0.2.8/mohupy/
--rw-r--r--   0 yibow      (501) staff       (20)     1002 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.377498 MohuPy-0.2.8/mohupy/config/
--rw-r--r--   0 yibow      (501) staff       (20)      460 2023-11-29 07:37:14.000000 MohuPy-0.2.8/mohupy/config/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      268 2023-11-29 07:40:11.000000 MohuPy-0.2.8/mohupy/config/tnorms.py
--rw-r--r--   0 yibow      (501) staff       (20)     1233 2023-11-28 09:03:14.000000 MohuPy-0.2.8/mohupy/constant.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.379864 MohuPy-0.2.8/mohupy/core/
--rw-r--r--   0 yibow      (501) staff       (20)     1329 2024-04-06 07:57:17.000000 MohuPy-0.2.8/mohupy/core/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      549 2024-04-06 07:30:36.000000 MohuPy-0.2.8/mohupy/core/attribute.py
--rw-r--r--   0 yibow      (501) staff       (20)     6309 2024-04-06 06:10:13.000000 MohuPy-0.2.8/mohupy/core/attributeClass.py
--rw-r--r--   0 yibow      (501) staff       (20)     1656 2024-04-06 07:09:37.000000 MohuPy-0.2.8/mohupy/core/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     1922 2024-04-06 07:11:34.000000 MohuPy-0.2.8/mohupy/core/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)    22524 2024-04-06 07:29:37.000000 MohuPy-0.2.8/mohupy/core/funcitonClass.py
--rw-r--r--   0 yibow      (501) staff       (20)     2702 2024-04-06 07:29:47.000000 MohuPy-0.2.8/mohupy/core/function.py
--rw-r--r--   0 yibow      (501) staff       (20)     5156 2024-04-06 06:33:31.000000 MohuPy-0.2.8/mohupy/core/fuzzarray.py
--rw-r--r--   0 yibow      (501) staff       (20)     2905 2024-04-06 07:37:10.000000 MohuPy-0.2.8/mohupy/core/fuzznums.py
--rw-r--r--   0 yibow      (501) staff       (20)    20399 2024-04-06 07:11:56.000000 MohuPy-0.2.8/mohupy/core/operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     2661 2024-04-06 07:21:11.000000 MohuPy-0.2.8/mohupy/core/operationClass.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.380615 MohuPy-0.2.8/mohupy/core/operationLib/
--rw-r--r--   0 yibow      (501) staff       (20)      617 2024-04-06 06:52:42.000000 MohuPy-0.2.8/mohupy/core/operationLib/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4127 2024-04-06 06:47:12.000000 MohuPy-0.2.8/mohupy/core/operationLib/algebraic.py
--rw-r--r--   0 yibow      (501) staff       (20)     4169 2024-04-06 06:57:19.000000 MohuPy-0.2.8/mohupy/core/operationLib/algebraicoperation.py
--rw-r--r--   0 yibow      (501) staff       (20)     1214 2024-04-06 06:48:09.000000 MohuPy-0.2.8/mohupy/core/operationLib/einstein.py
--rw-r--r--   0 yibow      (501) staff       (20)     1181 2024-04-06 07:14:44.000000 MohuPy-0.2.8/mohupy/core/operationpackage.py
--rw-r--r--   0 yibow      (501) staff       (20)     1722 2024-04-06 06:36:47.000000 MohuPy-0.2.8/mohupy/core/regedit.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.381190 MohuPy-0.2.8/mohupy/function/
--rw-r--r--   0 yibow      (501) staff       (20)      420 2023-09-23 06:14:48.000000 MohuPy-0.2.8/mohupy/function/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     9147 2023-10-01 12:31:19.000000 MohuPy-0.2.8/mohupy/function/func.py
--rw-r--r--   0 yibow      (501) staff       (20)     4505 2023-10-01 12:31:54.000000 MohuPy-0.2.8/mohupy/function/mem_func.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.381372 MohuPy-0.2.8/mohupy/generator/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 MohuPy-0.2.8/mohupy/generator/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.382726 MohuPy-0.2.8/mohupy/lib/
--rw-r--r--   0 yibow      (501) staff       (20)     1333 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/lib/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      491 2023-11-28 10:38:49.000000 MohuPy-0.2.8/mohupy/lib/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     3968 2024-04-06 07:49:52.000000 MohuPy-0.2.8/mohupy/lib/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4673 2024-04-06 07:51:48.000000 MohuPy-0.2.8/mohupy/lib/io.py
--rw-r--r--   0 yibow      (501) staff       (20)     2405 2023-11-29 05:15:05.000000 MohuPy-0.2.8/mohupy/lib/measure.py
--rw-r--r--   0 yibow      (501) staff       (20)     2940 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/lib/other.py
--rw-r--r--   0 yibow      (501) staff       (20)     2226 2024-01-23 13:45:06.000000 MohuPy-0.2.8/mohupy/lib/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)      468 2024-04-06 07:53:05.000000 MohuPy-0.2.8/mohupy/lib/string.py
--rw-r--r--   0 yibow      (501) staff       (20)     4902 2024-04-06 07:54:21.000000 MohuPy-0.2.8/mohupy/lib/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.383212 MohuPy-0.2.8/mohupy/math/
--rw-r--r--   0 yibow      (501) staff       (20)      318 2023-11-29 08:28:01.000000 MohuPy-0.2.8/mohupy/math/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      494 2023-11-29 05:40:06.000000 MohuPy-0.2.8/mohupy/math/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     8536 2024-04-06 07:55:41.000000 MohuPy-0.2.8/mohupy/math/product.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.384217 MohuPy-0.2.8/mohupy/measure/
--rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 MohuPy-0.2.8/mohupy/measure/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)    11003 2023-11-28 12:01:09.000000 MohuPy-0.2.8/mohupy/measure/fuzzmeas.py
--rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 MohuPy-0.2.8/mohupy/measure/hasse.py
--rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-04-02 03:39:44.000000 MohuPy-0.2.8/mohupy/measure/indices.py
--rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 MohuPy-0.2.8/mohupy/measure/integral.py
--rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 MohuPy-0.2.8/mohupy/measure/utils.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.384801 MohuPy-0.2.8/mohupy/random/
--rw-r--r--   0 yibow      (501) staff       (20)      342 2024-04-06 03:45:30.000000 MohuPy-0.2.8/mohupy/random/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)      489 2023-11-29 05:39:47.000000 MohuPy-0.2.8/mohupy/random/base.py
--rw-r--r--   0 yibow      (501) staff       (20)     4245 2024-04-06 07:47:24.000000 MohuPy-0.2.8/mohupy/random/rand.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.385965 MohuPy-0.2.8/mohupy/regedit/
--rw-r--r--   0 yibow      (501) staff       (20)     1100 2024-04-06 07:43:14.000000 MohuPy-0.2.8/mohupy/regedit/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)     4492 2024-04-06 07:43:49.000000 MohuPy-0.2.8/mohupy/regedit/algebraic_operation.py
--rw-r--r--   0 yibow      (501) staff       (20)     3327 2023-12-23 07:12:54.000000 MohuPy-0.2.8/mohupy/regedit/construct.py
--rw-r--r--   0 yibow      (501) staff       (20)     4539 2023-11-29 05:10:14.000000 MohuPy-0.2.8/mohupy/regedit/distance.py
--rw-r--r--   0 yibow      (501) staff       (20)     6913 2023-11-29 09:13:44.000000 MohuPy-0.2.8/mohupy/regedit/plotlib.py
--rw-r--r--   0 yibow      (501) staff       (20)     2685 2024-04-06 07:46:44.000000 MohuPy-0.2.8/mohupy/regedit/random.py
--rw-r--r--   0 yibow      (501) staff       (20)     2724 2024-04-06 07:47:03.000000 MohuPy-0.2.8/mohupy/regedit/str2num.py
--rw-r--r--   0 yibow      (501) staff       (20)      757 2024-04-06 07:57:39.000000 MohuPy-0.2.8/mohupy/runtime.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386090 MohuPy-0.2.8/mohupy/tensor/
--rw-r--r--   0 yibow      (501) staff       (20)      161 2024-04-06 05:45:55.000000 MohuPy-0.2.8/mohupy/tensor/__init__.py
-drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-06 08:34:23.386312 MohuPy-0.2.8/mohupy/utils/
--rw-r--r--   0 yibow      (501) staff       (20)      163 2023-11-28 12:06:14.000000 MohuPy-0.2.8/mohupy/utils/__init__.py
--rw-r--r--   0 yibow      (501) staff       (20)       38 2024-04-06 08:34:23.387323 MohuPy-0.2.8/setup.cfg
--rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 MohuPy-0.2.8/setup.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.172280 mohupy-0.3.0/
+-rw-r--r--   0 yibow      (501) staff       (20)     1061 2023-01-29 07:30:33.000000 mohupy-0.3.0/LICENSE
+-rw-r--r--   0 yibow      (501) staff       (20)     9385 2024-04-12 16:02:30.171718 mohupy-0.3.0/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     8791 2024-04-12 15:58:42.000000 mohupy-0.3.0/README.md
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.155672 mohupy-0.3.0/mohupy/
+-rw-r--r--   0 yibow      (501) staff       (20)      719 2024-04-12 09:14:36.000000 mohupy-0.3.0/mohupy/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.156957 mohupy-0.3.0/mohupy/config/
+-rw-r--r--   0 yibow      (501) staff       (20)      258 2024-04-11 08:33:14.000000 mohupy-0.3.0/mohupy/config/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      675 2024-04-12 07:24:07.000000 mohupy-0.3.0/mohupy/config/main.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.159119 mohupy-0.3.0/mohupy/core/
+-rw-r--r--   0 yibow      (501) staff       (20)      592 2024-04-11 08:33:45.000000 mohupy-0.3.0/mohupy/core/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      592 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/attribute.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6305 2024-04-10 07:12:41.000000 mohupy-0.3.0/mohupy/core/attributeClass.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1656 2024-04-09 05:08:59.000000 mohupy-0.3.0/mohupy/core/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1232 2024-04-11 08:32:33.000000 mohupy-0.3.0/mohupy/core/constant.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3008 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)    24312 2024-04-11 07:52:35.000000 mohupy-0.3.0/mohupy/core/funcitonClass.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2999 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/function.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5679 2024-04-11 07:30:48.000000 mohupy-0.3.0/mohupy/core/fuzzarray.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3434 2024-04-11 07:31:57.000000 mohupy-0.3.0/mohupy/core/fuzznums.py
+-rw-r--r--   0 yibow      (501) staff       (20)    20515 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2891 2024-04-11 08:47:40.000000 mohupy-0.3.0/mohupy/core/operationClass.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.159875 mohupy-0.3.0/mohupy/core/operationLib/
+-rw-r--r--   0 yibow      (501) staff       (20)      617 2024-04-06 06:52:42.000000 mohupy-0.3.0/mohupy/core/operationLib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4126 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/operationLib/algebraic.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4169 2024-04-06 06:57:19.000000 mohupy-0.3.0/mohupy/core/operationLib/algebraicoperation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1214 2024-04-06 06:48:09.000000 mohupy-0.3.0/mohupy/core/operationLib/einstein.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1301 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/core/operationpackage.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1722 2024-04-06 06:36:47.000000 mohupy-0.3.0/mohupy/core/regedit.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.160004 mohupy-0.3.0/mohupy/corelib/
+-rw-r--r--   0 yibow      (501) staff       (20)      449 2024-04-12 08:29:26.000000 mohupy-0.3.0/mohupy/corelib/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.161268 mohupy-0.3.0/mohupy/corelib/function/
+-rw-r--r--   0 yibow      (501) staff       (20)     1355 2024-04-12 08:32:45.000000 mohupy-0.3.0/mohupy/corelib/function/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1806 2024-04-12 08:02:17.000000 mohupy-0.3.0/mohupy/corelib/function/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2533 2024-04-12 06:58:38.000000 mohupy-0.3.0/mohupy/corelib/function/extension.py
+-rw-r--r--   0 yibow      (501) staff       (20)      709 2024-04-12 05:58:58.000000 mohupy-0.3.0/mohupy/corelib/function/io.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1294 2024-04-12 07:08:12.000000 mohupy-0.3.0/mohupy/corelib/function/math.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1385 2024-04-12 06:23:42.000000 mohupy-0.3.0/mohupy/corelib/function/measure.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1837 2024-04-12 06:36:00.000000 mohupy-0.3.0/mohupy/corelib/function/plot.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1339 2024-04-12 08:32:45.000000 mohupy-0.3.0/mohupy/corelib/function/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)      570 2024-04-12 06:40:29.000000 mohupy-0.3.0/mohupy/corelib/function/string.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.162237 mohupy-0.3.0/mohupy/corelib/lib/
+-rw-r--r--   0 yibow      (501) staff       (20)      677 2024-04-12 07:01:30.000000 mohupy-0.3.0/mohupy/corelib/lib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      490 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/lib/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2186 2024-04-12 08:01:12.000000 mohupy-0.3.0/mohupy/corelib/lib/classConstruct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5415 2024-04-11 12:52:18.000000 mohupy-0.3.0/mohupy/corelib/lib/classIO.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2163 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/lib/classMeasure.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1894 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/lib/classPlot.py
+-rw-r--r--   0 yibow      (501) staff       (20)      451 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/lib/classString.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4221 2024-04-11 15:35:23.000000 mohupy-0.3.0/mohupy/corelib/lib/classUtils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.162751 mohupy-0.3.0/mohupy/corelib/math/
+-rw-r--r--   0 yibow      (501) staff       (20)      225 2024-04-12 07:03:49.000000 mohupy-0.3.0/mohupy/corelib/math/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      493 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/math/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     7986 2024-04-10 13:39:10.000000 mohupy-0.3.0/mohupy/corelib/math/classProduct.py
+-rw-r--r--   0 yibow      (501) staff       (20)      826 2024-04-12 07:09:17.000000 mohupy-0.3.0/mohupy/corelib/math/product.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.163205 mohupy-0.3.0/mohupy/corelib/random/
+-rw-r--r--   0 yibow      (501) staff       (20)      323 2024-04-12 07:11:22.000000 mohupy-0.3.0/mohupy/corelib/random/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      487 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/random/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)      823 2024-04-12 07:26:07.000000 mohupy-0.3.0/mohupy/corelib/random/function.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2207 2024-04-11 15:58:49.000000 mohupy-0.3.0/mohupy/corelib/random/randclass.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.163932 mohupy-0.3.0/mohupy/corelib/regedit/
+-rw-r--r--   0 yibow      (501) staff       (20)      441 2024-04-12 07:20:27.000000 mohupy-0.3.0/mohupy/corelib/regedit/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3200 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/regedit/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4588 2024-04-11 07:43:33.000000 mohupy-0.3.0/mohupy/corelib/regedit/distance.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6888 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/regedit/plotlib.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2712 2024-04-12 07:17:48.000000 mohupy-0.3.0/mohupy/corelib/regedit/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2700 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/corelib/regedit/str2num.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.164164 mohupy-0.3.0/mohupy/function/
+-rw-r--r--   0 yibow      (501) staff       (20)      391 2024-04-12 05:51:52.000000 mohupy-0.3.0/mohupy/function/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     9168 2024-04-12 07:27:53.000000 mohupy-0.3.0/mohupy/function/formula.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.164780 mohupy-0.3.0/mohupy/generator/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2023-10-01 08:16:28.000000 mohupy-0.3.0/mohupy/generator/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     4525 2024-04-12 05:51:14.000000 mohupy-0.3.0/mohupy/generator/membershipfunc.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.165283 mohupy-0.3.0/mohupy/library/
+-rw-r--r--   0 yibow      (501) staff       (20)      163 2024-04-11 15:11:36.000000 mohupy-0.3.0/mohupy/library/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      355 2024-04-12 07:30:32.000000 mohupy-0.3.0/mohupy/library/random.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.166519 mohupy-0.3.0/mohupy/measure/
+-rw-r--r--   0 yibow      (501) staff       (20)      710 2023-11-29 05:09:11.000000 mohupy-0.3.0/mohupy/measure/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)    10999 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/measure/fuzzmeas.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5312 2023-10-01 12:26:14.000000 mohupy-0.3.0/mohupy/measure/hasse.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6189 2024-04-02 03:39:44.000000 mohupy-0.3.0/mohupy/measure/indices.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6566 2023-12-01 08:41:17.000000 mohupy-0.3.0/mohupy/measure/integral.py
+-rw-r--r--   0 yibow      (501) staff       (20)     5549 2023-11-25 10:47:47.000000 mohupy-0.3.0/mohupy/measure/utils.py
+-rw-r--r--   0 yibow      (501) staff       (20)      899 2024-04-12 07:21:32.000000 mohupy-0.3.0/mohupy/runtime.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.167891 mohupy-0.3.0/mohupy/tensor/
+-rw-r--r--   0 yibow      (501) staff       (20)      257 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/tensor/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1843 2024-04-10 05:26:42.000000 mohupy-0.3.0/mohupy/tensor/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     6263 2024-04-11 08:26:49.000000 mohupy-0.3.0/mohupy/tensor/function.py
+-rw-r--r--   0 yibow      (501) staff       (20)    13162 2024-04-11 15:52:03.000000 mohupy-0.3.0/mohupy/tensor/fuzztensor.py
+-rw-r--r--   0 yibow      (501) staff       (20)    10059 2024-04-11 15:50:57.000000 mohupy-0.3.0/mohupy/tensor/operation.py
+-rw-r--r--   0 yibow      (501) staff       (20)     3437 2024-04-11 15:52:33.000000 mohupy-0.3.0/mohupy/tensor/operationFunc.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2352 2024-04-11 15:55:38.000000 mohupy-0.3.0/mohupy/tensor/utils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.168013 mohupy-0.3.0/mohupy/tensorlib/
+-rw-r--r--   0 yibow      (501) staff       (20)      301 2024-04-12 08:29:36.000000 mohupy-0.3.0/mohupy/tensorlib/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.169158 mohupy-0.3.0/mohupy/tensorlib/function/
+-rw-r--r--   0 yibow      (501) staff       (20)     1044 2024-04-12 08:32:45.000000 mohupy-0.3.0/mohupy/tensorlib/function/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1617 2024-04-12 08:00:09.000000 mohupy-0.3.0/mohupy/tensorlib/function/construct.py
+-rw-r--r--   0 yibow      (501) staff       (20)      520 2024-04-12 08:08:16.000000 mohupy-0.3.0/mohupy/tensorlib/function/extension.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1041 2024-04-12 07:42:10.000000 mohupy-0.3.0/mohupy/tensorlib/function/io.py
+-rw-r--r--   0 yibow      (501) staff       (20)      162 2024-04-12 08:09:22.000000 mohupy-0.3.0/mohupy/tensorlib/function/math.py
+-rw-r--r--   0 yibow      (501) staff       (20)      478 2024-04-12 08:12:59.000000 mohupy-0.3.0/mohupy/tensorlib/function/measure.py
+-rw-r--r--   0 yibow      (501) staff       (20)      674 2024-04-12 08:16:37.000000 mohupy-0.3.0/mohupy/tensorlib/function/plot.py
+-rw-r--r--   0 yibow      (501) staff       (20)      535 2024-04-12 08:32:45.000000 mohupy-0.3.0/mohupy/tensorlib/function/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)      328 2024-04-12 08:18:35.000000 mohupy-0.3.0/mohupy/tensorlib/function/string.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.170328 mohupy-0.3.0/mohupy/tensorlib/lib/
+-rw-r--r--   0 yibow      (501) staff       (20)      698 2024-04-12 07:36:52.000000 mohupy-0.3.0/mohupy/tensorlib/lib/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      490 2024-04-11 08:51:12.000000 mohupy-0.3.0/mohupy/tensorlib/lib/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2789 2024-04-11 11:48:57.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classConstruct.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1940 2024-04-11 13:08:04.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classIO.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1453 2024-04-12 08:11:16.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classMeasure.py
+-rw-r--r--   0 yibow      (501) staff       (20)     1089 2024-04-11 15:37:35.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classPlot.py
+-rw-r--r--   0 yibow      (501) staff       (20)      458 2024-04-11 15:33:10.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classString.py
+-rw-r--r--   0 yibow      (501) staff       (20)      517 2024-04-11 15:40:34.000000 mohupy-0.3.0/mohupy/tensorlib/lib/classUtils.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.170522 mohupy-0.3.0/mohupy/tensorlib/math/
+-rw-r--r--   0 yibow      (501) staff       (20)      162 2024-04-12 07:34:16.000000 mohupy-0.3.0/mohupy/tensorlib/math/__init__.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.171031 mohupy-0.3.0/mohupy/tensorlib/random/
+-rw-r--r--   0 yibow      (501) staff       (20)      295 2024-04-12 08:24:21.000000 mohupy-0.3.0/mohupy/tensorlib/random/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)      486 2024-04-09 14:49:37.000000 mohupy-0.3.0/mohupy/tensorlib/random/base.py
+-rw-r--r--   0 yibow      (501) staff       (20)      330 2024-04-12 08:25:57.000000 mohupy-0.3.0/mohupy/tensorlib/random/random.py
+-rw-r--r--   0 yibow      (501) staff       (20)      768 2024-04-12 08:22:14.000000 mohupy-0.3.0/mohupy/tensorlib/random/randomClass.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.171273 mohupy-0.3.0/mohupy/utils/
+-rw-r--r--   0 yibow      (501) staff       (20)      292 2024-04-12 09:14:03.000000 mohupy-0.3.0/mohupy/utils/__init__.py
+-rw-r--r--   0 yibow      (501) staff       (20)     2940 2024-04-12 03:58:33.000000 mohupy-0.3.0/mohupy/utils/other.py
+drwxr-xr-x   0 yibow      (501) staff       (20)        0 2024-04-12 16:02:30.171455 mohupy-0.3.0/mohupy.egg-info/
+-rw-r--r--   0 yibow      (501) staff       (20)     9385 2024-04-12 16:02:30.000000 mohupy-0.3.0/mohupy.egg-info/PKG-INFO
+-rw-r--r--   0 yibow      (501) staff       (20)     3199 2024-04-12 16:02:30.000000 mohupy-0.3.0/mohupy.egg-info/SOURCES.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        1 2024-04-12 16:02:30.000000 mohupy-0.3.0/mohupy.egg-info/dependency_links.txt
+-rw-r--r--   0 yibow      (501) staff       (20)       39 2024-04-12 16:02:30.000000 mohupy-0.3.0/mohupy.egg-info/requires.txt
+-rw-r--r--   0 yibow      (501) staff       (20)        7 2024-04-12 16:02:30.000000 mohupy-0.3.0/mohupy.egg-info/top_level.txt
+-rw-r--r--   0 yibow      (501) staff       (20)       38 2024-04-12 16:02:30.172336 mohupy-0.3.0/setup.cfg
+-rw-r--r--   0 yibow      (501) staff       (20)      900 2024-02-13 17:46:21.000000 mohupy-0.3.0/setup.py
```

### Comparing `MohuPy-0.2.8/LICENSE` & `mohupy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/constant.py` & `mohupy-0.3.0/mohupy/core/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午5:03
+#  Date: 2024/4/7 下午1:23
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 import numpy as np
 
 ZERO_1 = np.float_(1e-1)
 ZERO_2 = np.float_(1e-2)
 ZERO_3 = np.float_(1e-3)
 ZERO_4 = np.float_(1e-4)
 ZERO_5 = np.float_(1e-5)
```

### Comparing `MohuPy-0.2.8/mohupy/core/attributeClass.py` & `mohupy-0.3.0/mohupy/core/attributeClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,68 +9,68 @@
 
 import numpy as np
 
 from .base import Attribute
 from .fuzznums import Fuzznum
 from .fuzzarray import Fuzzarray
 
-from ..constant import Approx
+from .constant import Approx
+
 
 class Report(Attribute):
     """
         Report printout
     """
 
     def function(self, x):
         if isinstance(x, Fuzznum):
+            if x.md is None and x.nmd is None:
+                return f'<>'
             if x.mtype == 'qrofn':
                 return f'<{np.round(x.md, 4)},{np.round(x.nmd, 4)}>'
             if x.mtype == 'ivfn':
                 return f'<{np.round(x.md, 4)},{np.round(x.nmd, 4)}>'
             if x.mtype == 'qrohfn':
                 if len(x.md) > 8 >= len(x.nmd):
                     return f'<{np.round(x.md[:8], 4)}..., {np.round(x.nmd, 4)}>'
                 if len(x.nmd) > 8 >= len(x.md):
                     return f'<{np.round(x.md, 4)}, {np.round(x.nmd[:8], 4)}...>'
                 if len(x.md) > 8 and len(x.nmd) > 8:
                     return f'<{np.round(x.md[:8], 4)}..., {np.round(x.nmd[:8], 4)}...>'
                 else:
                     return f'<{np.round(x.md, 4)}, {np.round(x.nmd, 4)}>'
-            if x.md is None and x.nmd is None:
-                return f'<>'
         if isinstance(x, Fuzzarray):
             p = str(x.array).replace('\n', '\n' + ' ' * 10)
             return f'Fuzzarray({p}, qrung={x.qrung}, mtype={x.mtype})'
         raise TypeError(f'Unsupported data types:{type(x)}.')
 
 
 class Str(Attribute):
     def function(self, x):
         if isinstance(x, Fuzznum):
+            if x.md is None and x.nmd is None:
+                return f'<>'
             if x.mtype == 'qrofn':
                 return f'<{np.round(x.md, 4)},{np.round(x.nmd, 4)}>'
             if x.mtype == 'ivfn':
                 return f'<{np.round(x.md, 4)},{np.round(x.nmd, 4)}>'
             if x.mtype == 'qrohfn':
                 if len(x.md) > 8 >= len(x.nmd):
                     return f'<{np.round(x.md[:8], 4)}..., {np.round(x.nmd, 4)}>'
                 if len(x.nmd) > 8 >= len(x.md):
                     return f'<{np.round(x.md, 4)}, {np.round(x.nmd[:8], 4)}...>'
                 if len(x.md) > 8 and len(x.nmd) > 8:
                     return f'<{np.round(x.md[:8], 4)}..., {np.round(x.nmd[:8], 4)}...>'
                 else:
                     return f'<{np.round(x.md, 4)}, {np.round(x.nmd, 4)}>'
-            if x.md is None and x.nmd is None:
-                return f'<>'
         if isinstance(x, Fuzzarray):
             return str(x.array)
         raise TypeError(f'Unsupported data types:{type(x)}.')
 
 
-
 class Score(Attribute):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 return x.md ** x.qrung - x.nmd ** x.qrung
             if x.mtype == 'ivfn':
                 m = x.md[0] ** x.qrung + x.md[1] ** x.qrung
@@ -84,15 +84,14 @@
                     nn = ((x.nmd ** x.qrung).sum()) / len(x.nmd)
                     return mm - nn
         if isinstance(x, Fuzzarray):
             # TODO: 模糊集
             pass
 
 
-
 class Accuracy(Attribute):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 return x.md ** x.qrung + x.nmd ** x.qrung
             if x.mtype == 'ivfn':
                 m = x.md[0] ** x.qrung + x.md[1] ** x.qrung
@@ -106,15 +105,14 @@
                     nn = ((x.nmd ** x.qrung).sum()) / len(x.nmd)
                     return mm + nn
         if isinstance(x, Fuzzarray):
             # TODO: 模糊集
             pass
 
 
-
 class Indeterminacy(Attribute):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 acc = x.md ** x.qrung + x.nmd ** x.qrung
                 if acc == np.round(1., Approx.round):
                     return np.round(0., Approx.round)
@@ -138,15 +136,14 @@
                     else:
                         return (1. - mm - nn) ** (1. / x.qrung)
         if isinstance(x, Fuzzarray):
             # TODO: 模糊集
             pass
 
 
-
 class Complement(Attribute):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 newf = copy.deepcopy(x)
                 newf.md = x.nmd
                 newf.nmd = x.md
```

### Comparing `MohuPy-0.2.8/mohupy/core/base.py` & `mohupy-0.3.0/mohupy/core/base.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/core/construct.py` & `mohupy-0.3.0/mohupy/core/construct.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
 #  Date: 2024/4/6 下午3:07
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
+from typing import Union
+
 import numpy as np
 
 from .fuzznums import Fuzznum
 from .fuzzarray import Fuzzarray
 
 from .base import Construct
 
@@ -30,41 +32,68 @@
         This class is just a class for generating a fuzzy array,
             specifically implemented with function. Similar to the numpy.array method.
     """
 
     def function(self, x):
         if x is None:
             return Fuzzarray()
-        y = x
         if isinstance(x, Fuzznum):
-            fl = np.asarray(y, dtype=object)
-            flat = fl.flatten()
-            r = np.random.choice(flat)
-            newset = Fuzzarray(r.qrung, r.mtype)
-            newset.array = fl
+            newset = Fuzzarray(x.qrung)
+            newset.array = x
             return newset
-        if isinstance(x, (list, tuple, np.ndarray)):
+        if isinstance(x, Fuzzarray):
+            return x
+        if isinstance(x, Union[list, tuple, np.ndarray]):
             y = np.asarray(x, dtype=object)
-            y = y.flatten()
-            mt = y[0].mtype
-            for i in y:
-                if i.mtype != mt:
-                    raise TypeError(f'Unsupported mtype: {i.mtype}.')
-                mt = i.mtype
 
             t = np.random.choice(y)
             qrung = t.qrung
-            mtype = t.mtype
-
-            newset = Fuzzarray(qrung, mtype)
-            newset.array = np.array(x, dtype=object)
-            return newset
 
+            def checkdata(data: Fuzznum):
+                from ..config import Config
+                if data.mtype != Config.mtype:
+                    raise TypeError(f'Fuzzy type {data.mtype} and {Config.mtype} do not match.')
+                if data.qrung != qrung:
+                    raise TypeError(f'Fuzzy qrung {data.qrung} and {qrung} do not match.')
+                return True
+
+            vec_checkdata = np.vectorize(checkdata)
+            if np.all(vec_checkdata(y)):
+                newset = Fuzzarray(qrung)
+                newset.array = y
+                return newset
         raise TypeError(f'Unsupported type: {type(x)}.')
 
 
+        # if isinstance(x, Fuzznum):
+        #     fl = np.asarray(y, dtype=object)
+        #     flat = fl.flatten()
+        #     r = np.random.choice(flat)
+        #     newset = Fuzzarray(r.qrung, r.mtype)
+        #     newset.array = fl
+        #     return newset
+        # if isinstance(x, (list, tuple, np.ndarray)):
+        #     y = np.asarray(x, dtype=object)
+        #     y = y.flatten()
+        #     mt = y[0].mtype
+        #     for i in y:
+        #         if i.mtype != mt:
+        #             raise TypeError(f'Unsupported mtype: {i.mtype}.')
+        #         mt = i.mtype
+        #
+        #     t = np.random.choice(y)
+        #     qrung = t.qrung
+        #     mtype = t.mtype
+        #
+        #     newset = Fuzzarray(qrung, mtype)
+        #     newset.array = np.array(x, dtype=object)
+        #     return newset
+        #
+        # raise TypeError(f'Unsupported type: {type(x)}.')
+
+
 def fuzznum(qrung=None, md=None, nmd=None) -> Fuzznum:
     return FuzzNum()(qrung, md, nmd)
 
 
 def fuzzset(x=None) -> Fuzzarray:
     return FuzzSet()(x)
```

### Comparing `MohuPy-0.2.8/mohupy/core/funcitonClass.py` & `mohupy-0.3.0/mohupy/core/funcitonClass.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 import numpy as np
 
 from .base import Function
 from .fuzznums import Fuzznum
 from .fuzzarray import Fuzzarray
 
-from ..constant import Approx
+from .constant import Approx
+from ..config import Config
 
 
 class InitializeNum(Function):
     """
         Initialization Method Class of Fuzzy Numbers(Fuzznum)
     """
 
@@ -74,29 +75,39 @@
 
             return mtype, memDegree, nonMemDegree
 
         raise TypeError(f'Unsupported data type or type error, md:{type(md)} and nmd:{type(nmd)}.')
 
 
 class InitializeSet(Function):
-    def function(self, qrung, mtype):
-        if qrung is not None or mtype is not None:
-            from .base import FuzzType
-            assert mtype in FuzzType, f'Unsupported fuzzy types, mtype:{mtype}.'
+    # def function(self, qrung, mtype):
+    #     if qrung is not None or mtype is not None:
+    #         from .base import FuzzType
+    #         assert mtype in FuzzType, f'Unsupported fuzzy types, mtype:{mtype}.'
+    #         assert qrung > 0, f'Qrung must be greater than 0, qrung:{qrung}.'
+    #
+    #         qrung = qrung
+    #         mtype = mtype
+    #     else:
+    #         qrung = None
+    #         mtype = None
+    #     return qrung, mtype
+
+    def function(self, qrung):
+        if qrung is not None:
             assert qrung > 0, f'Qrung must be greater than 0, qrung:{qrung}.'
 
             qrung = qrung
-            mtype = mtype
         else:
             qrung = None
-            mtype = None
-        return qrung, mtype
+
+        return qrung, Config.mtype
 
 
-class Validity(Function):
+class FuzzValidity(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 if 0. <= x.md <= 1. and 0. <= x.nmd <= 1. \
                         and 0. <= x.md ** x.qrung + x.nmd ** x.qrung <= 1.:
                     return True
                 else:
@@ -130,20 +141,25 @@
                 elif a4:
                     # print('a4')
                     return True
                 else:
                     return False
             raise TypeError(f'Unsupported mtype(type:{x.mtype}).')
         if isinstance(x, Fuzzarray):
-            vec_func = np.vectorize(lambda u: Validity()(u))
+            if x.size == 0:
+                return True
+            vec_func = np.vectorize(lambda u: FuzzValidity()(u))
             return vec_func(x.array)
 
 
-class Empty(Function):
-    def function(self, x, onlyfn):
+class FuzzEmpty(Function):
+    def __init__(self, onlyfn):
+        self.onlyfn = onlyfn
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 if x.md is None and x.nmd is None:
                     return True
                 else:
                     return False
             if x.mtype == 'ivfn':
@@ -154,418 +170,489 @@
             if x.mtype == 'qrohfn':
                 if x.md.size == 0 and x.nmd.size == 0:
                     return True
                 else:
                     return False
             raise TypeError(f'Unsupported mtype, ,type:{x.mtype}.')
         if isinstance(x, Fuzzarray):
-            if onlyfn:
-                vec_func = np.vectorize(lambda u: Empty()(u, onlyfn))
+            if x.size == 0:
+                return True
+            if self.onlyfn:
+                vec_func = np.vectorize(lambda u: FuzzEmpty(self.onlyfn)(u))
                 return vec_func(x.array)
-            else:
-                return True if x.size == 0 else False
+            return False
 
 
-class Initial(Function):
+class FuzzInitial(Function):
     """
         Determine whether the fuzzy set or fuzzy number is the initialized
         fuzzy set or fuzzy number
     """
 
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.qrung is not None:
                 return False
-            if x.mtype is not None:
-                return False
             if x.md is not None:
                 return False
             if x.nmd is not None:
                 return False
             return True
         if isinstance(x, Fuzzarray):
             if x.qrung is not None:
                 return False
-            if x.mtype is not None:
-                return False
             if x.array.size != 0:
                 return False
             return True
 
 
-class Convert(Function):
+class FuzzConvert(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrofn':
                 return x.md, x.nmd
             if x.mtype == 'ivfn':
                 return x.md.tolist(), x.nmd.tolist()
             if x.mtype == 'qrohfn':
                 return x.md.tolist(), x.nmd.tolist()
         raise TypeError(f'Unsupported type: {type(x)}.')
 
 
-class Qsort(Function):
-    def function(self, x, reverse=True):
+class FuzzQsort(Function):
+
+    def __init__(self, reverse):
+        self.reverse = reverse
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrohfn':
                 newfn = copy.deepcopy(x)
-                if reverse:
+                if self.reverse:
                     newfn.md = np.sort(x.md)
                     newfn.nmd = np.sort(x.nmd)
                 else:
                     newfn.md = np.abs(np.sort(-x.md))
                     newfn.nmd = np.abs(np.sort(-x.nmd))
                 return newfn
             else:
                 return x
         if isinstance(x, Fuzzarray):
-            vec_func = np.vectorize(lambda u: Qsort()(u, reverse=reverse))
-            newset = Fuzzarray(x.qrung, x.mtype)
+            vec_func = np.vectorize(lambda u: FuzzQsort(self.reverse)(u))
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array)
             return newset
 
 
-class Unique(Function):
+class FuzzUnique(Function):
     """
         Simplify the membership and non-membership degrees with Approx.round precision
     """
 
-    def function(self, x, onlyfn=False):
+    def __init__(self, onlyfn):
+        self.onlyfn = onlyfn
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             if x.mtype == 'qrohfn':
                 t = copy.deepcopy(x)
                 t.md = np.unique(x.md)
                 t.nmd = np.unique(x.nmd)
                 return t
             else:
                 return x
         if isinstance(x, Fuzzarray):
-            if onlyfn:
-                vec_func = np.vectorize(lambda u: Unique()(u, onlyfn))
-                newset = Fuzzarray(x.qrung, x.mtype)
+            if self.onlyfn:
+                vec_func = np.vectorize(lambda u: FuzzUnique(self.onlyfn)(u))
+                newset = Fuzzarray(x.qrung)
                 newset.array = vec_func(x.array)
                 return newset
             else:
                 uni = np.unique(x.array)
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 newset.array = uni
                 return newset
 
 
-class Transpose(Function):
+class FuzzTranspose(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
             return copy.copy(x)
         if isinstance(x, Fuzzarray):
             st = x.array
             s = st.T
 
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = s
             del st, s
             return newset
 
 
-class Append(Function):
+class FuzzAppend(Function):
     """
         1. 模糊数 + 模糊数
         2. 模糊数 + 模糊集
         3. 模糊集 + 模糊数
         4. 模糊集 + 模糊集
     """
 
-    def function(self, x, e):
-        if isinstance(x, Fuzznum) and isinstance(e, Fuzznum):
-            assert x.qrung == e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{e.qrung}).'
-            assert x.mtype == e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{e.mtype}).'
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = np.append(newset.array, [x, e])
-            return newset
-        if isinstance(x, Fuzznum) and isinstance(e, Fuzzarray):
-            if e.mtype is not None and e.qrung is not None:
-                assert x.qrung == e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{e.qrung}).'
-                assert x.mtype == e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{e.mtype}).'
-                e.array = np.insert(e.array, 0, x)
-                return e
-            else:
-                e.qrung = x.qrung
-                e.mtype = x.mtype
-                e.array = np.append(e.array, x)
-                return e
-        if isinstance(x, Fuzzarray) and isinstance(e, Fuzznum):
+    def __init__(self, e):
+        self.e = e
+
+    def function(self, x):
+        if isinstance(x, Fuzznum) and isinstance(self.e, Fuzznum):
+            assert x.qrung == self.e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{self.e.qrung}).'
+            assert x.mtype == self.e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{self.e.mtype}).'
+            newset = Fuzzarray(x.qrung)
+            newset.array = np.append(newset.array, [x, self.e])
+            return newset
+        if isinstance(x, Fuzznum) and isinstance(self.e, Fuzzarray):
+            if self.e.mtype is not None and self.e.qrung is not None:
+                assert x.qrung == self.e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{self.e.qrung}).'
+                assert x.mtype == self.e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{self.e.mtype}).'
+                self.e.array = np.insert(self.e.array, 0, x)
+                return self.e
+            else:
+                self.e.qrung = x.qrung
+                self.e.mtype = x.mtype
+                self.e.array = np.append(self.e.array, x)
+                return self.e
+        if isinstance(x, Fuzzarray) and isinstance(self.e, Fuzznum):
             if x.mtype is not None and x.qrung is not None:
-                assert x.qrung == e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{e.qrung}).'
-                assert x.mtype == e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{e.mtype}).'
-                x.array = np.append(x.array, e)
+                assert x.qrung == self.e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{self.e.qrung}).'
+                assert x.mtype == self.e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{self.e.mtype}).'
+                x.array = np.append(x.array, self.e)
                 return x
             else:
-                x.qrung = e.qrung
-                x.mtype = e.mtype
-                x.array = np.append(x.array, e)
+                x.qrung = self.e.qrung
+                x.mtype = self.e.mtype
+                x.array = np.append(x.array, self.e)
                 return x
-        if isinstance(x, Fuzzarray) and isinstance(e, Fuzzarray):
-            if x.mtype is not None and x.qrung is not None and e.mtype is not None and e.qrung is not None:
-                assert x.qrung == e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{e.qrung}).'
-                assert x.mtype == e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{e.mtype}).'
-                x.array = np.append(x.array, e.array)
+        if isinstance(x, Fuzzarray) and isinstance(self.e, Fuzzarray):
+            if x.mtype is not None and x.qrung is not None and self.e.mtype is not None and self.e.qrung is not None:
+                assert x.qrung == self.e.qrung, f'qrung mismatch(x.qrung:{x.qrung} and e.qrung:{self.e.qrung}).'
+                assert x.mtype == self.e.mtype, f'mtype mismatch(x.mtype:{x.mtype} and e.mtype:{self.e.mtype}).'
+                x.array = np.append(x.array, self.e.array)
                 return x
-            elif x.mtype is not None and x.qrung is not None and e.mtype is None and e.qrung is None:
-                x.array = np.append(x.array, e.array)
+            elif x.mtype is not None and x.qrung is not None and self.e.mtype is None and self.e.qrung is None:
+                x.array = np.append(x.array, self.e.array)
                 return x
-            elif x.mtype is None and x.qrung is None and e.mtype is not None and e.qrung is not None:
-                e.array = np.append(e.array, x.array)
-                return e
+            elif x.mtype is None and x.qrung is None and self.e.mtype is not None and self.e.qrung is not None:
+                self.e.array = np.append(self.e.array, x.array)
+                return self.e
             else:
                 return x
-        raise TypeError(f'Unsupported type({type(x)} and {type(e)}).')
+        raise TypeError(f'Unsupported type({type(x)} and {type(self.e)}).')
 
 
-class Remove(Function):
-    def function(self, x, e):
+class FuzzRemove(Function):
+
+    def __init__(self, e):
+        self.e = e
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             raise ValueError(f'Deletion is not supported for {str(x)}')
         if isinstance(x, Fuzzarray):
             assert x.size > 0, 'The set is empty, can not be removed.'
-            assert e in x.array, f'{x} is not in the set.'
-            x.array = np.delete(x.array, np.where(x.array == e))
+            assert self.e in x.array, f'{self.e} is not in the set.'
+            x.array = np.delete(x.array, np.where(x.array == self.e))
             return x
 
 
-class Pop(Function):
-    def function(self, x, i):
+class FuzzPop(Function):
+
+    def __init__(self, index):
+        self.index = index
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             raise ValueError(f'Deletion is not supported for {str(x)}')
         if isinstance(x, Fuzzarray):
-            x.array = np.delete(x.array, i)
+            x.array = np.delete(x.array, self.index)
             return x
 
 
-class Reshape(Function):
-    def function(self, x, *shape):
+class FuzzReshape(Function):
+
+    def __init__(self, *shape):
+        self.shape = shape
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = np.reshape(x, *shape)
+            newset = Fuzzarray(x.qrung)
+            newset.array = np.reshape(x, *self.shape)
             return newset
         if isinstance(x, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = x.array.reshape(*shape)
+            newset = Fuzzarray(x.qrung)
+            newset.array = x.array.reshape(*self.shape)
             return newset
 
 
-class Squeeze(Function):
-    def function(self, x, axis):
+class FuzzSqueeze(Function):
+
+    def __init__(self, axis):
+        self.axis = axis
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = np.squeeze(x.array, axis)
+            newset = Fuzzarray(x.qrung)
+            newset.array = np.squeeze(x.array, self.axis)
             return newset
 
 
-class Broadcast(Function):
-    def function(self, x, shape):
+class FuzzBroadcast(Function):
+
+    def __init__(self, *shape):
+        self.shape = shape
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = np.broadcast_to(x, shape)
+            newset = Fuzzarray(x.qrung)
+            newset.array = np.broadcast_to(x, self.shape)
             return newset
         if isinstance(x, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
-            newset.array = np.broadcast_to(x.array, shape)
+            newset = Fuzzarray(x.qrung)
+            newset.array = np.broadcast_to(x.array, self.shape)
             return newset
 
 
-class Clear(Function):
+class FuzzClear(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
             x.qrung = None
-            x.mtype = None
             x.md = None
             x.nmd = None
             return x
         if isinstance(x, Fuzzarray):
             x.array = np.array([], dtype=object)
             x.qrung = None
-            x.mtype = None
             return x
 
 
-class Ravel(Function):
+class FuzzRavel(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.ravel(x)
             return newset
         if isinstance(x, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.ravel(x.array)
             return newset
 
 
-class Flatten(Function):
+class FuzzFlatten(Function):
     def function(self, x):
         if isinstance(x, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.array([x])
             return newset
         if isinstance(x, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = x.array.flatten()
             return newset
 
 
-class GetMax(Function):
-    def function(self, x, show, axis):
+class FuzzGetMax(Function):
+
+    def __init__(self, show, axis):
+        self.show = show
+        self.axis = axis
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            if axis is None:
+            if self.axis is None:
                 index = np.unravel_index(np.argmax(x.array), x.shape)
-                if show:
+                if self.show:
                     print(index)
                 return x.array[index]
             else:
-                m = np.max(x.array, axis=axis)
+                m = np.max(x.array, axis=self.axis)
                 if isinstance(m, Fuzznum):
                     return m
                 if isinstance(m, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = m
                     return newset
 
 
-class GetMin(Function):
-    def function(self, x, show, axis):
+class FuzzGetMin(Function):
+
+    def __init__(self, show, axis):
+        self.show = show
+        self.axis = axis
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            if axis is None:
+            if self.axis is None:
                 index = np.unravel_index(np.argmin(x.array), x.shape)
-                if show:
+                if self.show:
                     print(index)
                 return x.array[index]
             else:
-                m = np.min(x.array, axis=axis)
+                m = np.min(x.array, axis=self.axis)
                 if isinstance(m, Fuzznum):
                     return m
                 if isinstance(m, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = m
                     return newset
 
 
-class GetFmax(Function):
-    def function(self, x, func, *args, show, axis):
+class FuzzGetFmax(Function):
+
+    def __init__(self, show, axis, func, *params):
+        self.show = show
+        self.axis = axis
+        self.func = func
+        self.params = params
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             raise TypeError(f'Unsupported type({type(x)})')
         if isinstance(x, Fuzzarray):
-            slist = func(x.array, *args)
-            if axis is None:
+            if self.func is None:
+                return FuzzGetMax(self.show, self.axis)(x)
+
+            slist = self.func(x.array, *self.params)
+            if self.axis is None:
                 index = np.unravel_index(np.argmax(slist), x.shape)
-                if show:
+                if self.show:
                     print(index)
                 return x.array[index]
             else:
-                m = np.max(slist, axis=axis)
+                m = np.max(slist, axis=self.axis)
                 if isinstance(m, Fuzznum):
                     return m
                 if isinstance(slist, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = m
                     return newset
 
 
-class GetFmin(Function):
-    def function(self, x, func, *args, show, axis):
+class FuzzGetFmin(Function):
+
+    def __init__(self, show, axis, func, *params):
+        self.show = show
+        self.axis = axis
+        self.func = func
+        self.params = params
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             raise TypeError(f'Unsupported type({type(x)})')
         if isinstance(x, Fuzzarray):
-            slist = func(x.array, *args)
-            if axis is None:
+            if self.func is None:
+                return FuzzGetMin(self.show, self.axis)(x)
+
+            slist = self.func(x.array, *self.params)
+            if self.axis is None:
                 index = np.unravel_index(np.argmin(slist), x.shape)
-                if show:
+                if self.show:
                     print(index)
                 return x.array[index]
             else:
-                m = np.min(slist, axis=axis)
+                m = np.min(slist, axis=self.axis)
                 if isinstance(m, Fuzznum):
                     return m
                 if isinstance(slist, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = m
                     return newset
 
 
-class GetSum(Function):
-    def function(self, x, axis, keepdims):
+class FuzzGetSum(Function):
+
+    def __init__(self, axis, keepdims):
+        self.axis = axis
+        self.keepdims = keepdims
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            if axis is None:
+            if self.axis is None:
                 return np.sum(x.array)
             else:
-                s = np.sum(x.array, axis=axis, keepdims=keepdims)
+                s = np.sum(x.array, axis=self.axis, keepdims=self.keepdims)
                 if isinstance(s, Fuzznum):
                     return s
                 if isinstance(s, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = s
                     return newset
 
 
-class GetProd(Function):
-    def function(self, x, axis, keepdims):
+class FuzzGetProd(Function):
+
+    def __init__(self, axis, keepdims):
+        self.axis = axis
+        self.keepdims = keepdims
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            if axis is None:
+            if self.axis is None:
                 return np.prod(x.array)
             else:
-                s = np.prod(x.array, axis=axis, keepdims=keepdims)
+                s = np.prod(x.array, axis=self.axis, keepdims=self.keepdims)
                 if isinstance(s, Fuzznum):
                     return s
                 if isinstance(s, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = s
                     return newset
 
 
-class Mean(Function):
-    def function(self, x, axis):
+class FuzzMean(Function):
+
+    def __init__(self, axis):
+        self.axis = axis
+
+    def function(self, x):
         if isinstance(x, Fuzznum):
             return x
         if isinstance(x, Fuzzarray):
-            if axis is None:
+            if self.axis is None:
                 return np.mean(x.array)
             else:
-                s = np.mean(x.array, axis=axis)
+                s = np.mean(x.array, axis=self.axis)
                 if isinstance(s, Fuzznum):
                     return s
                 if isinstance(s, np.ndarray):
-                    newset = Fuzzarray(x.qrung, x.mtype)
+                    newset = Fuzzarray(x.qrung)
                     newset.array = s
                     return newset
 
 
-class Normalize(Function):
-    def function(self, d1, d2, t):
+class FuzzNormalize(Function):
+
+    def __init__(self, tao):
+        self.tao = tao
+
+    def function(self, d1, d2):
         """
             The normalization function for two q-rung orthopair hesitant fuzzy numbers.
                 The parameter 't' is the risk factor of normalization process, which in
                 the interval [0, 1]. 't=1' indicates optimistic normalization and
                 't=0' indicates pessimistic normalization.
 
             Parameters
             ----------
                 d1 : Fuzznum
                     The first q-rung orthopair hesitant fuzzy number
                 d2 : Fuzznum
                     The second q-rung orthopair hesitant fuzzy number
-                t : float or np.float_
-                    The risk factor of normalization process
 
             References
             ----------
                 A. R. Mishra, S.-M. Chen, and P. Rani, “Multiattribute decision-making
                 based on Fermatean hesitant fuzzy sets and modified VIKOR method,”
                 Inform Sciences, vol. 607, pp. 1532–1549, 2022, doi: 10.1016/j.ins.2022.06.037.
         """
@@ -581,41 +668,41 @@
 
             if md_len > 0:
                 # Explain that the number of membership elements in d1 is greater than d2,
                 # and it is necessary to add elements of d2 membership.
                 i = 0.
                 m = d_2.md
                 while i < md_len:
-                    d_2.md = np.append(d_2.md, __adj(m, t))
+                    d_2.md = np.append(d_2.md, __adj(m, self.tao))
                     i += 1
             else:
                 # Explain that the number of membership elements in d1 is less than d2,
                 # and it is necessary to increase the elements of d1 membership.
                 i = 0.
                 m = d_1.md
                 while i < (-md_len):
-                    d_1.md = np.append(d_1.md, __adj(m, t))
+                    d_1.md = np.append(d_1.md, __adj(m, self.tao))
                     i += 1
 
             if nmd_len > 0:
                 # Explain that the number of membership elements in d1 is greater than d2,
                 # and it is necessary to add elements of d2 membership.
                 i = 0.
                 u = d_2.nmd
                 while i < nmd_len:
-                    d_2.nmd = np.append(d_2.nmd, __adj(u, t))
+                    d_2.nmd = np.append(d_2.nmd, __adj(u, self.tao))
                     i += 1
             else:
                 i = 0.
                 u = d_1.nmd
                 while i < (-nmd_len):
-                    d_1.nmd = np.append(d_1.nmd, __adj(u, t))
+                    d_1.nmd = np.append(d_1.nmd, __adj(u, self.tao))
                     i += 1
             return d_1.qsort(), d_2.qsort()
         else:
             raise TypeError(f'Unsupported fuzzy type, {d1.mtype} and {d2.mtype}')
 
 
 # TODO：待实现
-class Absolute(Function):
+class FuzzAbsolute(Function):
     def function(self, x, y):
         ValueError(f'Not yet implemented!')
```

### Comparing `MohuPy-0.2.8/mohupy/core/fuzzarray.py` & `mohupy-0.3.0/mohupy/core/fuzzarray.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 from .base import MohuBase
 
 
 class Fuzzarray(MohuBase):
     __array_priority__ = 200
     __array = np.array([], dtype=object)
 
-    def __init__(self, qrung=None, mtype=None):
+    def __init__(self, qrung=None):
         super().__init__()
         self.ndim = 0
         self.size = 0
         self.shape = ()
-        from .function import initializeSet
-        self.qrung, self.mtype = initializeSet(qrung, mtype)
+
+        from .funcitonClass import InitializeSet
+        self.qrung, self.mtype = InitializeSet()(qrung)
 
     def __len__(self):
         return len(self.__array)
 
     @property
     def array(self):
         return self.__array
@@ -52,138 +53,141 @@
             self.size = value.size
             self.shape = value.shape
         else:
             raise TypeError(f"Invalid fuzzy type.")
 
     @property
     def score(self):
-        from .attribute import score
-        vec_func = np.vectorize(score)
+        from .attributeClass import Score
+        vec_func = np.vectorize(Score())
         return vec_func(self.__array)
 
     @property
     def acc(self):
-        from .attribute import acc
-        vec_func = np.vectorize(acc)
+        from .attributeClass import Accuracy
+        vec_func = np.vectorize(Accuracy())
         return vec_func(self.__array)
 
     @property
     def ind(self):
-        from .attribute import ind
-        vec_func = np.vectorize(ind)
+        from .attributeClass import Indeterminacy
+        vec_func = np.vectorize(Indeterminacy())
         return vec_func(self.__array)
 
     @property
     def comp(self) -> 'Fuzzarray':
-        from .attribute import comp
-        vec_func = np.vectorize(comp)
-        newset = Fuzzarray(self.qrung, self.mtype)
+        from .attributeClass import Complement
+        vec_func = np.vectorize(Complement())
+        newset = Fuzzarray(self.qrung)
         newset.array = vec_func(self.__array)
         return newset
 
     @property
     def md(self):
-        def membership(t):
-            if isinstance(t.md, (int, float, np.float_, np.int_)):
-                return np.float_(t.md)
-            if isinstance(t.md, (np.ndarray, list)):
-                return np.array(t.md, dtype=object)
-
-        vec_func = np.vectorize(membership)
-        return vec_func(self.__array)
+        if self.__array.size != 0:
+            def membership(t):
+                if isinstance(t.md, (int, float, np.float_, np.int_)):
+                    return np.float_(t.md)
+                if isinstance(t.md, (np.ndarray, list)):
+                    return np.array(t.md, dtype=object)
+
+            vec_func = np.vectorize(membership)
+            return vec_func(self.__array)
+        return None
 
     @property
     def nmd(self):
-        def membership(t):
-            if isinstance(t.nmd, (int, float, np.float_, np.int_)):
-                return np.float_(t.nmd)
-            if isinstance(t.nmd, (np.ndarray, list)):
-                return np.array(t.nmd, dtype=object)
-
-        vec_func = np.vectorize(membership)
-        return vec_func(self.__array)
+        if self.__array.size != 0:
+            def membership(t):
+                if isinstance(t.nmd, (int, float, np.float_, np.int_)):
+                    return np.float_(t.nmd)
+                if isinstance(t.nmd, (np.ndarray, list)):
+                    return np.array(t.nmd, dtype=object)
+
+            vec_func = np.vectorize(membership)
+            return vec_func(self.__array)
+        return None
 
     @property
     def T(self) -> 'Fuzzarray':
-        from .function import transpose
-        return transpose(self)
+        from .funcitonClass import FuzzTranspose
+        return FuzzTranspose()(self)
 
     def valid(self):
-        from .function import valid
-        return valid(self)
+        from .funcitonClass import FuzzValidity
+        return FuzzValidity()(self)
 
     def empty(self, onlyfn=False):
-        from .function import empty
-        return empty(self, onlyfn)
+        from .funcitonClass import FuzzEmpty
+        return FuzzEmpty(onlyfn)(self)
 
     def initial(self):
-        from .function import initial
-        return initial(self)
+        from .funcitonClass import FuzzInitial
+        return FuzzInitial()(self)
 
     def qsort(self, reverse=False):
-        from .function import qsort
-        return qsort(self, reverse)
+        from .funcitonClass import FuzzQsort
+        return FuzzQsort(reverse)(self)
 
     def unique(self, onlyfn=False):
-        from .function import unique
-        return unique(self, onlyfn)
+        from .funcitonClass import FuzzUnique
+        return FuzzUnique(onlyfn)(self)
 
     def append(self, e):
-        from .function import append
-        return append(self, e)
+        from .funcitonClass import FuzzAppend
+        return FuzzAppend(e)(self)
 
     def reshape(self, *shape):
-        from .function import reshape
-        return reshape(self, *shape)
+        from .funcitonClass import FuzzReshape
+        return FuzzReshape(*shape)(self)
 
     def squeeze(self, axis=None):
-        from .function import squeeze
-        return squeeze(self, axis)
+        from .funcitonClass import FuzzSqueeze
+        return FuzzSqueeze(axis)(self)
 
     def clear(self):
-        from .function import clear
-        return clear(self)
+        from .funcitonClass import FuzzClear
+        return FuzzClear()(self)
 
     def ravel(self):
-        from .function import ravel
-        return ravel(self)
+        from .funcitonClass import FuzzRavel
+        return FuzzRavel()(self)
 
     def flatten(self):
-        from .function import flatten
-        return flatten(self)
+        from .funcitonClass import FuzzFlatten
+        return FuzzFlatten()(self)
 
     def max(self, show=False, axis=None):
-        from .function import getmax
-        return getmax(self, show, axis)
+        from .funcitonClass import FuzzGetMax
+        return FuzzGetMax(show, axis)(self)
 
     def min(self, show=False, axis=None):
-        from .function import getmin
-        return getmin(self, show, axis)
+        from .funcitonClass import FuzzGetMin
+        return FuzzGetMin(show, axis)(self)
 
     def sum(self, axis=None, keepdims=False):
-        from .function import getsum
-        return getsum(self, axis, keepdims)
+        from .funcitonClass import FuzzGetSum
+        return FuzzGetSum(axis, keepdims)(self)
 
     def prod(self, axis=None, keepdims=False):
-        from .function import getprod
-        return getprod(self, axis, keepdims)
+        from .funcitonClass import FuzzGetProd
+        return FuzzGetProd(axis, keepdims)(self)
 
     def mean(self, axis=None):
-        from .function import mean
-        return mean(self, axis)
+        from .funcitonClass import FuzzMean
+        return FuzzMean(axis)(self)
 
-    def fmax(self, func, *args, show=False, axis=None):
-        from .function import fmax
-        return fmax(self, func, *args, show, axis)
-
-    def fmin(self, func, *args, show=False, axis=None):
-        from .function import fmin
-        return fmin(self, func, *args, show, axis)
+    def fmax(self, func, *params, show=False, axis=None):
+        from .funcitonClass import FuzzGetFmax
+        return FuzzGetFmax(show, axis, func, *params)(self)
+
+    def fmin(self, func, *params, show=False, axis=None):
+        from .funcitonClass import FuzzGetFmin
+        return FuzzGetFmin(show, axis, func, *params)(self)
 
     def remove(self, e):
-        from .function import remove
-        return remove(self, e)
+        from .funcitonClass import FuzzRemove
+        return FuzzRemove(e)(self)
 
     def pop(self, e):
-        from .function import pop
-        return pop(self, e)
-
+        from .funcitonClass import FuzzPop
+        return FuzzPop(e)(self)
```

### Comparing `MohuPy-0.2.8/mohupy/core/operation.py` & `mohupy-0.3.0/mohupy/core/operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,32 +32,34 @@
         # 模糊数 + 模糊数
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return __add(x, y)
 
         # 模糊数 + 集合（广播）
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__add)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
         # 集合 + 模糊数（广播）
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             vec_func = np.vectorize(__add)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         # 集合 + 集合
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__add)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y.array)
             return newset
 
+        return NotImplemented
+
 
 def add(x, y):
     return Addition()(x, y)
 
 
 class Subtraction(Operation):
     def function(self, x, y):
@@ -77,32 +79,34 @@
         # 模糊数 - 模糊数
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return __sub(x, y)
 
         # 模糊数 - 集合（广播）
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__sub)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
         # 集合 - 模糊数（广播）
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             vec_func = np.vectorize(__sub)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         # 集合 - 集合
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__sub)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y.array)
             return newset
 
+        return NotImplemented
+
 
 def sub(x, y):
     return Subtraction()(x, y)
 
 
 class Multiplication(Operation):
     def function(self, x, y):
@@ -144,70 +148,72 @@
             return __mul(x, y)
 
         if isinstance(x, Fuzznum) and isinstance(y, (int, float, np.float_, np.int_)):
             return __mul(x, y)
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
         if isinstance(x, Fuzznum) and isinstance(y, np.ndarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y.array)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, np.ndarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, (int, float, np.float_, np.int_)):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         ### TODO: 数在前的都有点问题，因为不能直接让其等于 Fuzzarray.__mul__，需要在低下的函数 mul() 调整
         if isinstance(x, (int, float, np.float_, np.int_)) and isinstance(y, Fuzznum):
             return __mul(x, y)
 
         if isinstance(x, (int, float, np.float_, np.int_)) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(y.qrung, y.mtype)
+            newset = Fuzzarray(y.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
         if isinstance(x, np.ndarray) and isinstance(y, Fuzznum):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(y.qrung, y.mtype)
+            newset = Fuzzarray(y.qrung)
             newset.array = vec_func(x, y)
             return newset
 
         if isinstance(x, np.ndarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__mul)
-            newset = Fuzzarray(y.qrung, y.mtype)
+            newset = Fuzzarray(y.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
+        return NotImplemented
+
 
 def mul(x, y):
     return Multiplication()(x, y)
 
 
 class Division(Operation):
     def function(self, x, y):
@@ -238,48 +244,50 @@
             return __div(x, y)
 
         if isinstance(x, Fuzznum) and isinstance(y, (int, float, np.float_, np.int_)):
             return __div(x, y)
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y.array)
             return newset
 
         if isinstance(x, Fuzznum) and isinstance(y, np.ndarray):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y.array)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, np.ndarray):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, (int, float, np.float_, np.int_)):
             vec_func = np.vectorize(__div)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, y)
             return newset
 
+        return NotImplemented
+
 
 def div(x, y):
     return Division()(x, y)
 
 
 class Power(Operation):
     def __init__(self, p):
@@ -299,41 +307,43 @@
             return operation.power(p, x0)
 
         if isinstance(x, Fuzznum) and isinstance(self.p, (int, float, np.float_, np.int_)):
             return __pow(x, self.p)
 
         if isinstance(x, Fuzznum) and isinstance(self.p, np.ndarray):
             vec_func = np.vectorize(__pow)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x, self.p)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(self.p, (int, float, np.float_, np.int_)):
             vec_func = np.vectorize(__pow)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, self.p)
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(self.p, np.ndarray):
             vec_func = np.vectorize(__pow)
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = vec_func(x.array, self.p)
             return newset
 
+        return NotImplemented
+
 
 def pow(x, p):
     return Power(p)(x)
 
 
 class MatrixMul(Operation):
     def function(self, x: Fuzzarray, y: Fuzzarray):
         assert x.ndim > 0, f"input operand 0 does not have enough dimensions."
         assert y.ndim > 0, f"input operand 1 does not have enough dimensions."
 
-        newset = Fuzzarray(x.qrung, x.mtype)
+        newset = Fuzzarray(x.qrung)
         newset.array = x.array @ y.array
         return newset
 
 
 def matmul(x, y):
     return MatrixMul()(x, y)
 
@@ -363,14 +373,16 @@
             vec_func = np.vectorize(__eq)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__eq)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def equal(x, y):
     return Equal()(x, y)
 
 
 class Inequality(Operation):
     def function(self, x, y):
@@ -397,14 +409,16 @@
             vec_func = np.vectorize(__ne)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__ne)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def inequal(x, y):
     return Inequality()(x, y)
 
 
 class Lt(Operation):
     def function(self, x, y):
@@ -439,14 +453,16 @@
             vec_func = np.vectorize(__lt)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__lt)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def lt(x, y):
     return Lt()(x, y)
 
 
 class Gt(Operation):
     def function(self, x, y):
@@ -481,14 +497,16 @@
             vec_func = np.vectorize(__gt)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__gt)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def gt(x, y):
     return Gt()(x, y)
 
 
 class Le(Operation):
     def function(self, x, y):
@@ -523,14 +541,16 @@
             vec_func = np.vectorize(__le)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__le)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def le(x, y):
     return Le()(x, y)
 
 
 class Ge(Operation):
     def function(self, x, y):
@@ -565,14 +585,16 @@
             vec_func = np.vectorize(__ge)
             return vec_func(x.array, y)
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             vec_func = np.vectorize(__ge)
             return vec_func(x.array, y.array)
 
+        return NotImplemented
+
 
 def ge(x, y):
     return Ge()(x, y)
 
 
 class GetItem(Operation):
     def __init__(self, slices):
```

### Comparing `MohuPy-0.2.8/mohupy/core/operationClass.py` & `mohupy-0.3.0/mohupy/core/operationClass.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,66 +5,72 @@
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 from .operationLib import archimedeanDict
 
 
 class BasicOperation:
-    norms = 'algebraic'
+    # norms = 'algebraic'
 
     def __init__(self, qrung, mtype):
         self.qrung = qrung
         self.mtype = mtype
 
     def add(self, x, y):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['add'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def sub(self, x, y):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['sub'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def mul(self, x, y):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['mul'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def div(self, x, y):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['div'][self.mtype](x.md, x.nmd, y.md, y.nmd, self.qrung)[1]
         return newfn
 
     def power(self, l, x):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['pow'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
         return newfn
 
     def times(self, l, x):
         from .fuzznums import Fuzznum
+        from ..config import Config
         newfn = Fuzznum()
         newfn.mtype = self.mtype
         newfn.qrung = self.qrung
-        newfn.md = archimedeanDict[self.norms]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
-        newfn.nmd = archimedeanDict[self.norms]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
+        newfn.md = archimedeanDict[Config.arch]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[0]
+        newfn.nmd = archimedeanDict[Config.arch]['tim'][self.mtype](l, x.md, x.nmd, self.qrung)[1]
         return newfn
```

### Comparing `MohuPy-0.2.8/mohupy/core/operationLib/__init__.py` & `mohupy-0.3.0/mohupy/core/operationLib/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/core/operationLib/algebraic.py` & `mohupy-0.3.0/mohupy/core/operationLib/algebraic.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 
 from ..base import Archimedean
 
-from ...constant import Approx
+from ..constant import Approx
 
 """
 The following is a quick calculation of Algebraic norms in fuzzy number. 
 The code has been used for the calculation of 'Fuzznum' and 'Fuzzarray', 
 so the Archimedean class is no longer used to complete the operation.
 """
```

### Comparing `MohuPy-0.2.8/mohupy/core/operationLib/algebraicoperation.py` & `mohupy-0.3.0/mohupy/core/operationLib/algebraicoperation.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/core/operationLib/einstein.py` & `mohupy-0.3.0/mohupy/core/operationLib/einstein.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/core/regedit.py` & `mohupy-0.3.0/mohupy/core/regedit.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/function/func.py` & `mohupy-0.3.0/mohupy/function/formula.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/9/21 下午8:25
+#  Date: 2024/4/12 下午1:48
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 
 
@@ -20,15 +20,15 @@
             x:  float or np.ndarray
                 the independent variable
             *args:
                 two parameters, representing the sigmoid
                 function parameters.
         returns:
         -------
-            y:  np.float or np.ndarray
+            y:  np.float_ or np.ndarray
                 the sigmoid function value
 
     """
     assert len(args) == 2, 'parameter list length must be 2.'
     return 1. / (1. + np.exp(- args[0] * (x - args[1])))
 
 
@@ -48,15 +48,15 @@
         -------
             y:  np.float np.ndarray
                 the triangular function value
     """
     assert len(args) == 3, 'parameter must have exactly three elements.'
     assert args[0] <= args[1] <= args[2], 'parameters requires the three elements a <= b <= c.'
 
-    if type(x) != np.ndarray:
+    if isinstance(x, np.ndarray):
         x = np.array([x])
     y = np.zeros(len(x))
 
     # Left side
     if args[0] != args[1]:
         idx = np.nonzero(np.logical_and(args[0] < x, x < args[1]))[0]
         y[idx] = (x[idx] - args[0]) / float(args[1] - args[0])
@@ -90,15 +90,15 @@
         -------
             y:  float or np.ndarray
                 the z-shape function value
     """
     assert len(args) == 2, 'parameter list length must be 2.'
     assert args[0] <= args[1], 'a <= b is required.'
 
-    if type(x) != np.ndarray:
+    if isinstance(x, np.ndarray):
         x = np.array([x])
     y = np.ones(len(x))
 
     idx = np.logical_and(args[0] <= x, x < (args[0] + args[1]) / 2.)
     y[idx] = 1 - 2. * ((x[idx] - args[0]) / (args[1] - args[0])) ** 2.
 
     idx = np.logical_and((args[0] + args[1]) / 2. <= x, x <= args[1])
@@ -126,15 +126,15 @@
         returns:
             y:  float or np.ndarray
                 the trapezoidal function value
     """
     assert len(args) == 4, 'abcd parameter must have exactly four elements.'
     assert args[0] <= args[1] <= args[2] <= args[3], 'abcd requires the four elements \
                                           a <= b <= c <= d.'
-    if type(x) != np.ndarray:
+    if isinstance(x, np.ndarray):
         x = np.array([x])
     y = np.ones(len(x))
 
     idx = np.nonzero(x <= args[1])[0]
     y[idx] = trimf(x[idx], np.r_[args[0], args[1], args[1]])
 
     idx = np.nonzero(x >= args[2])[0]
@@ -167,15 +167,15 @@
         returns:
         -------
             y:  float or np.ndarray
                 the S-shape function value
     """
     assert len(args) == 2, 'parameter list length must be 2.'
     assert args[0] <= args[1], 'a <= b is required.'
-    if type(x) != np.ndarray:
+    if isinstance(x, np.ndarray):
         x = np.array([x])
     y = np.ones(len(x))
     idx = x <= args[0]
     y[idx] = 0
 
     idx = np.logical_and(args[0] <= x, x <= (args[0] + args[1]) / 2.)
     y[idx] = 2. * ((x[idx] - args[0]) / (args[1] - args[0])) ** 2.
@@ -234,15 +234,15 @@
         returns:
         -------
             y:  float or np.ndarray
                 the Bi-Gaussian function value
     """
     assert len(args) == 4, 'parameter list length must be 4.'
     assert args[0] <= args[2], 'args[0] <= args[2] is required.  See docstring.'
-    if type(x) != np.ndarray:
+    if isinstance(x, np.ndarray):
         x = np.asarray([x])
     y = np.ones(len(x))
     idx1 = x <= args[0]
     idx2 = x > args[2]
     y[idx1] = gaussmf(x[idx1], [args[0], args[1]])
     y[idx2] = gaussmf(x[idx2], [args[2], args[3]])
     if len(y) == 1:
```

### Comparing `MohuPy-0.2.8/mohupy/function/mem_func.py` & `mohupy-0.3.0/mohupy/generator/membershipfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/9/21 下午8:25
+#  Date: 2024/4/12 下午1:49
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 
 from matplotlib import pyplot as plt
 
 
-class memFunc(object):
+class MembershipFunc(object):
     """
         Membership function class. This class organizes 8 commonly used
         membership functions together. In addition, custom membership
         functions can be set.
 
         The format of the custom membership function is as follows.
         This is just an example, because the function's range is not in
@@ -59,17 +59,17 @@
     __VARI_END = 1.
     __LINSPACE = 100
 
     __func = None
     __parameters = None
 
     def __init__(self, func=None, *args):
-        from .func import (sigmf, trimf, zmf,
-                           trapmf, smf, gaussmf,
-                           gauss2mf, gbellmf)
+        from ..function import (sigmf, trimf, zmf,
+                               trapmf, smf, gaussmf,
+                               gauss2mf, gbellmf)
 
         func_list = [sigmf, trimf, zmf, trapmf, smf, gaussmf, gauss2mf, gbellmf]
         if func is None:
             pass
         elif func in func_list:
             self.__func = func
             self.__parameters = args
```

### Comparing `MohuPy-0.2.8/mohupy/lib/io.py` & `mohupy-0.3.0/mohupy/corelib/lib/classIO.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,161 +1,157 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午6:36
+#  Date: 2024/4/7 下午1:57
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 import warnings
 
 import numpy as np
 import pandas as pd
 
-from ..core import Fuzznum, Fuzzarray
-
+from ...core import Fuzznum, Fuzzarray
 from .base import Library
 
 
 class Savez(Library):
     """
         Save data to npz file
     """
+    def __init__(self, x: Fuzzarray):
+        self.fuzz = x
 
-    def function(self, x, path):
-        # from ..base.nums import Fuzznum
-        # from ..base.array import Fuzzarray
-        if isinstance(x, Fuzznum):
-            raise IOError(f'Invalid save for {type(x)}.')
-        if isinstance(x, Fuzzarray):
+    def function(self, path):
+        if isinstance(self.fuzz, Fuzznum):
+            raise IOError(f'Invalid save for {type(self.fuzz)}.')
+        if isinstance(self.fuzz, Fuzzarray):
             try:
                 np.savez_compressed(
                     path,
-                    array=x.array,
-                    mtype=x.mtype,
-                    qrung=x.qrung)
+                    array=self.fuzz.array,
+                    mtype=self.fuzz.mtype,
+                    qrung=self.fuzz.qrung)
             except IOError as e:
                 print(f'Save failed.' + str(e))
 
 
-def savez(x, path):
-    return Savez()(x, path)
-
-
 class Loadz(Library):
     """
         Load data from npz file
     """
-
-    def function(self, x, path):
-        # from ..base.nums import Fuzznum
-        # from ..base.array import Fuzzarray
-        if isinstance(x, Fuzznum):
-            raise IOError(f'Invalid load for {type(x)}.')
-        if isinstance(x, Fuzzarray):
-            if x.initial():
-                new = np.load(path, allow_pickle=True)
-                x.qrung = new['qrung']
-                x.mtype = new['mtype']
-                x.array = new['array']
-            else:
-                warnings.warn('Loading existing data will overwrite the original data!', Warning)
-                x = x.clear()
-                new = np.load(path, allow_pickle=True)
-                x.qrung = new['qrung']
-                x.mtype = new['mtype']
-                x.array = new['array']
-        raise IOError(f'Invalid load for {type(x)}.')
-
-
-def loadz(x, path):
-    return Loadz()(x, path)
+    def function(self, path):
+        newset = Fuzzarray()
+        new = np.load(path, allow_pickle=True)
+        from ...config import Config, set_mtype
+        mtype = str(new['mtype'])
+        if Config.mtype != new['mtype']:
+            warnings.warn(f'The fuzzy number type changed: ({Config.mtype} -> {mtype})', Warning)
+        set_mtype(mtype)
+        newset.qrung = int(new['qrung'])
+        newset.mtype = str(new['mtype'])
+        newset.array = new['array']
+        return newset
+
+        # if isinstance(self.fuzz, Fuzznum):
+        #     raise IOError(f'Invalid load for {type(self.fuzz)}.')
+        # if isinstance(self.fuzz, Fuzzarray):
+        #     if self.fuzz.initial():
+        #         new = np.load(path, allow_pickle=True)
+        #         from ...config import Config, set_mtype
+        #         mtype = new['mtype']
+        #         if Config.mtype != new['mtype']:
+        #             warnings.warn(f'The fuzzy number type changed: ({Config.mtype} -> {mtype})', Warning)
+        #         set_mtype(self.fuzz.mtype)
+        #
+        #         self.fuzz.qrung = new['qrung']
+        #         self.fuzz.mtype = new['mtype']
+        #         self.fuzz.array = new['array']
+        #     else:
+        #         warnings.warn('Loading existing data will overwrite the original data!', Warning)
+        #         self.fuzz = self.fuzz.clear()
+        #         new = np.load(path, allow_pickle=True)
+        #
+        #         from ...config import Config, set_mtype
+        #         mtype = new['mtype']
+        #         if Config.mtype != new['mtype']:
+        #             warnings.warn(f'The fuzzy number type changed: ({Config.mtype} -> {mtype})', Warning)
+        #         set_mtype(self.fuzz.mtype)
+        #
+        #         self.fuzz.qrung = new['qrung']
+        #         self.fuzz.mtype = new['mtype']
+        #         self.fuzz.array = new['array']
+        # raise IOError(f'Invalid load for {type(self.fuzz)}.')
 
 
 class ToCSV(Library):
     """
         Save a fuzzy set to a .csv file.
 
         This method only saves the fuzzy set, and does not save the related
         information of the set.
 
-        Parameters
-        ----------
-            f:  Fuzzarray
-                The fuzzy set.
-            path:  str
-                The path to the file.
-
         Returns
         -------
             Boolean
 
         Notes
         -----
             This method saves the fuzzy set to a.csv file.
     """
-    def __init__(self, header, index_col):
+    def __init__(self, fuzz: Fuzzarray, header, index_col):
+        self.fuzz = fuzz
         self.header = header
         self.index_col = index_col
 
-    def function(self, f: Fuzzarray, path: str, float_format: int):
-        if 0 <= f.ndim <= 2:
+    def function(self, path: str):
+        if 0 <= self.fuzz.ndim <= 2:
             try:
-                pd.DataFrame(f.array, columns=self.header, index=self.index_col).to_csv(path, float_format=f'%.{float_format}f')
+                if isinstance(self.fuzz.array, Fuzzarray):
+                    pd.DataFrame(self.fuzz.array, columns=self.header, index=self.index_col).to_csv(path)
+                else:
+                    pd.DataFrame(np.array(self.fuzz), columns=self.header, index=self.index_col).to_csv(path)
             except Exception as e:
-                print(f'{e}: Save failed.')
+                raise IOError(f'{e}: Save failed.')
         else:
-            raise ValueError(f'The ndim of fuzzy array is invalid: ndim={f.ndim}')
-
-
-def to_csv(x: Fuzzarray, path: str, header=None, index_col=None, float_format=5):
-    return ToCSV(header, index_col)(x, path, float_format)
+            raise ValueError(f'The ndim of fuzzy array is invalid: ndim={self.fuzz.ndim}')
 
 
 class LoadCSV(Library):
     """
         Load a fuzzy set from a.csv file.
 
         This method is used to load a fuzzy set table with unknown information. It
         is necessary to judge the content of the fuzzy table during loading. When
         initializing a fuzzy set, Q-rung and fuzzy set type are given, so it is necessary
         to judge whether a fuzzy set meets these two conditions. This method will only
         load when the fuzzy set table is equal to or satisfied with the initial fuzzy set
         condition.
 
-        Parameters
-        ----------
-            path:  str
-                The path to the file.
-            q:  int
-                The q rung of the fuzzy set.
-            mtype:  str
-                The type of the fuzzy set.
 
         Returns
         -------
             Fuzzarray
                 The fuzzy set.
 
         Notes
         -----
             This method loads the fuzzy set from a.csv file.
     """
-    def __init__(self, header, index_col):
+    def __init__(self, qrung, header, index_col):
+        self.qrung = qrung
         self.header = header
         self.index_col = index_col
 
-    def function(self, path: str, q: int, mtype: str):
+    def function(self, path: str):
         try:
             m = pd.read_csv(path, header=self.header, index_col=self.index_col).to_numpy()
-            from .string import str2fuzz
-            vec_func = np.vectorize(str2fuzz)
-            f = vec_func(m, q, mtype)
-
-            newset = Fuzzarray(q, mtype)
-            newset.array = f
-            return newset
+            from .classString import StrToFuzz
+            vec_func = np.vectorize(lambda x: StrToFuzz(self.qrung)(x))
+            newset = Fuzzarray(self.qrung)
+            try:
+                newset.array = vec_func(m)
+                return newset
+            except Exception as e:
+                Exception(f'Please check if the mtype type matches. error:{e}')
         except Exception as e:
             print(f'{e}: Load failed.')
-
-
-def load_csv(path: str, q: int, mtype: str, header='infer', index_col=0) -> Fuzzarray:
-    return LoadCSV(header, index_col)(path, q, mtype)
-
```

### Comparing `MohuPy-0.2.8/mohupy/lib/measure.py` & `mohupy-0.3.0/mohupy/corelib/lib/classMeasure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午7:09
+#  Date: 2024/4/7 下午2:00
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-"""
-    This file is an implementation of some fuzzy metrics, including distance metrics (implemented),
-    similar phase metrics, entropy metrics, and so on
-"""
+
 import numpy as np
 
 from .base import Library
 from ..regedit import fuzzDis
+from ...core import Fuzznum, Fuzzarray
+from ...config import Config
 
 
 class Distance(Library):
     def function(self, f1, f2, l, t, indeterminacy):
         """
             The generalized distance function for two Q-rung hesitant fuzzy elements.
             The parameter 'l' is the generic distance function parameter. 'l=1' indicates
@@ -33,24 +32,19 @@
                 l=2 indicates the Euclidean distance
             t: the parameter of the normalization function.
                 t=1 indicates optimistic normalization
                 t=0 indicates pessimistic normalization.
             indeterminacy: Bool
                 Determine whether the distance formula contains indeterminacy.
         """
-        mtype = f1.mtype
-        from ..core import Fuzznum, Fuzzarray
+
         if isinstance(f1, Fuzznum) and isinstance(f2, Fuzznum):
-            return fuzzDis[mtype](f1, f2, l, t, indeterminacy)
+            return fuzzDis[Config.mtype](f1, f2, l, t, indeterminacy)
         if isinstance(f1, Fuzznum) and isinstance(f2, Fuzzarray):
-            vec_func = np.vectorize(fuzzDis[mtype])
+            vec_func = np.vectorize(fuzzDis[Config.mtype])
             return vec_func(f1, f2.array, l, t, indeterminacy)
         if isinstance(f1, Fuzzarray) and isinstance(f2, Fuzznum):
-            vec_func = np.vectorize(fuzzDis[mtype])
+            vec_func = np.vectorize(fuzzDis[Config.mtype])
             return vec_func(f1.array, f2, l, t, indeterminacy)
         if isinstance(f1, Fuzzarray) and isinstance(f2, Fuzzarray):
-            vec_func = np.vectorize(fuzzDis[mtype])
+            vec_func = np.vectorize(fuzzDis[Config.mtype])
             return vec_func(f1.array, f2.array, l, t, indeterminacy)
-
-
-def distance(f1, f2, l=2, t=1, indeterminacy=True):
-    return Distance()(f1, f2, l, t, indeterminacy)
```

### Comparing `MohuPy-0.2.8/mohupy/lib/other.py` & `mohupy-0.3.0/mohupy/utils/other.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午7:46
+#  Date: 2024/4/12 上午11:58
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 from matplotlib import pyplot as plt
 
 import numpy as np
```

### Comparing `MohuPy-0.2.8/mohupy/lib/plotlib.py` & `mohupy-0.3.0/mohupy/corelib/lib/classPlot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午7:38
+#  Date: 2024/4/7 下午2:03
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 import numpy as np
 from matplotlib import pyplot as plt
 
 from .base import Library
 from ..regedit import fuzzPlot
-from ..core import Fuzznum, Fuzzarray
+from ...core import Fuzznum, Fuzzarray
+from ...config import Config
 
 
 class Plot(Library):
     def function(self, f: (Fuzzarray, Fuzznum), other, add, sub, mul, div,
                  color, color_area, alpha, label, legend):
 
         if color_area is None:
             color_area = ['red', 'green', 'blue', 'yellow']
 
         q = f.qrung
-        mtype = f.mtype
 
         plt.gca().spines['top'].set_linewidth(False)
         plt.gca().spines['bottom'].set_linewidth(True)
         plt.gca().spines['left'].set_linewidth(True)
         plt.gca().spines['right'].set_linewidth(False)
         plt.axis((0, 1.1, 0, 1.1))
         plt.axhline(y=0)
         plt.axvline(x=0)
 
         if isinstance(f, Fuzznum):
-            fuzzPlot[mtype](f,
+            fuzzPlot[Config.mtype](f,
                             other=other,
                             add=add,
                             sub=sub,
                             mul=mul,
                             div=div,
                             color=color,
                             color_area=color_area,
                             alpha=alpha)
         if isinstance(f, Fuzzarray):
-            plot_vec = np.vectorize(fuzzPlot[mtype])
+            plot_vec = np.vectorize(fuzzPlot[Config.mtype])
             plot_vec(f.array,
                      other=other,
                      color=color,
                      alpha=alpha,
                      add=add,
                      sub=sub,
                      mul=mul,
@@ -53,22 +54,7 @@
                      color_area=None)
 
         x = np.linspace(0, 1, 1000)
         y = (1 - x ** q) ** (1 / q)
         plt.plot(x, y, label=label)
         if legend: plt.legend(loc='upper right', fontsize='small')
         plt.show()
-
-
-def plot(f: (Fuzzarray, Fuzznum),
-         other=None,
-         add=None,
-         sub=None,
-         mul=None,
-         div=None,
-         color='red',
-         color_area=None,
-         alpha=0.3,
-         label='',
-         legend=False):
-    return Plot()(f, other, add, sub, mul, div,
-                  color, color_area, alpha, label, legend)
```

### Comparing `MohuPy-0.2.8/mohupy/math/product.py` & `mohupy-0.3.0/mohupy/corelib/math/classProduct.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/29 下午3:47
+#  Date: 2024/4/7 下午2:17
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
-from typing import Union
 
 import numpy as np
 
 from .base import Mathematics
-from ..core import Fuzznum, Fuzzarray
+from ...core import Fuzznum, Fuzzarray
 
 
 class Dot(Mathematics):
     def function(self, x, y):
         """
             Returns the dot product of two Fuzzarray.
 
@@ -32,42 +31,38 @@
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return x * y
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             if y.ndim == 0:
                 return np.dot(x, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.dot(x, y.array)
                 newset.array = result
                 return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             if x.ndim == 0:
                 return np.dot(x.array, y)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.dot(x.array, y)
                 newset.array = result
                 return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             if x.ndim == 0 and y.ndim == 0:
                 return np.dot(x.array, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.dot(x.array, y.array)
                 newset.array = result
                 return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def dot(x, y) -> Union[Fuzznum, Fuzzarray]:
-    return Dot()(x, y)
-
-
 class Inner(Mathematics):
     def function(self, x, y):
         """
             Returns the inner product of two Fuzzarray.
 
             Parameters
             ----------
@@ -84,42 +79,38 @@
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return x * y
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             if y.ndim == 0:
                 return np.inner(x, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.inner(x, y.array)
                 newset.array = result
                 return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             if x.ndim == 0:
                 return np.inner(x.array, y)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.inner(x.array, y)
                 newset.array = result
                 return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             if x.ndim == 0 and y.ndim == 0:
                 return np.inner(x.array, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 result = np.inner(x.array, y.array)
                 newset.array = result
                 return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def inner(x, y) -> Union[Fuzznum, Fuzzarray]:
-    return Inner()(x, y)
-
-
 class Outer(Mathematics):
     def function(self, x, y):
         """
             Returns the outer product of two Fuzzarray.
 
             Parameters
             ----------
@@ -131,41 +122,37 @@
             Returns
             -------
             Fuzzarray or np.float_
                 The outer product of x and y.
         """
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             result = np.outer(x, y)
-            newset = Fuzzarray(x.qrung, y.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = result
             return newset
 
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             result = np.outer(x, y.array)
             newset.array = result
             return newset
 
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             result = np.outer(x.array, y)
             newset.array = result
             return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             result = np.outer(x.array, y.array)
             newset.array = result
             return newset
         raise ValueError(f'Invalid input type {type(x)} and {type(y)}')
 
 
-def outer(x, y) -> Union[Fuzznum, Fuzzarray]:
-    return Outer()(x, y)
-
-
 class Cartadd(Mathematics):
     def function(self, x, y):
         """
             Returns the cartesian sum of two Fuzzarray.
 
             Parameters
             ----------
@@ -194,37 +181,33 @@
         """
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
             return np.add.outer(x, y)
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
             if y.ndim == 0:
                 return np.add.outer(x, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 newset.array = np.add.outer(x, y.array)
                 return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
             if x.ndim == 0:
                 return np.add.outer(x.array, y)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 newset.array = np.add.outer(x.array, y)
                 return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
             if x.ndim == 0 and y.ndim == 0:
                 return np.add.outer(x.array, y.array)
             else:
-                newset = Fuzzarray(x.qrung, x.mtype)
+                newset = Fuzzarray(x.qrung)
                 newset.array = np.add.outer(x.array, y.array)
                 return newset
 
 
-def cartadd(x, y) -> Union[Fuzznum, Fuzzarray]:
-    return Cartadd()(x, y)
-
-
 class Cartprod(Mathematics):
     def function(self, x, y):
         """
             Returns the cartesian product of two Fuzzarray.
 
             Parameters
             ----------
@@ -235,26 +218,22 @@
 
             Returns
             -------
             Fuzzarray or np.float_
                 The cartesian product of x and y.
         """
         if isinstance(x, Fuzznum) and isinstance(y, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.asarray(np.meshgrid(x, y))
             return newset
         if isinstance(x, Fuzznum) and isinstance(y, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.asarray(np.meshgrid(x, y.array))
             return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzznum):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.asarray(np.meshgrid(x.array, y))
             return newset
         if isinstance(x, Fuzzarray) and isinstance(y, Fuzzarray):
-            newset = Fuzzarray(x.qrung, x.mtype)
+            newset = Fuzzarray(x.qrung)
             newset.array = np.asarray(np.meshgrid(x.array, y.array))
             return newset
-
-
-def cartprod(x, y) -> Union[Fuzznum, Fuzzarray]:
-    return Cartprod()(x, y)
```

### Comparing `MohuPy-0.2.8/mohupy/measure/__init__.py` & `mohupy-0.3.0/mohupy/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/measure/fuzzmeas.py` & `mohupy-0.3.0/mohupy/measure/fuzzmeas.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import re
 
 import numpy as np
-from ..constant import Approx
+from ..core import Approx
 
 
 def dirac_meas(e, s):
     """
         Dirac_measure(Bool fuzzy measure). The Dirac measure is a simple
             0-1 fuzzy measure. The element and subset must be a subset of the set.
             When the element is in the subset the Dirac measure is 1. Otherwise, the
```

### Comparing `MohuPy-0.2.8/mohupy/measure/hasse.py` & `mohupy-0.3.0/mohupy/measure/hasse.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/measure/indices.py` & `mohupy-0.3.0/mohupy/measure/indices.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/measure/integral.py` & `mohupy-0.3.0/mohupy/measure/integral.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/measure/utils.py` & `mohupy-0.3.0/mohupy/measure/utils.py`

 * *Files identical despite different names*

### Comparing `MohuPy-0.2.8/mohupy/regedit/construct.py` & `mohupy-0.3.0/mohupy/corelib/regedit/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,106 +1,104 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午4:26
+#  Date: 2024/4/7 下午1:21
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 import numpy as np
 
-from ..core.regedit import Registry
-from ..core import Fuzzarray
+from ...core import Registry, Fuzzarray, Fuzznum
 
 fuzzZeros = Registry()
 fuzzPoss = Registry()
 fuzzNegs = Registry()
 
 
 ################################
 # qrofn
 ################################
 @fuzzZeros('qrofn')
 def zeros_qrofn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, 0., 0.), dtype=object)
-    newset = Fuzzarray(q, 'qrofn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzPoss('qrofn')
-def poss_qrofn(q, *n)  -> Fuzzarray:
+def poss_qrofn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, 1., 0.), dtype=object)
-    newset = Fuzzarray(q, 'qrofn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzNegs('qrofn')
 def negs_qrofn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, 0., 1.), dtype=object)
-    newset = Fuzzarray(q, 'qrofn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 ################################
 # ivfn
 ################################
 @fuzzZeros('ivfn')
 def zeros_ivfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, (0., 0.), (0., 0.)), dtype=object)
-    newset = Fuzzarray(q, 'ivfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzPoss('ivfn')
 def poss_ivfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, (1., 1.), (0., 0.)), dtype=object)
-    newset = Fuzzarray(q, 'ivfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzNegs('ivfn')
 def negs_ivfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, (0., 0.), (1., 1.)), dtype=object)
-    newset = Fuzzarray(q, 'ivfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 ################################
 # qrohfn
 ################################
 @fuzzZeros('qrohfn')
 def zeros_qrohfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, [0], [0]), dtype=object)
-    newset = Fuzzarray(q, 'qrohfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzPoss('qrohfn')
 def poss_qrohfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, [1], [0]), dtype=object)
-    newset = Fuzzarray(q, 'qrohfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
 @fuzzNegs('qrohfn')
 def negs_qrohfn(q, *n) -> Fuzzarray:
     s = np.full(n, Fuzznum(q, [0], [1]), dtype=object)
-    newset = Fuzzarray(q, 'qrohfn')
+    newset = Fuzzarray(q)
     newset.array = s
     return newset
 
 
-from ..core import Fuzznum
-
 fuzzZero = Registry()
 fuzzPos = Registry()
 fuzzNeg = Registry()
 
 ZERO_QROFN = lambda q: Fuzznum(q, 0., 0.)
 ZERO_IVFN = lambda q: Fuzznum(q, (0., 0.), (0., 0.))
 ZERO_QROHFN = lambda q: Fuzznum(q, [0.], [0.])
```

### Comparing `MohuPy-0.2.8/mohupy/regedit/distance.py` & `mohupy-0.3.0/mohupy/corelib/regedit/distance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午5:34
+#  Date: 2024/4/7 下午1:27
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import copy
 import numpy as np
 
-from ..core.regedit import Registry
+from ...core import Registry
 
 fuzzDis = Registry()
 
 
 @fuzzDis('qrofn')
 def distance_qrofn(f1,
                    f2,
@@ -100,21 +100,23 @@
     ----------
         A. R. Mishra, S.-M. Chen, and P. Rani, “Multiattribute decision-making
         based on Fermatean hesitant fuzzy sets and modified VIKOR method,”
         Inform Sciences, vol. 607, pp. 1532–1549, 2022, doi: 10.1016/j.ins.2022.06.037.
     """
     assert 0 <= t <= 1, "risk factor 't' must be in [0,1] range."
     assert d1.qrung == d2.qrung, "the qrung of two fuzzy number must be equal."
-    assert not d1.isEmpty() and not d2.isEmpty(), "the two q-rohfns must be not empty."
+    assert not d1.empty() and not d2.empty(), "the two q-rohfns must be not empty."
 
     d_1 = copy.deepcopy(d1)
     d_2 = copy.deepcopy(d2)
     q = d1.qrung
-    from ..core import normalize
-    d_1, d_2 = normalize(d_1, d_2, t)
+    # from ...core import normalize
+
+    from ...core.funcitonClass import FuzzNormalize
+    d_1, d_2 = FuzzNormalize(t)(d_1, d_2)
 
     mds = 0.
     nmds = 0.
 
     pi1 = d_1.ind
     pi2 = d_2.ind
     pi = np.fabs(pi1 ** q - pi2 ** q) ** l
@@ -127,7 +129,9 @@
     mds = mds / len(d_1.md)
     nmds = nmds / len(d_1.nmd)
 
     if indeterminacy:
         return (0.5 * (mds + nmds + pi)) ** (1 / l)
     else:
         return (0.5 * (mds + nmds)) ** (1 / l)
+
+
```

### Comparing `MohuPy-0.2.8/mohupy/regedit/plotlib.py` & `mohupy-0.3.0/mohupy/corelib/regedit/plotlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午6:24
+#  Date: 2024/4/7 下午1:31
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import numpy as np
 from matplotlib import pyplot as plt
 
-from ..core import Fuzznum
-from ..core.regedit import Registry
+from ...core import Fuzznum, Registry
 
 fuzzPlot = Registry()
 
 
 @fuzzPlot('qrofn')
 def plot_qrofn(x: Fuzznum,
                other: Fuzznum = None,
@@ -194,7 +193,9 @@
             alpha : float
                     The transparency of the Q-ROFN distribution.
             area:   None
             color_area: None
     """
     # TODO: q-ROHFN scatter plot is not implemented yet
     raise ValueError('q-rung orthopair hesitant fuzzy number scatter plot is not implemented yet')
+
+
```

### Comparing `MohuPy-0.2.8/mohupy/regedit/random.py` & `mohupy-0.3.0/mohupy/corelib/regedit/random.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午3:12
+#  Date: 2024/4/7 下午1:24
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
+
 import numpy as np
 np.set_printoptions(suppress=True)
 
-from ..core.regedit import Registry
-from ..constant import Approx
+from ...core import Registry, Approx
 
 fuzzRandom = Registry()
 
 
 @fuzzRandom('qrofn')
 def random_qrofn(q, minnum=None, maxnum=None):
     """
@@ -27,15 +27,15 @@
             maxnum: int
                 Maximum number of generated
 
         Returns
         -------
             Fuzznum
     """
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, 0., 0.)
     while True:
         newfn.md = np.round(np.random.rand(), Approx.round)
         newfn.nmd = np.round(np.random.rand(), Approx.round)
         if newfn.valid():
             break
     return newfn
@@ -55,15 +55,15 @@
             maxnum: int
                 Maximum number of generated
 
         Returns
         -------
             fuzznum
     """
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, (0., 0.), (0., 0.))
     while True:
         newfn.md = np.round(np.asarray([np.random.rand(), np.random.rand()]), Approx.round)
         newfn.nmd = np.round(np.asarray([np.random.rand(), np.random.rand()]), Approx.round)
         if newfn.valid():
             break
     return newfn
@@ -82,18 +82,21 @@
             maxnum: int
                 Maximum number of generated
 
         Returns
         -------
             fuzznum
     """
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, [], [])
     newfn.md = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
     newfn.nmd = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
     while True:
         newfn.md = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
         newfn.nmd = np.round(np.random.rand(np.random.randint(minnum, maxnum)), Approx.round)
         if newfn.valid():
             break
     return newfn
 
+
+def fuzz_random_seed(seed):
+    np.random.seed(seed)
```

### Comparing `MohuPy-0.2.8/mohupy/regedit/str2num.py` & `mohupy-0.3.0/mohupy/corelib/regedit/str2num.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-#  Copyright (c) yibocat 2023 All Rights Reserved
+#  Copyright (c) yibocat 2024 All Rights Reserved
 #  Python: 3.10.9
-#  Date: 2023/11/28 下午5:07
+#  Date: 2024/4/7 下午1:29
 #  Author: yibow
 #  Email: yibocat@yeah.net
 #  Software: MohuPy
 
 import re
 import numpy as np
 
-from ..core import Fuzznum
-from ..core.regedit import Registry
+from ...core import Fuzznum, Registry
 
 fuzzString = Registry()
 
 
 @fuzzString('qrofn')
 def str2qrofn(s: str, q) -> Fuzznum:
     """
@@ -26,15 +25,15 @@
         Returns
         -------
             Fuzznum
 
         Notes: When the input data is 0, it should be set to ZERO
         Q-rung fuzzy convert function accepts the form: [x,x]
     """
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, 0., 0.)
     t = re.findall(r'^<(\d.*?\d)>$', s)
     assert len(t) == 1, \
         'data format error.'
     x = re.findall(r'\d.?\d*', t[0])
     assert len(x) == 2, \
         'data format error.'
@@ -42,15 +41,15 @@
     newfn.nmd = float(x[1])
     assert newfn.valid(), f'data format is correct, but the data is invalid: {s}'
     return newfn
 
 
 @fuzzString('ivfn')
 def str2ivfn(s: str, q) -> Fuzznum:
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, (0., 0.), (0., 0.))
     t2 = re.findall(r'\[(\d.*?\d)\s?]', s)
     assert len(t2) == 2, \
         'data format error.'
     md = re.findall(r'\d.?\d*', t2[0])
     nmd = re.findall(r'\d.?\d*', t2[1])
     assert len(md) == 2 and len(nmd) == 2, \
@@ -76,20 +75,20 @@
         [[x,x,x,x],[x,x,x,x]].
 
         Parameters
         ----------
             s : str
                 Input data.
             q : int
-                Q-rung.
+                q-rung.
         Returns
         -------
             MohuQROHFN
     """
-    from ..core import fuzznum
+    from ...core import fuzznum
     newfn = fuzznum(q, [], [])
     t2 = re.findall(r'\[(\d.*?\d)\s*?]', s)
     assert len(t2) == 2, f'data format error:{t2}'
     md = re.findall(r'\d.?\d*', t2[0])
     nmd = re.findall(r'\d.?\d*', t2[1])
 
     for i in range(len(md)):
```

### Comparing `MohuPy-0.2.8/mohupy/runtime.py` & `mohupy-0.3.0/mohupy/runtime.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 # from .core.interface import mohuParent
 
 # Initialize fuzzy parent class, also indicates the currently used fuzzy number type
 # It is worth noting: fuzzyParent is a dictionary whose keys represent parent classes
 # and values represent subclasses.
 # fuzzParent = mohuParent.memo
 
-from .regedit import *
+from .corelib.regedit import *
 from .core import FuzzType, archimedeanDict
+from .corelib.regedit import (fuzzZeros, fuzzPoss, fuzzNegs,
+                              fuzzDis, fuzzString, fuzzRandom, fuzzPlot)
 
 
 class info:
     type = FuzzType
     archDict = archimedeanDict
 
     zeros = fuzzZeros
```

### Comparing `MohuPy-0.2.8/setup.py` & `mohupy-0.3.0/setup.py`

 * *Files identical despite different names*

