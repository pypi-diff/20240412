# Comparing `tmp/gpt-researcher-0.2.0.tar.gz` & `tmp/gpt-researcher-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.0.tar", last modified: Thu Apr  4 09:18:12 2024, max compression
+gzip compressed data, was "gpt-researcher-0.2.1.tar", last modified: Fri Apr 12 13:13:27 2024, max compression
```

## Comparing `gpt-researcher-0.2.0.tar` & `gpt-researcher-0.2.1.tar`

### file list

```diff
@@ -1,96 +1,99 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.253180 gpt-researcher-0.2.0/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12547 2024-04-04 09:18:12.252490 gpt-researcher-0.2.0/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    11824 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.205573 gpt-researcher-0.2.0/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.210380 gpt-researcher-0.2.0/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.212787 gpt-researcher-0.2.0/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.213781 gpt-researcher-0.2.0/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.215222 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2526 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.216696 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.218234 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.222356 gpt-researcher-0.2.0/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8604 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12120 2024-04-01 16:02:57.000000 gpt-researcher-0.2.0/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    12175 2024-04-01 16:15:31.000000 gpt-researcher-0.2.0/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.224475 gpt-researcher-0.2.0/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.225284 gpt-researcher-0.2.0/gpt_researcher/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.226657 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.227955 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6033 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/detailed_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.228973 gpt-researcher-0.2.0/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.230415 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.231881 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2023-11-13 18:29:19.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.233419 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.234848 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.236022 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.237553 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.239021 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.240840 gpt-researcher-0.2.0/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.242324 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.243746 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.245148 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.246366 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.247619 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.251357 gpt-researcher-0.2.0/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.0/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     4851 2024-04-01 15:55:37.000000 gpt-researcher-0.2.0/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/validators.py
--rw-r--r--   0 assafel    (501) staff       (20)     2872 2024-04-01 15:55:34.000000 gpt-researcher-0.2.0/gpt_researcher/utils/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-04 09:18:12.208930 gpt-researcher-0.2.0/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12547 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2629 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      322 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       15 2024-04-04 09:18:12.000000 gpt-researcher-0.2.0/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1150 2024-03-31 16:54:34.000000 gpt-researcher-0.2.0/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-04 09:18:12.253338 gpt-researcher-0.2.0/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-04 09:17:55.000000 gpt-researcher-0.2.0/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.974448 gpt-researcher-0.2.1/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:13:27.973739 gpt-researcher-0.2.1/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    11791 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.921752 gpt-researcher-0.2.1/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.926774 gpt-researcher-0.2.1/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.928909 gpt-researcher-0.2.1/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.930193 gpt-researcher-0.2.1/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.931705 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.933318 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.935220 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.938618 gpt-researcher-0.2.1/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8815 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-12 13:09:04.000000 gpt-researcher-0.2.1/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12802 2024-04-12 13:10:44.000000 gpt-researcher-0.2.1/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.940280 gpt-researcher-0.2.1/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.941189 gpt-researcher-0.2.1/gpt_researcher/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.942818 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.944584 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6033 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/detailed_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.945656 gpt-researcher-0.2.1/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.947194 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.948694 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.949809 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.951351 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.952754 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-12 13:06:43.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.954170 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.955547 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.957002 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.958742 gpt-researcher-0.2.1/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.960096 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.961632 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.963550 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.965288 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.966951 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.972544 gpt-researcher-0.2.1/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-12 12:40:03.000000 gpt-researcher-0.2.1/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/utils/validators.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2872 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/utils/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.925126 gpt-researcher-0.2.1/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       15 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1130 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-12 13:13:27.974663 gpt-researcher-0.2.1/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-12 13:13:07.000000 gpt-researcher-0.2.1/setup.py
```

### Comparing `gpt-researcher-0.2.0/LICENSE` & `gpt-researcher-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/PKG-INFO` & `gpt-researcher-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.0
+Version: 0.2.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -57,15 +57,15 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/a00c89a6-a295-4dd0-b58d-098a31c40fda
+https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -78,17 +78,17 @@
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
+- Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
-- Tavily API integration (high-level explanation of core concepts)
 
 ## Quickstart
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 <br />
 
 > **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
```

### Comparing `gpt-researcher-0.2.0/README.md` & `gpt-researcher-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/a00c89a6-a295-4dd0-b58d-098a31c40fda
+https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -60,17 +60,17 @@
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
+- Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
-- Tavily API integration (high-level explanation of core concepts)
 
 ## Quickstart
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 <br />
 
 > **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/config/config.py` & `gpt-researcher-0.2.1/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/context/compression.py` & `gpt-researcher-0.2.1/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/context/retriever.py` & `gpt-researcher-0.2.1/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import os
 
 from colorama import Fore, Style
 from langchain_openai import AzureChatOpenAI
 
 '''
-Please note: Needs additional env vars such as: 
-    AZURE_OPENAI_ENDPOINT  e.g. https://xxxx.openai.azure.com/", 
-    OPENAI_API_VERSION, 
-    OPENAI_API_TYPE
+Please note:
+Needs additional env vars such as: 
+    AZURE_OPENAI_ENDPOINT  e.g. https://xxxx.openai.azure.com/",
+    AZURE_OPENAI_API_KEY e.g "xxxxxxxxxxxxxxxxxxxxx",
+    OPENAI_API_VERSION, e.g. "2024-03-01-preview" but needs to updated over time as API verison updates,
+    AZURE_EMBEDDING_MODEL e.g. "ada2" The Azure OpenAI embedding model deployment name.
 
-Note new entry in config.py to specify the Azure OpenAI embedding model name:
-self.azure_embedding_model = os.getenv('AZURE_EMBEDDING_MODEL', "INSERT_EMBEDDIGN_MODEL_DEPLOYMENT_NAME")
+config.py settings for Azure OpenAI should look like:
+    self.embedding_provider = os.getenv('EMBEDDING_PROVIDER', 'azureopenai')
+    self.llm_provider = os.getenv('LLM_PROVIDER', "azureopenai")
+    self.fast_llm_model = os.getenv('FAST_LLM_MODEL', "gpt-3.5-turbo-16k") #Deployment name of your GPT3.5T model as per azure OpenAI studio deployment section
+    self.smart_llm_model = os.getenv('SMART_LLM_MODEL', "gpt4")  #Deployment name of your GPT4 1106-Preview+ (GPT4T) model as per azure OpenAI studio deployment section
 '''
 class AzureOpenAIProvider:
 
     def __init__(
         self,
         deployment_name,
         temperature,
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/master/agent.py` & `gpt-researcher-0.2.1/gpt_researcher/master/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,90 +1,102 @@
 import asyncio
 import time
+
 from gpt_researcher.config import Config
-from gpt_researcher.master.functions import *
 from gpt_researcher.context.compression import ContextCompressor
+from gpt_researcher.master.functions import *
 from gpt_researcher.memory import Memory
 from gpt_researcher.utils.enum import ReportType
+
+
 class GPTResearcher:
     """
     GPT Researcher
     """
+
     def __init__(
         self,
-        query: str, 
-        report_type: str=ReportType.ResearchReport.value,
-        source_urls=None, 
-        config_path=None, 
+        query: str,
+        report_type: str = ReportType.ResearchReport.value,
+        source_urls=None,
+        config_path=None,
         websocket=None,
         agent=None,
         role=None,
-        parent_query="",
-        subtopics=[],
-        visited_urls=set()
+        parent_query: str = "",
+        subtopics: list = [],
+        visited_urls: set = set()
     ):
         """
         Initialize the GPT Researcher class.
         Args:
-            query:
-            report_type:
-            config_path:
-            websocket:
+            query: str,
+            report_type: str
+            source_urls
+            config_path
+            websocket
+            agent
+            role
+            parent_query: str
+            subtopics: list
+            visited_urls: set
         """
         self.query = query
         self.agent = agent
         self.role = role
         self.report_type = report_type
         self.websocket = websocket
         self.cfg = Config(config_path)
         self.retriever = get_retriever(self.cfg.retriever)
         self.context = []
         self.source_urls = source_urls
         self.memory = Memory(self.cfg.embedding_provider)
         self.visited_urls = visited_urls
-        
+
         # Only relevant for DETAILED REPORTS
         # --------------------------------------
 
         # Stores the main query of the detailed report
         self.parent_query = parent_query
 
         # Stores all the user provided subtopics
         self.subtopics = subtopics
 
     async def conduct_research(self):
         """
         Runs the GPT Researcher to conduct research
         """
         print(f"🔎 Running research for '{self.query}'...")
+        
         # Generate Agent
-        self.agent, self.role = await choose_agent(self.query, self.cfg)
+        if not (self.agent and self.role):
+            self.agent, self.role = await choose_agent(self.query, self.cfg)
         await stream_output("logs", self.agent, self.websocket)
 
         # If specified, the researcher will use the given urls as the context for the research.
         if self.source_urls:
             self.context = await self.get_context_by_urls(self.source_urls)
         else:
             self.context = await self.get_context_by_search(self.query)
-        
+
         time.sleep(2)
-    
+
     async def write_report(self, existing_headers: list = []):
         """
         Writes the report based on research conducted
 
         Returns:
             str: The report
         """
         # Write Research Report
         if self.report_type == "custom_report":
             self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
-        
+
         await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
-        
+
         if self.report_type == "custom_report":
             self.role = (
                 self.cfg.agent_role if self.cfg.agent_role else self.role
             )
         elif self.report_type == "subtopic_report":
             report = await generate_report(
                 query=self.query,
@@ -94,22 +106,22 @@
                 websocket=self.websocket,
                 cfg=self.cfg,
                 main_topic=self.parent_query,
                 existing_headers=existing_headers
             )
         else:
             report = await generate_report(
-                query=self.query, 
+                query=self.query,
                 context=self.context,
-                agent_role_prompt=self.role, 
+                agent_role_prompt=self.role,
                 report_type=self.report_type,
-                websocket=self.websocket, 
+                websocket=self.websocket,
                 cfg=self.cfg
             )
-        
+
         return report
 
     async def get_context_by_urls(self, urls):
         """
             Scrapes and compresses the context from the given urls
         """
         new_search_urls = await self.get_new_urls(urls)
@@ -123,23 +135,23 @@
         """
            Generates the context for the research task by searching the query and scraping the results
         Returns:
             context: List of context
         """
         context = []
         # Generate Sub-Queries including original query
-        sub_queries = await get_sub_queries(query, self.role, self.cfg) + [query]
+        sub_queries = await get_sub_queries(query, self.role, self.cfg, self.parent_query, self.report_type) + [query]
         await stream_output("logs",
                             f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
                             self.websocket)
 
         # Using asyncio.gather to process the sub_queries asynchronously
         context = await asyncio.gather(*[self.process_sub_query(sub_query) for sub_query in sub_queries])
         return context
-    
+
     async def process_sub_query(self, sub_query: str):
         """Takes in a sub query and scrapes urls based on it and gathers context.
 
         Args:
             sub_query (str): The sub-query generated from the original query
 
         Returns:
@@ -179,55 +191,56 @@
             sub_query:
 
         Returns:
             Summary
         """
         # Get Urls
         retriever = self.retriever(sub_query)
-        search_results = retriever.search(max_results=self.cfg.max_search_results_per_query)
+        search_results = retriever.search(
+            max_results=self.cfg.max_search_results_per_query)
         new_search_urls = await self.get_new_urls([url.get("href") for url in search_results])
 
         # Scrape Urls
         # await stream_output("logs", f"📝Scraping urls {new_search_urls}...\n", self.websocket)
         await stream_output("logs", f"🤔 Researching for relevant information...\n", self.websocket)
         scraped_content_results = scrape_urls(new_search_urls, self.cfg)
         return scraped_content_results
 
     async def get_similar_content_by_query(self, query, pages):
         await stream_output("logs", f"📝 Getting relevant content based on query: {query}...", self.websocket)
         # Summarize Raw Data
-        context_compressor = ContextCompressor(documents=pages, embeddings=self.memory.get_embeddings())
+        context_compressor = ContextCompressor(
+            documents=pages, embeddings=self.memory.get_embeddings())
         # Run Tasks
         return context_compressor.get_context(query, max_results=8)
 
-
     ########################################################################################
 
     # DETAILED REPORT
-    
+
     async def write_introduction(self):
         # Construct Report Introduction from main topic research
         introduction = await get_report_introduction(self.query, self.context, self.role, self.cfg, self.websocket)
-        
+
         return introduction
 
     async def get_subtopics(self):
         """
         This async function generates subtopics based on user input and other parameters.
-        
+
         Returns:
           The `get_subtopics` function is returning the `subtopics` that are generated by the
         `construct_subtopics` function.
         """
         await stream_output("logs", f"🤔 Generating subtopics...", self.websocket)
-        
+
         subtopics = await construct_subtopics(
             task=self.query,
             data=self.context,
             config=self.cfg,
             # This is a list of user provided subtopics
             subtopics=self.subtopics,
         )
 
         await stream_output("logs", f"📋Subtopics: {subtopics}", self.websocket)
-        
-        return subtopics
+
+        return subtopics
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/master/functions.py` & `gpt-researcher-0.2.1/gpt_researcher/master/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import markdown
 
 from gpt_researcher.master.prompts import *
 from gpt_researcher.scraper.scraper import Scraper
 from gpt_researcher.utils.llm import *
 
-
 def get_retriever(retriever):
     """
     Gets the retriever
     Args:
         retriever: retriever name
 
     Returns:
@@ -74,15 +73,15 @@
         )
         agent_dict = json.loads(response)
         return agent_dict["server"], agent_dict["agent_role_prompt"]
     except Exception as e:
         return "Default Agent", "You are an AI critical thinker research assistant. Your sole purpose is to write well written, critically acclaimed, objective and structured reports on given text."
 
 
-async def get_sub_queries(query, agent_role_prompt, cfg):
+async def get_sub_queries(query: str, agent_role_prompt: str, cfg, parent_query: str, report_type:str):
     """
     Gets the sub queries
     Args:
         query: original query
         agent_role_prompt: agent role prompt
         cfg: Config
 
@@ -91,15 +90,15 @@
 
     """
     max_research_iterations = cfg.max_iterations if cfg.max_iterations else 1
     response = await create_chat_completion(
         model=cfg.smart_llm_model,
         messages=[
             {"role": "system", "content": f"{agent_role_prompt}"},
-            {"role": "user", "content": generate_search_queries_prompt(query, max_iterations=max_research_iterations)}],
+            {"role": "user", "content": generate_search_queries_prompt(query, parent_query, report_type, max_iterations=max_research_iterations)}],
         temperature=0,
         llm_provider=cfg.llm_provider
     )
     sub_queries = json.loads(response)
     return sub_queries
 
 
@@ -223,15 +222,15 @@
         main_topic:
         existing_headers:
 
     Returns:
         report:
 
     """
-    generate_prompt = get_report_by_type(report_type)
+    generate_prompt = get_prompt_by_report_type(report_type)
     report = ""
 
     if report_type == "subtopic_report":
         content = f"{generate_prompt(query, existing_headers, main_topic, context, cfg.report_format, cfg.total_words)}"
     else:
         content = (
             f"{generate_prompt(query, context, cfg.report_format, cfg.total_words)}")
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/master/prompts.py` & `gpt-researcher-0.2.1/gpt_researcher/master/prompts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 from datetime import datetime, timezone
 
 from gpt_researcher.utils.enum import ReportType
 
 
-def generate_search_queries_prompt(question, max_iterations=3):
+def generate_search_queries_prompt(question: str, parent_query: str, report_type: str, max_iterations: int=3,):
     """ Generates the search queries prompt for the given question.
-    Args: question (str): The question to generate the search queries prompt for
+    Args: 
+        question (str): The question to generate the search queries prompt for
+        parent_query (str): The main question (only relevant for detailed reports)
+        report_type (str): The report type
+        max_iterations (int): The maximum number of search queries to generate
+    
     Returns: str: The search queries prompt for the given question
     """
+    
+    if report_type == ReportType.DetailedReport.value:
+        task = f"{parent_query} : {question}"
+    else:
+        task = question
 
-    return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{question}"' \
+    return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{task}"' \
            f'Use the current date if needed: {datetime.now().strftime("%B %d, %Y")}.\n' \
            f'Also include in the queries specified task details such as locations, names, etc.\n' \
            f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].'
 
 
 def generate_report_prompt(question, context, report_format="apa", total_words=1000):
     """ Generates the report prompt for the given question and research summary.
@@ -84,25 +94,14 @@
     return f'"""{context}""" Using the above information, generate an outline for a research report in Markdown syntax' \
            f' for the following question or topic: "{question}". The outline should provide a well-structured framework' \
            ' for the research report, including the main sections, subsections, and key points to be covered.' \
            ' The research report should be detailed, informative, in-depth, and a minimum of 1,200 words.' \
            ' Use appropriate Markdown syntax to format the outline and ensure readability.'
 
 
-def get_report_by_type(report_type):
-    report_type_mapping = {
-        ReportType.ResearchReport.value: generate_report_prompt,
-        ReportType.ResourceReport.value: generate_resource_report_prompt,
-        ReportType.OutlineReport.value: generate_outline_report_prompt,
-        ReportType.CustomReport.value: generate_custom_report_prompt,
-        ReportType.SubtopicReport.value: generate_subtopic_report_prompt
-    }
-    return report_type_mapping[report_type]
-
-
 def auto_agent_instructions():
     return """
         This task involves researching a given topic, regardless of its complexity or the availability of a definitive answer. The research is conducted by a specific server, defined by its type and role, with each server requiring distinct instructions.
         Agent
         The server is determined by the field of the topic and the specific name of the server that could be utilized to research the topic provided. Agents are categorized by their area of expertise, and each server type is associated with a corresponding emoji.
 
         examples:
@@ -217,7 +216,24 @@
         Using the above latest information, Prepare a detailed report introduction on the topic -- {question}.
         - The introduction should be succinct, well-structured, informative with markdown syntax.
         - As this introduction will be part of a larger report, do NOT include any other sections, which are generally present in a report.
         - The introduction should be preceded by an H1 heading with a suitable topic for the entire report.
         - You must include hyperlinks with markdown syntax ([url website](url)) related to the sentences wherever necessary.
         Assume that the current date is {datetime.now(timezone.utc).strftime('%B %d, %Y')} if required.
     """
+
+
+report_type_mapping = {
+    ReportType.ResearchReport.value: generate_report_prompt,
+    ReportType.ResourceReport.value: generate_resource_report_prompt,
+    ReportType.OutlineReport.value: generate_outline_report_prompt,
+    ReportType.CustomReport.value: generate_custom_report_prompt,
+    ReportType.SubtopicReport.value: generate_subtopic_report_prompt
+}
+
+
+def get_prompt_by_report_type(report_type):
+    prompt_by_type = report_type_mapping.get(report_type)
+    if not prompt_by_type:
+        raise Exception(f"Invalid report type: {report_type}.\n"
+                        f"Please use one of the following: {', '.join(report.name for report in ReportType)}")
+    return prompt_by_type
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.2.1/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/report_type/basic_report/basic_report.py` & `gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher/utils/llm.py` & `gpt-researcher-0.2.1/gpt_researcher/utils/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,23 +119,29 @@
             input_variables=["task", "data", "subtopics", "max_subtopics"],
             partial_variables={
                 "format_instructions": parser.get_format_instructions()},
         )
 
         print(f"\n🤖 Calling {config.smart_llm_model}...\n")
 
-        model = ChatOpenAI(model=config.smart_llm_model)
+        if config.llm_provider == "openai":
+            model = ChatOpenAI(model=config.smart_llm_model)
+        elif config.llm_provider == "azureopenai":
+            from langchain_openai import AzureChatOpenAI
+            model = AzureChatOpenAI(model=config.smart_llm_model)
+        else:
+            return []
 
         chain = prompt | model | parser
 
         output = chain.invoke({
             "task": task,
             "data": data,
             "subtopics": subtopics,
             "max_subtopics": config.max_subtopics
         })
 
         return output
 
     except Exception as e:
         print("Exception in parsing subtopics : ", e)
-        return subtopics
+        return subtopics
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher/utils/websocket_manager.py` & `gpt-researcher-0.2.1/gpt_researcher/utils/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.0/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.2.1/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.0
+Version: 0.2.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -57,15 +57,15 @@
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
 ## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/a00c89a6-a295-4dd0-b58d-098a31c40fda
+https://github.com/assafelovic/gpt-researcher/assets/13554167/d5df04a9-631a-4509-aa55-2049b5a9e9bc
 
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
@@ -78,17 +78,17 @@
 - 📄 Export research reports to PDF, Word and more...
 
 ## 📖 Documentation
 
 Please see [here](https://docs.tavily.com/docs/gpt-researcher/getting-started) for full documentation on:
 
 - Getting started (installation, setting up the environment, simple examples)
+- Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
-- Tavily API integration (high-level explanation of core concepts)
 
 ## Quickstart
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 <br />
 
 > **Step 1** - Download the project and navigate to its directory. You'll encounter two options: Virtual Environment and Poetry. Select either Step-2 or Step-3 based on your familiarity with each.:
```

### Comparing `gpt-researcher-0.2.0/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.2.1/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 gpt_researcher/retrievers/bing/bing.py
 gpt_researcher/retrievers/duckduckgo/__init__.py
 gpt_researcher/retrievers/duckduckgo/duckduckgo.py
 gpt_researcher/retrievers/google/__init__.py
 gpt_researcher/retrievers/google/google.py
 gpt_researcher/retrievers/searx/__init__.py
 gpt_researcher/retrievers/searx/searx.py
+gpt_researcher/retrievers/serpapi/__init__.py
+gpt_researcher/retrievers/serpapi/serpapi.py
 gpt_researcher/retrievers/serper/__init__.py
 gpt_researcher/retrievers/serper/serper.py
 gpt_researcher/retrievers/tavily_news/__init__.py
 gpt_researcher/retrievers/tavily_news/tavily_news.py
 gpt_researcher/retrievers/tavily_search/__init__.py
 gpt_researcher/retrievers/tavily_search/tavily_search.py
 gpt_researcher/scraper/__init__.py
```

### Comparing `gpt-researcher-0.2.0/pyproject.toml` & `gpt-researcher-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 description = "GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks."
 authors = ["Tavily <support@tavily.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-asyncio = ">=3.4.3"
 beautifulsoup4 = ">=4.12.2"
 colorama = ">=0.4.6"
 duckduckgo_search = ">=4.1.1"
 md2pdf = ">=1.0.1"
 openai = ">=1.3.3"
 playwright = ">=1.39.0"
 python-dotenv = ">=1.0.0"
```

### Comparing `gpt-researcher-0.2.0/setup.py` & `gpt-researcher-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.2.0",
+    version="0.2.1",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

