# Comparing `tmp/paramount-0.3.4.tar.gz` & `tmp/paramount-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramount-0.3.4.tar", last modified: Mon Apr  8 09:54:28 2024, max compression
+gzip compressed data, was "paramount-0.3.5.tar", last modified: Thu Apr 11 22:49:48 2024, max compression
```

## Comparing `paramount-0.3.4.tar` & `paramount-0.3.5.tar`

### file list

```diff
@@ -1,40 +1,38 @@
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.930074 paramount-0.3.4/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)    35446 2024-03-28 16:22:26.000000 paramount-0.3.4/LICENSE
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       41 2024-03-28 16:22:26.000000 paramount-0.3.4/MANIFEST.in
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     4467 2024-04-08 09:54:28.929852 paramount-0.3.4/PKG-INFO
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     3884 2024-03-28 16:22:26.000000 paramount-0.3.4/README.md
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.922721 paramount-0.3.4/paramount/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       42 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/__init__.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.923949 paramount-0.3.4/paramount/client/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/client/__init__.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.924480 paramount-0.3.4/paramount/client/dist/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 18:50:40.000000 paramount-0.3.4/paramount/client/dist/__init__.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.926014 paramount-0.3.4/paramount/client/dist/assets/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 18:50:40.000000 paramount-0.3.4/paramount/client/dist/assets/__init__.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)   310507 2024-04-08 09:53:28.000000 paramount-0.3.4/paramount/client/dist/assets/index-BJ6RFJE2.css
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)  1695166 2024-04-08 09:53:28.000000 paramount-0.3.4/paramount/client/dist/assets/index-C-vbeAtz.js
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)      461 2024-04-08 09:53:28.000000 paramount-0.3.4/paramount/client/dist/index.html
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1497 2024-03-28 18:50:40.000000 paramount-0.3.4/paramount/client/dist/vite.svg
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.928813 paramount-0.3.4/paramount/server/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/__init__.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)    12054 2024-04-08 09:53:28.000000 paramount-0.3.4/paramount/server/api.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1338 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/cli.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.929456 paramount-0.3.4/paramount/server/db_connector/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/db_connector/__init__.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1203 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/db_connector/csv.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1376 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/db_connector/db.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     8297 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/db_connector/postgres.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     2351 2024-03-28 19:37:48.000000 paramount-0.3.4/paramount/server/library_functions.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.929604 paramount-0.3.4/paramount/server/pages/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/pages/__init__.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     6619 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/record.py
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       79 2024-03-28 16:22:26.000000 paramount-0.3.4/paramount/server/wsgi.py
-drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-08 09:54:28.923799 paramount-0.3.4/paramount.egg-info/
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)     4467 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/PKG-INFO
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)      882 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/SOURCES.txt
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)        1 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/dependency_links.txt
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       56 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/entry_points.txt
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       95 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/requires.txt
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       10 2024-04-08 09:54:28.000000 paramount-0.3.4/paramount.egg-info/top_level.txt
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)       38 2024-04-08 09:54:28.930117 paramount-0.3.4/setup.cfg
--rw-r--r--   0 hakimkhalafi   (501) staff       (20)      955 2024-04-08 09:53:28.000000 paramount-0.3.4/setup.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.831182 paramount-0.3.5/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)    35446 2024-03-28 16:22:26.000000 paramount-0.3.5/LICENSE
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       41 2024-03-28 16:22:26.000000 paramount-0.3.5/MANIFEST.in
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     3232 2024-04-11 22:49:48.830984 paramount-0.3.5/PKG-INFO
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     2648 2024-04-11 21:10:59.000000 paramount-0.3.5/README.md
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.826570 paramount-0.3.5/paramount/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       42 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/__init__.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.827475 paramount-0.3.5/paramount/client/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/client/__init__.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.827834 paramount-0.3.5/paramount/client/dist/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:33:43.000000 paramount-0.3.5/paramount/client/dist/__init__.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.828338 paramount-0.3.5/paramount/client/dist/assets/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:33:43.000000 paramount-0.3.5/paramount/client/dist/assets/__init__.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)   310507 2024-04-11 22:33:43.000000 paramount-0.3.5/paramount/client/dist/assets/index-BJ6RFJE2.css
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)  1695236 2024-04-11 22:33:43.000000 paramount-0.3.5/paramount/client/dist/assets/index-xv9gWSXP.js
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)      461 2024-04-11 22:33:43.000000 paramount-0.3.5/paramount/client/dist/index.html
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1497 2024-04-11 22:33:42.000000 paramount-0.3.5/paramount/client/dist/vite.svg
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.829968 paramount-0.3.5/paramount/server/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/server/__init__.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)    12054 2024-04-11 21:57:36.000000 paramount-0.3.5/paramount/server/api.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1338 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/server/cli.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.830689 paramount-0.3.5/paramount/server/db_connector/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        0 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/server/db_connector/__init__.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1955 2024-04-11 22:43:12.000000 paramount-0.3.5/paramount/server/db_connector/csv.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     1414 2024-04-11 22:47:36.000000 paramount-0.3.5/paramount/server/db_connector/db.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     8297 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/server/db_connector/postgres.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     2432 2024-04-11 21:58:04.000000 paramount-0.3.5/paramount/server/library_functions.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     7430 2024-04-11 22:48:08.000000 paramount-0.3.5/paramount/server/record.py
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       79 2024-03-28 16:22:26.000000 paramount-0.3.5/paramount/server/wsgi.py
+drwxr-xr-x   0 hakimkhalafi   (501) staff       (20)        0 2024-04-11 22:49:48.827340 paramount-0.3.5/paramount.egg-info/
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)     3232 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/PKG-INFO
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)      847 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/SOURCES.txt
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)        1 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/dependency_links.txt
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       56 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/entry_points.txt
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       95 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/requires.txt
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       10 2024-04-11 22:49:48.000000 paramount-0.3.5/paramount.egg-info/top_level.txt
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)       38 2024-04-11 22:49:48.831226 paramount-0.3.5/setup.cfg
+-rw-r--r--   0 hakimkhalafi   (501) staff       (20)      955 2024-04-11 22:45:28.000000 paramount-0.3.5/setup.py
```

### Comparing `paramount-0.3.4/LICENSE` & `paramount-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/client/dist/assets/index-BJ6RFJE2.css` & `paramount-0.3.5/paramount/client/dist/assets/index-BJ6RFJE2.css`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/client/dist/assets/index-C-vbeAtz.js` & `paramount-0.3.5/paramount/client/dist/assets/index-xv9gWSXP.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -55940,86 +55940,86 @@
     const o = n.chat_list,
         i = n.chat_list_role_param,
         s = n.chat_list_content_param,
         a = {},
         l = n.chat_list_references_list,
         u = n.chat_list_references_titles,
         c = n.chat_list_references_urls;
-    if (!(!t || !t[e])) return t[e][l].forEach(d => {
+    if (!(!t || !t[e])) return (p = t[e][l]) == null || p.forEach(d => {
         a[d[c]] || (a[d[c]] = d)
     }), x.jsxs("div", {
         className: "py-6",
         children: [x.jsx("div", {
             className: "flex justify-between items-center mb-4",
             children: x.jsx("h1", {
                 className: "text-base font-semibold",
                 children: "Reviewing one by one"
             })
-        }), o ? x.jsxs(x.Fragment, {
+        }), !o || !i || !s ? x.jsx("p", {
+            className: "text-center font-semibold mt-8 mb-4",
+            children: "Please set your chat_list and related config settings in paramount.toml to display chat view."
+        }) : x.jsxs(x.Fragment, {
             children: [x.jsx("div", {
                 className: "overflow-y-scroll max-h-[400px] p-4 border-2 rounded-xl shadow-md border-sky-600",
-                children: t[e][o] && ((p = t[e][o]) == null ? void 0 : p.slice(1).map((d, f) => x.jsx("div", {
+                children: Array.isArray(t[e][o]) ? t[e][o].slice(1).map((d, f) => x.jsx("div", {
                     className: "py-4 px-2 border-b-[1px] border-neutral-200",
                     children: x.jsxs("div", {
                         className: "flex flex-col",
                         children: [x.jsx("h2", {
-                            className: `text-base font-semibold mb-2
-                    ${d[i]==="user"?"text-sky-500":"text-orange-500"}`,
+                            className: `text-base font-semibold mb-2 ${d[i]==="user"?"text-sky-500":"text-orange-500"}`,
                             children: d[i]
                         }), x.jsx("p", {
                             children: d[s]
                         }), x.jsx("div", {
                             className: "flex flex-wrap items-center mt-4",
-                            children: t[e][o].length - 2 === f && Object.values(a).map((h, g) => x.jsx("a", {
+                            children: t[e][o].length - 2 === f && c && Object.values(a).map((h, g) => x.jsx("a", {
                                 href: h[c],
                                 target: "_blank",
-                                className: `m-1 px-4 py-2 bg-sky-500 text-white rounded-lg hover:text-white
-                                  w-fit text-ellipsis whitespace-nowrap overflow-hidden max-w-[250px]`,
+                                rel: "noopener noreferrer",
+                                className: "m-1 px-4 py-2 bg-sky-500 text-white rounded-lg hover:text-white w-fit text-ellipsis whitespace-nowrap overflow-hidden max-w-[250px]",
                                 children: h[u] || h[c]
                             }, g))
                         })]
                     })
-                }, f)))
+                }, f)) : x.jsx("p", {
+                    className: "text-center font-semibold mt-8 mb-4",
+                    children: "No chat data available."
+                })
             }), t[e][o] && x.jsxs("div", {
                 className: "p-4 flex justify-center items-center space-x-4 my-4",
                 children: [x.jsxs("button", {
                     type: "button",
-                    className: `py-2 px-4 text-white bg-green-500 focus:outline-0 rounded-lg
-              flex items-center hover:bg-green-600 shadow-md`,
+                    className: "py-2 px-4 text-white bg-green-500 focus:outline-0 rounded-lg flex items-center hover:bg-green-600 shadow-md",
                     style: {
                         transition: ".2s ease-in-out 0s"
                     },
                     onClick: () => r("accept"),
                     children: [x.jsx("div", {
                         className: "h-5 w-5 mr-2",
                         children: x.jsx(t2, {})
                     }), x.jsx("span", {
                         className: "font-semibold",
                         children: "Accept"
                     })]
                 }), x.jsxs("button", {
                     type: "button",
-                    className: `py-2 px-4 text-white bg-rose-500 focus:outline-0 rounded-lg
-              flex items-center hover:bg-rose-600 shadow-md`,
+                    className: "py-2 px-4 text-white bg-rose-500 focus:outline-0 rounded-lg flex items-center hover:bg-rose-600 shadow-md",
                     style: {
                         transition: ".2s ease-in-out 0s"
                     },
                     onClick: () => r("reject"),
                     children: [x.jsx("div", {
                         className: "h-5 w-5 mr-2",
                         children: x.jsx(aw, {})
                     }), x.jsx("span", {
                         className: "font-semibold",
                         children: "Reject"
                     })]
                 })]
             })]
-        }) : x.jsx("p", {
-            className: "text-center font-semibold mt-8 mb-4",
-            children: "Please set your chat_list config settings in paramount.toml to display chat view"
         })]
     })
 }
 
 function n2({
     open: n,
     setOpen: t,
```

### Comparing `paramount-0.3.4/paramount/client/dist/vite.svg` & `paramount-0.3.5/paramount/client/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/server/api.py` & `paramount-0.3.5/paramount/server/api.py`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/server/cli.py` & `paramount-0.3.5/paramount/server/cli.py`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/server/db_connector/db.py` & `paramount-0.3.5/paramount/server/db_connector/db.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         pass
 
     @abstractmethod
     def update_ground_truth(self, df, table_name):
         pass
 
     @abstractmethod
-    def get_recordings(self, table_name, evaluated_rows_only, split_by_id, identifier_column_name, identifier_value):
+    def get_recordings(self, table_name, evaluated_rows_only, split_by_id, identifier_column_name, identifier_value,
+                       recording_ids):
         pass
 
     @abstractmethod
     def get_sessions(self, table_name, split_by_id, identifier_column_name, identifier_value):
         pass
```

### Comparing `paramount-0.3.4/paramount/server/db_connector/postgres.py` & `paramount-0.3.5/paramount/server/db_connector/postgres.py`

 * *Files identical despite different names*

### Comparing `paramount-0.3.4/paramount/server/library_functions.py` & `paramount-0.3.5/paramount/server/library_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     return toml.load(config_path)
 
 
 def default_config():
     default = {
         "record": {
             "enabled": True,
+            "fire_and_forget": False,
+            "replay_enabled": True,
             "function_url": "http://localhost:9000"
         },
         "db": {
             "type": "csv",
             "postgres": {
                 "connection_string": ""
             }
@@ -31,17 +33,17 @@
         "api": {
             "endpoint": "http://localhost",
             "port": 9001,
             "split_by_id": False,
             "identifier_colname": ""
         },
         "ui": {
-            "meta_cols": [''],
-            "input_cols": [''],
-            "output_cols": ['']
+            "meta_cols": ['recorded_at'],
+            "input_cols": [],
+            "output_cols": []
         }
     }
     return default
 
 
 def get_result_from_colname(result, output_col):
     '''
```

### Comparing `paramount-0.3.4/paramount/server/record.py` & `paramount-0.3.5/paramount/server/record.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,54 +42,58 @@
         return tuple(serialize_item(item) for item in response)  # Handle each tuple item.
     elif callable(response):  # Check if it is a generator function, eg. LLM streaming is on (with SSE)
         return False
     else:
         return serialize_item(response)
 
 
-def record(flask_app):
+def record(flask_app=None):
     config = load_config()
 
     db_type = config['db']['type']
 
     connection_string = ""
     if db_type in config['db']:
         db_config = config['db'].get(db_type)
         if db_config and 'connection_string' in db_config:
             connection_string = db_config['connection_string']
 
     db_instance = db.get_database(db_type, connection_string)
 
     is_live = config['record']['enabled']
-    print(f"Paramount enabled: {is_live}")
+    fire_and_forget = config['record'].get('fire_and_forget', True)
+    replay_enabled = config['record'].get('replay_enabled', True)
+    print(f"Paramount enabled: {is_live}. Fire and forget mode: {fire_and_forget}. Replay enabled: {replay_enabled}")
+    print(f"Flask app available: {flask_app is not None}")
 
     def decorator(func):
         endpoint = f'/paramount_functions/{func.__name__}'
 
         # Define the Flask view function.
-        @flask_app.route(endpoint, methods=['POST'])  # TODO: Password protect endpoint by default (+2FA?)
-        def view_func():
-            # Here we grab the JSON data from the request
-            data = request.json
-
-            # In the end separate handling of args/kwargs was not necessary
-            # Here we use kwargs syntax for all vars (in order to not pass unnamed vars)
-            func_kwargs = data.get('args', {})
-            additional_kwargs = data.get('kwargs', {})
-            func_kwargs.update(additional_kwargs)
-
-            # Call the actual function with the provided keyword arguments.
-            result = func(**func_kwargs)
-
-            # Serialize the result and return as JSON
-            serialized_result = serialize_response(result)
-            if serialized_result:
-                return jsonify(serialized_result)
-            else:
-                return jsonify({'Error': 'Streaming/SSE unsupported'}), 501  # SSE / streaming unsupported
+        if flask_app and replay_enabled:
+            @flask_app.route(endpoint, methods=['POST'])  # TODO: Password protect endpoint by default (+2FA?)
+            def view_func():
+                # Here we grab the JSON data from the request
+                data = request.json
+
+                # In the end separate handling of args/kwargs was not necessary
+                # Here we use kwargs syntax for all vars (in order to not pass unnamed vars)
+                func_kwargs = data.get('args', {})
+                additional_kwargs = data.get('kwargs', {})
+                func_kwargs.update(additional_kwargs)
+
+                # Call the actual function with the provided keyword arguments.
+                result = func(**func_kwargs)
+
+                # Serialize the result and return as JSON
+                serialized_result = serialize_response(result)
+                if serialized_result:
+                    return jsonify(serialized_result)
+                else:
+                    return jsonify({'Error': 'Streaming/SSE unsupported'}), 501  # SSE / streaming unsupported
 
         def wrapper(*args, **kwargs):
             if not is_live:
                 return func(*args, **kwargs)
             else:
                 try:
                     func_params = inspect.signature(func).parameters
@@ -129,27 +133,32 @@
                         'paramount__evaluation': "",
                         'paramount__recording_id': str(uuid.uuid4()),
                         'paramount__recorded_at': timestamp_now,
                         'paramount__evaluated_at': timestamp_now,
                         'paramount__function_name': func.__name__,
                         'paramount__execution_time': end_time - start_time,
                         **{f'input_{k}': v for k, v in args_dict.items()}}  # prefix for column name: to differentiate
+                    if not hasattr(serialized_result, '__iter__') or isinstance(serialized_result,
+                                                                                (str, bytes, bytearray, memoryview)):
+                        # In order to not iterate over strings, bytes, or other uniterable objects.
+                        serialized_result = [serialized_result]
                     for i, output in enumerate(serialized_result, start=1):
                         if isinstance(output, dict):
                             for key, value in output.items():
                                 result_data[f'output__{i}_{key}'] = value
                         else:
                             result_data[f'output__{i}'] = output
                     df = pd.DataFrame([result_data])
                     df['paramount__recorded_at'] = pd.to_datetime(df['paramount__recorded_at'])
                     df['paramount__evaluated_at'] = pd.to_datetime(df['paramount__evaluated_at'])
 
                     # Fire and forget for this heavy operation
                     threading.Thread(target=db_instance.create_or_append,
-                                     args=(df, 'paramount_data', 'paramount__recording_id'), daemon=True).start()
+                                     args=(df, 'paramount_data', 'paramount__recording_id'),
+                                     daemon=fire_and_forget).start()
 
                 except Exception as e:
                     err_tcb = traceback.format_exc()
                     print(f"PARAMOUNT: Wrapper logic issue: {e}: {err_tcb}")
 
                 return result
```

### Comparing `paramount-0.3.4/setup.py` & `paramount-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
    name='paramount',
-   version='0.3.4',
+   version='0.3.5',
    description='Business Evals for LLMs',
    long_description=long_description,
    long_description_content_type='text/markdown',
    entry_points={
        'console_scripts': ['paramount=paramount.server.cli:main'],
    },
    author='Hakim K',
```

