# Comparing `tmp/gpt-researcher-0.5.3.tar.gz` & `tmp/gpt-researcher-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.5.3.tar", last modified: Thu May 23 13:15:12 2024, max compression
+gzip compressed data, was "gpt-researcher-0.5.4.tar", last modified: Sat May 25 06:45:01 2024, max compression
```

## Comparing `gpt-researcher-0.5.3.tar` & `gpt-researcher-0.5.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.659529 gpt-researcher-0.5.3/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:15:12.658830 gpt-researcher-0.5.3/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    12159 2024-05-23 11:18:14.000000 gpt-researcher-0.5.3/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.603698 gpt-researcher-0.5.3/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.604254 gpt-researcher-0.5.3/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.605643 gpt-researcher-0.5.3/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.606715 gpt-researcher-0.5.3/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.3/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.607823 gpt-researcher-0.5.3/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.3/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.612545 gpt-researcher-0.5.3/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.3/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.615100 gpt-researcher-0.5.3/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.3/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.3/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.3/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.616808 gpt-researcher-0.5.3/gpt_researcher/document/
--rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/gpt_researcher/document/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/gpt_researcher/document/document.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.617665 gpt-researcher-0.5.3/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.619193 gpt-researcher-0.5.3/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.620790 gpt-researcher-0.5.3/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.622002 gpt-researcher-0.5.3/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.3/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.625159 gpt-researcher-0.5.3/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.3/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.3/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12450 2024-05-23 13:10:15.000000 gpt-researcher-0.5.3/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    14872 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.627424 gpt-researcher-0.5.3/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.3/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.5.3/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.628756 gpt-researcher-0.5.3/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      500 2024-05-23 13:00:48.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.630583 gpt-researcher-0.5.3/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.632291 gpt-researcher-0.5.3/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.634346 gpt-researcher-0.5.3/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.636631 gpt-researcher-0.5.3/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.638421 gpt-researcher-0.5.3/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.640301 gpt-researcher-0.5.3/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.642461 gpt-researcher-0.5.3/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2028 2024-05-23 13:06:48.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.644175 gpt-researcher-0.5.3/gpt_researcher/retrievers/yahoo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/yahoo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1125 2024-05-23 13:13:40.000000 gpt-researcher-0.5.3/gpt_researcher/retrievers/yahoo/yahoo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.646231 gpt-researcher-0.5.3/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.647621 gpt-researcher-0.5.3/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.649242 gpt-researcher-0.5.3/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.650874 gpt-researcher-0.5.3/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.652290 gpt-researcher-0.5.3/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.653877 gpt-researcher-0.5.3/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.657508 gpt-researcher-0.5.3/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.3/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.3/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-23 13:15:12.610899 gpt-researcher-0.5.3/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    12882 2024-05-23 13:15:12.000000 gpt-researcher-0.5.3/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2781 2024-05-23 13:15:12.000000 gpt-researcher-0.5.3/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-23 13:15:12.000000 gpt-researcher-0.5.3/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      393 2024-05-23 13:15:12.000000 gpt-researcher-0.5.3/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-23 13:15:12.000000 gpt-researcher-0.5.3/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.3/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-23 13:15:12.659718 gpt-researcher-0.5.3/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-23 13:14:55.000000 gpt-researcher-0.5.3/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.119402 gpt-researcher-0.5.4/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    13156 2024-05-25 06:45:01.118579 gpt-researcher-0.5.4/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    12433 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.061152 gpt-researcher-0.5.4/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.062386 gpt-researcher-0.5.4/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.064471 gpt-researcher-0.5.4/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      859 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.066075 gpt-researcher-0.5.4/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6151 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2405 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2720 2024-05-20 05:44:03.000000 gpt-researcher-0.5.4/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2986 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.067197 gpt-researcher-0.5.4/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.073089 gpt-researcher-0.5.4/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2388 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.076362 gpt-researcher-0.5.4/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1796 2024-05-09 12:40:13.000000 gpt-researcher-0.5.4/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.078599 gpt-researcher-0.5.4/gpt_researcher/document/
+-rw-r--r--   0 assafel    (501) staff       (20)       67 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/document/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2229 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/document/document.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.079623 gpt-researcher-0.5.4/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      282 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.081008 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.082880 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.084643 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2074 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/groq/groq.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.085999 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2457 2024-05-21 05:23:12.000000 gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.089506 gpt-researcher-0.5.4/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.5.4/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)    10219 2024-05-21 05:18:28.000000 gpt-researcher-0.5.4/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12330 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    14933 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.091342 gpt-researcher-0.5.4/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1697 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.091951 gpt-researcher-0.5.4/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      445 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.093279 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.094991 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.096614 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.098303 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.100010 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2418 2024-05-16 08:47:07.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.101550 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2149 2024-05-16 08:47:07.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.103031 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1926 2024-05-25 06:33:59.000000 gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.104624 gpt-researcher-0.5.4/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.106019 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.107625 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.109277 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.110959 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.112711 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.116835 gpt-researcher-0.5.4/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.5.4/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      341 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5323 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.5.4/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-25 06:45:01.071230 gpt-researcher-0.5.4/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    13156 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2782 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      392 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-25 06:45:00.000000 gpt-researcher-0.5.4/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1182 2024-05-20 06:53:38.000000 gpt-researcher-0.5.4/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-25 06:45:01.119677 gpt-researcher-0.5.4/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-25 06:42:57.000000 gpt-researcher-0.5.4/setup.py
```

### Comparing `gpt-researcher-0.5.3/LICENSE` & `gpt-researcher-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/PKG-INFO` & `gpt-researcher-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.3
+Version: 0.5.4
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
@@ -38,14 +39,15 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
+- Current LLMs are limited to short token outputs which are not sufficient for long detailed research reports (2k+ words).
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
 - Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
 
 ## Demo
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
```

### Comparing `gpt-researcher-0.5.3/README.md` & `gpt-researcher-0.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
@@ -20,14 +21,15 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
+- Current LLMs are limited to short token outputs which are not sufficient for long detailed research reports (2k+ words).
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
 - Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
 
 ## Demo
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
```

### Comparing `gpt-researcher-0.5.3/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.5.4/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.5.4/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/backend/server.py` & `gpt-researcher-0.5.4/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/backend/utils.py` & `gpt-researcher-0.5.4/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/backend/websocket_manager.py` & `gpt-researcher-0.5.4/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/config/config.py` & `gpt-researcher-0.5.4/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/context/compression.py` & `gpt-researcher-0.5.4/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/context/retriever.py` & `gpt-researcher-0.5.4/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/document/document.py` & `gpt-researcher-0.5.4/gpt_researcher/document/document.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.5.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.5.4/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.5.4/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/master/agent.py` & `gpt-researcher-0.5.4/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/master/functions.py` & `gpt-researcher-0.5.4/gpt_researcher/master/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,14 @@
     match retriever:
         case "tavily":
             from gpt_researcher.retrievers import TavilySearch
             retriever = TavilySearch
         case "google":
             from gpt_researcher.retrievers import GoogleSearch
             retriever = GoogleSearch
-        case "yahoo":
-            from gpt_researcher.retrievers import YahooSearch
-            retriever = YahooSearch
         case "searx":
             from gpt_researcher.retrievers import SearxSearch
             retriever = SearxSearch
         case "serpapi":
             from gpt_researcher.retrievers import SerpApiSearch
             retriever = SerpApiSearch
         case "googleSerp":
```

### Comparing `gpt-researcher-0.5.3/gpt_researcher/master/prompts.py` & `gpt-researcher-0.5.4/gpt_researcher/master/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         task = f"{parent_query} - {question}"
     else:
         task = question
 
     return f'Write {max_iterations} google search queries to search online that form an objective opinion from the following task: "{task}"' \
            f'Use the current date if needed: {datetime.now().strftime("%B %d, %Y")}.\n' \
            f'Also include in the queries specified task details such as locations, names, etc.\n' \
-           f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].'
+           f'You must respond with a list of strings in the following format: ["query 1", "query 2", "query 3"].\n' \
+           f'The response should contain ONLY the list.'
 
 
 def generate_report_prompt(question: str, context, report_source: str, report_format="apa", total_words=1000):
     """ Generates the report prompt for the given question and research summary.
     Args: question (str): The question to generate the report prompt for
             research_summary (str): The research summary to generate the report prompt for
     Returns: str: The report prompt for the given question and research summary
```

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.5.4/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Tavily API Retriever
 
 # libraries
 import os
 from tavily import TavilyClient
 from duckduckgo_search import DDGS
-from yahoo_search import search
 
 
 class TavilySearch():
     """
     Tavily API Retriever
     """
     def __init__(self, query, topic="general"):
@@ -52,10 +51,10 @@
             search_response = [{"href": obj["url"], "body": obj["content"]} for obj in sources]
         except Exception as e: # Fallback in case overload on Tavily Search API
             print(f"Error: {e}. Fallback to DuckDuckGo Search API...")
             try:
                 ddg = DDGS()
                 search_response = ddg.text(self.query, region='wt-wt', max_results=max_results)
             except Exception as e:
-                print(f"Error: {e}. Fallback to Yahoo Search API...")
-                search_response = [{"href": obj.link, "body": obj.text, "title": obj.title} for obj in search(self.query).pages]
+                print(f"Error: {e}. Failed fetching sources. Resulting in empty response.")
+                search_response = []
         return search_response
```

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.5.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/gpt_researcher/utils/llm.py` & `gpt-researcher-0.5.4/gpt_researcher/utils/llm.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,17 @@
             llm_provider = OpenAIProvider
         case "azureopenai":
             from ..llm_provider import AzureOpenAIProvider
             llm_provider = AzureOpenAIProvider
         case "google":
             from ..llm_provider import GoogleProvider
             llm_provider = GoogleProvider
+        case "groq":
+            from ..llm_provider import GroqProvider
+            llm_provider = GroqProvider
 
         case _:
             raise Exception("LLM provider not found.")
 
     return llm_provider
 
 
@@ -119,29 +122,30 @@
             input_variables=["task", "data", "subtopics", "max_subtopics"],
             partial_variables={
                 "format_instructions": parser.get_format_instructions()},
         )
 
         print(f"\n🤖 Calling {config.smart_llm_model}...\n")
 
-        if config.llm_provider == "openai":
-            model = ChatOpenAI(model=config.smart_llm_model)
-        elif config.llm_provider == "azureopenai":
-            from langchain_openai import AzureChatOpenAI
-            model = AzureChatOpenAI(model=config.smart_llm_model)
-        else:
-            return []
+        temperature = config.temperature
+        # temperature = 0 # Note: temperature throughout the code base is currently set to Zero
+        ProviderClass = get_provider(config.llm_provider)
+        provider = ProviderClass(model=config.smart_llm_model,
+                                 temperature=temperature,
+                                 max_tokens=config.smart_token_limit)
+        model = provider.llm
+
 
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

### Comparing `gpt-researcher-0.5.3/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.5.4/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.5.3
+Version: 0.5.4
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔎 GPT Researcher
-[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-blue?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Official%20Website-gptr.dev-teal?style=for-the-badge&logo=world&logoColor=white)](https://gptr.dev)
+[![Official Website](https://img.shields.io/badge/Documentation-GPTR-pink?logo=googledocs&logoColor=white&style=for-the-badge)](https://docs.gptr.dev)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/SK3KKuSD?style=for-the-badge)](https://discord.gg/SK3KKuSD)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/assafelovic/gpt-researcher?style=social)](https://github.com/assafelovic/gpt-researcher)
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/assafelovic/gpt-researcher/blob/master/examples/pip-run.ipynb)
 
@@ -38,14 +39,15 @@
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
+- Current LLMs are limited to short token outputs which are not sufficient for long detailed research reports (2k+ words).
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
 - Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
 
 ## Demo
 https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
```

### Comparing `gpt-researcher-0.5.3/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.5.4/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 gpt_researcher/document/__init__.py
 gpt_researcher/document/document.py
 gpt_researcher/llm_provider/__init__.py
 gpt_researcher/llm_provider/azureopenai/__init__.py
 gpt_researcher/llm_provider/azureopenai/azureopenai.py
 gpt_researcher/llm_provider/google/__init__.py
 gpt_researcher/llm_provider/google/google.py
+gpt_researcher/llm_provider/groq/__init__.py
+gpt_researcher/llm_provider/groq/groq.py
 gpt_researcher/llm_provider/openai/__init__.py
 gpt_researcher/llm_provider/openai/openai.py
 gpt_researcher/master/__init__.py
 gpt_researcher/master/agent.py
 gpt_researcher/master/functions.py
 gpt_researcher/master/prompts.py
 gpt_researcher/memory/__init__.py
@@ -48,16 +50,14 @@
 gpt_researcher/retrievers/searx/searx.py
 gpt_researcher/retrievers/serpapi/__init__.py
 gpt_researcher/retrievers/serpapi/serpapi.py
 gpt_researcher/retrievers/serper/__init__.py
 gpt_researcher/retrievers/serper/serper.py
 gpt_researcher/retrievers/tavily_search/__init__.py
 gpt_researcher/retrievers/tavily_search/tavily_search.py
-gpt_researcher/retrievers/yahoo/__init__.py
-gpt_researcher/retrievers/yahoo/yahoo.py
 gpt_researcher/scraper/__init__.py
 gpt_researcher/scraper/scraper.py
 gpt_researcher/scraper/arxiv/__init__.py
 gpt_researcher/scraper/arxiv/arxiv.py
 gpt_researcher/scraper/beautiful_soup/__init__.py
 gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
 gpt_researcher/scraper/newspaper/__init__.py
```

### Comparing `gpt-researcher-0.5.3/pyproject.toml` & `gpt-researcher-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.5.3/setup.py` & `gpt-researcher-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.5.3",
+    version="0.5.4",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

