# Comparing `tmp/pybpsapi-1.3.2.tar.gz` & `tmp/pybpsapi-1.3.3.tar.gz`

## Comparing `pybpsapi-1.3.2.tar` & `pybpsapi-1.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/CHANGELOG.MD
--rw-r--r--   0        0        0    10921 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/pybpsapi.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/LICENSE
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pybpsapi-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/CHANGELOG.MD
+-rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/pybpsapi.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/README.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 pybpsapi-1.3.3/PKG-INFO
```

### Comparing `pybpsapi-1.3.2/CHANGELOG.MD` & `pybpsapi-1.3.3/CHANGELOG.MD`

 * *Files 4% similar despite different names*

```diff
@@ -66,11 +66,16 @@
 - `CircularChecker` class now returns a sorted dict of new circulars
 
 # v1.3.1 - 23/6/2023
 
 ### Fixed
 - Changed the param name of /search to `query` from `title` to match API change
 
-# v1.3.2 - 24/7/23
+# v1.3.2 - 24/7/2023
 
 ### Fixed
-- Fixed dict key error in `CircularChecker` class.
+- Fixed dict key error in `CircularChecker` class.
+
+# v1.2.3 - 8/4/2024
+
+## Changed
+- The package now uses bpsapi.rajtech.me/latest/{category} instead of the params method for list and latest
```

### Comparing `pybpsapi-1.3.2/pybpsapi.py` & `pybpsapi-1.3.3/pybpsapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,72 @@
 import requests
 import pickle
 
 
 class API:
     """Methods which communicate with the API"""
 
-    def __init__(self, url="https://bpsapi.rajtech.me/v1/"):
+    def __init__(self, url="https://bpsapi.rajtech.me/"):
         self.url = url
 
         json = requests.get(self.url + "categories").json()
         if json['http_status'] == 200:
             self.categories = json['data']
         else:
             raise ConnectionError("Invalid API Response. API says there are no categories.")
 
     # /latest endpoint
-    def latest(self, category: str or int) -> dict or None:
+    def latest(self, category: str or int) -> dict | None:
         """The `/latest` endpoint returns the latest circular from a particular category"""
         if type(category) == int:
             category = int(category)
+
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
             if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
-        params = {'category': category}
-
-        request = requests.get(self.url + "latest", params=params)
+        request = requests.get(f"{self.url}latest/{category}")
         json = request.json()
+
         try:
             json['http_status']
         except KeyError:
             raise ConnectionError("Invalid API Response")
         if json['http_status'] == 200:
             return json['data']
 
     # /list endpoint
-    def list(self, category: str or int, amount: int = -1) -> list or None:
+    def list(self, category: str or int, amount: int = -1) -> list | None:
         """The `/list` endpoint returns a list of circulars from a particular category"""
         if type(category) == int:
             category = int(category)
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
             if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
         if amount < -1:
             amount = -1
 
-        params = {'category': category}
-
-        request = requests.get(self.url + "list", params=params)
+        request = requests.get(f"{self.url}list/{category}")
         json = request.json()
+
         try:
             json['http_status']
         except KeyError:
             raise ConnectionError("Invalid API Response")
         if json['http_status'] == 200:
             return json['data'] if amount == -1 else json['data'][:amount]
 
-    def search(self, query: str or int, amount: int = 1) -> dict or None:
+    def search(self, query: str or int, amount: int = 1) -> dict | None:
         """The `/search` endpoint lets you search for a circular by its name or ID"""
         if query.isdigit() and len(query) == 4:
             query = int(query)
         elif type(query) != str:
             raise ValueError("Invalid Query")
 
         params = {'query': query, 'amount': amount}
@@ -81,15 +80,15 @@
         except KeyError:
             raise ConnectionError("Invalid API Response")
 
         if json['http_status'] == 200:
             return json['data']
 
     # /getpng endpoint
-    def getpng(self, url: str) -> list or None:
+    def getpng(self, url: str) -> list | None:
         """The `/getpng` endpoint lets you get the pngs from a circular"""
         if type(url) != str:
             raise ValueError("Invalid URL")
 
         params = {'url': url}
 
         request = requests.get(self.url + "getpng", params=params)
@@ -102,21 +101,22 @@
             raise ConnectionError("Invalid API Response")
 
         if json['http_status'] == 200:
             return json['data']
 
 
 class CircularChecker:
-    def __init__(self, category, url: str = "https://bpsapi.rajtech.me/v1/", cache_method=None, debug: bool = False,
+    def __init__(self, category, url: str = "https://bpsapi.rajtech.me/", cache_method=None, debug: bool = False,
                  **kwargs):
         self.url = url
         self.category = category
         self._cache = []
 
         json = requests.get(self.url + "categories").json()
+
         if json['http_status'] == 200:
             self.categories = json['data']
         else:
             raise ConnectionError("Invalid API Response. API says there are no categories.")
 
         if debug:
             self.set_cache = self._set_cache
@@ -127,15 +127,14 @@
             if not 1 < category < 100:
                 raise ValueError("Invalid category Number")
 
         else:
             if category not in self.categories:
                 raise ValueError("Invalid category Name")
 
-        self._params = {'category': category}
         self.cache_method = cache_method
 
         if cache_method is not None:
             if cache_method == "database":
                 try:
                     self.db_name = kwargs['db_name']
                     self.db_path = kwargs['db_path']
@@ -213,33 +212,36 @@
             with open(self.pickle_path + f"/{self.pickle_name}.pickle", "wb") as f:
                 pickle.dump(data, f)
 
         else:
             self._cache = data
 
     def _refresh_cache(self):
-        request = requests.get(self.url + "list", params=self._params)
+        request = requests.get(f"{self.url}list/{self.category}")
         json = request.json()
+
         try:
             json['http_status']
         except KeyError:
             raise ValueError("Invalid API Response")
+
         if json['http_status'] == 200:
             self._set_cache(json['data'])
 
-    def check(self) -> list[dict] or list[None]:
+    def check(self) -> list[dict] | list[None]:
         return_dict = []
         old_cached = self.get_cache()
 
         if not old_cached:
             self._refresh_cache()
             return []
 
         self._cur.execute(f"SELECT * FROM {self.db_table} WHERE category = ?", (self.category,))
         res = self._cur.fetchone()
+
         if res is None:
             cache = []
         else:
             cache = pickle.loads(res[2])
 
         self._refresh_cache()
         final_dict = self.get_cache()
@@ -282,20 +284,20 @@
     def add(self, checker: CircularChecker, *args: CircularChecker):
         self._checkers.append(checker)
         for arg in args:
             if type(arg) != CircularChecker:
                 raise ValueError("Invalid CircularChecker Object")
             self._checkers.append(arg)
 
-    def create(self, category, url: str = "https://bpsapi.rajtech.me/v1/", cache_method=None, debug: bool = False,
+    def create(self, category, url: str = "https://bpsapi.rajtech.me/", cache_method=None, debug: bool = False,
                **kwargs):
         checker = CircularChecker(category, url, cache_method, debug, **kwargs)
         self._checkers.append(checker)
 
-    def check(self) -> dict[list[dict] or list[None]]:
+    def check(self) -> dict[list[dict]]:
         return_dict = {}
         for checker in self._checkers:
             return_dict[checker.category] = checker.check()
         return return_dict
 
     def refresh_cache(self):
         for checker in self._checkers:
```

### Comparing `pybpsapi-1.3.2/.github/workflows/python-publish.yml` & `pybpsapi-1.3.3/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   release:
     types: [published]
 
 permissions:
   contents: read
 
 jobs:
-  deploy:
+  publish:
 
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
```

### Comparing `pybpsapi-1.3.2/LICENSE` & `pybpsapi-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.3.2/README.md` & `pybpsapi-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.3.2/pyproject.toml` & `pybpsapi-1.3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pybpsapi"
-version = "1.3.2"
+version = "1.3.3"
 description = "This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system."
 author = "Raj Dave"
 author-email = "rajdave8002@gmail.com"
 homepage = "https://bpsapi.rajtech.me/"
 license = "MIT"
 keywords = ["bpsapi", "bps", "api", "wrapper", "python", "python3"]
 requires-python = ">=3.6"
```

### Comparing `pybpsapi-1.3.2/PKG-INFO` & `pybpsapi-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pybpsapi
-Version: 1.3.2
+Version: 1.3.3
 Summary: This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system.
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,bps,bpsapi,python,python3,wrapper
 Requires-Python: >=3.6
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```

