# Comparing `tmp/python-tgpt-0.5.8.tar.gz` & `tmp/python-tgpt-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tgpt-0.5.8.tar", last modified: Thu Mar 21 10:14:00 2024, max compression
+gzip compressed data, was "python-tgpt-0.6.0.tar", last modified: Fri Apr 12 03:30:10 2024, max compression
```

## Comparing `python-tgpt-0.5.8.tar` & `python-tgpt-0.6.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.503404 python-tgpt-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-03-21 10:14:00.503404 python-tgpt-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 10:14:00.503404 python-tgpt-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.491404 python-tgpt-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    77677 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10106 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.495405 python-tgpt-0.5.8/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    23471 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.499405 python-tgpt-0.5.8/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.503404 python-tgpt-0.5.8/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-21 10:14:00.000000 python-tgpt-0.5.8/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 10:14:00.503404 python-tgpt-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_blackboxai.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_gpt4free.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_koboldai.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_leo.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_opengpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_phind.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-21 10:13:38.000000 python-tgpt-0.5.8/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-04-12 03:30:09.000000 python-tgpt-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:30:10.082981 python-tgpt-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.066980 python-tgpt-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.066980 python-tgpt-0.6.0/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78689 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.070981 python-tgpt-0.6.0/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8709 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23471 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.074981 python-tgpt-0.6.0/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.078981 python-tgpt-0.6.0/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 03:30:10.000000 python-tgpt-0.6.0/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:30:10.078981 python-tgpt-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_blackboxai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_gpt4free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_koboldai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_leo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_opengpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-12 03:29:41.000000 python-tgpt-0.6.0/tests/test_webchatgpt.py
```

### Comparing `python-tgpt-0.5.8/LICENSE` & `python-tgpt-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/PKG-INFO` & `python-tgpt-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.5.8
+Version: 0.6.0
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -44,25 +44,28 @@
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: g4f>=0.2.6.1; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Provides-Extra: api
+Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: g4f>=0.2.6.1; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
 <!-- <h1 align="center"> python-tgpt </h1> -->
 <p align="center">
@@ -112,27 +115,28 @@
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
-- 🗨️ Enhanced conversational chat experience
-- 💾 Capability to save prompts and responses (Conversation)
-- 🔄 Ability to load previous conversations
-- ⌨️ Command-line interface
 - 🐍 Python package
+- 🌐 FastAPI for web integration
+- ⌨️ Command-line interface
+- 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
-- ⛓️ Chained requests via proxy
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- 🧠 Multiple LLM providers - **45+**
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- ⛓️ Chained requests via proxy
+- 🗨️ Enhanced conversational chat experience
+- 💾 Capability to save prompts and responses (Conversation)
+- 🔄 Ability to load previous conversations
+- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
@@ -149,15 +153,15 @@
 15. [Perplexity](https://www.perplexity.ai)
 
 
 <details>
 
 <summary>
 
-41+ Other models proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
+41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
 
 </summary>
 
 - To list working providers run:
    ```sh
    $ pytgpt gpt4free test -y
    ```
@@ -189,14 +193,16 @@
 
 3. Full installation:
 
    ```sh
    pip install  --upgrade "python-tgpt[all]"
    ```
 
+> `pip install -U "python-tgt[api]"` will install REST API dependencies.
+
 ## Usage
 
 This package offers a convenient command-line interface.
 
 > [!NOTE]
 > `phind` is the default *provider*.
 
@@ -357,15 +363,15 @@
 
 <summary>
 phind
 
 </summary>
 
 ```python
-import pytgp.phind as phind
+import pytgpt.phind as phind
 bot = phind.PHIND()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
@@ -532,15 +538,15 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -550,14 +556,15 @@
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
+  api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.5.8 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.0 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -24,21 +24,23 @@
 Requires-Dist: webchatgpt==0.2.9 Requires-Dist: GoogleBard1>=2.1.4 Requires-
 Dist: poe-api-wrapper==1.3.6 Requires-Dist: brotli==1.1.0 Requires-Dist:
 g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3 Provides-Extra: cli Requires-
 Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
 extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
 g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
-Requires-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra
-== "all" Requires-Dist: click==8.1.3; extra == "all" Requires-Dist:
-rich==13.3.4; extra == "all" Requires-Dist: clipman==3.1.0; extra == "all"
-Requires-Dist: pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6;
-extra == "all" Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist:
-python-dotenv==1.0.0; extra == "all"
+"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
+Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
+Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
+Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
+== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
+pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
+dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
+"all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -47,55 +49,57 @@
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
-available, fostering a smoother AI interaction experience. ### Features -
+available, fostering a smoother AI interaction experience. ### Features - ð
+Python package - ð FastAPI for web integration - â¨ï¸ Command-line
+interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
+response - ð Ready to use (No API key required) - ð¯ Customizable script
+generation and execution - ð Offline support for Large Language Models -
+ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
 ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
 prompts and responses (Conversation) - ð Ability to load previous
-conversations - â¨ï¸ Command-line interface - ð Python package - ð
-Stream and non-stream response - ð Ready to use (No API key required) -
-âï¸ Chained requests via proxy - ð¤ Pass [awesome-chatgpt prompts](https:/
-/github.com/f/awesome-chatgpt-prompts) easily - ð§  Multiple LLM providers -
-**45+** - ð¯ Customizable script generation and execution - ð Offline
-support for Large Language Models - ð¨ Image generation capabilities ##
-Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ Other models proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` ## Usage This
-package offers a convenient command-line interface. > [!NOTE] > `phind` is the
-default *provider*. - For a quick response: ```bash python -m pytgpt generate
-"" ``` - For interactive mode: ```bash python -m pytgpt interactive "" ``` Make
-use of flag `--provider` followed by the provider name of your choice. e.g `--
-provider koboldai` > To list all providers offered by gpt4free, use following
-commands: ```pytgpt gpt4free list providers``` You can also simply use `pytgpt`
-instead of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt`
-without any other command or option will automatically enter the `interactive`
-mode. Otherwise, you'll need to explicitly declare the desired action, for
-example, by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick
-response ```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('')
-print(resp) # Output : How may I help you. ``` 2. Get back whole response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
+awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
+LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
+(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
+opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
+*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
+**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
+- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
+*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
+github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
+gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
+*(Optional)* ## Installation and Usage ### Installation Download binaries for
+your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
+latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
+Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
+pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
+install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
+will install REST API dependencies. ## Usage This package offers a convenient
+command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
+quick response: ```bash python -m pytgpt generate "" ``` - For interactive
+mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
+followed by the provider name of your choice. e.g `--provider koboldai` > To
+list all providers offered by gpt4free, use following commands: ```pytgpt
+gpt4free list providers``` You can also simply use `pytgpt` instead of `python
+-m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
+command or option will automatically enter the `interactive` mode. Otherwise,
+you'll need to explicitly declare the desired action, for example, by running
+`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
+: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -113,15 +117,15 @@
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
 'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
 = openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
 pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
 Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
 print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgp.phind as
+bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
 phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
 import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
 print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
 [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
 be set to either `code` or `system_command`. ```python from pytgpt.leo import
 LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
 [!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
@@ -190,17 +194,19 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui` For more usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS]
-COMMAND [ARGS]... Options: -v, --version Show the version and exit. -h, --help
-Show this message and exit. Commands: awesome Perform CRUD operations on
-awesome-prompts generate Generate a quick response with AI gpt4free Discover
-gpt4free models, providers etc imager Generate images with pollinations.ai
-interactive Chat with AI interactively (Default) utils Utility endpoint for
-pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ## [CHANGELOG]
-(https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ##
-Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x]
-[gpt4free](https://github.com/xtekky/gpt4free)
+gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
+Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
+version and exit. -h, --help Show this message and exit. Commands: api FastAPI
+control endpoint awesome Perform CRUD operations on awesome-prompts generate
+Generate a quick response with AI gpt4free Discover gpt4free models, providers
+etc imager Generate images with pollinations.ai interactive Chat with AI
+interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
+Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python-tgpt-0.5.8/README.md` & `python-tgpt-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,27 +50,28 @@
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
-- 🗨️ Enhanced conversational chat experience
-- 💾 Capability to save prompts and responses (Conversation)
-- 🔄 Ability to load previous conversations
-- ⌨️ Command-line interface
 - 🐍 Python package
+- 🌐 FastAPI for web integration
+- ⌨️ Command-line interface
+- 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
-- ⛓️ Chained requests via proxy
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- 🧠 Multiple LLM providers - **45+**
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- ⛓️ Chained requests via proxy
+- 🗨️ Enhanced conversational chat experience
+- 💾 Capability to save prompts and responses (Conversation)
+- 🔄 Ability to load previous conversations
+- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
@@ -87,15 +88,15 @@
 15. [Perplexity](https://www.perplexity.ai)
 
 
 <details>
 
 <summary>
 
-41+ Other models proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
+41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
 
 </summary>
 
 - To list working providers run:
    ```sh
    $ pytgpt gpt4free test -y
    ```
@@ -127,14 +128,16 @@
 
 3. Full installation:
 
    ```sh
    pip install  --upgrade "python-tgpt[all]"
    ```
 
+> `pip install -U "python-tgt[api]"` will install REST API dependencies.
+
 ## Usage
 
 This package offers a convenient command-line interface.
 
 > [!NOTE]
 > `phind` is the default *provider*.
 
@@ -295,15 +298,15 @@
 
 <summary>
 phind
 
 </summary>
 
 ```python
-import pytgp.phind as phind
+import pytgpt.phind as phind
 bot = phind.PHIND()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
@@ -470,15 +473,15 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -488,14 +491,15 @@
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
+  api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
```

#### html2text {}

```diff
@@ -10,55 +10,57 @@
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
-available, fostering a smoother AI interaction experience. ### Features -
+available, fostering a smoother AI interaction experience. ### Features - ð
+Python package - ð FastAPI for web integration - â¨ï¸ Command-line
+interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
+response - ð Ready to use (No API key required) - ð¯ Customizable script
+generation and execution - ð Offline support for Large Language Models -
+ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
 ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
 prompts and responses (Conversation) - ð Ability to load previous
-conversations - â¨ï¸ Command-line interface - ð Python package - ð
-Stream and non-stream response - ð Ready to use (No API key required) -
-âï¸ Chained requests via proxy - ð¤ Pass [awesome-chatgpt prompts](https:/
-/github.com/f/awesome-chatgpt-prompts) easily - ð§  Multiple LLM providers -
-**45+** - ð¯ Customizable script generation and execution - ð Offline
-support for Large Language Models - ð¨ Image generation capabilities ##
-Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ Other models proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` ## Usage This
-package offers a convenient command-line interface. > [!NOTE] > `phind` is the
-default *provider*. - For a quick response: ```bash python -m pytgpt generate
-"" ``` - For interactive mode: ```bash python -m pytgpt interactive "" ``` Make
-use of flag `--provider` followed by the provider name of your choice. e.g `--
-provider koboldai` > To list all providers offered by gpt4free, use following
-commands: ```pytgpt gpt4free list providers``` You can also simply use `pytgpt`
-instead of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt`
-without any other command or option will automatically enter the `interactive`
-mode. Otherwise, you'll need to explicitly declare the desired action, for
-example, by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick
-response ```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('')
-print(resp) # Output : How may I help you. ``` 2. Get back whole response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
+awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
+LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
+(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
+opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
+*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
+**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
+- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
+*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
+github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
+gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
+*(Optional)* ## Installation and Usage ### Installation Download binaries for
+your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
+latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
+Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
+pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
+install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
+will install REST API dependencies. ## Usage This package offers a convenient
+command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
+quick response: ```bash python -m pytgpt generate "" ``` - For interactive
+mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
+followed by the provider name of your choice. e.g `--provider koboldai` > To
+list all providers offered by gpt4free, use following commands: ```pytgpt
+gpt4free list providers``` You can also simply use `pytgpt` instead of `python
+-m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
+command or option will automatically enter the `interactive` mode. Otherwise,
+you'll need to explicitly declare the desired action, for example, by running
+`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
+: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -76,15 +78,15 @@
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
 'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
 = openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
 pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
 Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
 print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgp.phind as
+bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
 phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
 import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
 print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
 [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
 be set to either `code` or `system_command`. ```python from pytgpt.leo import
 LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
 [!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
@@ -153,17 +155,19 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui` For more usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS]
-COMMAND [ARGS]... Options: -v, --version Show the version and exit. -h, --help
-Show this message and exit. Commands: awesome Perform CRUD operations on
-awesome-prompts generate Generate a quick response with AI gpt4free Discover
-gpt4free models, providers etc imager Generate images with pollinations.ai
-interactive Chat with AI interactively (Default) utils Utility endpoint for
-pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ## [CHANGELOG]
-(https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ##
-Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x]
-[gpt4free](https://github.com/xtekky/gpt4free)
+gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
+Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
+version and exit. -h, --help Show this message and exit. Commands: api FastAPI
+control endpoint awesome Perform CRUD operations on awesome-prompts generate
+Generate a quick response with AI gpt4free Discover gpt4free models, providers
+etc imager Generate images with pollinations.ai interactive Chat with AI
+interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
+Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python-tgpt-0.5.8/setup.py` & `python-tgpt-0.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,34 @@
     "clipman==3.1.0",
     "pyperclip==1.8.2",
     "colorama==0.4.6",
     "g4f>=0.2.6.1",
     "python-dotenv==1.0.0",
 ]
 
+api = [
+    "fastapi[all]==0.110.1",
+]
+
 EXTRA_REQUIRE = {
     "cli": cli_reqs,
-    "all": ["g4f[all]>=0.2.6.1", "matplotlib", "gpt4all==2.2.0"] + cli_reqs,
+    "api": api,
+    "all": ["g4f[all]>=0.2.6.1", "matplotlib", "gpt4all==2.2.0"] + cli_reqs + api,
 }
 
 DOCS_PATH = Path(__file__).parents[0] / "docs/README.md"
 PATH = Path("README.md")
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.5.8",
+    version="0.6.0",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python-tgpt-0.5.8/src/pytgpt/__init__.py` & `python-tgpt-0.6.0/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/base.py` & `python-tgpt-0.6.0/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/blackboxai/main.py` & `python-tgpt-0.6.0/src/pytgpt/blackboxai/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import re
 import json
-import yaml
 import requests
 from pytgpt.utils import Optimizers
 from pytgpt.utils import Conversation
 from pytgpt.utils import AwesomePrompts
 
 session = requests.Session()
```

### Comparing `python-tgpt-0.5.8/src/pytgpt/console.py` & `python-tgpt-0.6.0/src/pytgpt/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -1157,14 +1157,21 @@
     @staticmethod
     @tgpt2_.group()  # For awesome-prompts
     @click.help_option("-h", "--help")
     def awesome():
         """Perform CRUD operations on awesome-prompts"""
         pass
 
+    @staticmethod
+    @tgpt2_.group()
+    @click.help_option("-h", "--help")
+    def api():
+        """FastAPI control endpoint"""
+        pass
+
 
 class ChatInteractive:
     """Interactive command"""
 
     @staticmethod
     @click.command(context_settings=this.context_settings)
     @click.option(
@@ -2340,14 +2347,49 @@
             rich.print(Markdown(update.latest()["body"]))
         elif executable:
             rich.print(update.executable())
         else:
             rich.print_json(data=update.latest())
 
 
+class API:
+    """API control endpoint"""
+
+    @staticmethod
+    @click.command(context_settings=this.context_settings)
+    @click.option(
+        "-p",
+        "--port",
+        type=click.INT,
+        default=8000,
+        help="Port for listening requests",
+    )
+    @click.option(
+        "-b",
+        "--bind",
+        default="127.0.0.1",
+        help="Address to serve from",
+    )
+    @click.option(
+        "-l",
+        "--log-level",
+        type=click.Choice(
+            ["debug", "info", "warning", "errror", "critical"],
+        ),
+        default="info",
+    )
+    @click.help_option("-h", "--help")
+    def run(port, bind, log_level):
+        """Launch FastAPI"""
+        import uvicorn
+        from pytgpt.api import app
+
+        uvicorn.run(app, host=bind, port=port, log_level=log_level)
+
+
 def make_commands():
     """Make pytgpt chained commands"""
     # webchatgpt
     # Intergration with WebChatGPT https://github.com/Simatwa/WebChatGPT
     EntryGroup.tgpt2_.add_command(webchatgpt, "webchatgpt")
 
     # generate
@@ -2373,14 +2415,17 @@
     EntryGroup.awesome.add_command(Awesome.search)
     EntryGroup.awesome.add_command(Awesome.update)
     EntryGroup.awesome.add_command(Awesome.whole)
 
     # Image generator
     EntryGroup.tgpt2_.add_command(ImageGen.generate_image, "imager")
 
+    # FastAPI
+    EntryGroup.api.add_command(API.run)
+
 
 # @this.handle_exception
 def main(*args):
     """Fireup console programmically"""
     sys.argv += list(args)
     args = sys.argv
     if len(args) == 1:
```

### Comparing `python-tgpt-0.5.8/src/pytgpt/gemini/main.py` & `python-tgpt-0.6.0/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/gpt4all/main.py` & `python-tgpt-0.6.0/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/gpt4free/main.py` & `python-tgpt-0.6.0/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/gpt4free/utils.py` & `python-tgpt-0.6.0/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/groq/main.py` & `python-tgpt-0.6.0/src/pytgpt/groq/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,13 +250,13 @@
                 return response["choices"][0]["delta"]["content"]
             return response["choices"][0]["message"]["content"]
         except KeyError:
             return ""
 
 
 if __name__ == "__main__":
-    bot = GROQ("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")
+    bot = GROQ("grog api key")
 
     resp = bot.ask("coding", stream=True)
 
     for val in resp:
         print(json.dumps(val, indent=4))
```

### Comparing `python-tgpt-0.5.8/src/pytgpt/imager/imager.py` & `python-tgpt-0.6.0/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/koboldai/main.py` & `python-tgpt-0.6.0/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/leo/main.py` & `python-tgpt-0.6.0/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/llama2/main.py` & `python-tgpt-0.6.0/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/openai/main.py` & `python-tgpt-0.6.0/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/opengpt/main.py` & `python-tgpt-0.6.0/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/perplexity/main.py` & `python-tgpt-0.6.0/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/phind/main.py` & `python-tgpt-0.6.0/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/poe/main.py` & `python-tgpt-0.6.0/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/utils.py` & `python-tgpt-0.6.0/src/pytgpt/utils.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/pytgpt/webchatgpt/main.py` & `python-tgpt-0.6.0/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/src/python_tgpt.egg-info/PKG-INFO` & `python-tgpt-0.6.0/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.5.8
+Version: 0.6.0
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -44,25 +44,28 @@
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
 Requires-Dist: g4f>=0.2.6.1; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Provides-Extra: api
+Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: g4f>=0.2.6.1; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
 <!-- <h1 align="center"> python-tgpt </h1> -->
 <p align="center">
@@ -112,27 +115,28 @@
 This project enables seamless interaction with over **45 free LLM providers** without requiring an API Key and generating images as well.
 
 The name *python-tgpt* draws inspiration from its parent project [tgpt](https://github.com/aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this Python adaptation, users can effortlessly engage with a number of free LLMs available, fostering a smoother AI interaction experience.
 
 
 ### Features
 
-- 🗨️ Enhanced conversational chat experience
-- 💾 Capability to save prompts and responses (Conversation)
-- 🔄 Ability to load previous conversations
-- ⌨️ Command-line interface
 - 🐍 Python package
+- 🌐 FastAPI for web integration
+- ⌨️ Command-line interface
+- 🧠 Multiple LLM providers - **45+**
 - 🌊 Stream and non-stream response
 - 🚀 Ready to use (No API key required)
-- ⛓️ Chained requests via proxy
-- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- 🧠 Multiple LLM providers - **45+**
 - 🎯 Customizable script generation and execution
 - 🔌 Offline support for Large Language Models
 - 🎨 Image generation capabilities
+- ⛓️ Chained requests via proxy
+- 🗨️ Enhanced conversational chat experience
+- 💾 Capability to save prompts and responses (Conversation)
+- 🔄 Ability to load previous conversations
+- 🤖 Pass [awesome-chatgpt prompts](https://github.com/f/awesome-chatgpt-prompts) easily
 
 ## Providers
 
 These are simply the hosts of the LLMs, which include:
 
 1. [Leo](https://brave.com/leo/) - **Brave**
 2. [Koboldai](https://koboldai-koboldcpp-tiefighter.hf.space)
@@ -149,15 +153,15 @@
 15. [Perplexity](https://www.perplexity.ai)
 
 
 <details>
 
 <summary>
 
-41+ Other models proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
+41+ providers proudly offered by [gpt4free](https://github.com/xtekky/gpt4free).
 
 </summary>
 
 - To list working providers run:
    ```sh
    $ pytgpt gpt4free test -y
    ```
@@ -189,14 +193,16 @@
 
 3. Full installation:
 
    ```sh
    pip install  --upgrade "python-tgpt[all]"
    ```
 
+> `pip install -U "python-tgt[api]"` will install REST API dependencies.
+
 ## Usage
 
 This package offers a convenient command-line interface.
 
 > [!NOTE]
 > `phind` is the default *provider*.
 
@@ -357,15 +363,15 @@
 
 <summary>
 phind
 
 </summary>
 
 ```python
-import pytgp.phind as phind
+import pytgpt.phind as phind
 bot = phind.PHIND()
 print(bot.chat("<Your-prompt>"))
 ```
 
 </details>
 
 <details>
@@ -532,15 +538,15 @@
 > To load previous conversations from a `.txt` file, use the `-fp` or `--filepath` flag. If no flag is passed, the default one will be used. To load context from a file without altering its content, use the `--retain-file` flag.
 
 ## Dynamic Provider
 
 Version **0.4.6** also introduces dynamic provider called `g4fauto`, which represents the fastest working g4f-based provider.
 
 > [!TIP]
-> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`
+> To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */docs* and */redoc* respectively.
 
 <details>
 
 <summary>
 
 For more usage info run `$ pytgpt --help`
 
@@ -550,14 +556,15 @@
 Usage: pytgpt [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -v, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
+  api          FastAPI control endpoint
   awesome      Perform CRUD operations on awesome-prompts
   generate     Generate a quick response with AI
   gpt4free     Discover gpt4free models, providers etc
   imager       Generate images with pollinations.ai
   interactive  Chat with AI interactively (Default)
   utils        Utility endpoint for pytgpt
   webchatgpt   Reverse Engineered ChatGPT Web-Version
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.5.8 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.6.0 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -24,21 +24,23 @@
 Requires-Dist: webchatgpt==0.2.9 Requires-Dist: GoogleBard1>=2.1.4 Requires-
 Dist: poe-api-wrapper==1.3.6 Requires-Dist: brotli==1.1.0 Requires-Dist:
 g4f>=0.2.6.1 Requires-Dist: Helpingai-T2==0.3 Provides-Extra: cli Requires-
 Dist: click==8.1.3; extra == "cli" Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli" Requires-Dist: pyperclip==1.8.2;
 extra == "cli" Requires-Dist: colorama==0.4.6; extra == "cli" Requires-Dist:
 g4f>=0.2.6.1; extra == "cli" Requires-Dist: python-dotenv==1.0.0; extra ==
-"cli" Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
-Requires-Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra
-== "all" Requires-Dist: click==8.1.3; extra == "all" Requires-Dist:
-rich==13.3.4; extra == "all" Requires-Dist: clipman==3.1.0; extra == "all"
-Requires-Dist: pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6;
-extra == "all" Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist:
-python-dotenv==1.0.0; extra == "all"
+"cli" Provides-Extra: api Requires-Dist: fastapi[all]==0.110.1; extra == "api"
+Provides-Extra: all Requires-Dist: g4f[all]>=0.2.6.1; extra == "all" Requires-
+Dist: matplotlib; extra == "all" Requires-Dist: gpt4all==2.2.0; extra == "all"
+Requires-Dist: click==8.1.3; extra == "all" Requires-Dist: rich==13.3.4; extra
+== "all" Requires-Dist: clipman==3.1.0; extra == "all" Requires-Dist:
+pyperclip==1.8.2; extra == "all" Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all" Requires-Dist: python-
+dotenv==1.0.0; extra == "all" Requires-Dist: fastapi[all]==0.110.1; extra ==
+"all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
 _[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]_[_c_o_v_e_r_a_g_e_]
    _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
   _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
                         _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
@@ -47,55 +49,57 @@
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
 without requiring an API Key and generating images as well. The name *python-
 tgpt* draws inspiration from its parent project [tgpt](https://github.com/
 aandrew-me/tgpt), which operates on [Golang](https://go.dev/). Through this
 Python adaptation, users can effortlessly engage with a number of free LLMs
-available, fostering a smoother AI interaction experience. ### Features -
+available, fostering a smoother AI interaction experience. ### Features - ð
+Python package - ð FastAPI for web integration - â¨ï¸ Command-line
+interface - ð§  Multiple LLM providers - **45+** - ð Stream and non-stream
+response - ð Ready to use (No API key required) - ð¯ Customizable script
+generation and execution - ð Offline support for Large Language Models -
+ð¨ Image generation capabilities - âï¸ Chained requests via proxy -
 ð¨ï¸ Enhanced conversational chat experience - ð¾ Capability to save
 prompts and responses (Conversation) - ð Ability to load previous
-conversations - â¨ï¸ Command-line interface - ð Python package - ð
-Stream and non-stream response - ð Ready to use (No API key required) -
-âï¸ Chained requests via proxy - ð¤ Pass [awesome-chatgpt prompts](https:/
-/github.com/f/awesome-chatgpt-prompts) easily - ð§  Multiple LLM providers -
-**45+** - ð¯ Customizable script generation and execution - ð Offline
-support for Large Language Models - ð¨ Image generation capabilities ##
-Providers These are simply the hosts of the LLMs, which include: 1. [Leo]
-(https://brave.com/leo/) - **Brave** 2. [Koboldai](https://koboldai-koboldcpp-
-tiefighter.hf.space) 3. [OpenGPTs](https://opengpts-example-vz4y4ooboq-
-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com) *(API key required)* 5.
-[WebChatGPT](https://github.com/Simatwa/WebChatGPT) - **OpenAI** *(Session ID
-required)* 6. [Gemini](https://github.com/Simatwa/bard) - **Google** *(Session
-ID required)* 9. [Phind](https://www.phind.com) - *default* 10. [Llama2](https:
-//www.llama2.ai) 11. [Blackboxai](https://www.blackbox.ai) 12. [gpt4all](https:
-//gpt4all.io) *(Offline)* 13. [Poe](https://poe.com) - Poe|Quora *(Session ID
-required)* 14. [Groq](https://console.groq.com/playground) *(API Key required)*
-15. [Perplexity](https://www.perplexity.ai) 41+ Other models proudly offered by
-[gpt4free](https://github.com/xtekky/gpt4free). - To list working providers
-run: ```sh $ pytgpt gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10]
-(https://python.org) *(Optional)* ## Installation and Usage ### Installation
-Download binaries for your system from [here.](https://github.com/Simatwa/
-python-tgpt/releases/latest/) Alternatively, you can install non-binaries. *
-(Recommended)* 1. Developers: ```sh pip install --upgrade python-tgpt ``` 2.
-Commandline: ```sh pip install --upgrade "python-tgpt[cli]" ``` 3. Full
-installation: ```sh pip install --upgrade "python-tgpt[all]" ``` ## Usage This
-package offers a convenient command-line interface. > [!NOTE] > `phind` is the
-default *provider*. - For a quick response: ```bash python -m pytgpt generate
-"" ``` - For interactive mode: ```bash python -m pytgpt interactive "" ``` Make
-use of flag `--provider` followed by the provider name of your choice. e.g `--
-provider koboldai` > To list all providers offered by gpt4free, use following
-commands: ```pytgpt gpt4free list providers``` You can also simply use `pytgpt`
-instead of `python -m pytgpt`. Starting from version 0.2.7, running `$ pytgpt`
-without any other command or option will automatically enter the `interactive`
-mode. Otherwise, you'll need to explicitly declare the desired action, for
-example, by running `$ pytgpt generate`. ### Developer Docs 1. Generate a quick
-response ```python from pytgpt.leo import LEO bot = LEO() resp = bot.chat('')
-print(resp) # Output : How may I help you. ``` 2. Get back whole response
-```python from pytgpt.leo import LEO bot = LEO() resp = bot.ask('
+conversations - ð¤ Pass [awesome-chatgpt prompts](https://github.com/f/
+awesome-chatgpt-prompts) easily ## Providers These are simply the hosts of the
+LLMs, which include: 1. [Leo](https://brave.com/leo/) - **Brave** 2. [Koboldai]
+(https://koboldai-koboldcpp-tiefighter.hf.space) 3. [OpenGPTs](https://
+opengpts-example-vz4y4ooboq-uc.a.run.app/) 4. [OpenAI](https://chat.openai.com)
+*(API key required)* 5. [WebChatGPT](https://github.com/Simatwa/WebChatGPT) -
+**OpenAI** *(Session ID required)* 6. [Gemini](https://github.com/Simatwa/bard)
+- **Google** *(Session ID required)* 9. [Phind](https://www.phind.com) -
+*default* 10. [Llama2](https://www.llama2.ai) 11. [Blackboxai](https://
+www.blackbox.ai) 12. [gpt4all](https://gpt4all.io) *(Offline)* 13. [Poe](https:
+//poe.com) - Poe|Quora *(Session ID required)* 14. [Groq](https://
+console.groq.com/playground) *(API Key required)* 15. [Perplexity](https://
+www.perplexity.ai) 41+ providers proudly offered by [gpt4free](https://
+github.com/xtekky/gpt4free). - To list working providers run: ```sh $ pytgpt
+gpt4free test -y ``` ## Prerequisites - [x] [Python>=3.10](https://python.org)
+*(Optional)* ## Installation and Usage ### Installation Download binaries for
+your system from [here.](https://github.com/Simatwa/python-tgpt/releases/
+latest/) Alternatively, you can install non-binaries. *(Recommended)* 1.
+Developers: ```sh pip install --upgrade python-tgpt ``` 2. Commandline: ```sh
+pip install --upgrade "python-tgpt[cli]" ``` 3. Full installation: ```sh pip
+install --upgrade "python-tgpt[all]" ``` > `pip install -U "python-tgt[api]"`
+will install REST API dependencies. ## Usage This package offers a convenient
+command-line interface. > [!NOTE] > `phind` is the default *provider*. - For a
+quick response: ```bash python -m pytgpt generate "" ``` - For interactive
+mode: ```bash python -m pytgpt interactive "" ``` Make use of flag `--provider`
+followed by the provider name of your choice. e.g `--provider koboldai` > To
+list all providers offered by gpt4free, use following commands: ```pytgpt
+gpt4free list providers``` You can also simply use `pytgpt` instead of `python
+-m pytgpt`. Starting from version 0.2.7, running `$ pytgpt` without any other
+command or option will automatically enter the `interactive` mode. Otherwise,
+you'll need to explicitly declare the desired action, for example, by running
+`$ pytgpt generate`. ### Developer Docs 1. Generate a quick response ```python
+from pytgpt.leo import LEO bot = LEO() resp = bot.chat('') print(resp) # Output
+: How may I help you. ``` 2. Get back whole response ```python from pytgpt.leo
+import LEO bot = LEO() resp = bot.ask('
  Output """ {'completion': "I'm so excited to share with you the incredible
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwJ2',
 'exception': None} """ ``` #### Stream Response Just add parameter `stream`
 with value `true`. 1. Text Generated only ```python from pytgpt.leo import LEO
 bot = LEO() resp = bot.chat('', stream=True) for value in resp: print(value) #
 output """ How may How may I help How may I help you How may I help you today?
@@ -113,15 +117,15 @@
 experiences...", 'stop_reason': None, 'truncated': False, 'stop': None,
 'model': 'llama-2-13b-chat', 'log_id': 'cmpl-3NmRt5A5Djqo2jXtXLBwxx',
 'exception': None} """ ``` Openai ```python import pytgpt.openai as openai bot
 = openai.OPENAI("") print(bot.chat("")) ``` Koboldai ```python import
 pytgpt.koboldai as koboldai bot = koboldai.KOBOLDAI() print(bot.chat("")) ```
 Opengpt ```python import pytgpt.opengpt as opengpt bot = opengpt.OPENGPT()
 print(bot.chat("")) ``` Bard ```python import pytgpt.bard as bard bot =
-bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgp.phind as
+bard.BARD('') print(bot.chat("")) ``` phind ```python import pytgpt.phind as
 phind bot = phind.PHIND() print(bot.chat("")) ``` Gpt4free providers ```python
 import pytgpt.gpt4free as gpt4free bot = gpt4free.GPT4FREE(provider="Aura")
 print(bot.chat("")) ``` To obtain more tailored responses, consider utilizing
 [optimizers](pytgpt/utils.py) using the `optimizer` parameter. Its values can
 be set to either `code` or `system_command`. ```python from pytgpt.leo import
 LEO bot = LEO() resp = bot.ask('', optimizer='code') print(resp) ``` >
 [!IMPORTANT] > Commencing from [v0.1.0](https://github.com/Simatwa/python-tgpt/
@@ -190,17 +194,19 @@
 a `.env` file in your current directory or export them in your `~/.zshrc` file.
 > To load previous conversations from a `.txt` file, use the `-fp` or `--
 filepath` flag. If no flag is passed, the default one will be used. To load
 context from a file without altering its content, use the `--retain-file` flag.
 ## Dynamic Provider Version **0.4.6** also introduces dynamic provider called
 `g4fauto`, which represents the fastest working g4f-based provider. > [!TIP] >
 To launch web interface for g4f-based providers simply run `$ pytgpt gpt4free
-gui` For more usage info run `$ pytgpt --help` ``` Usage: pytgpt [OPTIONS]
-COMMAND [ARGS]... Options: -v, --version Show the version and exit. -h, --help
-Show this message and exit. Commands: awesome Perform CRUD operations on
-awesome-prompts generate Generate a quick response with AI gpt4free Discover
-gpt4free models, providers etc imager Generate images with pollinations.ai
-interactive Chat with AI interactively (Default) utils Utility endpoint for
-pytgpt webchatgpt Reverse Engineered ChatGPT Web-Version ``` ## [CHANGELOG]
-(https://github.com/Simatwa/python-tgpt/blob/main/docs/CHANGELOG.md) ##
-Acknowledgements 1. [x] [tgpt](https://github.com/aandrew-me/tgpt) 2. [x]
-[gpt4free](https://github.com/xtekky/gpt4free)
+gui`. `$ pytgpt api run` will start the REST-API. Access docs and redoc at */
+docs* and */redoc* respectively. For more usage info run `$ pytgpt --help` ```
+Usage: pytgpt [OPTIONS] COMMAND [ARGS]... Options: -v, --version Show the
+version and exit. -h, --help Show this message and exit. Commands: api FastAPI
+control endpoint awesome Perform CRUD operations on awesome-prompts generate
+Generate a quick response with AI gpt4free Discover gpt4free models, providers
+etc imager Generate images with pollinations.ai interactive Chat with AI
+interactively (Default) utils Utility endpoint for pytgpt webchatgpt Reverse
+Engineered ChatGPT Web-Version ``` ## [CHANGELOG](https://github.com/Simatwa/
+python-tgpt/blob/main/docs/CHANGELOG.md) ## Acknowledgements 1. [x] [tgpt]
+(https://github.com/aandrew-me/tgpt) 2. [x] [gpt4free](https://github.com/
+xtekky/gpt4free)
```

### Comparing `python-tgpt-0.5.8/src/python_tgpt.egg-info/SOURCES.txt` & `python-tgpt-0.6.0/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 README.md
 setup.py
 src/pytgpt/__init__.py
 src/pytgpt/__main__.py
 src/pytgpt/base.py
 src/pytgpt/console.py
 src/pytgpt/utils.py
+src/pytgpt/api/__init__.py
+src/pytgpt/api/__main__.py
+src/pytgpt/api/v1.py
 src/pytgpt/blackboxai/__init__.py
 src/pytgpt/blackboxai/main.py
 src/pytgpt/gemini/__init__.py
 src/pytgpt/gemini/main.py
 src/pytgpt/gpt4all/__init__.py
 src/pytgpt/gpt4all/main.py
 src/pytgpt/gpt4free/__init__.py
```

### Comparing `python-tgpt-0.5.8/tests/test_imager.py` & `python-tgpt-0.6.0/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python-tgpt-0.5.8/tests/test_utils.py` & `python-tgpt-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

