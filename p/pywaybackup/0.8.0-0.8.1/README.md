# Comparing `tmp/pywaybackup-0.8.0.tar.gz` & `tmp/pywaybackup-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywaybackup-0.8.0.tar", last modified: Mon Apr  8 14:35:27 2024, max compression
+gzip compressed data, was "pywaybackup-0.8.1.tar", last modified: Fri Apr 12 12:41:33 2024, max compression
```

## Comparing `pywaybackup-0.8.0.tar` & `pywaybackup-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,21 @@
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       98 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/.gitignore
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1065 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/LICENSE
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4925 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4572 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/README.md
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.910350 pywaybackup-0.8.0/dev/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      477 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/dev/pip_build.sh
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      551 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/dev/venv_create.sh
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.910350 pywaybackup-0.8.0/pywaybackup/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4606 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/SnapshotCollection.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1644 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/Verbosity.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/pywaybackup/__init__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       21 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/__version__.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)    11873 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/archive.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     2290 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/arguments.py
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      815 2024-04-08 14:34:18.000000 pywaybackup-0.8.0/pywaybackup/main.py
-drwxr-xr-x   0 bitdruid  (1000) bitdruid  (1000)        0 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/pywaybackup.egg-info/
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     4925 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/PKG-INFO
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)      480 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/SOURCES.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)        1 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/dependency_links.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       52 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/entry_points.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       30 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/requires.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       12 2024-04-08 14:35:27.000000 pywaybackup-0.8.0/pywaybackup.egg-info/top_level.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       53 2024-04-08 14:04:38.000000 pywaybackup-0.8.0/requirements.txt
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)       38 2024-04-08 14:35:27.913683 pywaybackup-0.8.0/setup.cfg
--rw-r--r--   0 bitdruid  (1000) bitdruid  (1000)     1091 2024-04-03 10:05:23.000000 pywaybackup-0.8.0/setup.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1065 2024-02-25 19:19:33.000000 pywaybackup-0.8.1/LICENSE
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4925 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4572 2024-04-12 12:30:31.000000 pywaybackup-0.8.1/README.md
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/pywaybackup/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4606 2024-04-12 12:30:05.000000 pywaybackup-0.8.1/pywaybackup/SnapshotCollection.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1644 2024-04-12 12:30:31.000000 pywaybackup-0.8.1/pywaybackup/Verbosity.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)        0 2024-02-25 19:19:33.000000 pywaybackup-0.8.1/pywaybackup/__init__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       21 2024-04-12 12:40:47.000000 pywaybackup-0.8.1/pywaybackup/__version__.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)    11879 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/archive.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     2329 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/arguments.py
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)      868 2024-04-12 12:40:16.000000 pywaybackup-0.8.1/pywaybackup/main.py
+drwxr-xr-x   0 manjaro   (1000) manjaro   (1001)        0 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/pywaybackup.egg-info/
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     4925 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/PKG-INFO
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)      416 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/SOURCES.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)        1 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/dependency_links.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       52 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/entry_points.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       30 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/requires.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       12 2024-04-12 12:41:33.000000 pywaybackup-0.8.1/pywaybackup.egg-info/top_level.txt
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)       38 2024-04-12 12:41:33.239507 pywaybackup-0.8.1/setup.cfg
+-rw-r--r--   0 manjaro   (1000) manjaro   (1001)     1091 2024-02-26 09:18:12.000000 pywaybackup-0.8.1/setup.py
```

### Comparing `pywaybackup-0.8.0/LICENSE` & `pywaybackup-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.0/PKG-INFO` & `pywaybackup-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.8.0
+Version: 0.8.1
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
```

### Comparing `pywaybackup-0.8.0/README.md` & `pywaybackup-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.0/pywaybackup/SnapshotCollection.py` & `pywaybackup-0.8.1/pywaybackup/SnapshotCollection.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.0/pywaybackup/Verbosity.py` & `pywaybackup-0.8.1/pywaybackup/Verbosity.py`

 * *Files identical despite different names*

### Comparing `pywaybackup-0.8.0/pywaybackup/archive.py` & `pywaybackup-0.8.1/pywaybackup/archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,20 +252,20 @@
     """
     Parse the response code of the Wayback Machine and return a human-readable message.
     """
     if response_code in RESPONSE_CODE_DICT:
         return RESPONSE_CODE_DICT[response_code]
     return "Unknown response code"
 
-def save_csv(output: str):
+def save_csv(csv_path: str):
     """
     Write a CSV file with the list of snapshots.
     """
     import csv
     if sc.count_list() > 0:
         v.write("\nSaving CSV file...")
-        os.makedirs(os.path.abspath(output), exist_ok=True)
-        with open(os.path.join(output, "waybackup.csv"), mode='w') as file:
+        os.makedirs(os.path.abspath(csv_path), exist_ok=True)
+        with open(os.path.join(csv_path, "waybackup.csv"), mode='w') as file:
             row = csv.DictWriter(file, sc.SNAPSHOT_COLLECTION[0].keys())
             row.writeheader()
             for snapshot in sc.SNAPSHOT_COLLECTION:
                 row.writerow(snapshot)
```

### Comparing `pywaybackup-0.8.0/pywaybackup/arguments.py` & `pywaybackup-0.8.1/pywaybackup/arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     exclusive_required.add_argument('-c', '--current', action='store_true', help='Download the latest version of each file snapshot (opt range in y)')
     exclusive_required.add_argument('-f', '--full', action='store_true', help='Download snapshots of all timestamps (opt range in y)')
     exclusive_required.add_argument('-s', '--save', action='store_true', help='Save a page to the wayback machine')
 
     optional = parser.add_argument_group('optional')
     optional.add_argument('-l', '--list', action='store_true', help='Only print snapshots (opt range in y)')
     optional.add_argument('-e', '--explicit', action='store_true', help='Search only for the explicit given url')
-    optional.add_argument('-o', '--output', type=str, help='Output folder')
+    optional.add_argument('-o', '--output', type=str, help='Output folder defaults to current directory')
     optional.add_argument('-r', '--range', type=int, help='Range in years to search')
     optional.add_argument('--start', type=int, help='Start timestamp format: YYYYMMDDhhmmss')
     optional.add_argument('--end', type=int, help='End timestamp format: YYYYMMDDhhmmss')
 
     special = parser.add_argument_group('special')
-    special.add_argument('--csv', action='store_true', help='Save a csv file with the list of snapshots inside the output folder')
+    special.add_argument('--csv', type=str, nargs='?', const=True, help='Save a csv file on a given path or defaults to the output folder')
     special.add_argument('--no-redirect', action='store_true', help='Do not follow redirects by archive.org')
     special.add_argument('--verbosity', type=str, default="standard", choices=["standard", "progress", "json"], help='Verbosity level')
     special.add_argument('--retry', type=int, default=0, metavar="X-TIMES", help='Retry failed downloads (opt tries as int, else infinite)')
     special.add_argument('--worker', type=int, default=1, metavar="AMOUNT", help='Number of worker (simultaneous downloads)')
 
     args = parser.parse_args()
```

### Comparing `pywaybackup-0.8.0/pywaybackup/main.py` & `pywaybackup-0.8.1/pywaybackup/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,22 +11,24 @@
     if args.full:
         mode = "full"
     if args.current:
         mode = "current"
 
     if args.output is None:
         args.output = os.path.join(os.getcwd(), "waybackup_snapshots")
+    if args.csv is True:
+        args.csv = args.output
 
     if args.save:
         archive.save_page(args.url)
     else:
         archive.query_list(args.url, args.range, args.start, args.end, args.explicit, mode)
         if args.list:
             archive.print_list()
         else:
             archive.download_list(args.output, args.retry, args.no_redirect, args.worker)
         if args.csv:
-            archive.save_csv(args.output)
+            archive.save_csv(args.csv)
     v.close()
 
 if __name__ == "__main__":
     main()
```

### Comparing `pywaybackup-0.8.0/pywaybackup.egg-info/PKG-INFO` & `pywaybackup-0.8.1/pywaybackup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywaybackup
-Version: 0.8.0
+Version: 0.8.1
 Summary: Download snapshots from the Wayback Machine
 Home-page: https://github.com/bitdruid/python-wayback-machine-downloader
 Author: bitdruid
 Author-email: bitdruid@outlook.com
 License: MIT
 Keywords: wayback machine internet archive
 Description-Content-Type: text/markdown
```

### Comparing `pywaybackup-0.8.0/setup.py` & `pywaybackup-0.8.1/setup.py`

 * *Files identical despite different names*

