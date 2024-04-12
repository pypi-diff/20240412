# Comparing `tmp/comic-parser-0.0.1.tar.gz` & `tmp/comic-parser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comic-parser-0.0.1.tar", last modified: Sat Mar 30 08:39:24 2024, max compression
+gzip compressed data, was "comic-parser-0.0.2.tar", last modified: Fri Apr 12 11:54:57 2024, max compression
```

## Comparing `comic-parser-0.0.1.tar` & `comic-parser-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 08:39:24.139571 comic-parser-0.0.1/
--rw-rw-rw-   0        0        0      400 2024-03-30 08:39:24.136580 comic-parser-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-30 08:39:04.000000 comic-parser-0.0.1/README.md
--rw-rw-rw-   0        0        0      509 2024-03-30 08:38:31.000000 comic-parser-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-30 08:39:24.139571 comic-parser-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-30 08:39:24.101672 comic-parser-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-30 08:39:24.108653 comic-parser-0.0.1/src/comic-parser/
--rw-rw-rw-   0        0        0      569 2024-03-30 08:38:08.000000 comic-parser-0.0.1/src/comic-parser/comic-parser.py
-drwxrwxrwx   0        0        0        0 2024-03-30 08:39:24.133587 comic-parser-0.0.1/src/comic_parser.egg-info/
--rw-rw-rw-   0        0        0      400 2024-03-30 08:39:24.000000 comic-parser-0.0.1/src/comic_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-03-30 08:39:24.000000 comic-parser-0.0.1/src/comic_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 08:39:24.000000 comic-parser-0.0.1/src/comic_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-30 08:39:24.000000 comic-parser-0.0.1/src/comic_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.856152 comic-parser-0.0.2/
+-rw-rw-rw-   0        0        0     1095 2024-04-08 12:22:08.000000 comic-parser-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1757 2024-04-12 11:54:57.854158 comic-parser-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-03-30 08:39:04.000000 comic-parser-0.0.2/README.md
+-rw-rw-rw-   0        0        0      735 2024-04-12 11:54:28.000000 comic-parser-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 11:54:57.856152 comic-parser-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.812222 comic-parser-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.823373 comic-parser-0.0.2/src/comicParser/
+-rw-rw-rw-   0        0        0      153 2024-04-12 11:20:55.000000 comic-parser-0.0.2/src/comicParser/__init__.py
+-rw-rw-rw-   0        0        0      784 2024-04-12 11:40:37.000000 comic-parser-0.0.2/src/comicParser/comicParser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:54:57.851959 comic-parser-0.0.2/src/comic_parser.egg-info/
+-rw-rw-rw-   0        0        0     1757 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-04-12 11:54:57.000000 comic-parser-0.0.2/src/comic_parser.egg-info/top_level.txt
```

### Comparing `comic-parser-0.0.1/src/comic-parser/comic-parser.py` & `comic-parser-0.0.2/src/comicParser/comicParser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import os
 import img2pdf
 from PIL import Image
 
-for pathRoot, subdirsRoot, filesRoot in os.walk('./'):
-    for dirNames in subdirsRoot:
-        imagenes = []
+# comic parser
+class ComicParser:
 
-        for path, subdirs, files in os.walk(dirNames):
-            for name in files:
-                if ".py" not in name and ".pdf" not in name and ".db" not in name:
-                    imagenes.append(os.path.join(path, name))
+    # init method or constructor
+    def __init__(self, parameters):
+        print (parameters)
+        for pathRoot, subdirsRoot, filesRoot in os.walk('./'):
+            for dirNames in subdirsRoot:
+                imagenes = []
 
-        imagenes.sort()
+                for path, subdirs, files in os.walk(dirNames):
+                    for name in files:
+                        if ".py" not in name and ".pdf" not in name and ".db" not in name:
+                            imagenes.append(os.path.join(path, name))
 
-        with open(os.path.basename(os.getcwd() + dirNames) + ".pdf", "wb") as manga:
-            manga.write(img2pdf.convert(imagenes))
+                imagenes.sort()
+
+                with open(os.path.basename(os.getcwd() + dirNames) + ".pdf", "wb") as manga:
+                    manga.write(img2pdf.convert(imagenes))
```

