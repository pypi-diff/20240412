# Comparing `tmp/chapter_sync-0.3.3.tar.gz` & `tmp/chapter_sync-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chapter_sync-0.3.3.tar", max compression
+gzip compressed data, was "chapter_sync-0.3.4.tar", max compression
```

## Comparing `chapter_sync-0.3.3.tar` & `chapter_sync-0.3.4.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0      185 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/LICENSE
--rw-r--r--   0        0        0     4725 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/README.md
--rw-r--r--   0        0        0     2328 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/__init__.py
--rw-r--r--   0        0        0       76 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/__main__.py
--rw-r--r--   0        0        0     3793 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/chapter.py
--rw-r--r--   0        0        0       73 2024-04-10 14:11:28.182999 chapter_sync-0.3.3/src/chapter_sync/cli/__init__.py
--rw-r--r--   0        0        0     5296 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/base.py
--rw-r--r--   0        0        0     1895 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/chapter.py
--rw-r--r--   0        0        0      659 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/db.py
--rw-r--r--   0        0        0     4303 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/series.py
--rw-r--r--   0        0        0     1808 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cli/subscriber.py
--rw-r--r--   0        0        0     1933 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/console.py
--rw-r--r--   0        0        0     2434 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/cover.py
--rw-r--r--   0        0        0     1923 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/db.py
--rw-r--r--   0        0        0     1531 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/email.py
--rw-r--r--   0        0        0    14814 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/epub.py
--rw-r--r--   0        0        0      276 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/__init__.py
--rw-r--r--   0        0        0     1908 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/base.py
--rw-r--r--   0        0        0     5821 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/custom.py
--rw-r--r--   0        0        0     3767 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/handlers/royal_road.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/__init__.py
--rw-r--r--   0        0        0      575 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/alembic.ini
--rw-r--r--   0        0        0     1396 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/env.py
--rw-r--r--   0        0        0      635 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/script.py.mako
--rw-r--r--   0        0        0     3886 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/migrations/versions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/py.typed
--rw-r--r--   0        0        0     3091 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/request.py
--rw-r--r--   0        0        0     5169 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/schema.py
--rw-r--r--   0        0        0     6131 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/series.py
--rw-r--r--   0        0        0     3160 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/subscriber.py
--rw-r--r--   0        0        0     4235 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/sync.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/templates/__init__.py
--rw-r--r--   0        0        0    14204 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/templates/base.css
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/__init__.py
--rw-r--r--   0        0        0      123 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/__main__.py
--rw-r--r--   0        0        0     2897 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/chapter.py
--rw-r--r--   0        0        0     2077 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/dependencies.py
--rw-r--r--   0        0        0      880 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/main.py
--rw-r--r--   0        0        0     1661 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/routes.py
--rw-r--r--   0        0        0     2467 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/series.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/__init__.py
--rw-r--r--   0        0        0     1033 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/app.css
--rw-r--r--   0        0        0     4286 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/favicon.ico
--rw-r--r--   0        0        0      392 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/icon.svg
--rw-r--r--   0        0        0       59 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/static/styles.css
--rw-r--r--   0        0        0     2999 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/subscriber.py
--rw-r--r--   0        0        0        0 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/__init__.py
--rw-r--r--   0        0        0      854 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/base.html
--rw-r--r--   0        0        0     2004 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/chapter.html
--rw-r--r--   0        0        0     2989 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/header.html
--rw-r--r--   0        0        0     3213 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/index.html
--rw-r--r--   0        0        0     1418 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/macros.html
--rw-r--r--   0        0        0      985 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/series.html
--rw-r--r--   0        0        0     1603 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/subscriber.html
--rw-r--r--   0        0        0     1252 2024-04-10 14:11:28.186999 chapter_sync-0.3.3/src/chapter_sync/web/templates/subscribers.html
--rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 chapter_sync-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      282 2024-04-12 13:43:52.211235 chapter_sync-0.3.4/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-12 13:43:52.211235 chapter_sync-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4725 2024-04-12 13:43:52.211235 chapter_sync-0.3.4/README.md
+-rw-r--r--   0        0        0     2328 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/__init__.py
+-rw-r--r--   0        0        0       76 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/__main__.py
+-rw-r--r--   0        0        0     3793 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/chapter.py
+-rw-r--r--   0        0        0       73 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/base.py
+-rw-r--r--   0        0        0     1895 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/chapter.py
+-rw-r--r--   0        0        0      659 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/db.py
+-rw-r--r--   0        0        0     4303 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/series.py
+-rw-r--r--   0        0        0     1808 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cli/subscriber.py
+-rw-r--r--   0        0        0     1933 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/console.py
+-rw-r--r--   0        0        0     2434 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/cover.py
+-rw-r--r--   0        0        0     1923 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/db.py
+-rw-r--r--   0        0        0     1531 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/email.py
+-rw-r--r--   0        0        0    14814 2024-04-12 13:43:52.215235 chapter_sync-0.3.4/src/chapter_sync/epub.py
+-rw-r--r--   0        0        0      276 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/handlers/__init__.py
+-rw-r--r--   0        0        0     1908 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/handlers/base.py
+-rw-r--r--   0        0        0     5821 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/handlers/custom.py
+-rw-r--r--   0        0        0     3767 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/handlers/royal_road.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/alembic.ini
+-rw-r--r--   0        0        0     1396 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/script.py.mako
+-rw-r--r--   0        0        0     3886 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/migrations/versions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/py.typed
+-rw-r--r--   0        0        0     3091 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/request.py
+-rw-r--r--   0        0        0     5169 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/schema.py
+-rw-r--r--   0        0        0     6131 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/series.py
+-rw-r--r--   0        0        0     3160 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/subscriber.py
+-rw-r--r--   0        0        0     4235 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/sync.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/templates/__init__.py
+-rw-r--r--   0        0        0    14204 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/templates/base.css
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/__init__.py
+-rw-r--r--   0        0        0     2897 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/chapter.py
+-rw-r--r--   0        0        0     2128 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/dependencies.py
+-rw-r--r--   0        0        0      926 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/main.py
+-rw-r--r--   0        0        0     1661 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/routes.py
+-rw-r--r--   0        0        0     2467 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/series.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/static/__init__.py
+-rw-r--r--   0        0        0     1033 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/static/app.css
+-rw-r--r--   0        0        0     4286 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/static/favicon.ico
+-rw-r--r--   0        0        0      392 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/static/icon.svg
+-rw-r--r--   0        0        0       59 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/static/styles.css
+-rw-r--r--   0        0        0     2999 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/subscriber.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/base.html
+-rw-r--r--   0        0        0     2004 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/chapter.html
+-rw-r--r--   0        0        0     2989 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/header.html
+-rw-r--r--   0        0        0     3213 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/index.html
+-rw-r--r--   0        0        0     1418 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/macros.html
+-rw-r--r--   0        0        0      985 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/series.html
+-rw-r--r--   0        0        0     1603 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/subscriber.html
+-rw-r--r--   0        0        0     1252 2024-04-12 13:43:52.219235 chapter_sync-0.3.4/src/chapter_sync/web/templates/subscribers.html
+-rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 chapter_sync-0.3.4/PKG-INFO
```

### Comparing `chapter_sync-0.3.3/LICENSE` & `chapter_sync-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/README.md` & `chapter_sync-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/pyproject.toml` & `chapter_sync-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chapter-sync"
-version = "0.3.3"
+version = "0.3.4"
 description = ""
 authors = [
     "Dan Cardin <ddcardin@gmail.com>",
 ]
 license = "Apache-2.0"
 repository = "https://github.com/dancardin/sqlalchemy-declarative-extensions"
 readme = 'README.md'
@@ -31,15 +31,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 alembic = ">=1.9.0"
 Pillow = "^9.0.0"
 beautifulsoup4 = "^4.9.3"
-cappa = ">=0.17.3"
+cappa = ">=0.18.1"
 html5lib = "^1.1"
 pendulum = ">=2"
 python-dotenv = "*"
 requests = "*"
 rich = "*"
 sqlalchemy = ">=2.0"
 xmltodict = "*"
```

### Comparing `chapter_sync-0.3.3/src/chapter_sync/chapter.py` & `chapter_sync-0.3.4/src/chapter_sync/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cli/base.py` & `chapter_sync-0.3.4/src/chapter_sync/cli/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         Subscriber | Series | Sync | Watch | Chapter | Db | Web | None
     ]
 
     database_name: Annotated[
         str,
         cappa.Arg(short=True, long=True, default=cappa.Env("DATABASE_NAME")),
         Doc("The name of the database file. Defaults to 'chapter_sync.sqlite'."),
-    ] = "chapter_sync.sqlite"
+    ] = "chapter-sync.sqlite"
     verbose: Annotated[
         int,
         cappa.Arg(short=True, long=True, action=cappa.ArgAction.count),
         Doc("Increase verbosity."),
     ] = 0
     tty: Annotated[bool | None, cappa.Arg(long="--tty/--no-tty")] = None
 
@@ -148,29 +148,27 @@
             "The number of times to perform a sync. Defaults to 0, which will sync until stopped."
         ),
     ] = 0
 
 
 @dataclass
 class Web:
-    host: Annotated[
-        str, cappa.Arg(short=True, long=True, default=cappa.Env("HOST"))
-    ] = "127.0.0.1"
+    host: Annotated[str, cappa.Arg(long=True, default=cappa.Env("HOST"))] = "127.0.0.1"
     port: Annotated[
         int, cappa.Arg(short=True, long=True, default=cappa.Env("PORT"))
     ] = 8000
     root_path: Annotated[str, cappa.Arg(long=True, default=cappa.Env("ROOT_PATH"))] = ""
 
-    def __call__(self):
+    def __call__(self, command: ChapterSync):
         import uvicorn
 
         from chapter_sync.web.main import create_app
 
         uvicorn.run(
-            create_app(),
+            create_app(command),
             host=self.host,
             port=self.port,
             root_path=self.root_path,
         )
 
 
 def run():
```

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cli/chapter.py` & `chapter_sync-0.3.4/src/chapter_sync/cli/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cli/db.py` & `chapter_sync-0.3.4/src/chapter_sync/cli/db.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cli/series.py` & `chapter_sync-0.3.4/src/chapter_sync/cli/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cli/subscriber.py` & `chapter_sync-0.3.4/src/chapter_sync/cli/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/console.py` & `chapter_sync-0.3.4/src/chapter_sync/console.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/cover.py` & `chapter_sync-0.3.4/src/chapter_sync/cover.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/db.py` & `chapter_sync-0.3.4/src/chapter_sync/db.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/email.py` & `chapter_sync-0.3.4/src/chapter_sync/email.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/epub.py` & `chapter_sync-0.3.4/src/chapter_sync/epub.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/handlers/base.py` & `chapter_sync-0.3.4/src/chapter_sync/handlers/base.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/handlers/custom.py` & `chapter_sync-0.3.4/src/chapter_sync/handlers/custom.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/handlers/royal_road.py` & `chapter_sync-0.3.4/src/chapter_sync/handlers/royal_road.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/migrations/alembic.ini` & `chapter_sync-0.3.4/src/chapter_sync/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/migrations/env.py` & `chapter_sync-0.3.4/src/chapter_sync/migrations/env.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/migrations/script.py.mako` & `chapter_sync-0.3.4/src/chapter_sync/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py` & `chapter_sync-0.3.4/src/chapter_sync/migrations/versions/63139caea00e_initial_tables.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/request.py` & `chapter_sync-0.3.4/src/chapter_sync/request.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/schema.py` & `chapter_sync-0.3.4/src/chapter_sync/schema.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/series.py` & `chapter_sync-0.3.4/src/chapter_sync/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/subscriber.py` & `chapter_sync-0.3.4/src/chapter_sync/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/sync.py` & `chapter_sync-0.3.4/src/chapter_sync/sync.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/templates/base.css` & `chapter_sync-0.3.4/src/chapter_sync/templates/base.css`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/chapter.py` & `chapter_sync-0.3.4/src/chapter_sync/web/chapter.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/dependencies.py` & `chapter_sync-0.3.4/src/chapter_sync/web/dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from functools import cache
 from typing import Annotated
 
 import pendulum
 from dataclass_settings import Env, load_settings
-from fastapi import Depends
+from fastapi import Depends, Request
 from fastapi.templating import Jinja2Templates
 from sqlalchemy.orm import Session
 
 from chapter_sync.cli import base
 from chapter_sync.console import Console
 from chapter_sync.email import EmailClient
 
@@ -22,16 +22,16 @@
 
 
 @cache
 def config():
     return load_settings(Config)
 
 
-def chapter_sync():
-    return base.ChapterSync(None)
+def chapter_sync(request: Request) -> base.ChapterSync:
+    return request.app.extra["command"]
 
 
 def database(
     chapter_sync: Annotated[base.ChapterSync, Depends(chapter_sync)],
     alembic_config=None,
 ) -> Generator[Session, None, None]:
     url = base.database_url(chapter_sync)
```

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/main.py` & `chapter_sync-0.3.4/src/chapter_sync/web/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import importlib.resources
 import logging
 
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 
-from chapter_sync.cli.base import alembic_config, database_url
-from chapter_sync.web.dependencies import chapter_sync, database
+from chapter_sync.cli.base import ChapterSync, alembic_config, database_url
+from chapter_sync.web.dependencies import database
 from chapter_sync.web.routes import routes
 
 
-def create_app(routes=routes):
+def create_app(command: ChapterSync, routes=routes):
     logging.basicConfig(level="INFO")
 
-    boostrap_db()
+    boostrap_db(command)
 
-    app = FastAPI()
+    app = FastAPI(command=command)
 
     static_dir = importlib.resources.files("chapter_sync.web.static")
     app.mount("/static", StaticFiles(directory=str(static_dir)), name="static")
 
     for route in routes:
         app.add_api_route(
             path=route["path"],
             endpoint=route["endpoint"],
             methods=[route["method"]],
         )
 
     return app
 
 
-def boostrap_db():
-    app = chapter_sync()
-    url = database_url(app)
+def boostrap_db(command: ChapterSync):
+    url = database_url(command)
     alembic = alembic_config(url)
-    list(database(app, alembic))
+    list(database(command, alembic))
```

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/routes.py` & `chapter_sync-0.3.4/src/chapter_sync/web/routes.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/series.py` & `chapter_sync-0.3.4/src/chapter_sync/web/series.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/static/app.css` & `chapter_sync-0.3.4/src/chapter_sync/web/static/app.css`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/static/favicon.ico` & `chapter_sync-0.3.4/src/chapter_sync/web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/subscriber.py` & `chapter_sync-0.3.4/src/chapter_sync/web/subscriber.py`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/base.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/chapter.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/chapter.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/header.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/header.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/index.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/macros.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/macros.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/series.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/series.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/subscriber.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/subscriber.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/src/chapter_sync/web/templates/subscribers.html` & `chapter_sync-0.3.4/src/chapter_sync/web/templates/subscribers.html`

 * *Files identical despite different names*

### Comparing `chapter_sync-0.3.3/PKG-INFO` & `chapter_sync-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chapter-sync
-Version: 0.3.3
+Version: 0.3.4
 Summary: 
 Home-page: https://github.com/dancardin/sqlalchemy-declarative-extensions
 License: Apache-2.0
 Keywords: chapter,sync,epub,ebook,leech
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: alembic (>=1.9.0)
 Requires-Dist: beautifulsoup4 (>=4.9.3,<5.0.0)
-Requires-Dist: cappa (>=0.17.3)
+Requires-Dist: cappa (>=0.18.1)
 Requires-Dist: dataclass-settings (>=0.2.3,<0.3.0)
 Requires-Dist: fastapi
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: jinja2
 Requires-Dist: pendulum (>=2)
 Requires-Dist: pydantic (>=2)
 Requires-Dist: python-dotenv
```

