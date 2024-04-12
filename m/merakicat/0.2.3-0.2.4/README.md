# Comparing `tmp/merakicat-0.2.3.tar.gz` & `tmp/merakicat-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merakicat-0.2.3.tar", last modified: Wed Apr 10 21:23:47 2024, max compression
+gzip compressed data, was "merakicat-0.2.4.tar", last modified: Fri Apr 12 16:51:37 2024, max compression
```

## Comparing `merakicat-0.2.3.tar` & `merakicat-0.2.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.483371 merakicat-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.471371 merakicat-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.475371 merakicat-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-10 21:23:37.000000 merakicat-0.2.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 21:23:37.000000 merakicat-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 21:23:37.000000 merakicat-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-10 21:23:37.000000 merakicat-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-10 21:23:37.000000 merakicat-0.2.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-10 21:23:37.000000 merakicat-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 21:23:37.000000 merakicat-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-10 21:23:37.000000 merakicat-0.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-04-10 21:23:47.483371 merakicat-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-10 21:23:37.000000 merakicat-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.475371 merakicat-0.2.3/files/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-10 21:23:37.000000 merakicat-0.2.3/files/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.479371 merakicat-0.2.3/images/
--rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/botcongrats.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/cisco_meraki.png
--rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/createbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/mc_quick.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/merakicat.png
--rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/newapp.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-10 21:23:37.000000 merakicat-0.2.3/images/newbot.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-10 21:23:37.000000 merakicat-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-10 21:23:37.000000 merakicat-0.2.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 21:23:47.483371 merakicat-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-10 21:23:37.000000 merakicat-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.471371 merakicat-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.483371 merakicat-0.2.3/src/merakicat/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.483371 merakicat-0.2.3/src/merakicat/batch_helper/
--rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/batch_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/batch_helper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/batch_helper/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/bulk_check.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/bulk_migrate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_cfg_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_cloud_mon.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_file_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_get_nms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55397 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_pedia.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_register.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_splitcheck_serials.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    35749 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/mc_user_info.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    93515 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/merakicat.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 21:23:37.000000 merakicat-0.2.3/src/merakicat/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 21:23:47.483371 merakicat-0.2.3/src/merakicat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11724 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 21:23:47.000000 merakicat-0.2.3/src/merakicat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-10 21:23:37.000000 merakicat-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.393708 merakicat-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-12 16:51:28.000000 merakicat-0.2.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-12 16:51:28.000000 merakicat-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 16:51:28.000000 merakicat-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-12 16:51:28.000000 merakicat-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-12 16:51:28.000000 merakicat-0.2.4/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 16:51:28.000000 merakicat-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 16:51:28.000000 merakicat-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 16:51:28.000000 merakicat-0.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-04-12 16:51:37.389708 merakicat-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-12 16:51:28.000000 merakicat-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 16:51:28.000000 merakicat-0.2.4/files/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.385708 merakicat-0.2.4/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    55062 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/botcongrats.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    78377 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/cisco_meraki.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54965 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/createbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1774034 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/mc_quick.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12826 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/merakicat.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22117 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/newapp.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    87754 2024-04-12 16:51:28.000000 merakicat-0.2.4/images/newbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-12 16:51:28.000000 merakicat-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 16:51:28.000000 merakicat-0.2.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:51:37.393708 merakicat-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-12 16:51:28.000000 merakicat-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.381708 merakicat-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat/batch_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/batch_helper/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/bulk_check.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      397 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/bulk_migrate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6424 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_cfg_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4629 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_cloud_mon.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1215 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_file_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_get_nms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54918 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_pedia.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      631 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8817 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_register.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2215 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_splitcheck_serials.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35749 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/mc_user_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    90886 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/merakicat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 16:51:28.000000 merakicat-0.2.4/src/merakicat/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:51:37.389708 merakicat-0.2.4/src/merakicat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11871 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 16:51:37.000000 merakicat-0.2.4/src/merakicat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 16:51:28.000000 merakicat-0.2.4/tox.ini
```

### Comparing `merakicat-0.2.3/.gitignore` & `merakicat-0.2.4/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Miscellaneous files
 src/merakicat/batch_helper_preview.json
 src/merakicat/test.txt
 
+# BBEdit files
+*.bbprojectd
+*.bbnotebookd
+
 # App-created files and logs
 files/*.cfg
 files/*.pdf
 files/*.docx
 files/*.ab0
 files/*.ab1
 files/*.pd
```

### Comparing `merakicat-0.2.3/CONTRIBUTING.rst` & `merakicat-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/HISTORY.md` & `merakicat-0.2.4/HISTORY.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # History
 
+## 0.2.4 (04-12-2024)
+
+  - Added Private VLAN -> Port Isolation to encyclopedia.
+  - Removed older bot code.
+  - Updated AUTHORS.rst.
+  - Updated .gitignore
+
 ## 0.2.3 (04-10-2024)
 
   - Translate now checks to make sure that the target switches have the same number of ports as the sources.
 
 ## 0.2.2 (04-10-2024)
 
   - Added environment variable to specify a Meraki Oragnization name.
@@ -45,54 +52,54 @@
 
 ## 0.1.3 (03-21-2024)
 
   - Code beautification with flake8.
   - Setting up for publishing automation.
   - Changed directory structure for publishing.
   - Released on PyPI.
-  
+
 ## 0.0.14 (03-19-2024)
 
   - Option added for check with drag and drop files in bot mode.
   - Added missing timing in check report in bot mode.
   - Still not yet released on PyPI.
-  
+
 ## 0.0.13 (03-18-2024)
 
   - Option added for detailed check report "with detail".
-  
+
 ## 0.0.12 (03-15-2024)
 
   - Option for PDF vs. DOCX reporting in checker.
   - Layer 3 Interfaces (interface VLAN) supported.
   - Static routes supported.
   - Command added for "demo report".
-  
+
 ## 0.0.11 (03-12-2024)
 
   - New reporting in checker.
   - Port-channel LACP is working and fast.
-  
+
 ## 0.0.10 (03-08-2024)
 
   - Using a single mc_pedia.
-  
+
 ## 0.0.9 (03-07-2024)
 
   - Using both config_pedia and check_pedia.
   - Changed to ngrok API for bot functionality
-  
+
 ## 0.0.8 (03-01-2024)
 
   - Lots of comment blocks added.
-  
+
 ## 0.0.7 (03-01-2024)
 
   - Now using batch port updates to Meraki dashboard.
-  
+
 ## 0.0.6 (03-01-2024)
 
   - Some light refactoring of mc_translate module.
   - More prep work for Uplink config.
 
 ## 0.0.5 (02-29-2024)
```

### Comparing `merakicat-0.2.3/LICENSE` & `merakicat-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/Makefile` & `merakicat-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/PKG-INFO` & `merakicat-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.3
+Version: 0.2.4
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,17 +28,17 @@
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
- 
+
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
- 
+
 This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
 
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
@@ -51,22 +51,23 @@
  - Port Speed
  - Port Duplex
  - Port Type
  - PoE Enabled
  - Allowed VLANs
  - Data VLAN
  - Voice VLAN
+ - Private VLAN
  - Layer 3 Interface
  - STP RootGuard
  - STP Loop Guard
  - STP BPDU Guard
  - Etherchannel LACP
  - NM Ports
 
- 
+
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
 # Prerequisites for using in Bot mode
@@ -115,30 +116,30 @@
 
     ```
     # These exports are used for Webex bot mode:
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
-    
+
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
 
-To run merakicat as a Bot, just start it without any parameters:  
+To run merakicat as a Bot, just start it without any parameters:
 
 ```
 cd src/merakicat
 python merakicat.py
 ```
 **Bot commands include the following:**
 
@@ -241,14 +242,21 @@
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.4 (04-12-2024)
+
+  - Added Private VLAN -> Port Isolation to encyclopedia.
+  - Removed older bot code.
+  - Updated AUTHORS.rst.
+  - Updated .gitignore
+
 ## 0.2.3 (04-10-2024)
 
   - Translate now checks to make sure that the target switches have the same number of ports as the sources.
 
 ## 0.2.2 (04-10-2024)
 
   - Added environment variable to specify a Meraki Oragnization name.
@@ -290,54 +298,54 @@
 
 ## 0.1.3 (03-21-2024)
 
   - Code beautification with flake8.
   - Setting up for publishing automation.
   - Changed directory structure for publishing.
   - Released on PyPI.
-  
+
 ## 0.0.14 (03-19-2024)
 
   - Option added for check with drag and drop files in bot mode.
   - Added missing timing in check report in bot mode.
   - Still not yet released on PyPI.
-  
+
 ## 0.0.13 (03-18-2024)
 
   - Option added for detailed check report "with detail".
-  
+
 ## 0.0.12 (03-15-2024)
 
   - Option for PDF vs. DOCX reporting in checker.
   - Layer 3 Interfaces (interface VLAN) supported.
   - Static routes supported.
   - Command added for "demo report".
-  
+
 ## 0.0.11 (03-12-2024)
 
   - New reporting in checker.
   - Port-channel LACP is working and fast.
-  
+
 ## 0.0.10 (03-08-2024)
 
   - Using a single mc_pedia.
-  
+
 ## 0.0.9 (03-07-2024)
 
   - Using both config_pedia and check_pedia.
   - Changed to ngrok API for bot functionality
-  
+
 ## 0.0.8 (03-01-2024)
 
   - Lots of comment blocks added.
-  
+
 ## 0.0.7 (03-01-2024)
 
   - Now using batch port updates to Meraki dashboard.
-  
+
 ## 0.0.6 (03-01-2024)
 
   - Some light refactoring of mc_translate module.
   - More prep work for Uplink config.
 
 ## 0.0.5 (02-29-2024)
```

### Comparing `merakicat-0.2.3/README.md` & `merakicat-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
- 
+
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
- 
+
 This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
 
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
@@ -21,22 +21,23 @@
  - Port Speed
  - Port Duplex
  - Port Type
  - PoE Enabled
  - Allowed VLANs
  - Data VLAN
  - Voice VLAN
+ - Private VLAN
  - Layer 3 Interface
  - STP RootGuard
  - STP Loop Guard
  - STP BPDU Guard
  - Etherchannel LACP
  - NM Ports
 
- 
+
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
 # Prerequisites for using in Bot mode
@@ -85,30 +86,30 @@
 
     ```
     # These exports are used for Webex bot mode:
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
-    
+
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
 
-To run merakicat as a Bot, just start it without any parameters:  
+To run merakicat as a Bot, just start it without any parameters:
 
 ```
 cd src/merakicat
 python merakicat.py
 ```
 **Bot commands include the following:**
```

### Comparing `merakicat-0.2.3/images/botcongrats.jpg` & `merakicat-0.2.4/images/botcongrats.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/cisco_meraki.png` & `merakicat-0.2.4/images/cisco_meraki.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/createbot.jpg` & `merakicat-0.2.4/images/createbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/mc_quick.gif` & `merakicat-0.2.4/images/mc_quick.gif`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/merakicat.png` & `merakicat-0.2.4/images/merakicat.png`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/newapp.jpg` & `merakicat-0.2.4/images/newapp.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/images/newbot.jpg` & `merakicat-0.2.4/images/newbot.jpg`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/setup.py` & `merakicat-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/batch_helper/__init__.py` & `merakicat-0.2.4/src/merakicat/batch_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/batch_helper/config.py` & `merakicat-0.2.4/src/merakicat/batch_helper/config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/batch_helper/exceptions.py` & `merakicat-0.2.4/src/merakicat/batch_helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_cfg_check.py` & `merakicat-0.2.4/src/merakicat/mc_cfg_check.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_claim.py` & `merakicat-0.2.4/src/merakicat/mc_claim.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_cloud_mon.py` & `merakicat-0.2.4/src/merakicat/mc_cloud_mon.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_file_exists.py` & `merakicat-0.2.4/src/merakicat/mc_file_exists.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_get_config.py` & `merakicat-0.2.4/src/merakicat/mc_get_config.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_get_nms.py` & `merakicat-0.2.4/src/merakicat/mc_get_nms.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_pedia.py` & `merakicat-0.2.4/src/merakicat/mc_pedia.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,19 @@
 
 #####################################################################################
 '''
 
 
 mc_pedia = {
 
-    'version': "v0.1.6",
-    'dated': "04/10/2024",
+    'version': "v0.1.7",
+    'dated': "04/12/2024",
 
     'switch': {
-        
+
         'switch_name': {
             'name': "Hostname",
             'support':"✓",
             'translatable':"✓",
             'regex': '^hostname',
             'iosxe': "\
 \
@@ -84,15 +84,15 @@
 if not switch_name_obj == []:\n\
     switch_name = switch_name_obj[0].re_match_typed('^hostname\s(\S+)',default='Switch')\n\
 if switch_name == '':\n\
     switch_name = 'Switch'\n\
 host_name = switch_name\n\
 if debug:\n\
     print(f'switch_name = {switch_name}')\n",
-            
+
             'meraki': {
                 'skip': 'post_process',
                 'default': 'Auto negotiate',
                 'post_process': "\
 \
 urls = list()\n\
 blurb = 'This was a conversion from a Catalyst IOSXE config.'\n\
@@ -147,52 +147,52 @@
        if not e.message['errors'][0] == 'Cannot stack switches that are already part of a switch stack':\n\
            print(f'Cannot create switch stack {switch_name} with {sw_list}.')\n\
 return_vals = ['urls','networkId','switchStackId']\n\
 if debug:\n\
     print(f'dir() = {dir()}')\n"
             }
         },
-        
+
         'vtp':{
             'name': "VTP",
             'support':"",
             'translatable':"",
             'regex': '^vtp',
             'meraki': {
                 'skip': True
             },
             'iosxe': "vtp = parse.find_objects('^vtp')\n",
             'url':"https://documentation.meraki.com/MS/Port_and_VLAN_Configuration/Integrating_the_MS_Access_Switch_into_a_Cisco_VTP_domain",
             'note':"Not required"
         },
-        
+
         'mls':{
             'name': "QoS",
             'support':"✓",
             'translatable':"",
             'regex': '^mls',
             'meraki': {
                 'skip': True
             },
             'iosxe': "mls = parse.find_objects('^mls')\n",
             'url':"https://documentation.meraki.com/MS/Other_Topics/MS_Switch_Quality_of_Service_Defined",
             'note':"Network-wide"
         },
-        
+
         'rstp':{
             'name':"Spanning Tree RSTP",
             'support':"✓",
             'translatable':"✓",
             'regex': '^spanning-tree mode rapid-pvst',
             'meraki': {
                 'skip': True
             },
             'iosxe': "rstp = parse.find_objects('^spanning-tree mode rapid-pvst')\n"
         },
-        
+
         'spanning':{
             'name':"Spanning Tree",
             'support':"",
             'translatable':"",
             'regex': '^spanning-tree',
             'meraki': {
                 'skip': True
@@ -201,394 +201,394 @@
 spanning = ''\n\
 if parse.find_objects('^spanning-tree extend system-id') == '':\n\
     if parse.find_objects('^spanning-tree mode rapid-pvst') == '':\n\
         spanning = parse.find_objects('^spanning-tree\s+(\S.+)')\n",
             'url':"https://documentation.meraki.com/MS/Port_and_VLAN_Configuration/Configuring_Spanning_Tree_on_Meraki_Switches_(MS)",
             'note':"Only Supports RSTP"
         },
-        
+
         'snmp':{
             'name': "SNMP",
             'support':"",
             'translatable':"",
             'regex': '^snmp',
             'meraki': {
                 'skip': True
             },
             'iosxe':"snmp = parse.find_objects('^snmp')\n",
             'url': "https://documentation.meraki.com/General_Administration/Monitoring_and_Reporting/SNMP_Overview_and_Configuration",
             'note': "Configured network-wide"
         },
-        
+
         'logging_host':{
             'name': "Syslog",
             'support':"",
             'translatable':"",
             'regex': '^logging',
             'meraki': {
                 'skip': True
             },
             'iosxe':"logging_host = parse.find_objects('^logging')\n",
             'url': "https://documentation.meraki.com/General_Administration/Monitoring_and_Reporting/Syslog_Server_Overview_and_Configuration",
             'note': "Configured network-wide"
         },
-        
+
         'ntp':{
             'name':"NTP",
             'support':"",
             'translatable':"",
             'regex': '^ntp',
             'meraki': {
                 'skip': True
             },
             'iosxe':"ntp = parse.find_objects('^ntp')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Configured by default"
         },
-        
+
         'access_list':{
             'name': "Access-List",
             'support':"",
             'translatable':"",
             'regex': '^access-list',
             'meraki': {
                 'skip': True
             },
             'iosxe': "access_list = parse.find_objects('^access-list')\n",
             'url':"https://documentation.meraki.com/MS/Access_Control/Meraki_MS_Group_Policy_Access_Control_Lists",
             'note':"Group Policies"
         },
-        
+
         'extended_access_list':{
             'name': "Extended ACL",
             'support':"",
             'translatable':"",
             'regex': '^ip\saccess-list',
             'meraki': {
                 'skip': True
             },
             'iosxe': "extended_access_list = parse.find_objects('^ip\saccess-list')\n",
             'url':"https://documentation.meraki.com/MS/Access_Control/Meraki_MS_Group_Policy_Access_Control_Lists",
             'note':"Group Policies"
         },
-        
+
         'port_mirror':{
             'name': "Port mirroring",
             'support': "✓",
             'translatable':"",
             'regex': '^monitor',
             'meraki': {
                 'skip': True
             },
             'iosxe': "port_mirror = parse.find_objects('^monitor')\n"
         },
-        
+
         'aaa':{
             'name': "AAA",
             'support':"",
             'translatable':"",
             'regex': '^aaa',
             'meraki': {
                 'skip': True
             },
             'iosxe': "aaa = parse.find_objects('^aaa')\n",
             'url':"https://documentation.meraki.com/General_Administration/Managing_Dashboard_Access/Managing_Dashboard_Administrators_and_Permissions",
             'note':"Built in Meraki dashboard"
         },
-        
+
         'dot1x':{
             'name': "802.1x",
             'support': "✓",
             'translatable':"",
             'regex': '^aaa authentication dot1x',
             'meraki': {
                 'skip': True
             },
             'iosxe': "dot1x = parse.find_objects('^aaa authentication dot1x')\n",
             'url':"https://documentation.meraki.com/MS/Access_Control/MS_Switch_Access_Policies_(802.1X)",
             'note':"Network-wide"
         },
-        
+
         'netflow':{
             'name': "NetFlow",
             'support':"✓",
             'translatable':"",
             'regex': '^flow\sexporter',
             'meraki': {
                 'skip': True
             },
             'iosxe': "netflow = parse.find_objects('^flow\sexporter')\n",
             'url':"https://documentation.meraki.com/MS/Monitoring_and_Reporting/MS_NetFlow_and_Encrypted_Traffic_Analytics",
             'note':"Network-wide"
         },
-        
+
         'dhcp':{
             'name':"DHCP server",
             'support':"✓",
             'translatable':"",
             'regex': '^ip\sdhcp\spool',
             'meraki': {
                 'skip': True
             },
             'iosxe':"dhcp = parse.find_objects('^ip\sdhcp\spool')\n"
         },
-        
+
         'banner':{
             'name': "Banner",
             'support':"",
             'translatable':"",
             'regex': '^banner',
             'meraki': {
                 'skip': True
             },
             'iosxe': "banner = parse.find_objects('^banner')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not required"
         },
-        
+
         'radius':{
             'name':"Radius",
             'support':"✓",
             'translatable':"",
             'regex': '^radius-server|^radius\sserver',
             'meraki': {
                 'skip': True
             },
             'iosxe':"radius = parse.find_objects('^radius-server|^radius\sserver')\n"
         },
-        
+
         'http_server':{
             'name': "HTTP server",
             'support':"",
             'translatable':"",
             'regex': '^ip\shttp',
             'meraki': {
                 'skip': True
             },
             'iosxe': "http_server = parse.find_objects('^ip\shttp')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not required"
         },
-        
+
         'stack':{
             'name': "Stack",
             'support':"✓",
             'translatable':"✓",
             'regex': '^switch',
             'meraki': {
                 'skip': True
             },
             'iosxe': "\
 stack = parse.find_objects('^switch')\n\
 if len(stack) == 1:\n\
     stack = []\n"
         },
-        
+
         'mab_vlan_mac':{
             'name': "MAB VLAN MAC Auth",
             'support':"",
             'translatable':"",
             'regex': '^mab\srequest\sformat',
             'meraki': {
                 'skip': True
             },
             'iosxe': "mab_vlan_mac = parse.find_objects('^mab\srequest\sformat')\n",
             'url':"https://documentation.meraki.com/MS/Access_Control/MS_Switch_Access_Policies_(802.1X)",
             'note':"MAB with RADIUS is supported"
         },
-        
+
         'vlan':{
             'name': "Layer 2 VLAN",
             'support':"",
             'translatable':"",
             'regex': '^vlan',
             'meraki': {
                 'skip': True
             },
             'iosxe': "vlan = parse.find_objects('^vlan')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Configured by default"
         },
-        
+
         'vmps':{
             'name': "VMPS",
             'support':"",
             'translatable':"",
             'regex': '^vpms',
             'meraki': {
                 'skip': True
             },
             'iosxe': "vmps = parse.find_objects('^vmps')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported as it is dated technology"
         },
-        
+
         'uplinkfast':{
             'name': "STP Uplinkfast",
             'support':"",
             'translatable':"",
             'regex': '^spanning-tree\suplinkfast',
             'meraki': {
                 'skip': True
             },
             'iosxe': "uplinkfast = parse.find_objects('^spanning-tree\suplinkfast')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'backbonefast':{
             'name': "STP Backbonefast",
             'support':"",
             'translatable':"",
             'regex': '^spanning-tree\sbackbonefast',
             'meraki': {
                 'skip': True
             },
             'iosxe': "backbonefast = parse.find_objects('^spanning-tree\sbackbonefast')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'loopguard':{
             'name': "STP Loopguard",
             'support':"",
             'translatable':"",
             'regex': '^vpms',
             'meraki': {
                 'skip': True
             },
             'iosxe': "loopguard = parse.find_objects('spanning-tree\sloopguard')\n",
             'note':"Supported at the port level"
         },
-        
+
         'dhcp_snooping':{
             'name': "DHCP Snooping",
             'support':"✓",
             'translatable':"",
             'regex': '^ip\sdhcp\ssnooping',
             'meraki': {
                 'skip': True
             },
             'iosxe': "dhcp_snooping = parse.find_objects('ip\sdhcp\ssnooping')\n",
             'url':"https://documentation.meraki.com/MS/Other_Topics/Dynamic_ARP_Inspection",
             'note':"Network-wide"
         },
-        
+
         'ip_source_guard':{
             'name': "IP Source Binding",
             'support':"",
             'translatable':"",
             'regex': '^ip\ssource\sbinding',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ip_source_guard = parse.find_objects('ip\ssource\sbinding')\n"
         },
-        
+
         'arp_inspection':{
             'name': "ARP Inspection",
             'support':"✓",
             'translatable':"",
             'regex': '^ip\sarp\sinspection',
             'meraki': {
                 'skip': True
             },
             'iosxe': "arp_inspection = parse.find_objects('^ip\sarp\sinspection')\n",
             'url':"https://documentation.meraki.com/MS/Other_Topics/Dynamic_ARP_Inspection",
             'note':"Network-wide"
         },
-        
+
         'arp_acl':{
             'name': "ARP Access-list",
             'support':"",
             'translatable':"",
             'regex': '^arp\saccess-list',
             'meraki': {
                 'skip': True
             },
             'iosxe': "arp_acl = parse.find_objects('^arp\saccess-list')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'psp':{
             'name': "Protocol Storm Protection",
             'support':"",
             'translatable':"",
             'regex': '^psp',
             'meraki': {
                 'skip': True
             },
             'iosxe': "psp = parse.find_objects('^psp')\n",
             'url': "https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'udld':{
             'name': "UDLD",
             'support':"",
             'translatable':"",
             'regex': '^udld',
             'meraki': {
                 'skip': True
             },
             'iosxe': "udld = parse.find_objects('^udld')\n",
             'note':"Supported at the port level"
         },
-        
+
         'logging':{
             'name': "Logging",
             'support':"",
             'translatable':"",
             'regex': '^logging',
             'meraki': {
                 'skip': True
             },
             'iosxe': "logging = parse.find_objects('^logging')\n",
             'url': "https://documentation.meraki.com/General_Administration/Cross-Platform_Content/Meraki_Event_Log",
             'note':"Configured by default"
         },
-        
+
         'ip_sla':{
             'name': "IP SLA",
             'support':"",
             'translatable':"",
             'regex': '^ip\ssla',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ip_sla = parse.find_objects('^ip\ssla')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'multicast_igmp':{
             'name': "Multicast IGMP",
             'support':"",
             'translatable':"",
             'regex': '^ip\sigm',
             'meraki': {
                 'skip': True
             },
             'iosxe': "multicast_igmp = parse.find_objects('^ip\sigmp')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Configured by default"
         },
-        
+
         'multicast_pim':{
             'name': "Multicast PIM",
             'support':"✓",
             'translatable':"",
             'regex': '^ip\spim',
             'meraki': {
                 'skip': True
             },
             'iosxe': "multicast_pim = parse.find_objects('^ip\spim')\n"
         },
-        
+
         'static_routing':{
             'name': "Static routing",
             'support':"✓",
             'translatable':"✓",
             'regex': '^ip\sroute|^ip\sdefault-gateway',
             'iosxe': "\
 static_routing = list()\n\
@@ -619,171 +619,171 @@
         if 'switchStackId' in switch_dict.keys():\n\
             dashboard.switch.createNetworkSwitchStackRoutingStaticRoute(switch_dict['networkId'],switch_dict['switchStackId'],route['subnet'],route['gw'])\n\
         else:\n\
             if len(sw_list) == 1:\n\
                 dashboard.switch.createDeviceSwitchRoutingStaticRoute(swlist[0],route['subnet'],route['gw'])\n"
             }
         },
-        
+
         'ipv6':{
             'name': "IPv6",
             'support':"✓",
             'translatable':"",
             'regex': '^ipv6',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ipv6 = parse.find_objects('^ipv6')\n"
         },
-        
+
         'rip':{
             'name': "RIP",
             'support':"",
             'translatable':"",
             'regex': '^router rip',
             'meraki': {
                 'skip': True
             },
             'iosxe': "rip = parse.find_objects('^router rip')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Not Supported"
         },
-        
+
         'eigrp':{
             'name': "EIGRP",
             'support':"",
             'translatable':"",
             'regex': '^router eigrp',
             'meraki': {
                 'skip': True
             },
             'iosxe': "eigrp = parse.find_objects('^router eigrp')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Not Supported"
         },
-        
+
         'ospf':{
             'name': "OSPFv2",
             'support':"✓",
             'translatable':"",
             'regex': '^router ospf',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ospf = parse.find_objects('^router ospf')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Supported on MS250 and above"
         },
-        
+
         'ospfv3':{
             'name': "OSPFv3",
             'support':"",
             'translatable':"",
             'regex': '^router ospfv3',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ospfv3 = parse.find_objects('^router ospfv3')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Not Supported"
         },
-        
+
         'bgp':{
             'name': "BGP",
             'support':"",
             'translatable':"",
             'regex': '^router bgp',
             'meraki': {
                 'skip': True
             },
             'iosxe': "bgp = parse.find_objects('^router bgp')\n",
             'url':"https://documentation.meraki.com/MX/Networks_and_Routing/Border_Gateway_Protocol_(BGP)",
             'note':"Currently supported on MX only"
         },
-        
+
         'isis':{
             'name': "IS-IS",
             'support':"",
             'translatable':"",
             'regex': '^router isis',
             'meraki': {
                 'skip': True
             },
             'iosxe': "isis = parse.find_objects('^router isis')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Not Supported"
         },
-        
+
         'vrf': {
             'name': "VRF",
             'support':"",
             'translatable':"",
             'regex': '^vpms',
             'meraki': {
                 'skip': True
             },
             'iosxe': "vrf = parse.find_objects('^vrf')\n",
             'url':"https://documentation.meraki.com/MS/Layer_3_Switching/MS_Layer_3_Switching_and_Routing",
             'note':"Not Supported"
         }
     },
-    
+
     'port': {
-        
+
         'name': {
             'name': "Port Description",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sdescription\s+(\S.+)',
             'meraki': {
                 'skip': False,
                 'default': ''
             },
             'iosxe': "name = child.re_match_typed(regex=r'\sdescription\s+(\S.+)')\n"
         },
-        
+
         'active': {
             'name': "Port Status",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\s(shutdown)',
             'meraki': {
                 'skip': False,
                 'default': 'true'
             },
             'iosxe': "\
 shut = child.re_match_typed(regex=r'\s(shutdown)')\n\
 active = 'true' if shut == '' else 'false'\n"
         },
-        
+
         'speed': {
             'name': "Port Speed",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sspeed\s+(\S.*)',
             'meraki': {
                 'skip': True,
                 'default': ''
             },
             'iosxe': "speed = child.re_match_typed(regex=r'\sspeed\s+(\S.*)')\n"
         },
-        
+
         'duplex': {
             'name': "Port Duplex",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sduplex\s+(\S.+)',
             'meraki': {
                 'skip': True,
                 'default': ''
             },
             'iosxe': "duplex = child.re_match_typed(regex=r'\sduplex\s+(\S.+)')\n",\
-            
+
         },
-        
+
         'linkNegotiation': {
             'iosxe': "",
             'regex': '',
             'meraki': {
                 'skip': 'post_process',
                 'default': 'Auto negotiate',
                 'post_process': "\
@@ -804,101 +804,103 @@
                 linkNegotiation += 'full duplex (forced)'\n\
     except KeyError:\n\
         linkNegotiation += '(auto)'\n\
 except:\n\
     linkNegotiation = 'Auto negotiate'\n"
             }
         },
-        
+
         'type': {
             'name': "Port Type",
             'support':"✓",
             'translatable':"✓",
-            'regex': r'\sswitchport\smode\s+(\S.+)',
+            'regex': r'\sswitchport\smode(?:\s\S+-\S+)?\s(access|trunk|host)',
             'meraki': {
                 'skip': False,
                 'default': 'trunk'
             },
-            'iosxe': "type = child.re_match_typed(regex=r'\sswitchport\smode\s+(\S.+)')\n"
+            'iosxe': "type = child.re_match_typed(regex=r'\sswitchport\smode(?:\s\S+-\S+)?\s(access|trunk|host)')\n\
+type = 'access' if type == 'host' else type\n"
         },
-        
+
         'poeEnabled': {
             'name': "PoE Enabled",
             'support':"✓",
             'translatable':"✓",
             'uplink':"",
             'regex': r'\spower\sinline\s+(\S.+)',
             'meraki': {
                 'skip': False,
                 'default': True
             },
             'iosxe': "poeEnabled = not child.re_match_typed(regex=r'\spower\sinline\s+(\S.+)')=='never'\n"
         },
-        
+
         'allowedVlans': {
             'name': "Allowed VLANs",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sswitchport\strunk\sallowed\svlan\s+(\S.*)',
             'meraki': {
                 'skip': False,
                 'default': '1-1000'
             },
             'iosxe': "allowedVlans = child.re_match_typed(regex=r'\sswitchport\strunk\sallowed\svlan\s+(\S.*)')\n"
         },
-        
+
         'vlan': {
             'name': "Native VLAN",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sswitchport\strunk\snative\svlan\s+(\S.*)',
             'meraki': {
                 'skip': False,
                 'default': '1'
             },
             'iosxe': "vlan = child.re_match_typed(regex=r'\sswitchport\strunk\snative\svlan\s+(\S.*)')\n"
         },
-        
+
         'vlan': {
             'name': "Data VLAN",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sswitchport\svlan\s+(\S.*)',
             'meraki': {
                 'skip': False,
                 'default': '1'
             },
             'iosxe': "vlan = child.re_match_typed(regex=r'\sswitchport\svlan\s+(\S.*)')\n"
         },
-        
+
         'voiceVlan': {
             'name': "Voice VLAN",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sswitchport\svoice\svlan\s+(\S.*)',
             'meraki': {
                 'skip': False,
                 'default': None
             },
             'iosxe': "voiceVlan = child.re_match_typed(regex=r'\sswitchport\svoice\svlan\s+(\S.*)')\n"
         },
-        
-        'private_vlan': {
+
+        'isolationEnabled': {
             'name': "Private VLAN",
-            'support':"",
-            'translatable':"",
+            'support':"✓",
+            'translatable':"✓",
             'regex': r'\sswitchport\smode\sprivate-vlan?(\S.*)',
             'meraki': {
-                'skip': True
+                'skip': False,
+                'default': False
             },
-            'iosxe': "private_vlan = child.re_match_typed(regex=r'\sswitchport\smode\sprivate-vlan?(\S.*)')\n",
+            'iosxe': "isolationEnabled = True if not child.re_match_typed(regex=r'\sswitchport\smode\sprivate-vlan?(\S.*)') == '' else False\n",
             'url':"https://documentation.meraki.com/MS/Port_and_VLAN_Configuration/Restricting_Traffic_with_Isolated_Switch_Ports",
             'note':"Port Isolation can be used"
         },
-        
+
         'l3_interface': {
             'name': "Layer 3 Interface",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sip\saddress\s(\S.*)',
             'meraki': {
                 'skip': 'post_ports',
@@ -944,51 +946,51 @@
             print(f'We had an issue creating {ma[2]}.')\n\
             unconf_ports.append(ma[2])\n\
     x+=1\n\
 return_vals = ['l3_ports','conf_ports','unconf_ports']\n"
             },
             'iosxe': "l3_interface = child.re_match_typed(regex=r'\sip\saddress\s(\S.*)')\n"
         },
-        
+
         'root_guard': {
             'name': "STP Root Guard",
             'support':"✓",
             'translatable':"✓",
             'iosxe': "root_guard = 'yes'\n",
             'regex': r'\sspanning-tree\sguard\sroot?(\S.+)',
             'meraki': {
                 'skip': True,
                 'default': ''
             }
         },
-        
+
         'loop_guard': {
             'name': "STP Loop Guard",
             'support':"✓",
             'translatable':"✓",
             'iosxe': "loop_guard = 'yes'\n",
             'regex': r'\sspanning-tree\sguard\sloop?(\S.+)',
             'meraki': {
                 'skip': True,
                 'default': ''
             }
         },
-        
+
         'bpdu_guard': {
             'name': "STP BPDU Guard",
             'support':"✓",
             'translatable':"✓",
             'iosxe': "bpdu_guard =  'yes'\n",
             'regex': r'\sspanning-tree\sbpduguard?(\S.+)',
             'meraki': {
                 'skip': True,
                 'default': ''
             }
         },
-        
+
         'stpGuard': {
             'iosxe': "",
             'regex': '',
             'meraki': {
                 'skip': 'post_process',
                 'post_process': "\
 \
@@ -1009,174 +1011,174 @@
 except:\n\
     pass\n\
 if debug:\n\
     print(f'stpGuard = {stpGuard}')\n",
                 'default': 'disabled'
             }
         },
-        
+
         'pruning': {
             'name': "Pruning",
             'support':"",
             'translatable':"",
             'regex': r'\sswitchport\strunk\spruning?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "pruning = child.re_match_typed(regex=r'\sswitchport\strunk\spruning?(\S.*)')\n",
             'url':"https://documentation.meraki.com/General_Administration/Tools_and_Troubleshooting/Fundamentals_of_802.1Q_VLAN_Tagging",
             'note':"Not required"
         },
-        
+
         'stp_port': {
             'name': "STP Port Priority",
             'support':"",
             'translatable':"",
             'regex': r'\sspanning-tree\sport-priority?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "stp_port = child.re_match_typed(regex=r'\sspanning-tree\sport-priority?(\S.*)')\n"
         },
-        
+
         'portfast': {
             'name': "STP Portfast",
             'support':"✓",
             'translatable':"✓",
             'regex': r'\sspanning-tree\sportfast?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "portfast = child.re_match_typed(regex=r'\sspanning-tree\sportfast?(\S.*)')\n",
             'url':"https://documentation.meraki.com/MS/Deployment_Guides/Advanced_MS_Setup_Guide",
             'note':"Automatic Edge Port"
         },
-        
+
         'storm_control': {
             'name': "Storm Control",
             'support':"",
             'translatable':"",
             'regex': r'\sstorm-control?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "storm_control = child.re_match_typed(regex=r'\sstorm-control?(\S.*)')\n",
             'url':"https://documentation.meraki.com/MS/Other_Topics/Storm_Control_for_MS",
             'note':"Configured network-wide"
         },
-        
+
         'protected': {
             'name': "Protected",
             'support':"✓",
             'translatable':"",
             'regex': r'\sswitchport\sprotected?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "protected = child.re_match_typed(regex=r'\sswitchport\sprotected?(\S.*)')\n",
             'url':"https://documentation.meraki.com/MS/Port_and_VLAN_Configuration/Restricting_Traffic_with_Isolated_Switch_Ports",
             'note':"Port Isolation"
         },
-        
+
         'port_security': {
             'name': "Port Security",
             'support':"✓",
             'translatable':"",
             'regex': r'\sswitchport\sport-security?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "port_security = child.re_match_typed(regex=r'\sswitchport\sport-security?(\S.*)')\n"
         },
-        
+
         'port_udld': {
             'name': "Port UDLD",
             'support':"✓",
             'translatable':"",
             'regex': r'\sudld\sport?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "port_udld = child.re_match_typed(regex=r'\sudld\sport?(\S.*)')\n"
         },
-        
+
         'lldp': {
             'name': "LLDP",
             'support':"",
             'translatable':"",
             'regex': r'\slldp?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "lldp = child.re_match_typed(regex=r'\slldp?(\S.*)')\n",
             'url':"https://documentation.meraki.com/General_Administration/Other_Topics/LLDP_Support_on_Cisco_Meraki_Products#ms",
             'note':"Always on"
         },
-        
+
         'ipv6': {
             'name': "IPv6",
             'support':"",
             'translatable':"",
             'regex': r'\sipv6?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "ipv6 = child.re_match_typed(regex=r'\sipv6?(\S.*)')\n",
             'url':"https://documentation.meraki.com/MS",
             'note':"Not Supported"
         },
-        
+
         'directed_broadcast': {
             'name': "IP Directed Broadcast",
             'support':"",
             'translatable':"",
             'regex': r'\sip\sdirected-broadcast?(\S.*)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "directed_broadcast = child.re_match_typed(regex=r'\sip\sdirected-broadcast?(\S.*)')\n"
         },
-        
+
         'etherchannel_cisco': {
             'name': "Etherchannel Classic",
             'support':"",
             'translatable':"",
             'regex': r'^\schannel-group\s\d+\smode\s(on)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "etherchannel_cisco = 'on'\n",
             'url':"https://documentation.meraki.com/General_Administration/Tools_and_Troubleshooting/Link_Aggregation_and_Load_Balancing",
             'note':"Only LACP is supported"
         },
-        
+
         'etherchannel_pagp': {
             'name': "Etherchannel PAgP",
             'support':"",
             'translatable':"",
             'regex': r'^\schannel-group\s\d+\smode\s(auto|desirable)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "etherchannel_pagp = child.re_match_typed('^\schannel-group\s\d+\smode\s(auto|desirable)')\n",
             'url':"https://documentation.meraki.com/General_Administration/Tools_and_Troubleshooting/Link_Aggregation_and_Load_Balancing",
             'note':"Only LACP is supported"
         },
-        
+
         'etherchannel_lacp': {
             'name': "Etherchannel LACP",
             'support':"✓",
             'translatable':"✓",
             'regex': r'^\schannel-group\s\d+\smode\s(active|passive)',
             'meraki': {
                 'skip': True
             },
             'iosxe': "etherchannel_lacp = child.re_match_typed('^\schannel-group\s(\d+)')\n"
         },
-        
+
         'etherchannel': {
             'iosxe': "",
             'regex': '',
             'meraki': {
                 'skip': 'post_ports',
                 'post_process': "\
 if 'etherchannel_lacp' in intf_settings:\n\
@@ -1256,29 +1258,29 @@
         continue\n\
     x+=1\n\
 return_vals = ['channel_port_dict']\n"
             }
         }
     },
     'layer3': {
-        
+
         'interfaceIp': {
             'iosxe': "",
             'regex': '',
             'meraki': {
                 'skip': 'post_process',
                 'post_process': "\
 interfaceIp = ''\n\
 if 'l3_interface' in intf_settings.keys():\n\
     import re\n\
     if not intf_settings['l3_interface'] == '':\n\
         interfaceIp = re.findall(r'(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})\s\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}', intf_settings['l3_interface'])[0]\n"
             }
         },
-        
+
         'subnet': {
             'iosxe': "",
             'regex': '',
             'meraki': {
                 'skip': 'post_process',
                 'post_process': "\
 if 'l3_interface' in intf_settings.keys():\n\
@@ -1560,17 +1562,17 @@
 }
 
 
 def index_mc_pedia(index_args):
     blurb = "\n\n\
 ==============================\n\
       Index of mc_pedia\n"
-    
+
     if len(index_args) == 0:
-        blurb+="     All Reportable Items\n"        
+        blurb+="     All Reportable Items\n"
     elif "support" in index_args:
         if "translatable" in index_args:
             blurb+="Supported & Translatable Items\n"
         else:
             blurb+="       Supported Items\n"
     elif "translatable" in index_args:
         blurb+="     Translatable Items\n"
```

### Comparing `merakicat-0.2.3/src/merakicat/mc_ping.py` & `merakicat-0.2.4/src/merakicat/mc_ping.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_register.py` & `merakicat-0.2.4/src/merakicat/mc_register.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_splitcheck_serials.py` & `merakicat-0.2.4/src/merakicat/mc_splitcheck_serials.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_translate.py` & `merakicat-0.2.4/src/merakicat/mc_translate.py`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/src/merakicat/mc_user_info.py` & `merakicat-0.2.4/src/merakicat/mc_user_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 # For netmiko to connect to a switch directly
 # IOS_USERNAME = "admin"
 # IOS_PASSWORD = "password"
 # IOS_SECRET = "secret"
 # IOS_PORT = 22
 
-# Webex Teams Bot Access Token for this Bot 
+# Webex Teams Bot Access Token for this Bot
 # TEAMS_BOT_TOKEN = "ZTZjMDc5ZTUtN2Q5NS00NzNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN2_PF84_1eb65fdf-9643-417f-9974-ad72cae0e10f"
 
-# Webex Teams Bot email address for this Bot 
+# Webex Teams Bot email address for this Bot
 # TEAMS_BOT_EMAIL = "mybot@webex.bot"
 
-# Webex Teams Bot email address for this Bot 
+# Webex Teams Bot email address for this Bot
 # TEAMS_BOT_APP_NAME = "My Bot"
 
 # Webex Teams user email who can access our bot
 # TEAMS_EMAILS = ["somebody@google.com"]
 
 # For meraki SDK to connect to a Dahsboard account
 # MERAKI_API_KEY = "99NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN90"
```

### Comparing `merakicat-0.2.3/src/merakicat/merakicat.py` & `merakicat-0.2.4/src/merakicat/merakicat.py`

 * *Files 3% similar despite different names*

```diff
@@ -289,15 +289,15 @@
         print(f"meraki_orgs = {meraki_orgs}")
     x = 0
     while x <= len(meraki_orgs) - 1:
         if meraki_orgs[x]['name'] == meraki_org_name:
             try:
                 raw_nets = dashboard.organizations.getOrganizationNetworks(
                     organizationId=meraki_orgs[x]['id'])
-    
+
             except meraki.exceptions.APIError:
                 print("We were unable to get the list of networks" +
                       f" for {meraki_orgs[x]['name']}.")
                 sys.exit()
             if debug:
                 print(raw_nets)
             y = 0
@@ -336,56 +336,36 @@
         if not bot_app_name:
             print("TEAMS_BOT_APP_NAME")
         if not bot_url:
             print("TEAMS_BOT_URL")
         sys.exit()
 
     # Create a Bot Object
-    #   Note: debug mode prints out more details about processing to terminal
-    #   Note: the `approved_users=approved_users` line commented out and shown
-    #   as reference
     #
     # Example: How to limit the approved Webex Teams accounts for interaction
     # List of email accounts of approved users to talk with the bot
     # approved_users = [
     #     "josmith@demo.local",
     # ]
 
     if debug:
         print(f"teams_emails = {teams_emails}")
 
-    """
-    bot = TeamsBot(
-        bot_app_name,
-        teams_bot_token=teams_token,
-        teams_bot_url=bot_url,
-        teams_bot_email=bot_email,
-        debug=debug,
-        # Comment out the approved_users lines if you don't care...
-        approved_users=teams_emails,
-        webhook_resource_event=[
-            {"resource": "messages", "event": "created"},
-            {"resource": "attachmentActions", "event": "created"},
-        ],
-    )
-    """
     bot = WebexBot(
         teams_token,
         bot_name=bot_app_name,
         # Comment out the approved_users lines if you don't care...
         approved_users=teams_emails,
         # approved_domains=[],
         # approved_rooms=[],
         threads=False,
         help_command=RunHelp(),
         log_level="ERROR"
     )
 
-
-
 # Create a custom bot greeting function, returned when no /command is given.
 # The default behavior of the bot is to return the '/help' command response
 # If there is an English language command line, try to work with that.
 
 
 def greeting(incoming_msg):
 
@@ -409,14 +389,15 @@
 
     if BOT:
         # If first word from the user's input was Bot's first name, remove it
         if user_text.split()[0] == bot_fname:
             user_text = user_text.split(bot_fname + ' ', 1)[1]
 
     if debug:
+        print(f"user_text = {user_text}")
         print(f"command = {command}")
 
     # If the user asked for timing, we will try to give it to them
     times = False
     regex = r'\swith\stimings|\swith\stiming|\swith\stime|\swith\stimes'
     if re.search(regex, user_text, re.IGNORECASE) is not None:
         user_text = re.sub(regex, '', user_text, re.IGNORECASE)
@@ -1299,15 +1280,15 @@
 
     start_time = time.time()
     timing = ""
 
     # Import the global stateful variables
     global host_id, times
 
-    # Since we weren't passed a config filespec, check for a hostname or 
+    # Since we weren't passed a config filespec, check for a hostname or
     # IP address
     if host == "":
         return ("You need to enter a host FQDN or IP address.")
     else:
         # We were passed a hostname or IP address...
         # Update the global stateful variable for later
         host_id = host
@@ -2169,65 +2150,14 @@
          "Migrate a Catalyst switch to a Meraki switch - register, claim & \
 translate"],
 
         ["* **demo report**",
          "Create a demo report for all features currently in the feature \
 encyclopedia"]])
 
-    """
-    bot.add_command("help", "This list of commands", greeting)
-
-    bot.add_command("check [host _FQDN or IP address_ | file _filespec_] \
-[with timing] [with details]",
-                    "Check a Catalyst switch config for both translatable \
-and possible Meraki features",
-                    greeting)
-
-    bot.add_command("check _drag-and-drop files_ [with timing] [with details]\
-",
-                    "Check one or more Catalyst switch config files for both \
-translatable and possible Meraki features",
-                    greeting)
-
-    bot.add_command("check [network _Meraki network_] [with timing] \
-[with details]",
-                    "Check the configs of cloud monitored Catalyst switches \
-for both translatable and possible Meraki features",
-                    greeting)
-
-    bot.add_command("register [host _FQDN or IP address_] [with timing]",
-                    "Register a Catalyst switch to the Meraki Dashboard",
-                    greeting)
-
-    bot.add_command("claim [_Meraki serial numbers_] [to _Meraki network \
-name_] [with timing]",
-                    "Claim Catalyst switches to a Meraki Network",
-                    greeting)
-
-    bot.add_command("translate [host _FQDN or IP address_ | file _filespec_] \
-[to _Meraki serial numbers_] [with timing]",
-                    "Translate a Catalyst switch config from a file or host \
-to claimed Meraki serial numbers",
-                    greeting)
-
-    bot.add_command("migrate [host _FQDN or IP address_] [to _Meraki network \
-name_] [with timing]",
-                    "Migrate a Catalyst switch to a Meraki switch - register,\
- claim & translate",
-                    greeting)
-
-    bot.add_command("demo report",
-                    "Create a demo report for all features currently in the \
-feature encyclopedia",
-                    greeting)
-
-    # Every bot includes a default "/echo" command.  You can remove it, or any
-    # other command with the remove_command(command) method.
-    bot.remove_command("/echo")
-    """
     bot.add_command(RunHelp())
     bot.add_command(RunCheck())
     bot.add_command(RunRegister())
     bot.add_command(RunClaim())
     bot.add_command(RunTranslate())
     bot.add_command(RunMigrate())
     bot.add_command(RunDemo())
```

### Comparing `merakicat-0.2.3/src/merakicat.egg-info/PKG-INFO` & `merakicat-0.2.4/src/merakicat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merakicat
-Version: 0.2.3
+Version: 0.2.4
 Summary: An app to check and translate Catalyst switch configs to Meraki.
 Home-page: https://github.com/ecoen66/merakicat
 Author: Ed Coen
 Author-email: ecoen@cisco.com
 License: MIT license
 Keywords: merakicat,catalyst,meraki,cisco,migration,webexteamsbot
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,17 +28,17 @@
 Requires-Dist: docx2pdf==0.1.8
 Requires-Dist: requests==2.31.0
 
 [![published](https://static.production.devnetcloud.com/codeexchange/assets/images/devnet-published.svg)](https://developer.cisco.com/codeexchange/github/repo/ecoen66/merakicat)
 # ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/merakicat.png) merakicat
 
 This package makes migrating [Cisco](https://www.cisco.com) Catalyst switches to [Meraki](https:www.meraki.com) Dashboard much easier. #merakicat
- 
+
 ![merakicat](https://github.com/ecoen66/merakicat/raw/main/images/mc_quick.gif)
- 
+
 This Python app can be run in Webex Teams [Bot mode](#Bot) or in [command-line mode](#command-line).  It can also be called from shell scripts for [bulk-mode](#bulk-mode).
 
 Below is the list of configurations the tool can currently translate:
 
 switch:
  - Hostname
  - Spanning Tree RSTP
@@ -51,22 +51,23 @@
  - Port Speed
  - Port Duplex
  - Port Type
  - PoE Enabled
  - Allowed VLANs
  - Data VLAN
  - Voice VLAN
+ - Private VLAN
  - Layer 3 Interface
  - STP RootGuard
  - STP Loop Guard
  - STP BPDU Guard
  - Etherchannel LACP
  - NM Ports
 
- 
+
 Once installed, you can print the entire index of the feature encyclopedia, or to print the index based on either supported and translatable items or both, enter:
 ```
 cd src/merakicat
 python mc_pedia [support] [translatable]
 ```
 
 # Prerequisites for using in Bot mode
@@ -115,30 +116,30 @@
 
     ```
     # These exports are used for Webex bot mode:
     export TEAMS_BOT_TOKEN=<your bot's token>
     export TEAMS_BOT_EMAIL=<your bot's email>
     export TEAMS_BOT_APP_NAME=<your bot's name>
     export TEAMS_EMAILS=<a comma delimited list of email addresses the bot will respond to>
-    
+
     # These exports are required regardless of mode:
     export IOS_USERNAME=<the ssh username for the Catalyst switches>
     export IOS_PASSWORD=<the ssh password for the Catalyst switches>
     export IOS_SECRET=<the CLI secret password for the Catalyst switches>
     export IOS_PORT=<the ssh port number for the Catalyst switches - usually 22>
     export MERAKI_API_KEY=<your meraki dashboard API key>
     export MERAKI_ORG_NAME =<your meraki organization name>
     ```
 In addition to these settings, various debugs and a choice of PDF vs. DOCX report format can be enabled in the mc_user_info.py file.
 
     > Note: For PDF report generation, MS Word must be installed on the host with merakicat.
 
 # Bot
 
-To run merakicat as a Bot, just start it without any parameters:  
+To run merakicat as a Bot, just start it without any parameters:
 
 ```
 cd src/merakicat
 python merakicat.py
 ```
 **Bot commands include the following:**
 
@@ -241,14 +242,21 @@
 `Catalyst_2_Meraki_Config_Checker` by [Fady Sharobeem](https://github.com/fadysharobeem).
 
 The bot functionality is based on the `webex_bot` project by [Finbarr Brady](https://github.com/fbradyirl).
 
 
 # History
 
+## 0.2.4 (04-12-2024)
+
+  - Added Private VLAN -> Port Isolation to encyclopedia.
+  - Removed older bot code.
+  - Updated AUTHORS.rst.
+  - Updated .gitignore
+
 ## 0.2.3 (04-10-2024)
 
   - Translate now checks to make sure that the target switches have the same number of ports as the sources.
 
 ## 0.2.2 (04-10-2024)
 
   - Added environment variable to specify a Meraki Oragnization name.
@@ -290,54 +298,54 @@
 
 ## 0.1.3 (03-21-2024)
 
   - Code beautification with flake8.
   - Setting up for publishing automation.
   - Changed directory structure for publishing.
   - Released on PyPI.
-  
+
 ## 0.0.14 (03-19-2024)
 
   - Option added for check with drag and drop files in bot mode.
   - Added missing timing in check report in bot mode.
   - Still not yet released on PyPI.
-  
+
 ## 0.0.13 (03-18-2024)
 
   - Option added for detailed check report "with detail".
-  
+
 ## 0.0.12 (03-15-2024)
 
   - Option for PDF vs. DOCX reporting in checker.
   - Layer 3 Interfaces (interface VLAN) supported.
   - Static routes supported.
   - Command added for "demo report".
-  
+
 ## 0.0.11 (03-12-2024)
 
   - New reporting in checker.
   - Port-channel LACP is working and fast.
-  
+
 ## 0.0.10 (03-08-2024)
 
   - Using a single mc_pedia.
-  
+
 ## 0.0.9 (03-07-2024)
 
   - Using both config_pedia and check_pedia.
   - Changed to ngrok API for bot functionality
-  
+
 ## 0.0.8 (03-01-2024)
 
   - Lots of comment blocks added.
-  
+
 ## 0.0.7 (03-01-2024)
 
   - Now using batch port updates to Meraki dashboard.
-  
+
 ## 0.0.6 (03-01-2024)
 
   - Some light refactoring of mc_translate module.
   - More prep work for Uplink config.
 
 ## 0.0.5 (02-29-2024)
```

### Comparing `merakicat-0.2.3/src/merakicat.egg-info/SOURCES.txt` & `merakicat-0.2.4/src/merakicat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merakicat-0.2.3/tox.ini` & `merakicat-0.2.4/tox.ini`

 * *Files identical despite different names*

