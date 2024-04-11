# Comparing `tmp/arxiv_client-0.3.0.tar.gz` & `tmp/arxiv_client-0.3.1.tar.gz`

## Comparing `arxiv_client-0.3.0.tar` & `arxiv_client-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/__about__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/__init__.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/article.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/author.py
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/category.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/client.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/link.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/src/arxiv_client/query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/LICENSE
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/README.md
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 arxiv_client-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/__about__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/__init__.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/article.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/author.py
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/category.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/client.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/link.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/src/arxiv_client/query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/README.md
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 arxiv_client-0.3.1/PKG-INFO
```

### Comparing `arxiv_client-0.3.0/src/arxiv_client/article.py` & `arxiv_client-0.3.1/src/arxiv_client/article.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     The datetime that the retrieved version was submitted
     """
     _raw_entry: feedparser.FeedParserDict = field(repr=False)
     """
     The raw feedparser entry for the article, helpful for debugging
     """
 
-    _id_prefix_length = len("http://arxiv.org/abs/")
+    _id_prefix = "http://arxiv.org/abs/"
 
     def __init__(
         self,
         arxiv_id: str,
         title: str,
         categories: list[str],
         primary_category: Category | None,
@@ -148,22 +148,26 @@
         """
         Create an article from a feed entry
 
         :param entry: The feed entry
         :return: The article
         """
 
+        # The arXiv ID is provided correctly in RSS feeds
         # https://info.arxiv.org/help/api/user-manual.html#3321-title-id-published-and-updated
-        arxiv_id = entry.id[Article._id_prefix_length :]
+        arxiv_id = entry.id
+        if arxiv_id.startswith(Article._id_prefix):
+            arxiv_id = arxiv_id[len(Article._id_prefix) :]
         title = entry.title if hasattr(entry, "title") else "0"
+        primary_cat = entry.get("arxiv_primary_category", {}).get("term")
         return cls(
             arxiv_id=arxiv_id,
             title=title,
             categories=[tag["term"] for tag in entry.tags],
-            primary_category=Category(entry.get("arxiv_primary_category", {}).get("term")),
+            primary_category=Category(primary_cat) if primary_cat else None,
             authors=[Author.from_feed_author(author) for author in entry.authors],
             summary=entry.summary,
             comment=entry.get("arxiv_comment"),
             links=[Link.from_feed_link(link) for link in entry.links],
             journal_ref=entry.get("arxiv_journal_ref"),
             doi=entry.get("arxiv_doi"),
             published=datetime.fromisoformat(entry.published),
```

### Comparing `arxiv_client-0.3.0/src/arxiv_client/author.py` & `arxiv_client-0.3.1/src/arxiv_client/author.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/src/arxiv_client/category.py` & `arxiv_client-0.3.1/src/arxiv_client/category.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/src/arxiv_client/client.py` & `arxiv_client-0.3.1/src/arxiv_client/client.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/src/arxiv_client/link.py` & `arxiv_client-0.3.1/src/arxiv_client/link.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/src/arxiv_client/query.py` & `arxiv_client-0.3.1/src/arxiv_client/query.py`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/.gitignore` & `arxiv_client-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/LICENSE` & `arxiv_client-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/README.md` & `arxiv_client-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/pyproject.toml` & `arxiv_client-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arxiv_client-0.3.0/PKG-INFO` & `arxiv_client-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arxiv-client
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python3 client for the arXiv API
 Project-URL: Source, https://github.com/linjer/arxiv-client
 Author: Jerry Lin
 License: MIT License
         
         Copyright (c) 2024 Jerry Lin
```

