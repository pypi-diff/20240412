# Comparing `tmp/walkmate-1.2.2.tar.gz` & `tmp/walkmate-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walkmate-1.2.2.tar", last modified: Thu Jul 30 16:47:45 2020, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `walkmate-1.2.2.tar` & `walkmate-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/
--rw-r--r--   0 joel       (501) staff       (20)     4704 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)      240 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/SOURCES.txt
--rw-r--r--   0 joel       (501) staff       (20)      238 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/requires.txt
--rw-r--r--   0 joel       (501) staff       (20)        9 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/top_level.txt
--rw-r--r--   0 joel       (501) staff       (20)        1 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate.egg-info/dependency_links.txt
--rw-r--r--   0 joel       (501) staff       (20)     4704 2020-07-30 16:47:45.000000 walkmate-1.2.2/PKG-INFO
--rw-r--r--   0 joel       (501) staff       (20)     1071 2020-07-30 16:15:15.000000 walkmate-1.2.2/LICENSE.md
-drwxr-xr-x   0 joel       (501) staff       (20)        0 2020-07-30 16:47:45.000000 walkmate-1.2.2/walkmate/
--rw-r--r--   0 joel       (501) staff       (20)       56 2020-07-30 16:42:32.000000 walkmate-1.2.2/walkmate/__init__.py
--rw-r--r--   0 joel       (501) staff       (20)     1805 2020-07-30 16:42:14.000000 walkmate-1.2.2/walkmate/__main__.py
--rw-r--r--   0 joel       (501) staff       (20)     3169 2020-07-30 16:15:15.000000 walkmate-1.2.2/README.md
--rw-r--r--   0 joel       (501) staff       (20)      733 2020-07-30 16:15:15.000000 walkmate-1.2.2/setup.py
--rw-r--r--   0 joel       (501) staff       (20)     1069 2020-07-30 16:47:45.000000 walkmate-1.2.2/setup.cfg
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 walkmate-1.3.1/src/__init__.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 walkmate-1.3.1/src/files.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 walkmate-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 walkmate-1.3.1/LICENSE.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 walkmate-1.3.1/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 walkmate-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 walkmate-1.3.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `walkmate-1.2.2/LICENSE.md` & `walkmate-1.3.1/LICENSE.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-MIT License
+# MIT License
 
-Copyright (c) 2020 Joel Lefkowitz
+Copyright (c) 2024 Joel Lefkowitz
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

