# Comparing `tmp/noveldown-1.2.1.tar.gz` & `tmp/noveldown-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noveldown-1.2.1.tar", max compression
+gzip compressed data, was "noveldown-1.2.2.tar", max compression
```

## Comparing `noveldown-1.2.1.tar` & `noveldown-1.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-04-28 17:42:16.623638 noveldown-1.2.1/LICENSE
--rw-r--r--   0        0        0     2099 2023-04-28 17:42:16.623638 noveldown-1.2.1/README.md
--rw-r--r--   0        0        0      317 2023-04-28 17:42:16.770638 noveldown-1.2.1/noveldown/__init__.py
--rw-r--r--   0        0        0     1798 2023-04-28 17:42:16.770638 noveldown-1.2.1/noveldown/api.py
--rw-r--r--   0        0        0     2646 2023-10-02 19:06:02.600027 noveldown-1.2.1/noveldown/cli.py
--rw-r--r--   0        0        0     1237 2023-04-28 17:42:16.771638 noveldown-1.2.1/noveldown/sources/__init__.py
--rw-r--r--   0        0        0     5895 2023-10-02 19:31:47.098610 noveldown-1.2.1/noveldown/sources/base_source.py
--rw-r--r--   0        0        0     2395 2023-04-28 17:42:16.771638 noveldown-1.2.1/noveldown/sources/source_pale.py
--rw-r--r--   0        0        0     2482 2023-04-28 17:42:16.771638 noveldown-1.2.1/noveldown/sources/source_practical_guide_to_evil.py
--rw-r--r--   0        0        0     2072 2023-10-02 19:23:26.383905 noveldown-1.2.1/noveldown/sources/source_wandering_inn.py
--rw-r--r--   0        0        0     4344 2023-10-02 19:32:30.819060 noveldown-1.2.1/noveldown/utils.py
--rw-r--r--   0        0        0      744 2023-10-02 19:37:22.599392 noveldown-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3058 1970-01-01 00:00:00.000000 noveldown-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-28 17:42:16.623638 noveldown-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2099 2023-04-28 17:42:16.623638 noveldown-1.2.2/README.md
+-rw-r--r--   0        0        0      182 2024-04-12 14:37:23.584643 noveldown-1.2.2/noveldown/__init__.py
+-rw-r--r--   0        0        0     1798 2023-04-28 17:42:16.770638 noveldown-1.2.2/noveldown/api.py
+-rw-r--r--   0        0        0     2646 2024-04-11 19:47:19.282019 noveldown-1.2.2/noveldown/cli.py
+-rw-r--r--   0        0        0     1237 2023-04-28 17:42:16.771638 noveldown-1.2.2/noveldown/sources/__init__.py
+-rw-r--r--   0        0        0     6213 2024-04-11 20:01:06.172623 noveldown-1.2.2/noveldown/sources/base_source.py
+-rw-r--r--   0        0        0     2395 2023-04-28 17:42:16.771638 noveldown-1.2.2/noveldown/sources/source_pale.py
+-rw-r--r--   0        0        0     2482 2023-04-28 17:42:16.771638 noveldown-1.2.2/noveldown/sources/source_practical_guide_to_evil.py
+-rw-r--r--   0        0        0     2072 2024-04-11 19:45:31.423375 noveldown-1.2.2/noveldown/sources/source_wandering_inn.py
+-rw-r--r--   0        0        0     4358 2024-04-11 19:35:47.009722 noveldown-1.2.2/noveldown/utils.py
+-rw-r--r--   0        0        0     1042 2024-04-12 14:36:26.543360 noveldown-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 noveldown-1.2.2/PKG-INFO
```

### Comparing `noveldown-1.2.1/LICENSE` & `noveldown-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/README.md` & `noveldown-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/api.py` & `noveldown-1.2.2/noveldown/api.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/cli.py` & `noveldown-1.2.2/noveldown/cli.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/sources/__init__.py` & `noveldown-1.2.2/noveldown/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/sources/base_source.py` & `noveldown-1.2.2/noveldown/sources/base_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,36 @@
         return self._chapter_getter(self, self.content_raw)
 
     async def get_raw_content(self, client: httpx.AsyncClient) -> str:
         """
         Fetch the raw page HTML and save it, returning the title.
         """
         # i love it when i spaghetti things for the sake of perf
-        res = await client.get(self.url)
 
         # exponential backoff
-        backoff = 0.1
-        while res.status_code == 429:
+        backoff = 0.5
+        while (res := await self.get_raw_content_or_null(client)) is None or res.status_code == 429:
             await asyncio.sleep(backoff)
-            res = await client.get(self.url)
             backoff *= 2
+
+            if backoff > 60:
+                res = requests_get(self.url)
+                break
         self.content_raw = res.text
 
         if not res.text.strip():
-            self.content_raw = requests.get(self.url, timeout=5).text
+            self.content_raw = requests_get(self.url).text
         return self.title
 
+    async def get_raw_content_or_null(self, client: httpx.AsyncClient) -> httpx.Response | None:
+        try:
+            return await client.get(self.url)
+        except Exception:
+            return None
+
 
 SectionedChapterList = list[tuple[str, list[Chapter]]]
 
 
 class BaseSource:
     """
     Override this class!
@@ -109,17 +117,15 @@
                 return flat_list
 
         # self.chapters is guaranteed to be a list, so
         # if the first check evaluates false it must be an empty list
         # which is the correct return type
         return self.chapters  # type: ignore
 
-    def set_chapter_range(
-        self, *, start: int | None = None, end: int | None = None
-    ) -> None:
+    def set_chapter_range(self, *, start: int | None = None, end: int | None = None) -> None:
         start = start or 0
         end = end or len(self.chapters_flattened)
         if self._chapter_urls and isinstance(self._chapter_urls[0], Chapter):
             self._chapter_urls = self._chapter_urls[start:end]
             return
 
         current_num = 0
@@ -141,18 +147,15 @@
         self._chapter_urls = new_chapter_urls
 
     def get_soup(self, url: str, content_raw: str | None = None) -> BeautifulSoup:
         if content_raw is not None:
             if content_raw.strip():
                 # if it is an empty page we go again
                 return BeautifulSoup(content_raw, "lxml")
-        return BeautifulSoup(requests.get(url, timeout=5).text, "lxml")
-
-    def get_text_from_url(self, url: str) -> str:
-        return requests.get(url, timeout=5).text
+        return BeautifulSoup(requests_get(url).text, "lxml")
 
     def __repr__(self) -> str:
         return (
             textwrap.dedent(
                 f"""
             {self.id}: {self.title} - {" ".join(self.authors)}
             url: {self.url}
@@ -185,7 +188,17 @@
         """
         Given a chapter URL, return clean HTML to be put
         directly into the EPUB.
 
         :param `content_raw`: parse an already-downloaded HTML file.
         """
         raise NotImplementedError
+
+
+def requests_get(url: str) -> requests.Response:
+    return requests.get(
+        url,
+        timeout=5,
+        headers={
+            "User-Agent": "",
+        },
+    )
```

### Comparing `noveldown-1.2.1/noveldown/sources/source_pale.py` & `noveldown-1.2.2/noveldown/sources/source_pale.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/sources/source_practical_guide_to_evil.py` & `noveldown-1.2.2/noveldown/sources/source_practical_guide_to_evil.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/sources/source_wandering_inn.py` & `noveldown-1.2.2/noveldown/sources/source_wandering_inn.py`

 * *Files identical despite different names*

### Comparing `noveldown-1.2.1/noveldown/utils.py` & `noveldown-1.2.2/noveldown/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import asyncio
 import imghdr
 import io
 from pathlib import Path
 from typing import AsyncIterator, Iterator, cast
 
 import httpx
-import requests
 from ebooklib import epub
 
-from .sources.base_source import BaseSource, Chapter, SectionedChapterList
+from .sources.base_source import BaseSource, Chapter, SectionedChapterList, requests_get
 
 STYLE_CSS = """
 body { background-color: #ffffff;
 text-align: justify;
 margin: 2%;
 adobe-hyphenate: none; }
 pre { font-size: x-small; }
@@ -35,33 +34,29 @@
 .smcap    {font-variant: small-caps;}
 .u        {text-decoration: underline;}
 .bold     {font-weight: bold;}
 .big { font-size: larger; }
 .small { font-size: smaller; }
 """
 
-MAX_DEFAULT_THREADS = 8
+MAX_DEFAULT_THREADS = 4
 
 
-async def magic(
-    source: BaseSource, threads: int = MAX_DEFAULT_THREADS
-) -> AsyncIterator[str]:
+async def magic(source: BaseSource, threads: int = MAX_DEFAULT_THREADS) -> AsyncIterator[str]:
     limits = httpx.Limits(
         max_connections=threads, max_keepalive_connections=threads, keepalive_expiry=5
     )
-    async with httpx.AsyncClient(limits=limits) as client:
+    async with httpx.AsyncClient(limits=limits, headers={"User-Agent": ""}) as client:
         functions = [chap.get_raw_content(client) for chap in source.chapters_flattened]
 
         for result in asyncio.as_completed(functions):
             yield await result
 
 
-def load_all_chapters(
-    source: BaseSource, threads: int = MAX_DEFAULT_THREADS
-) -> Iterator[str]:
+def load_all_chapters(source: BaseSource, threads: int = MAX_DEFAULT_THREADS) -> Iterator[str]:
     """
     Calls the property for each chapter to collect them all
     in memory asynchronously to be extra fast.
     """
     gen = magic(source, threads)
     loop = asyncio.get_event_loop()
     while True:
@@ -131,15 +126,15 @@
                 yield f"{sec_title} - {chap.title}"
 
     for i in chapter_htmls:
         book.add_item(i)
 
     book.spine = [*chapter_htmls]
     if source.cover_url:
-        image = requests.get(source.cover_url).content
+        image = requests_get(source.cover_url).content
         ext = imghdr.what(io.BytesIO(image))
         book.set_cover(f"cover.{ext}", image)
         book.spine.insert(0, "cover")
 
     book.add_item(epub.EpubNcx())
 
     dest_file = path / f"{source.title}.epub"
```

### Comparing `noveldown-1.2.1/PKG-INFO` & `noveldown-1.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: noveldown
-Version: 1.2.1
+Version: 1.2.2
 Summary: Webnovel downloader and EPUB converter
 Home-page: https://github.com/potatoeggy/noveldown
 License: LGPL-3.0-only
 Keywords: novel,epub,webnovel,download
-Author: Daniel Chen
-Author-email: danielchen04@hotmail.ca
+Author: potatoeggy
+Author-email: eggyrules@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: EbookLib (>=0.18.0,<0.19.0)
-Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: lxml (>=4.8.0,<5.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Documentation, https://github.com/potatoeggy/noveldown
 Project-URL: Repository, https://github.com/potatoeggy/noveldown
 Description-Content-Type: text/markdown
 
 # Noveldown
```

