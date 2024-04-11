# Comparing `tmp/pypi_tdb-0.0.5.tar.gz` & `tmp/pypi_tdb-0.0.6.tar.gz`

## Comparing `pypi_tdb-0.0.5.tar` & `pypi_tdb-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/__init__.py
--rw-r--r--   0        0        0     7865 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/__main__.py
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/addon.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/cli.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/config.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/db.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/html.js
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/html.py
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/rake.py
--rw-r--r--   0        0        0    13580 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/records.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/server.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/session.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/style.css
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/tdb/tags.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/LICENSE
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/readme.md
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pypi_tdb-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/__init__.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/__main__.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/addon.py
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/cli.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/config.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/db.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/html.js
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/html.py
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/rake.py
+-rw-r--r--   0        0        0    14417 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/records.py
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/server.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/session.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/style.css
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/tdb/tags.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/LICENSE
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/readme.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pypi_tdb-0.0.6/PKG-INFO
```

### Comparing `pypi_tdb-0.0.5/tdb/__main__.py` & `pypi_tdb-0.0.6/tdb/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,20 @@
             elif printout:
                 print("failed to add '"+str(e)+"'. missing expected interface 'get_addon_name'.")
 
 
 def main():
     if len(sys.argv) < 2 or "--help" in sys.argv or sys.argv[1] == "help":
         print("# tdb\n\nA text based database with tagging.\n\n```")
-        print("Usage: py -m tdb [add | edit | remove | template | show | open | listen] [text | options]")
+        print("Usage: py -m tdb [add | edit | rm | template | show | open | listen] [text | options]")
         print("".ljust(64,"-"))
         print("Commands:")
         print("add:".ljust(16)+"Make a record when text is supplied. Otherwise, open an editor to write one.")
         print("edit:".ljust(16)+"Open an editor with some view of the database, see options.")
-        print("remove:".ljust(16)+"Move matching records to the archive.")
+        print("rm:".ljust(16)+"Move matching records to the archive.")
         print("template:".ljust(16)+"Open an editor to write a record with the passed template file as a basis.")
         print("open:".ljust(16)+"Open tdbs files: tdb open ['archive', 'config', 'db']")
         print("listen:".ljust(16)+"Starts a server listening on passed port.")
         print("".ljust(64,"-"))
         tdb.cli.print_options()
         print("```")
         sys.exit(1)
@@ -82,29 +82,29 @@
         if text:
             tdb.records.add_record(text)
         else:
             print("No text provided. Record not added.")
             sys.exit(1)
 
     elif command == "show":
-        tdb.records.print_records(options)
+        tdb.records.print_db_records(options)
 
     elif command == "open":
         if "config" in sys.argv: tdb.cli.run(f"{tdb.config.get('editor')} {tdb.config.get_filename()}")
         elif "db" in sys.argv: tdb.cli.run(f"{tdb.config.get('editor')} {tdb.db.get_filename()}")
         elif "archive" in sys.argv: tdb.cli.run(f"{tdb.config.get('editor')} {tdb.db.get_archive()}")
         else:
             print("can't open '"+" ".join(sys.argv[2:])+"'.\noptions: 'config', 'db', or 'archive'")
             sys.exit(1)
     
-    elif command == "remove":
+    elif command == "rm":
         if options:
             records = tdb.records.split_db_records(options)
             if records:
-                print(tdb.records.stringify_records(records, {"as":"list"}))
+                tdb.records.print_records(records, {"as":"list"})
                 while True:
                     response = input(f"Archive {len(records)} record{'s' if len(records) > 1 else ''}? (y/n): ").lower()
                     if response in ["yes", "y"]: response = True
                     elif response in ["no", "n"]: response = False
                     if isinstance(response, bool): break
                 
                 if response and tdb.records.archive_records(records):
```

### Comparing `pypi_tdb-0.0.5/tdb/addon.py` & `pypi_tdb-0.0.6/tdb/addon.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     with open(path, "w+") as file:
         if path.endswith(".html"):
             #TODO this will allow multiple records with the same path to export together.
             #     however, this code runs for each export line, which is not performant.
             #     need a way to dedupe tag commands in some cases.
             records = [r for r in tdb.records.split_records(text) if path in r.text]
             for r in records: r.text = "\n".join([l for l in r.text.splitlines() if not l.startswith("@tdb")])
-            tdb.html.print_html(reversed([r.asdict() for r in records]), file)
+            tdb.html.print_html(reversed([r for r in records]), file)
         elif path.endswith(".json"):
             records = [r for r in tdb.records.split_records(text) if path in r.text]
             for r in records: r.text = "\n".join([l for l in r.text.splitlines() if not l.startswith("@tdb")])
             res = [r.asdict() for r in records]
             print(json.dumps(res, indent=2), file=file)
         elif path.endswith(".short"):
             out = "".join([str(r).splitlines()[0]+"\n" for r in records])
```

### Comparing `pypi_tdb-0.0.5/tdb/cli.py` & `pypi_tdb-0.0.6/tdb/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,60 @@
 from datetime import datetime, timedelta
 import sys
 import subprocess
 import shlex
+import platform
+
+
+class ANSICodes:
+    black = "\033[0;30m"
+    red = "\033[0;31m"
+    green = "\033[0;32m"
+    brown = "\033[0;33m"
+    blue = "\033[0;34m"
+    purple = "\033[0;35m"
+    cyan = "\033[0;36m"
+    light_gray = "\033[0;37m"
+    dark_gray = "\033[1;30m"
+    light_red = "\033[1;31m"
+    light_green = "\033[1;32m"
+    yellow = "\033[1;33m"
+    light_blue = "\033[1;34m"
+    light_purple = "\033[1;35m"
+    light_cyan = "\033[1;36m"
+    light_white = "\033[1;37m"
+    bold = "\033[1m"
+    faint = "\033[2m"
+    italic = "\033[3m"
+    underline = "\033[4m"
+    blink = "\033[5m"
+    negative = "\033[7m"
+    crossed = "\033[9m"
+    end = "\033[0m"
+
+
+def enable_ansi():
+    kernel32 = ctypes.windll.kernel32
+    ENABLE_PROCESSED_OUTPUT = 0x0001
+    ENABLE_VIRTUAL_TERMINAL_PROCESSING = 0x0004
+    out_handle = kernel32.GetStdHandle(subprocess.STD_OUTPUT_HANDLE)
+    # GetConsoleMode fails if the terminal isn't native.
+    mode = ctypes.c_int32()
+    if kernel32.GetConsoleMode(out_handle, ctypes.byref(mode)) == 0: return
+    if not (mode.value & ENABLE_VIRTUAL_TERMINAL_PROCESSING):
+        kernel32.SetConsoleMode(out_handle, mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING | ENABLE_PROCESSED_OUTPUT)
+
+
+if platform.system() == "Windows":
+    import ctypes
+    enable_ansi()
+    
+
+def isatty():
+    return sys.stdout.isatty()
 
 
 def get_text():
     if sys.stdin.isatty():
         text = " ".join(sys.argv[2:]).strip()
     else:
         text = sys.stdin.read()
```

### Comparing `pypi_tdb-0.0.5/tdb/config.py` & `pypi_tdb-0.0.6/tdb/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,22 +34,30 @@
 # path to database
 db_file = "{_db_file}"
 db_archive = "{_db_archive}"
 edit_ext = ".md"
 # options: {_editors}
 editor = "{_editor}" # command for editor
 addons = ["{_addon_file}"]
+"""+"""
+[tags]
+bug = {colour = "red"}
 """
 
+
 os.makedirs(_tdb_dir, exist_ok=True)
 
 if not os.path.exists(_conf_file): open(_conf_file, "w").write(_conf_text)
 
 
 def get_tdb_dir(): return _tdb_dir
 def get_filename(): return _conf_file
-def get(key):
+def _init():
     global _config
     if not _config:
         import tomllib
         _config = tomllib.load(open(_conf_file, "rb"))
-    return _config.get(key)
+
+def get(key, default=None):
+    _init()
+    if key in _config: default = _config.get(key)
+    return default
```

### Comparing `pypi_tdb-0.0.5/tdb/db.py` & `pypi_tdb-0.0.6/tdb/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,26 +75,40 @@
     global _db_inserts
     global _db_text
     _init()
     if _db_text and _db_text[-1] != '\n':
         text = '\n'+text
     insert(text, len(_db_text), len(_db_text))
 
-def append_immediate(text): open(get_filename(), "a").write(text)
+
+def append_fileline(text, path):
+    f = open(path, "a+")
+    f.seek(0, os.SEEK_END)
+    f.seek(max(0, f.tell()-1)) # potential utf-8 issues
+    if f.read() != '\n' and text[0] != '\n':
+        f.write('\n'+text)
+    else:
+        f.write(text)
+    f.close()
+
+
+def append_immediate(text):
+    append_fileline(text, get_filename())
+    
 
 def replace(old, new):
     global _db_inserts
     _init()
     # print("old:"+str([old]))
     id = _db_text.index(old)
     if id != -1:
         insert(new, id, id+len(old))
 
 def archive(text, remove=True):
-    open(get_archive(), "a").write(text)
+    append_fileline(text, get_archive())
     if remove: replace(text, "")
 
 
 def insert(text, start, end):
     global _db_inserts
     _init()
     _db_inserts.append([text, (start, end)])
```

### Comparing `pypi_tdb-0.0.5/tdb/html.js` & `pypi_tdb-0.0.6/tdb/html.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,14 +17,22 @@
         }
     }
     xmlHttp.open("POST", theUrl, true); // true for asynchronous 
     xmlHttp.setRequestHeader("Content-Type", "application/json");
     xmlHttp.send(data);
 };
 
+var allowedit = false;
+httpGet(window.origin + "/api/get.allowedit", function(response) {
+    response = JSON.parse(response);
+    if (response["ok"]) {
+        allowedit = response["allowedit"];
+    }
+});
+
 document.addEventListener("DOMContentLoaded", function() {
     const input = document.querySelector("input");
     if (input) {
         const container = document.getElementById("container");
 
         input.addEventListener("input", updateRecords);
         let searchParams = new URLSearchParams(window.location.search);
@@ -39,15 +47,15 @@
                 insertUrlParam("opts", encodeURI(input.value));
                 httpGet(url, function(response) {
                     response = JSON.parse(response);
                     if (response["ok"]) {
                         const before_scroll = window.scrollY;
                         container.innerHTML = response["records"];
                         for (var i = 0; i < container.children.length; i++) {
-                            if (container.children[i].className == "entry") {
+                            if (container.children[i].className == "entry" && allowedit) {
                                 var child = container.children[i];
                                 var edit = document.createElement("button");
                                 var remove = document.createElement("button");
                                 edit.style = " border: 0; background: none; box-shadow: none; border-radius: 0px;";
                                 remove.style = " border: 0; background: none; box-shadow: none; border-radius: 0px;";
                                 edit.textContent = "✏️";
                                 remove.textContent = "🗑️";
@@ -114,15 +122,15 @@
                                 edit.remove_button = remove;
                                 remove.onclick = remove_func;
                                 remove.edit_button = edit;
                                 child.appendChild(edit);
                                 child.appendChild(remove);
                             }
                         }
-                        if (mermaid) {
+                        if (typeof variable !== 'undefined') {
                             mermaid.run();
                         }
                         window.scrollTo({
                             top: before_scroll
                         });
                     }
                 });
```

### Comparing `pypi_tdb-0.0.5/tdb/html.py` & `pypi_tdb-0.0.6/tdb/html.py`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/tdb/rake.py` & `pypi_tdb-0.0.6/tdb/rake.py`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/tdb/records.py` & `pypi_tdb-0.0.6/tdb/records.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 def register_cmd(func):
     global _record_cmds
     _record_cmds.append(func)
     pass
 
 
 def make_record(date, text):
-    return f"\n[tdb:{date}] {text}"
+    return f"[tdb:{date}] {text}"
 
 
 def add_record(text):
     dt = tdb.db.get_mtime()
     ns = time.time_ns()
     # convert to microseconds for datetime compliance
     ns = int(ns/1E3)
@@ -226,31 +226,48 @@
         res = [r.asdict() for r in records]
         out = json.dumps(res, indent=2)
     elif options and options["as"] == "html":
         out = tdb.html.build_html(list(reversed(records)))
     elif options and options["as"] == "html_entries":
         out = tdb.html.build_html_entries(list(reversed(records)))
     elif options and options["as"] == "list":
-        out = "".join([str(r).splitlines()[0]+"\n" for r in records])
+        def list_line(record):
+            line = str(record).splitlines()[0]
+            for t, _ in record.tags:
+                if not "@"+t in line: line += " @"+t 
+            return line+"\n"
+        out = "".join([list_line(r) for r in records])
         out = out.strip()
     elif options and options["as"] == "tags":
         tags = {}
         for r in records:
             for t in r.tags:
                 if t[0] in tags: tags[t[0]] += 1
                 else: tags[t[0]] = 1
         out = json.dumps(tags, indent=2)
     else:
         out = "".join([str(r) for r in records])
         out = out.strip()
     return out
 
 
-def print_records(options=None):
-    if out := stringify_db_records(options): print(out)
+def print_records(records, options=None):
+    if out := stringify_records(records, options):
+        if tdb.cli.isatty():
+            for tag in tdb.tags.find_tags(out):
+                col = getattr(tdb.cli.ANSICodes, tdb.tags.get_colour(tag[0]))
+                out = out.replace("@"+tag[0], col+"@"+tag[0]+tdb.cli.ANSICodes.end)
+            # TODO: the [tdb:\1] here feels like it could be done better. Also, config colour for tdb header?
+            out = re_iso_record.sub(tdb.cli.ANSICodes.light_white+r"[tdb:\1] "+tdb.cli.ANSICodes.end, out)
+        print(out)
+
+
+def print_db_records(options=None):
+    if records := split_db_records(options):
+        print_records(records, options)
 
 
 def filter_records(records : list, options : list):
     max_id = len(records)
     filtered = records.copy()
 
     dates = options["dates"] if options else []
@@ -347,14 +364,15 @@
         nonlocal last
         nonlocal current
 
         if last:
             x,y = last["span"][1], current["span"][0]
             section = text[x:y]
             tags = tdb.tags.find_tags(section.lower())
+            tdb.tags.register(tags)
             last["text"] = section
             last["tags"] = tags
             last["span"] = (x ,y)
             records.append(last)
 
     for match in re_hex_record.finditer(text):
         nano = int(match.group(1), 16)
```

### Comparing `pypi_tdb-0.0.5/tdb/server.py` & `pypi_tdb-0.0.6/tdb/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,26 +19,27 @@
 class TdbServer(SimpleHTTPRequestHandler):
     """
     List files that are allowed to be sent
     """
     whitelist = []
 
     def do_GET(self):
-        query_list = None
-
+        query_list = []
+        allowedit = self.client_address[0] == "127.0.0.1"
+        
         # split the query out if need be
         if "?" in self.path:
             self.path, query_list = self.path.split("?")
             if "&" in query_list:
                 query_list = query_list.split("&")
             else:
                 query_list = [query_list]
         
-        # put the queries into a dict        
-        if query_list and self.path.startswith("/api/"):
+        # put the queries into a dict
+        if self.path.startswith("/api/"):
             queries = {}
             for q in query_list:
                 k, v = q.split("=", 1)
                 queries[k] = v
             
             options = ("web "+urllib.parse.unquote(queries["opts"])) if "opts" in queries else ""
             options = tdb.cli.parse_options(options)
@@ -51,17 +52,20 @@
             headers = {}
             headers["Content-Type"] = "text/json"
 
             if "/api/get.records" == self.path:
                 response["ok"] = True
                 response["records"] = tdb.records.stringify_db_records(options)
             elif "/api/get.tags" == self.path:
-                print("getting tags")
+                print("getting tags - not implemented")
                 response["ok"] = True
                 response["tags"] = "not implemented"
+            elif "/api/get.allowedit" == self.path:
+                response["ok"] = True
+                response["allowedit"] = allowedit
             else:
                 self.send_response(404)
                 for k, v in headers.items():
                     self.send_header(k, v)
                 response["error"] = "api call not found "+self.path
                 self.end_headers()
                 self.wfile.write(bytes(json.dumps(response), "utf-8"))
@@ -75,27 +79,27 @@
             return
         elif any(map(self.path.endswith, [".js", ".html", ".css"])):
             headers = {}
             out = ""
             if "/tdb/html.js" == self.path:
                 headers["Content-Type"] = "text/javascript"
                 self.path = os.path.abspath(os.path.dirname(__file__)+"/html.js")
-                out = open(self.path).read()
+                out = open(self.path, encoding="utf-8").read()
             elif "/tdb/mermaid.min.js" == self.path:
                 headers["Content-Type"] = "text/javascript"
                 self.path = tdb.html._mermaid_js_file
-                out = open(self.path).read()
+                out = open(self.path, encoding="utf-8").read()
             elif "/tdb/mermaid.css" == self.path:
                 headers["Content-Type"] = "text/css"
                 self.path = tdb.html._mermaid_css_file
-                out = open(self.path).read()
+                out = open(self.path, encoding="utf-8").read()
             elif "/tdb/style.css" == self.path:
                 headers["Content-Type"] = "text/css"
                 self.path = tdb.html._css_file
-                out = open(self.path).read()
+                out = open(self.path, encoding="utf-8").read()
             elif "/index.html" == self.path:
                 headers["Content-Type"] = "text/html"
                 out = tdb.html.build_html([], True)
             self.send_response(200)
             for k, v in headers.items():
                 self.send_header(k, v)
             self.end_headers()
@@ -103,56 +107,60 @@
         else:
             self.send_response(404)
             self.end_headers()
         pass
 
     def do_POST(self):
         response = {"ok": False}
+        allowedit = self.client_address[0] == "127.0.0.1"
         code = 200
         headers = {}
         headers["Content-Type"] = "text/json"
+        headers["Content-Length"] = 0
         try:
             db_lock.acquire()
             data_string = self.rfile.read(int(self.headers['Content-Length']))
             parsed = data_string.decode("utf-8")
             parsed = json.loads(parsed)
-            if "/api/add.record" == self.path:
+            if "/api/add.record" == self.path and allowedit:
                 if "text" in parsed:
                     tdb.records.add_record(parsed["text"])
                     response["ok"] = True
            
-            elif "/api/edit.record" == self.path:
+            elif "/api/edit.record" == self.path and allowedit:
                 if "text" in parsed and "date" in parsed:
                     options = tdb.cli.parse_options("web")
                     options["dates"] = tdb.cli.parse_options("web "+parsed["date"])["dates"]
                     records = tdb.records.split_db_records(options)
                     if len(records) == 1:
                         cpy = tdb.records.Record(**records[0].asdict())
                         cpy.text = parsed["text"] # TODO: The need to always add \n is annoying. text should be property a property and add it.
                         if not cpy.text.endswith("\n"): cpy.text += "\n" 
                         tdb.records.modify_db_records(records, [cpy])
                         tdb.db.serialise()
                         response["ok"] = True
 
-            elif "/api/remove.record" == self.path:
+            elif "/api/remove.record" == self.path and allowedit:
                 if "date" in parsed:
                     options = tdb.cli.parse_options("web")
                     options["dates"] = tdb.cli.parse_options("web "+parsed["date"])["dates"]
                     records = tdb.records.split_db_records(options)
                     if len(records) == 1:
                         tdb.records.archive_records(records)
                         tdb.db.serialise()
                         response["ok"] = True
 
             else: code = 404
+            payload = bytes(json.dumps(response)+"\r\n", "utf-8")
+            headers["Content-Length"] = len(payload)
+            self.send_response(code)
             for k, v in headers.items():
                 self.send_header(k, v)
-            self.send_response(code)
             self.end_headers()
-            self.wfile.write(bytes(json.dumps(response)+"\r\n", "utf-8"))
+            self.wfile.write(payload)
 
         finally:
             db_lock.release()
 
 
 def _get_best_family(*address):
     infos = socket.getaddrinfo(
```

### Comparing `pypi_tdb-0.0.5/tdb/session.py` & `pypi_tdb-0.0.6/tdb/session.py`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/tdb/style.css` & `pypi_tdb-0.0.6/tdb/style.css`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/.gitignore` & `pypi_tdb-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/LICENSE` & `pypi_tdb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypi_tdb-0.0.5/pyproject.toml` & `pypi_tdb-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypi-tdb"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Graham Hughes", email="graehu@gmail.com" },
 ]
 description = "tdb: text based database with tagging"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `pypi_tdb-0.0.5/readme.md` & `pypi_tdb-0.0.6/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # tdb
 
 A text based database with tagging.
 
 ```
-Usage: py -m tdb [add | edit | remove | template | show | open | listen] [text | options]
+Usage: py -m tdb [add | edit | rm | template | show | open | listen] [text | options]
 ----------------------------------------------------------------
 Commands:
 add:            Make a record when text is supplied. Otherwise, open an editor to write one.
 edit:           Open an editor with some view of the database, see options.
-remove:         Move matching records to the archive.
+rm:         Move matching records to the archive.
 template:       Open an editor to write a record with the passed template file as a basis.
 open:           Open tdbs files: tdb open ['archive', 'config', 'db']
 listen:         Starts a server listening on passed port.
 ----------------------------------------------------------------
 Options:
 span:           The records to select, example: span:7d is the last 7 days.
 as:             The format to see the records in. Only valid for show currently. [html, json, list, tags]
```

### Comparing `pypi_tdb-0.0.5/PKG-INFO` & `pypi_tdb-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypi-tdb
-Version: 0.0.5
+Version: 0.0.6
 Summary: tdb: text based database with tagging
 Project-URL: Homepage, https://github.com/graehu/tdb
 Project-URL: Bug Tracker, https://github.com/graehu/tdb/issues
 Author-email: Graham Hughes <graehu@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,20 +13,20 @@
 Description-Content-Type: text/markdown
 
 # tdb
 
 A text based database with tagging.
 
 ```
-Usage: py -m tdb [add | edit | remove | template | show | open | listen] [text | options]
+Usage: py -m tdb [add | edit | rm | template | show | open | listen] [text | options]
 ----------------------------------------------------------------
 Commands:
 add:            Make a record when text is supplied. Otherwise, open an editor to write one.
 edit:           Open an editor with some view of the database, see options.
-remove:         Move matching records to the archive.
+rm:         Move matching records to the archive.
 template:       Open an editor to write a record with the passed template file as a basis.
 open:           Open tdbs files: tdb open ['archive', 'config', 'db']
 listen:         Starts a server listening on passed port.
 ----------------------------------------------------------------
 Options:
 span:           The records to select, example: span:7d is the last 7 days.
 as:             The format to see the records in. Only valid for show currently. [html, json, list, tags]
```

