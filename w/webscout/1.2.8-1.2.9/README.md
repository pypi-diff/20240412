# Comparing `tmp/webscout-1.2.8.tar.gz` & `tmp/webscout-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.2.8.tar", last modified: Tue Apr  9 09:28:37 2024, max compression
+gzip compressed data, was "webscout-1.2.9.tar", last modified: Fri Apr 12 12:05:49 2024, max compression
```

## Comparing `webscout-1.2.8.tar` & `webscout-1.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.824119 webscout-1.2.8/
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.213994 webscout-1.2.8/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.257495 webscout-1.2.8/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.309498 webscout-1.2.8/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3846 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.349494 webscout-1.2.8/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     1754 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-04-02 10:54:23.000000 webscout-1.2.8/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-04-02 10:54:23.000000 webscout-1.2.8/LICENSE.md
--rw-rw-rw-   0        0        0    24645 2024-04-09 09:28:37.824119 webscout-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    22470 2024-04-09 09:23:09.000000 webscout-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 09:28:37.824119 webscout-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2817 2024-04-09 09:25:42.000000 webscout-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.665109 webscout-1.2.8/webscout/
--rw-rw-rw-   0        0        0    57985 2024-04-06 15:11:56.000000 webscout-1.2.8/webscout/AI.py
--rw-rw-rw-   0        0        0     2343 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/AIbase.py
--rw-rw-rw-   0        0        0    24123 2024-04-03 10:06:49.000000 webscout-1.2.8/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     8103 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/HelpingAI.py
--rw-rw-rw-   0        0        0     3309 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/LLM.py
--rw-rw-rw-   0        0        0      547 2024-04-07 06:11:57.000000 webscout-1.2.8/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-04-03 10:30:01.000000 webscout-1.2.8/webscout/__main__.py
--rw-rw-rw-   0        0        0    17059 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/cli.py
--rw-rw-rw-   0        0        0      276 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/exceptions.py
--rw-rw-rw-   0        0        0      692 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/models.py
--rw-rw-rw-   0        0        0    20140 2024-04-09 09:21:35.000000 webscout-1.2.8/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2605 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-04-09 09:19:36.000000 webscout-1.2.8/webscout/version.py
--rw-rw-rw-   0        0        0     3085 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    40670 2024-04-02 10:54:23.000000 webscout-1.2.8/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-04-09 09:28:37.801562 webscout-1.2.8/webscout.egg-info/
--rw-rw-rw-   0        0        0    24645 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      965 2024-04-09 09:28:36.000000 webscout-1.2.8/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      334 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-09 09:28:35.000000 webscout-1.2.8/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.785675 webscout-1.2.9/
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.784895 webscout-1.2.9/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.833863 webscout-1.2.9/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.903418 webscout-1.2.9/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3846 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:48.964442 webscout-1.2.9/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     1754 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-04-11 08:32:30.000000 webscout-1.2.9/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-04-11 08:32:30.000000 webscout-1.2.9/LICENSE.md
+-rw-rw-rw-   0        0        0    24513 2024-04-12 12:05:49.768680 webscout-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    22338 2024-04-11 08:32:30.000000 webscout-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:05:49.786678 webscout-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2817 2024-04-12 12:04:17.000000 webscout-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.350092 webscout-1.2.9/webscout/
+-rw-rw-rw-   0        0        0    57985 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AI.py
+-rw-rw-rw-   0        0        0     2343 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    24123 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     8103 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/HelpingAI.py
+-rw-rw-rw-   0        0        0     3309 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/LLM.py
+-rw-rw-rw-   0        0        0      519 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/__main__.py
+-rw-rw-rw-   0        0        0    17059 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/cli.py
+-rw-rw-rw-   0        0        0      276 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/exceptions.py
+-rw-rw-rw-   0        0        0      692 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/models.py
+-rw-rw-rw-   0        0        0    20622 2024-04-11 08:35:51.000000 webscout-1.2.9/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2605 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-04-12 12:04:27.000000 webscout-1.2.9/webscout/version.py
+-rw-rw-rw-   0        0        0     3085 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    40670 2024-04-11 08:32:30.000000 webscout-1.2.9/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:05:49.753666 webscout-1.2.9/webscout.egg-info/
+-rw-rw-rw-   0        0        0    24513 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      965 2024-04-12 12:05:48.000000 webscout-1.2.9/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      334 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 12:05:47.000000 webscout-1.2.9/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.2.8/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.2.9/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.2.9/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/networks/filepath_converter.py` & `webscout-1.2.9/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/networks/google_searcher.py` & `webscout-1.2.9/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/networks/network_configs.py` & `webscout-1.2.9/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.2.9/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/utilsdw/enver.py` & `webscout-1.2.9/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/DeepWEBS/utilsdw/logger.py` & `webscout-1.2.9/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/LICENSE.md` & `webscout-1.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/PKG-INFO` & `webscout-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.8
+Version: 1.2.9
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -353,48 +353,46 @@
 Here is an example of initializing the AsyncWEBS class:
 ```python3
 import asyncio
 import logging
 import sys
 from itertools import chain
 from random import shuffle
-
 import requests
 from webscout import AsyncWEBS
 
-# bypass curl-cffi NotImplementedError in windows https://curl-cffi.readthedocs.io/en/latest/faq/
+# If you have proxies, define them here
+proxies = None
+
 if sys.platform.lower().startswith("win"):
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 def get_words():
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     resp = requests.get(word_site)
     words = resp.text.splitlines()
     return words
 
 async def aget_results(word):
     async with AsyncWEBS(proxies=proxies) as WEBS:
-        results = [r async for r in WEBS.text(word, max_results=None)]
+        results = await WEBS.text(word, max_results=None)
         return results
 
 async def main():
     words = get_words()
     shuffle(words)
-    tasks = []
-    for word in words[:10]:
-        tasks.append(aget_results(word))
+    tasks = [aget_results(word) for word in words[:10]]
     results = await asyncio.gather(*tasks)
     print(f"Done")
     for r in chain.from_iterable(results):
         print(r)
-    
 
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main())
+logging.basicConfig(level=logging.DEBUG)
+
+await main()
 ```
 It is important to note that the WEBS and AsyncWEBS classes should always be used as a context manager (with statement).
 This ensures proper resource management and cleanup, as the context manager will automatically handle opening and closing the HTTP client connection.
 
 ## Exceptions
 
 Exceptions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.8 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.9 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
 now can transcribe yt videos Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -172,50 +172,48 @@
    To use the AsyncWEBS class, you can perform asynchronous operations using
  Python's asyncio library. To initialize an instance of the WEBS or AsyncWEBS
  classes, you can provide the following optional arguments: Here is an example
  of initializing the WEBS class: ```python3 from webscout import WEBS R = WEBS
 ().text("python programming", max_results=5) print(R) ``` Here is an example of
   initializing the AsyncWEBS class: ```python3 import asyncio import logging
    import sys from itertools import chain from random import shuffle import
-requests from webscout import AsyncWEBS # bypass curl-cffi NotImplementedError
-         in windows https://curl-cffi.readthedocs.io/en/latest/faq/ if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-AsyncWEBS(proxies=proxies) as WEBS: results = [r async for r in WEBS.text(word,
-max_results=None)] return results async def main(): words = get_words() shuffle
-  (words) tasks = [] for word in words[:10]: tasks.append(aget_results(word))
-        results = await asyncio.gather(*tasks) print(f"Done") for r in
-       chain.from_iterable(results): print(r) if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG) asyncio.run(main()) ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+requests from webscout import AsyncWEBS # If you have proxies, define them here
+           proxies = None if sys.platform.lower().startswith("win"):
+  asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) def
+ get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000" resp =
+ requests.get(word_site) words = resp.text.splitlines() return words async def
+ aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS: results =
+await WEBS.text(word, max_results=None) return results async def main(): words
+ = get_words() shuffle(words) tasks = [aget_results(word) for word in words[:
+      10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
  and yep.com ```python from webscout import WEBS # News search for the keyword
   'holiday' using DuckDuckGo.com and yep.com with WEBS() as WEBS: keywords =
         'holiday' WEBS_news_gen = WEBS.news( keywords, region="wt-wt",
 safesearch="off", timelimit="m", max_results=20 ) for r in WEBS_news_gen: print
    (r) ``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from
 webscout import WEBS # Map search for the keyword 'school' in 'anantnag' using
```

### Comparing `webscout-1.2.8/README.md` & `webscout-1.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -301,48 +301,46 @@
 Here is an example of initializing the AsyncWEBS class:
 ```python3
 import asyncio
 import logging
 import sys
 from itertools import chain
 from random import shuffle
-
 import requests
 from webscout import AsyncWEBS
 
-# bypass curl-cffi NotImplementedError in windows https://curl-cffi.readthedocs.io/en/latest/faq/
+# If you have proxies, define them here
+proxies = None
+
 if sys.platform.lower().startswith("win"):
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 def get_words():
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     resp = requests.get(word_site)
     words = resp.text.splitlines()
     return words
 
 async def aget_results(word):
     async with AsyncWEBS(proxies=proxies) as WEBS:
-        results = [r async for r in WEBS.text(word, max_results=None)]
+        results = await WEBS.text(word, max_results=None)
         return results
 
 async def main():
     words = get_words()
     shuffle(words)
-    tasks = []
-    for word in words[:10]:
-        tasks.append(aget_results(word))
+    tasks = [aget_results(word) for word in words[:10]]
     results = await asyncio.gather(*tasks)
     print(f"Done")
     for r in chain.from_iterable(results):
         print(r)
-    
 
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main())
+logging.basicConfig(level=logging.DEBUG)
+
+await main()
 ```
 It is important to note that the WEBS and AsyncWEBS classes should always be used as a context manager (with statement).
 This ensures proper resource management and cleanup, as the context manager will automatically handle opening and closing the HTTP client connection.
 
 ## Exceptions
 
 Exceptions:
```

#### html2text {}

```diff
@@ -144,50 +144,48 @@
    To use the AsyncWEBS class, you can perform asynchronous operations using
  Python's asyncio library. To initialize an instance of the WEBS or AsyncWEBS
  classes, you can provide the following optional arguments: Here is an example
  of initializing the WEBS class: ```python3 from webscout import WEBS R = WEBS
 ().text("python programming", max_results=5) print(R) ``` Here is an example of
   initializing the AsyncWEBS class: ```python3 import asyncio import logging
    import sys from itertools import chain from random import shuffle import
-requests from webscout import AsyncWEBS # bypass curl-cffi NotImplementedError
-         in windows https://curl-cffi.readthedocs.io/en/latest/faq/ if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-AsyncWEBS(proxies=proxies) as WEBS: results = [r async for r in WEBS.text(word,
-max_results=None)] return results async def main(): words = get_words() shuffle
-  (words) tasks = [] for word in words[:10]: tasks.append(aget_results(word))
-        results = await asyncio.gather(*tasks) print(f"Done") for r in
-       chain.from_iterable(results): print(r) if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG) asyncio.run(main()) ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+requests from webscout import AsyncWEBS # If you have proxies, define them here
+           proxies = None if sys.platform.lower().startswith("win"):
+  asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) def
+ get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000" resp =
+ requests.get(word_site) words = resp.text.splitlines() return words async def
+ aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS: results =
+await WEBS.text(word, max_results=None) return results async def main(): words
+ = get_words() shuffle(words) tasks = [aget_results(word) for word in words[:
+      10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
  and yep.com ```python from webscout import WEBS # News search for the keyword
   'holiday' using DuckDuckGo.com and yep.com with WEBS() as WEBS: keywords =
         'holiday' WEBS_news_gen = WEBS.news( keywords, region="wt-wt",
 safesearch="off", timelimit="m", max_results=20 ) for r in WEBS_news_gen: print
    (r) ``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from
 webscout import WEBS # Map search for the keyword 'school' in 'anantnag' using
```

### Comparing `webscout-1.2.8/setup.py` & `webscout-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #     exec(version_file.read())
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.2.8", 
+    version="1.2.9", 
     description="Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-1.2.8/webscout/AI.py` & `webscout-1.2.9/webscout/AI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/AIbase.py` & `webscout-1.2.9/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/AIutel.py` & `webscout-1.2.9/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/DWEBS.py` & `webscout-1.2.9/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/HelpingAI.py` & `webscout-1.2.9/webscout/HelpingAI.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/LLM.py` & `webscout-1.2.9/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/__init__.py` & `webscout-1.2.9/webscout/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,13 @@
 """
 
 import logging
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
-from .AIutel import appdir
 from .transcriber import transcriber
 
 
 __all__ = ["WEBS", "AsyncWEBS", "__version__", "cli"]
 
 logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-1.2.8/webscout/cli.py` & `webscout-1.2.9/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/models.py` & `webscout-1.2.9/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/transcriber.py` & `webscout-1.2.9/webscout/transcriber.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,497 +1,497 @@
-import requests
-import http.cookiejar as cookiejar
-import sys
-import json
-from xml.etree import ElementTree
-import re
-from requests import HTTPError
-import html.parser
-
-html_parser = html.parser.HTMLParser()
-import html
-
-def unescape(string):
-    return html.unescape(string)
-WATCH_URL = 'https://www.youtube.com/watch?v={video_id}'
-
-class TranscriptRetrievalError(Exception):
-    """
-    Base class for exceptions raised when a transcript cannot be retrieved.
-    """
-    ERROR_MESSAGE = '\nCould not retrieve a transcript for the video {video_url}!'
-    CAUSE_MESSAGE_INTRO = ' This is most likely caused by:\n\n{cause}'
-    CAUSE_MESSAGE = ''
-    GITHUB_REFERRAL = (
-        '\n\nIf you are sure that the described cause is not responsible for this error '
-        'and that a transcript should be retrievable, please create an issue at '
-        'https://github.com/OE-LUCIFER/Webscout/issues. '
-        'Please add which version of youtube_transcript_api you are using '
-        'and provide the information needed to replicate the error. '
-    )
-
-    def __init__(self, video_id):
-        self.video_id = video_id
-        super(TranscriptRetrievalError, self).__init__(self._build_error_message())
-
-    def _build_error_message(self):
-        cause = self.cause
-        error_message = self.ERROR_MESSAGE.format(video_url=WATCH_URL.format(video_id=self.video_id))
-
-        if cause:
-            error_message += self.CAUSE_MESSAGE_INTRO.format(cause=cause) + self.GITHUB_REFERRAL
-
-        return error_message
-
-    @property
-    def cause(self):
-        return self.CAUSE_MESSAGE
-
-class YouTubeRequestFailedError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'Request to YouTube failed: {reason}'
-
-    def __init__(self, video_id, http_error):
-        self.reason = str(http_error)
-        super(YouTubeRequestFailedError, self).__init__(video_id)
-
-    @property
-    def cause(self):
-        return self.CAUSE_MESSAGE.format(reason=self.reason)
-
-class VideoUnavailableError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'The video is no longer available'
-
-class InvalidVideoIdError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = (
-        'You provided an invalid video id. Make sure you are using the video id and NOT the url!\n\n'
-        'Do NOT run: `YouTubeTranscriptApi.get_transcript("https://www.youtube.com/watch?v=1234")`\n'
-        'Instead run: `YouTubeTranscriptApi.get_transcript("1234")`'
-    )
-
-class TooManyRequestsError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = (
-        'YouTube is receiving too many requests from this IP and now requires solving a captcha to continue. '
-        'One of the following things can be done to work around this:\n\
-        - Manually solve the captcha in a browser and export the cookie. '
-        'Read here how to use that cookie with '
-        'youtube-transcript-api: https://github.com/jdepoix/youtube-transcript-api#cookies\n\
-        - Use a different IP address\n\
-        - Wait until the ban on your IP has been lifted'
-    )
-
-class TranscriptsDisabledError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'Subtitles are disabled for this video'
-
-class NoTranscriptAvailableError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'No transcripts are available for this video'
-
-class NotTranslatableError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'The requested language is not translatable'
-
-class TranslationLanguageNotAvailableError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'The requested translation language is not available'
-
-class CookiePathInvalidError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'The provided cookie file was unable to be loaded'
-
-class CookiesInvalidError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'The cookies provided are not valid (may have expired)'
-
-class FailedToCreateConsentCookieError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = 'Failed to automatically give consent to saving cookies'
-
-class NoTranscriptFoundError(TranscriptRetrievalError):
-    CAUSE_MESSAGE = (
-        'No transcripts were found for any of the requested language codes: {requested_language_codes}\n\n'
-        '{transcript_data}'
-    )
-
-    def __init__(self, video_id, requested_language_codes, transcript_data):
-        self._requested_language_codes = requested_language_codes
-        self._transcript_data = transcript_data
-        super(NoTranscriptFoundError, self).__init__(video_id)
-
-    @property
-    def cause(self):
-        return self.CAUSE_MESSAGE.format(
-            requested_language_codes=self._requested_language_codes,
-            transcript_data=str(self._transcript_data),
-        )
-
-
-
-def _raise_http_errors(response, video_id):
-    try:
-        response.raise_for_status()
-        return response
-    except HTTPError as error:
-        raise YouTubeRequestFailedError(error, video_id)
-
-
-class TranscriptListFetcher(object):
-    def __init__(self, http_client):
-        self._http_client = http_client
-
-    def fetch(self, video_id):
-        return TranscriptList.build(
-            self._http_client,
-            video_id,
-            self._extract_captions_json(self._fetch_video_html(video_id), video_id),
-        )
-
-    def _extract_captions_json(self, html, video_id):
-        splitted_html = html.split('"captions":')
-
-        if len(splitted_html) <= 1:
-            if video_id.startswith('http://') or video_id.startswith('https://'):
-                raise InvalidVideoIdError(video_id)
-            if 'class="g-recaptcha"' in html:
-                raise TooManyRequestsError(video_id)
-            if '"playabilityStatus":' not in html:
-                raise VideoUnavailableError(video_id)
-
-            raise TranscriptsDisabledError(video_id)
-
-        captions_json = json.loads(
-            splitted_html[1].split(',"videoDetails')[0].replace('\n', '')
-        ).get('playerCaptionsTracklistRenderer')
-        if captions_json is None:
-            raise TranscriptsDisabledError(video_id)
-
-        if 'captionTracks' not in captions_json:
-            raise TranscriptsDisabledError(video_id)
-
-        return captions_json
-
-    def _create_consent_cookie(self, html, video_id):
-        match = re.search('name="v" value="(.*?)"', html)
-        if match is None:
-            raise FailedToCreateConsentCookieError(video_id)
-        self._http_client.cookies.set('CONSENT', 'YES+' + match.group(1), domain='.youtube.com')
-
-    def _fetch_video_html(self, video_id):
-        html = self._fetch_html(video_id)
-        if 'action="https://consent.youtube.com/s"' in html:
-            self._create_consent_cookie(html, video_id)
-            html = self._fetch_html(video_id)
-            if 'action="https://consent.youtube.com/s"' in html:
-                raise FailedToCreateConsentCookieError(video_id)
-        return html
-
-    def _fetch_html(self, video_id):
-        response = self._http_client.get(WATCH_URL.format(video_id=video_id), headers={'Accept-Language': 'en-US'})
-        return unescape(_raise_http_errors(response, video_id).text)
-
-
-class TranscriptList(object):
-    """
-    This object represents a list of transcripts. It can be iterated over to list all transcripts which are available
-    for a given YouTube video. Also it provides functionality to search for a transcript in a given language.
-    """
-
-    def __init__(self, video_id, manually_created_transcripts, generated_transcripts, translation_languages):
-        """
-        The constructor is only for internal use. Use the static build method instead.
-
-        :param video_id: the id of the video this TranscriptList is for
-        :type video_id: str
-        :param manually_created_transcripts: dict mapping language codes to the manually created transcripts
-        :type manually_created_transcripts: dict[str, Transcript]
-        :param generated_transcripts: dict mapping language codes to the generated transcripts
-        :type generated_transcripts: dict[str, Transcript]
-        :param translation_languages: list of languages which can be used for translatable languages
-        :type translation_languages: list[dict[str, str]]
-        """
-        self.video_id = video_id
-        self._manually_created_transcripts = manually_created_transcripts
-        self._generated_transcripts = generated_transcripts
-        self._translation_languages = translation_languages
-
-    @staticmethod
-    def build(http_client, video_id, captions_json):
-        """
-        Factory method for TranscriptList.
-
-        :param http_client: http client which is used to make the transcript retrieving http calls
-        :type http_client: requests.Session
-        :param video_id: the id of the video this TranscriptList is for
-        :type video_id: str
-        :param captions_json: the JSON parsed from the YouTube pages static HTML
-        :type captions_json: dict
-        :return: the created TranscriptList
-        :rtype TranscriptList:
-        """
-        translation_languages = [
-            {
-                'language': translation_language['languageName']['simpleText'],
-                'language_code': translation_language['languageCode'],
-            } for translation_language in captions_json.get('translationLanguages', [])
-        ]
-
-        manually_created_transcripts = {}
-        generated_transcripts = {}
-
-        for caption in captions_json['captionTracks']:
-            if caption.get('kind', '') == 'asr':
-                transcript_dict = generated_transcripts
-            else:
-                transcript_dict = manually_created_transcripts
-
-            transcript_dict[caption['languageCode']] = Transcript(
-                http_client,
-                video_id,
-                caption['baseUrl'],
-                caption['name']['simpleText'],
-                caption['languageCode'],
-                caption.get('kind', '') == 'asr',
-                translation_languages if caption.get('isTranslatable', False) else [],
-            )
-
-        return TranscriptList(
-            video_id,
-            manually_created_transcripts,
-            generated_transcripts,
-            translation_languages,
-        )
-
-    def __iter__(self):
-        return iter(list(self._manually_created_transcripts.values()) + list(self._generated_transcripts.values()))
-
-    def find_transcript(self, language_codes):
-        """
-        Finds a transcript for a given language code. Manually created transcripts are returned first and only if none
-        are found, generated transcripts are used. If you only want generated transcripts use
-        `find_manually_created_transcript` instead.
-
-        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
-        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
-        it fails to do so.
-        :type languages: list[str]
-        :return: the found Transcript
-        :rtype Transcript:
-        :raises: NoTranscriptFound
-        """
-        return self._find_transcript(language_codes, [self._manually_created_transcripts, self._generated_transcripts])
-
-    def find_generated_transcript(self, language_codes):
-        """
-        Finds an automatically generated transcript for a given language code.
-
-        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
-        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
-        it fails to do so.
-        :type languages: list[str]
-        :return: the found Transcript
-        :rtype Transcript:
-        :raises: NoTranscriptFound
-        """
-        return self._find_transcript(language_codes, [self._generated_transcripts])
-
-    def find_manually_created_transcript(self, language_codes):
-        """
-        Finds a manually created transcript for a given language code.
-
-        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
-        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
-        it fails to do so.
-        :type languages: list[str]
-        :return: the found Transcript
-        :rtype Transcript:
-        :raises: NoTranscriptFound
-        """
-        return self._find_transcript(language_codes, [self._manually_created_transcripts])
-
-    def _find_transcript(self, language_codes, transcript_dicts):
-        for language_code in language_codes:
-            for transcript_dict in transcript_dicts:
-                if language_code in transcript_dict:
-                    return transcript_dict[language_code]
-
-        raise NoTranscriptFoundError(
-            self.video_id,
-            language_codes,
-            self
-        )
-
-    def __str__(self):
-        return (
-            'For this video ({video_id}) transcripts are available in the following languages:\n\n'
-            '(MANUALLY CREATED)\n'
-            '{available_manually_created_transcript_languages}\n\n'
-            '(GENERATED)\n'
-            '{available_generated_transcripts}\n\n'
-            '(TRANSLATION LANGUAGES)\n'
-            '{available_translation_languages}'
-        ).format(
-            video_id=self.video_id,
-            available_manually_created_transcript_languages=self._get_language_description(
-                str(transcript) for transcript in self._manually_created_transcripts.values()
-            ),
-            available_generated_transcripts=self._get_language_description(
-                str(transcript) for transcript in self._generated_transcripts.values()
-            ),
-            available_translation_languages=self._get_language_description(
-                '{language_code} ("{language}")'.format(
-                    language=translation_language['language'],
-                    language_code=translation_language['language_code'],
-                ) for translation_language in self._translation_languages
-            )
-        )
-
-    def _get_language_description(self, transcript_strings):
-        description = '\n'.join(' - {transcript}'.format(transcript=transcript) for transcript in transcript_strings)
-        return description if description else 'None'
-
-
-class Transcript(object):
-    def __init__(self, http_client, video_id, url, language, language_code, is_generated, translation_languages):
-        """
-        You probably don't want to initialize this directly. Usually you'll access Transcript objects using a
-        TranscriptList.
-
-        :param http_client: http client which is used to make the transcript retrieving http calls
-        :type http_client: requests.Session
-        :param video_id: the id of the video this TranscriptList is for
-        :type video_id: str
-        :param url: the url which needs to be called to fetch the transcript
-        :param language: the name of the language this transcript uses
-        :param language_code:
-        :param is_generated:
-        :param translation_languages:
-        """
-        self._http_client = http_client
-        self.video_id = video_id
-        self._url = url
-        self.language = language
-        self.language_code = language_code
-        self.is_generated = is_generated
-        self.translation_languages = translation_languages
-        self._translation_languages_dict = {
-            translation_language['language_code']: translation_language['language']
-            for translation_language in translation_languages
-        }
-
-    def fetch(self, preserve_formatting=False):
-        """
-        Loads the actual transcript data.
-        :param preserve_formatting: whether to keep select HTML text formatting
-        :type preserve_formatting: bool
-        :return: a list of dictionaries containing the 'text', 'start' and 'duration' keys
-        :rtype [{'text': str, 'start': float, 'end': float}]:
-        """
-        response = self._http_client.get(self._url, headers={'Accept-Language': 'en-US'})
-        return _TranscriptParser(preserve_formatting=preserve_formatting).parse(
-            _raise_http_errors(response, self.video_id).text,
-        )
-
-    def __str__(self):
-        return '{language_code} ("{language}"){translation_description}'.format(
-            language=self.language,
-            language_code=self.language_code,
-            translation_description='[TRANSLATABLE]' if self.is_translatable else ''
-        )
-
-    @property
-    def is_translatable(self):
-        return len(self.translation_languages) > 0
-
-    def translate(self, language_code):
-        if not self.is_translatable:
-            raise NotTranslatableError(self.video_id)
-
-        if language_code not in self._translation_languages_dict:
-            raise TranslationLanguageNotAvailableError(self.video_id)
-
-        return Transcript(
-            self._http_client,
-            self.video_id,
-            '{url}&tlang={language_code}'.format(url=self._url, language_code=language_code),
-            self._translation_languages_dict[language_code],
-            language_code,
-            True,
-            [],
-        )
-
-
-class _TranscriptParser(object):
-    _FORMATTING_TAGS = [
-        'strong',  # important
-        'em',  # emphasized
-        'b',  # bold
-        'i',  # italic
-        'mark',  # marked
-        'small',  # smaller
-        'del',  # deleted
-        'ins',  # inserted
-        'sub',  # subscript
-        'sup',  # superscript
-    ]
-
-    def __init__(self, preserve_formatting=False):
-        self._html_regex = self._get_html_regex(preserve_formatting)
-
-    def _get_html_regex(self, preserve_formatting):
-        if preserve_formatting:
-            formats_regex = '|'.join(self._FORMATTING_TAGS)
-            formats_regex = r'<\/?(?!\/?(' + formats_regex + r')\b).*?\b>'
-            html_regex = re.compile(formats_regex, re.IGNORECASE)
-        else:
-            html_regex = re.compile(r'<[^>]*>', re.IGNORECASE)
-        return html_regex
-
-    def parse(self, plain_data):
-        return [
-            {
-                'text': re.sub(self._html_regex, '', unescape(xml_element.text)),
-                'start': float(xml_element.attrib['start']),
-                'duration': float(xml_element.attrib.get('dur', '0.0')),
-            }
-            for xml_element in ElementTree.fromstring(plain_data)
-            if xml_element.text is not None
-        ]
-
-WATCH_URL = 'https://www.youtube.com/watch?v={video_id}'
-
-class transcriber(object):
-    @classmethod
-    def list_transcripts(cls, video_id, proxies=None, cookies=None):
-        with requests.Session() as http_client:
-            if cookies:
-                http_client.cookies = cls._load_cookies(cookies, video_id)
-            http_client.proxies = proxies if proxies else {}
-            return TranscriptListFetcher(http_client).fetch(video_id)
-
-    @classmethod
-    def get_transcripts(cls, video_ids, languages=('en',), continue_after_error=False, proxies=None,
-                        cookies=None, preserve_formatting=False):
-
-        assert isinstance(video_ids, list), "`video_ids` must be a list of strings"
-
-        data = {}
-        unretrievable_videos = []
-
-        for video_id in video_ids:
-            try:
-                data[video_id] = cls.get_transcript(video_id, languages, proxies, cookies, preserve_formatting)
-            except Exception as exception:
-                if not continue_after_error:
-                    raise exception
-
-                unretrievable_videos.append(video_id)
-
-        return data, unretrievable_videos
-
-    @classmethod
-    def get_transcript(cls, video_id, languages=('en',), proxies=None, cookies=None, preserve_formatting=False):
-        assert isinstance(video_id, str), "`video_id` must be a string"
-        return cls.list_transcripts(video_id, proxies, cookies).find_transcript(languages).fetch(preserve_formatting=preserve_formatting)
-
-    @classmethod
-    def _load_cookies(cls, cookies, video_id):
-        try:
-            cookie_jar = cookiejar.MozillaCookieJar()
-            cookie_jar.load(cookies)
-            if not cookie_jar:
-                raise CookiesInvalidError(video_id)
-            return cookie_jar
-        except:
+import requests
+import http.cookiejar as cookiejar
+import sys
+import json
+from xml.etree import ElementTree
+import re
+from requests import HTTPError
+import html.parser
+
+html_parser = html.parser.HTMLParser()
+import html
+
+def unescape(string):
+    return html.unescape(string)
+WATCH_URL = 'https://www.youtube.com/watch?v={video_id}'
+
+class TranscriptRetrievalError(Exception):
+    """
+    Base class for exceptions raised when a transcript cannot be retrieved.
+    """
+    ERROR_MESSAGE = '\nCould not retrieve a transcript for the video {video_url}!'
+    CAUSE_MESSAGE_INTRO = ' This is most likely caused by:\n\n{cause}'
+    CAUSE_MESSAGE = ''
+    GITHUB_REFERRAL = (
+        '\n\nIf you are sure that the described cause is not responsible for this error '
+        'and that a transcript should be retrievable, please create an issue at '
+        'https://github.com/OE-LUCIFER/Webscout/issues. '
+        'Please add which version of webscout you are using '
+        'and provide the information needed to replicate the error. '
+    )
+
+    def __init__(self, video_id):
+        self.video_id = video_id
+        super(TranscriptRetrievalError, self).__init__(self._build_error_message())
+
+    def _build_error_message(self):
+        cause = self.cause
+        error_message = self.ERROR_MESSAGE.format(video_url=WATCH_URL.format(video_id=self.video_id))
+
+        if cause:
+            error_message += self.CAUSE_MESSAGE_INTRO.format(cause=cause) + self.GITHUB_REFERRAL
+
+        return error_message
+
+    @property
+    def cause(self):
+        return self.CAUSE_MESSAGE
+
+class YouTubeRequestFailedError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'Request to YouTube failed: {reason}'
+
+    def __init__(self, video_id, http_error):
+        self.reason = str(http_error)
+        super(YouTubeRequestFailedError, self).__init__(video_id)
+
+    @property
+    def cause(self):
+        return self.CAUSE_MESSAGE.format(reason=self.reason)
+
+class VideoUnavailableError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'The video is no longer available'
+
+class InvalidVideoIdError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = (
+        'You provided an invalid video id. Make sure you are using the video id and NOT the url!\n\n'
+        'Do NOT run: `YouTubeTranscriptApi.get_transcript("https://www.youtube.com/watch?v=1234")`\n'
+        'Instead run: `YouTubeTranscriptApi.get_transcript("1234")`'
+    )
+
+class TooManyRequestsError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = (
+        'YouTube is receiving too many requests from this IP and now requires solving a captcha to continue. '
+        'One of the following things can be done to work around this:\n\
+        - Manually solve the captcha in a browser and export the cookie. '
+        'Read here how to use that cookie with '
+        'youtube-transcript-api: https://github.com/jdepoix/youtube-transcript-api#cookies\n\
+        - Use a different IP address\n\
+        - Wait until the ban on your IP has been lifted'
+    )
+
+class TranscriptsDisabledError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'Subtitles are disabled for this video'
+
+class NoTranscriptAvailableError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'No transcripts are available for this video'
+
+class NotTranslatableError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'The requested language is not translatable'
+
+class TranslationLanguageNotAvailableError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'The requested translation language is not available'
+
+class CookiePathInvalidError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'The provided cookie file was unable to be loaded'
+
+class CookiesInvalidError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'The cookies provided are not valid (may have expired)'
+
+class FailedToCreateConsentCookieError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = 'Failed to automatically give consent to saving cookies'
+
+class NoTranscriptFoundError(TranscriptRetrievalError):
+    CAUSE_MESSAGE = (
+        'No transcripts were found for any of the requested language codes: {requested_language_codes}\n\n'
+        '{transcript_data}'
+    )
+
+    def __init__(self, video_id, requested_language_codes, transcript_data):
+        self._requested_language_codes = requested_language_codes
+        self._transcript_data = transcript_data
+        super(NoTranscriptFoundError, self).__init__(video_id)
+
+    @property
+    def cause(self):
+        return self.CAUSE_MESSAGE.format(
+            requested_language_codes=self._requested_language_codes,
+            transcript_data=str(self._transcript_data),
+        )
+
+
+
+def _raise_http_errors(response, video_id):
+    try:
+        response.raise_for_status()
+        return response
+    except HTTPError as error:
+        raise YouTubeRequestFailedError(error, video_id)
+
+
+class TranscriptListFetcher(object):
+    def __init__(self, http_client):
+        self._http_client = http_client
+
+    def fetch(self, video_id):
+        return TranscriptList.build(
+            self._http_client,
+            video_id,
+            self._extract_captions_json(self._fetch_video_html(video_id), video_id),
+        )
+
+    def _extract_captions_json(self, html, video_id):
+        splitted_html = html.split('"captions":')
+
+        if len(splitted_html) <= 1:
+            if video_id.startswith('http://') or video_id.startswith('https://'):
+                raise InvalidVideoIdError(video_id)
+            if 'class="g-recaptcha"' in html:
+                raise TooManyRequestsError(video_id)
+            if '"playabilityStatus":' not in html:
+                raise VideoUnavailableError(video_id)
+
+            raise TranscriptsDisabledError(video_id)
+
+        captions_json = json.loads(
+            splitted_html[1].split(',"videoDetails')[0].replace('\n', '')
+        ).get('playerCaptionsTracklistRenderer')
+        if captions_json is None:
+            raise TranscriptsDisabledError(video_id)
+
+        if 'captionTracks' not in captions_json:
+            raise TranscriptsDisabledError(video_id)
+
+        return captions_json
+
+    def _create_consent_cookie(self, html, video_id):
+        match = re.search('name="v" value="(.*?)"', html)
+        if match is None:
+            raise FailedToCreateConsentCookieError(video_id)
+        self._http_client.cookies.set('CONSENT', 'YES+' + match.group(1), domain='.youtube.com')
+
+    def _fetch_video_html(self, video_id):
+        html = self._fetch_html(video_id)
+        if 'action="https://consent.youtube.com/s"' in html:
+            self._create_consent_cookie(html, video_id)
+            html = self._fetch_html(video_id)
+            if 'action="https://consent.youtube.com/s"' in html:
+                raise FailedToCreateConsentCookieError(video_id)
+        return html
+
+    def _fetch_html(self, video_id):
+        response = self._http_client.get(WATCH_URL.format(video_id=video_id), headers={'Accept-Language': 'en-US'})
+        return unescape(_raise_http_errors(response, video_id).text)
+
+
+class TranscriptList(object):
+    """
+    This object represents a list of transcripts. It can be iterated over to list all transcripts which are available
+    for a given YouTube video. Also it provides functionality to search for a transcript in a given language.
+    """
+
+    def __init__(self, video_id, manually_created_transcripts, generated_transcripts, translation_languages):
+        """
+        The constructor is only for internal use. Use the static build method instead.
+
+        :param video_id: the id of the video this TranscriptList is for
+        :type video_id: str
+        :param manually_created_transcripts: dict mapping language codes to the manually created transcripts
+        :type manually_created_transcripts: dict[str, Transcript]
+        :param generated_transcripts: dict mapping language codes to the generated transcripts
+        :type generated_transcripts: dict[str, Transcript]
+        :param translation_languages: list of languages which can be used for translatable languages
+        :type translation_languages: list[dict[str, str]]
+        """
+        self.video_id = video_id
+        self._manually_created_transcripts = manually_created_transcripts
+        self._generated_transcripts = generated_transcripts
+        self._translation_languages = translation_languages
+
+    @staticmethod
+    def build(http_client, video_id, captions_json):
+        """
+        Factory method for TranscriptList.
+
+        :param http_client: http client which is used to make the transcript retrieving http calls
+        :type http_client: requests.Session
+        :param video_id: the id of the video this TranscriptList is for
+        :type video_id: str
+        :param captions_json: the JSON parsed from the YouTube pages static HTML
+        :type captions_json: dict
+        :return: the created TranscriptList
+        :rtype TranscriptList:
+        """
+        translation_languages = [
+            {
+                'language': translation_language['languageName']['simpleText'],
+                'language_code': translation_language['languageCode'],
+            } for translation_language in captions_json.get('translationLanguages', [])
+        ]
+
+        manually_created_transcripts = {}
+        generated_transcripts = {}
+
+        for caption in captions_json['captionTracks']:
+            if caption.get('kind', '') == 'asr':
+                transcript_dict = generated_transcripts
+            else:
+                transcript_dict = manually_created_transcripts
+
+            transcript_dict[caption['languageCode']] = Transcript(
+                http_client,
+                video_id,
+                caption['baseUrl'],
+                caption['name']['simpleText'],
+                caption['languageCode'],
+                caption.get('kind', '') == 'asr',
+                translation_languages if caption.get('isTranslatable', False) else [],
+            )
+
+        return TranscriptList(
+            video_id,
+            manually_created_transcripts,
+            generated_transcripts,
+            translation_languages,
+        )
+
+    def __iter__(self):
+        return iter(list(self._manually_created_transcripts.values()) + list(self._generated_transcripts.values()))
+
+    def find_transcript(self, language_codes):
+        """
+        Finds a transcript for a given language code. Manually created transcripts are returned first and only if none
+        are found, generated transcripts are used. If you only want generated transcripts use
+        `find_manually_created_transcript` instead.
+
+        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
+        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
+        it fails to do so.
+        :type languages: list[str]
+        :return: the found Transcript
+        :rtype Transcript:
+        :raises: NoTranscriptFound
+        """
+        return self._find_transcript(language_codes, [self._manually_created_transcripts, self._generated_transcripts])
+
+    def find_generated_transcript(self, language_codes):
+        """
+        Finds an automatically generated transcript for a given language code.
+
+        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
+        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
+        it fails to do so.
+        :type languages: list[str]
+        :return: the found Transcript
+        :rtype Transcript:
+        :raises: NoTranscriptFound
+        """
+        return self._find_transcript(language_codes, [self._generated_transcripts])
+
+    def find_manually_created_transcript(self, language_codes):
+        """
+        Finds a manually created transcript for a given language code.
+
+        :param language_codes: A list of language codes in a descending priority. For example, if this is set to
+        ['de', 'en'] it will first try to fetch the german transcript (de) and then fetch the english transcript (en) if
+        it fails to do so.
+        :type languages: list[str]
+        :return: the found Transcript
+        :rtype Transcript:
+        :raises: NoTranscriptFound
+        """
+        return self._find_transcript(language_codes, [self._manually_created_transcripts])
+
+    def _find_transcript(self, language_codes, transcript_dicts):
+        for language_code in language_codes:
+            for transcript_dict in transcript_dicts:
+                if language_code in transcript_dict:
+                    return transcript_dict[language_code]
+
+        raise NoTranscriptFoundError(
+            self.video_id,
+            language_codes,
+            self
+        )
+
+    def __str__(self):
+        return (
+            'For this video ({video_id}) transcripts are available in the following languages:\n\n'
+            '(MANUALLY CREATED)\n'
+            '{available_manually_created_transcript_languages}\n\n'
+            '(GENERATED)\n'
+            '{available_generated_transcripts}\n\n'
+            '(TRANSLATION LANGUAGES)\n'
+            '{available_translation_languages}'
+        ).format(
+            video_id=self.video_id,
+            available_manually_created_transcript_languages=self._get_language_description(
+                str(transcript) for transcript in self._manually_created_transcripts.values()
+            ),
+            available_generated_transcripts=self._get_language_description(
+                str(transcript) for transcript in self._generated_transcripts.values()
+            ),
+            available_translation_languages=self._get_language_description(
+                '{language_code} ("{language}")'.format(
+                    language=translation_language['language'],
+                    language_code=translation_language['language_code'],
+                ) for translation_language in self._translation_languages
+            )
+        )
+
+    def _get_language_description(self, transcript_strings):
+        description = '\n'.join(' - {transcript}'.format(transcript=transcript) for transcript in transcript_strings)
+        return description if description else 'None'
+
+
+class Transcript(object):
+    def __init__(self, http_client, video_id, url, language, language_code, is_generated, translation_languages):
+        """
+        You probably don't want to initialize this directly. Usually you'll access Transcript objects using a
+        TranscriptList.
+
+        :param http_client: http client which is used to make the transcript retrieving http calls
+        :type http_client: requests.Session
+        :param video_id: the id of the video this TranscriptList is for
+        :type video_id: str
+        :param url: the url which needs to be called to fetch the transcript
+        :param language: the name of the language this transcript uses
+        :param language_code:
+        :param is_generated:
+        :param translation_languages:
+        """
+        self._http_client = http_client
+        self.video_id = video_id
+        self._url = url
+        self.language = language
+        self.language_code = language_code
+        self.is_generated = is_generated
+        self.translation_languages = translation_languages
+        self._translation_languages_dict = {
+            translation_language['language_code']: translation_language['language']
+            for translation_language in translation_languages
+        }
+
+    def fetch(self, preserve_formatting=False):
+        """
+        Loads the actual transcript data.
+        :param preserve_formatting: whether to keep select HTML text formatting
+        :type preserve_formatting: bool
+        :return: a list of dictionaries containing the 'text', 'start' and 'duration' keys
+        :rtype [{'text': str, 'start': float, 'end': float}]:
+        """
+        response = self._http_client.get(self._url, headers={'Accept-Language': 'en-US'})
+        return _TranscriptParser(preserve_formatting=preserve_formatting).parse(
+            _raise_http_errors(response, self.video_id).text,
+        )
+
+    def __str__(self):
+        return '{language_code} ("{language}"){translation_description}'.format(
+            language=self.language,
+            language_code=self.language_code,
+            translation_description='[TRANSLATABLE]' if self.is_translatable else ''
+        )
+
+    @property
+    def is_translatable(self):
+        return len(self.translation_languages) > 0
+
+    def translate(self, language_code):
+        if not self.is_translatable:
+            raise NotTranslatableError(self.video_id)
+
+        if language_code not in self._translation_languages_dict:
+            raise TranslationLanguageNotAvailableError(self.video_id)
+
+        return Transcript(
+            self._http_client,
+            self.video_id,
+            '{url}&tlang={language_code}'.format(url=self._url, language_code=language_code),
+            self._translation_languages_dict[language_code],
+            language_code,
+            True,
+            [],
+        )
+
+
+class _TranscriptParser(object):
+    _FORMATTING_TAGS = [
+        'strong',  # important
+        'em',  # emphasized
+        'b',  # bold
+        'i',  # italic
+        'mark',  # marked
+        'small',  # smaller
+        'del',  # deleted
+        'ins',  # inserted
+        'sub',  # subscript
+        'sup',  # superscript
+    ]
+
+    def __init__(self, preserve_formatting=False):
+        self._html_regex = self._get_html_regex(preserve_formatting)
+
+    def _get_html_regex(self, preserve_formatting):
+        if preserve_formatting:
+            formats_regex = '|'.join(self._FORMATTING_TAGS)
+            formats_regex = r'<\/?(?!\/?(' + formats_regex + r')\b).*?\b>'
+            html_regex = re.compile(formats_regex, re.IGNORECASE)
+        else:
+            html_regex = re.compile(r'<[^>]*>', re.IGNORECASE)
+        return html_regex
+
+    def parse(self, plain_data):
+        return [
+            {
+                'text': re.sub(self._html_regex, '', unescape(xml_element.text)),
+                'start': float(xml_element.attrib['start']),
+                'duration': float(xml_element.attrib.get('dur', '0.0')),
+            }
+            for xml_element in ElementTree.fromstring(plain_data)
+            if xml_element.text is not None
+        ]
+
+WATCH_URL = 'https://www.youtube.com/watch?v={video_id}'
+
+class transcriber(object):
+    @classmethod
+    def list_transcripts(cls, video_id, proxies=None, cookies=None):
+        with requests.Session() as http_client:
+            if cookies:
+                http_client.cookies = cls._load_cookies(cookies, video_id)
+            http_client.proxies = proxies if proxies else {}
+            return TranscriptListFetcher(http_client).fetch(video_id)
+
+    @classmethod
+    def get_transcripts(cls, video_ids, languages=('en',), continue_after_error=False, proxies=None,
+                        cookies=None, preserve_formatting=False):
+
+        assert isinstance(video_ids, list), "`video_ids` must be a list of strings"
+
+        data = {}
+        unretrievable_videos = []
+
+        for video_id in video_ids:
+            try:
+                data[video_id] = cls.get_transcript(video_id, languages, proxies, cookies, preserve_formatting)
+            except Exception as exception:
+                if not continue_after_error:
+                    raise exception
+
+                unretrievable_videos.append(video_id)
+
+        return data, unretrievable_videos
+
+    @classmethod
+    def get_transcript(cls, video_id, languages=('en',), proxies=None, cookies=None, preserve_formatting=False):
+        assert isinstance(video_id, str), "`video_id` must be a string"
+        return cls.list_transcripts(video_id, proxies, cookies).find_transcript(languages).fetch(preserve_formatting=preserve_formatting)
+
+    @classmethod
+    def _load_cookies(cls, cookies, video_id):
+        try:
+            cookie_jar = cookiejar.MozillaCookieJar()
+            cookie_jar.load(cookies)
+            if not cookie_jar:
+                raise CookiesInvalidError(video_id)
+            return cookie_jar
+        except:
             raise CookiePathInvalidError(video_id)
```

### Comparing `webscout-1.2.8/webscout/utils.py` & `webscout-1.2.9/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/webscout_search.py` & `webscout-1.2.9/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout/webscout_search_async.py` & `webscout-1.2.9/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.2.8/webscout.egg-info/PKG-INFO` & `webscout-1.2.9/webscout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.2.8
+Version: 1.2.9
 Summary: Search for words, documents, images, videos, news, maps and text translation using the Google, DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and now can transcribe yt videos
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -353,48 +353,46 @@
 Here is an example of initializing the AsyncWEBS class:
 ```python3
 import asyncio
 import logging
 import sys
 from itertools import chain
 from random import shuffle
-
 import requests
 from webscout import AsyncWEBS
 
-# bypass curl-cffi NotImplementedError in windows https://curl-cffi.readthedocs.io/en/latest/faq/
+# If you have proxies, define them here
+proxies = None
+
 if sys.platform.lower().startswith("win"):
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 def get_words():
     word_site = "https://www.mit.edu/~ecprice/wordlist.10000"
     resp = requests.get(word_site)
     words = resp.text.splitlines()
     return words
 
 async def aget_results(word):
     async with AsyncWEBS(proxies=proxies) as WEBS:
-        results = [r async for r in WEBS.text(word, max_results=None)]
+        results = await WEBS.text(word, max_results=None)
         return results
 
 async def main():
     words = get_words()
     shuffle(words)
-    tasks = []
-    for word in words[:10]:
-        tasks.append(aget_results(word))
+    tasks = [aget_results(word) for word in words[:10]]
     results = await asyncio.gather(*tasks)
     print(f"Done")
     for r in chain.from_iterable(results):
         print(r)
-    
 
-if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG)
-    asyncio.run(main())
+logging.basicConfig(level=logging.DEBUG)
+
+await main()
 ```
 It is important to note that the WEBS and AsyncWEBS classes should always be used as a context manager (with statement).
 This ensures proper resource management and cleanup, as the context manager will automatically handle opening and closing the HTTP client connection.
 
 ## Exceptions
 
 Exceptions:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.2.8 Summary: Search for words,
+Metadata-Version: 2.1 Name: webscout Version: 1.2.9 Summary: Search for words,
 documents, images, videos, news, maps and text translation using the Google,
 DuckDuckGo.com, yep.com, phind.com, you.com, etc Also containes AI models and
 now can transcribe yt videos Author: OEvortex Author-email:
 helpingai5@gmail.com License: HelpingAI Simplified Universal License Project-
 URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki Project-URL:
 Source, https://github.com/OE-LUCIFER/Webscout Project-URL: Tracker, https://
 github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube, https://
@@ -172,50 +172,48 @@
    To use the AsyncWEBS class, you can perform asynchronous operations using
  Python's asyncio library. To initialize an instance of the WEBS or AsyncWEBS
  classes, you can provide the following optional arguments: Here is an example
  of initializing the WEBS class: ```python3 from webscout import WEBS R = WEBS
 ().text("python programming", max_results=5) print(R) ``` Here is an example of
   initializing the AsyncWEBS class: ```python3 import asyncio import logging
    import sys from itertools import chain from random import shuffle import
-requests from webscout import AsyncWEBS # bypass curl-cffi NotImplementedError
-         in windows https://curl-cffi.readthedocs.io/en/latest/faq/ if
-     sys.platform.lower().startswith("win"): asyncio.set_event_loop_policy
-(asyncio.WindowsSelectorEventLoopPolicy()) def get_words(): word_site = "https:
- //www.mit.edu/~ecprice/wordlist.10000" resp = requests.get(word_site) words =
- resp.text.splitlines() return words async def aget_results(word): async with
-AsyncWEBS(proxies=proxies) as WEBS: results = [r async for r in WEBS.text(word,
-max_results=None)] return results async def main(): words = get_words() shuffle
-  (words) tasks = [] for word in words[:10]: tasks.append(aget_results(word))
-        results = await asyncio.gather(*tasks) print(f"Done") for r in
-       chain.from_iterable(results): print(r) if __name__ == "__main__":
-    logging.basicConfig(level=logging.DEBUG) asyncio.run(main()) ``` It is
-important to note that the WEBS and AsyncWEBS classes should always be used as
-a context manager (with statement). This ensures proper resource management and
- cleanup, as the context manager will automatically handle opening and closing
-  the HTTP client connection. ## Exceptions Exceptions: - `WebscoutE`: Raised
-when there is a generic exception during the API request. ## usage of webscout
-  ### 1. `text()` - text search by DuckDuckGo.com and Yep.com ```python from
-webscout import WEBS # Text search for 'live free or die' using DuckDuckGo.com
-    and Yep.com with WEBS() as WEBS: for r in WEBS.text('live free or die',
-region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) for
-     r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
-   timelimit='y', max_results=10): print(r) ``` ### 2. `answers()` - instant
-  answers by DuckDuckGo.com and Yep.com ```python from webscout import WEBS #
-Instant answers for the query "sun" using DuckDuckGo.com and Yep.com with WEBS
-  () as WEBS: for r in WEBS.answers("sun"): print(r) ``` ### 3. `images()` -
-image search by DuckDuckGo.com and Yep.com ```python from webscout import WEBS
-  # Image search for the keyword 'butterfly' using DuckDuckGo.com and Yep.com
-   with WEBS() as WEBS: keywords = 'butterfly' WEBS_images_gen = WEBS.images
-   ( keywords, region="wt-wt", safesearch="off", size=None, type_image=None,
- layout=None, license_image=None, max_results=10, ) for r in WEBS_images_gen:
-print(r) ``` ### 4. `videos()` - video search by DuckDuckGo.com ```python from
-       webscout import WEBS # Video search for the keyword 'tesla' using
-   DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla' WEBS_videos_gen =
-    WEBS.videos( keywords, region="wt-wt", safesearch="off", timelimit="w",
-       resolution="high", duration="medium", max_results=10, ) for r in
+requests from webscout import AsyncWEBS # If you have proxies, define them here
+           proxies = None if sys.platform.lower().startswith("win"):
+  asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy()) def
+ get_words(): word_site = "https://www.mit.edu/~ecprice/wordlist.10000" resp =
+ requests.get(word_site) words = resp.text.splitlines() return words async def
+ aget_results(word): async with AsyncWEBS(proxies=proxies) as WEBS: results =
+await WEBS.text(word, max_results=None) return results async def main(): words
+ = get_words() shuffle(words) tasks = [aget_results(word) for word in words[:
+      10]] results = await asyncio.gather(*tasks) print(f"Done") for r in
+chain.from_iterable(results): print(r) logging.basicConfig(level=logging.DEBUG)
+ await main() ``` It is important to note that the WEBS and AsyncWEBS classes
+   should always be used as a context manager (with statement). This ensures
+      proper resource management and cleanup, as the context manager will
+    automatically handle opening and closing the HTTP client connection. ##
+Exceptions Exceptions: - `WebscoutE`: Raised when there is a generic exception
+ during the API request. ## usage of webscout ### 1. `text()` - text search by
+ DuckDuckGo.com and Yep.com ```python from webscout import WEBS # Text search
+ for 'live free or die' using DuckDuckGo.com and Yep.com with WEBS() as WEBS:
+   for r in WEBS.text('live free or die', region='wt-wt', safesearch='off',
+timelimit='y', max_results=10): print(r) for r in WEBS.text('live free or die',
+region='wt-wt', safesearch='off', timelimit='y', max_results=10): print(r) ```
+ ### 2. `answers()` - instant answers by DuckDuckGo.com and Yep.com ```python
+     from webscout import WEBS # Instant answers for the query "sun" using
+ DuckDuckGo.com and Yep.com with WEBS() as WEBS: for r in WEBS.answers("sun"):
+  print(r) ``` ### 3. `images()` - image search by DuckDuckGo.com and Yep.com
+```python from webscout import WEBS # Image search for the keyword 'butterfly'
+ using DuckDuckGo.com and Yep.com with WEBS() as WEBS: keywords = 'butterfly'
+  WEBS_images_gen = WEBS.images( keywords, region="wt-wt", safesearch="off",
+size=None, type_image=None, layout=None, license_image=None, max_results=10, )
+  for r in WEBS_images_gen: print(r) ``` ### 4. `videos()` - video search by
+   DuckDuckGo.com ```python from webscout import WEBS # Video search for the
+ keyword 'tesla' using DuckDuckGo.com with WEBS() as WEBS: keywords = 'tesla'
+  WEBS_videos_gen = WEBS.videos( keywords, region="wt-wt", safesearch="off",
+timelimit="w", resolution="high", duration="medium", max_results=10, ) for r in
  WEBS_videos_gen: print(r) ``` ### 5. `news()` - news search by DuckDuckGo.com
  and yep.com ```python from webscout import WEBS # News search for the keyword
   'holiday' using DuckDuckGo.com and yep.com with WEBS() as WEBS: keywords =
         'holiday' WEBS_news_gen = WEBS.news( keywords, region="wt-wt",
 safesearch="off", timelimit="m", max_results=20 ) for r in WEBS_news_gen: print
    (r) ``` ### 6. `maps()` - map search by DuckDuckGo.com and ```python from
 webscout import WEBS # Map search for the keyword 'school' in 'anantnag' using
```

### Comparing `webscout-1.2.8/webscout.egg-info/SOURCES.txt` & `webscout-1.2.9/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

