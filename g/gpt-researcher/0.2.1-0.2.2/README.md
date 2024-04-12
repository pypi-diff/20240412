# Comparing `tmp/gpt-researcher-0.2.1.tar.gz` & `tmp/gpt-researcher-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.1.tar", last modified: Fri Apr 12 13:13:27 2024, max compression
+gzip compressed data, was "gpt-researcher-0.2.2.tar", last modified: Fri Apr 12 13:20:52 2024, max compression
```

## Comparing `gpt-researcher-0.2.1.tar` & `gpt-researcher-0.2.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.974448 gpt-researcher-0.2.1/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:13:27.973739 gpt-researcher-0.2.1/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    11791 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.921752 gpt-researcher-0.2.1/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.926774 gpt-researcher-0.2.1/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.928909 gpt-researcher-0.2.1/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.930193 gpt-researcher-0.2.1/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.931705 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.933318 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.935220 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.938618 gpt-researcher-0.2.1/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.1/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8815 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-12 13:09:04.000000 gpt-researcher-0.2.1/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    12802 2024-04-12 13:10:44.000000 gpt-researcher-0.2.1/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.940280 gpt-researcher-0.2.1/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.1/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.941189 gpt-researcher-0.2.1/gpt_researcher/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.942818 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.944584 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6033 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/detailed_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.945656 gpt-researcher-0.2.1/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.947194 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.948694 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.949809 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.951351 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.952754 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-12 13:06:43.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.954170 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.955547 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.957002 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.958742 gpt-researcher-0.2.1/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.960096 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.961632 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.963550 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.965288 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.966951 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.972544 gpt-researcher-0.2.1/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.1/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-12 12:40:03.000000 gpt-researcher-0.2.1/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/utils/validators.py
--rw-r--r--   0 assafel    (501) staff       (20)     2872 2024-04-01 15:55:34.000000 gpt-researcher-0.2.1/gpt_researcher/utils/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:13:27.925126 gpt-researcher-0.2.1/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       15 2024-04-12 13:13:27.000000 gpt-researcher-0.2.1/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1130 2024-04-09 08:07:24.000000 gpt-researcher-0.2.1/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-12 13:13:27.974663 gpt-researcher-0.2.1/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-12 13:13:07.000000 gpt-researcher-0.2.1/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.545206 gpt-researcher-0.2.2/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:20:52.544508 gpt-researcher-0.2.2/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    11791 2024-04-09 08:07:24.000000 gpt-researcher-0.2.2/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.501074 gpt-researcher-0.2.2/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.2/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.505266 gpt-researcher-0.2.2/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.2/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2101 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.507045 gpt-researcher-0.2.2/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.2/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.2/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.507637 gpt-researcher-0.2.2/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-01 15:55:37.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.508709 gpt-researcher-0.2.2/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:37.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-09 08:07:24.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.509761 gpt-researcher-0.2.2/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-03-31 16:54:34.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.510886 gpt-researcher-0.2.2/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-31 16:54:34.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-03-31 16:54:34.000000 gpt-researcher-0.2.2/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.513364 gpt-researcher-0.2.2/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.2/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8922 2024-04-12 13:20:00.000000 gpt-researcher-0.2.2/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-12 13:09:04.000000 gpt-researcher-0.2.2/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12803 2024-04-12 13:17:40.000000 gpt-researcher-0.2.2/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.514606 gpt-researcher-0.2.2/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.2/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-01 15:55:37.000000 gpt-researcher-0.2.2/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.515196 gpt-researcher-0.2.2/gpt_researcher/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.516275 gpt-researcher-0.2.2/gpt_researcher/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.517359 gpt-researcher-0.2.2/gpt_researcher/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6033 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/report_type/detailed_report/detailed_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.518083 gpt-researcher-0.2.2/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.519384 gpt-researcher-0.2.2/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.520525 gpt-researcher-0.2.2/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.522060 gpt-researcher-0.2.2/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.523527 gpt-researcher-0.2.2/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-03-31 16:54:34.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.525280 gpt-researcher-0.2.2/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-12 13:06:43.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.526924 gpt-researcher-0.2.2/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.528533 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.530231 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.531995 gpt-researcher-0.2.2/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.533507 gpt-researcher-0.2.2/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.534714 gpt-researcher-0.2.2/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.536502 gpt-researcher-0.2.2/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.537982 gpt-researcher-0.2.2/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.539294 gpt-researcher-0.2.2/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.543429 gpt-researcher-0.2.2/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.2/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-12 12:40:03.000000 gpt-researcher-0.2.2/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-09 08:07:24.000000 gpt-researcher-0.2.2/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/utils/validators.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2872 2024-04-01 15:55:34.000000 gpt-researcher-0.2.2/gpt_researcher/utils/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-12 13:20:52.504115 gpt-researcher-0.2.2/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    12514 2024-04-12 13:20:52.000000 gpt-researcher-0.2.2/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-04-12 13:20:52.000000 gpt-researcher-0.2.2/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-12 13:20:52.000000 gpt-researcher-0.2.2/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-12 13:20:52.000000 gpt-researcher-0.2.2/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       15 2024-04-12 13:20:52.000000 gpt-researcher-0.2.2/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1130 2024-04-09 08:07:24.000000 gpt-researcher-0.2.2/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-12 13:20:52.545367 gpt-researcher-0.2.2/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-12 13:20:09.000000 gpt-researcher-0.2.2/setup.py
```

### Comparing `gpt-researcher-0.2.1/LICENSE` & `gpt-researcher-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/PKG-INFO` & `gpt-researcher-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.1
+Version: 0.2.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.2.1/README.md` & `gpt-researcher-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/config/config.py` & `gpt-researcher-0.2.2/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/context/compression.py` & `gpt-researcher-0.2.2/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/context/retriever.py` & `gpt-researcher-0.2.2/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.2.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.2.2/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.2.2/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/master/agent.py` & `gpt-researcher-0.2.2/gpt_researcher/master/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             subtopics: list
             visited_urls: set
         """
         self.query = query
         self.agent = agent
         self.role = role
         self.report_type = report_type
+        self.report_prompt = get_prompt_by_report_type(self.report_type)  # this validates the report type
         self.websocket = websocket
         self.cfg = Config(config_path)
         self.retriever = get_retriever(self.cfg.retriever)
         self.context = []
         self.source_urls = source_urls
         self.memory = Memory(self.cfg.embedding_provider)
         self.visited_urls = visited_urls
```

### Comparing `gpt-researcher-0.2.1/gpt_researcher/master/functions.py` & `gpt-researcher-0.2.2/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/master/prompts.py` & `gpt-researcher-0.2.2/gpt_researcher/master/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,9 +231,9 @@
 }
 
 
 def get_prompt_by_report_type(report_type):
     prompt_by_type = report_type_mapping.get(report_type)
     if not prompt_by_type:
         raise Exception(f"Invalid report type: {report_type}.\n"
-                        f"Please use one of the following: {', '.join(report.name for report in ReportType)}")
+                        f"Please use one of the following: {', '.join(report.value for report in ReportType)}")
     return prompt_by_type
```

### Comparing `gpt-researcher-0.2.1/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.2.2/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/report_type/basic_report/basic_report.py` & `gpt-researcher-0.2.2/gpt_researcher/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.2.2/gpt_researcher/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.2.2/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.2.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/utils/llm.py` & `gpt-researcher-0.2.2/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher/utils/websocket_manager.py` & `gpt-researcher-0.2.2/gpt_researcher/utils/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.2.2/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.1
+Version: 0.2.2
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.2.1/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.2.2/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/pyproject.toml` & `gpt-researcher-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.1/setup.py` & `gpt-researcher-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.2.1",
+    version="0.2.2",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

