# Comparing `tmp/linkwiz-0.2.3.tar.gz` & `tmp/linkwiz-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkwiz-0.2.3.tar", max compression
+gzip compressed data, was "linkwiz-0.2.4.tar", max compression
```

## Comparing `linkwiz-0.2.3.tar` & `linkwiz-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    18092 2024-03-22 03:44:25.505161 linkwiz-0.2.3/LICENSE
--rw-r--r--   0        0        0      978 2024-03-29 14:28:36.318957 linkwiz-0.2.3/README.md
--rw-r--r--   0        0        0        0 2024-03-22 03:44:25.505161 linkwiz-0.2.3/linkwiz/__init__.py
--rw-r--r--   0        0        0      585 2024-03-29 15:05:24.259476 linkwiz-0.2.3/linkwiz/__main__.py
--rw-r--r--   0        0        0     1787 2024-03-29 14:58:49.114500 linkwiz-0.2.3/linkwiz/browser.py
--rw-r--r--   0        0        0     2774 2024-03-29 14:58:35.684558 linkwiz-0.2.3/linkwiz/config.py
--rw-r--r--   0        0        0     1141 2024-03-29 15:05:37.469420 linkwiz-0.2.3/linkwiz/core.py
--rw-r--r--   0        0        0     4007 2024-03-22 03:44:25.508495 linkwiz-0.2.3/linkwiz/gui.py
--rw-r--r--   0        0        0     1259 2024-03-29 14:09:22.480561 linkwiz-0.2.3/linkwiz/install.py
--rw-r--r--   0        0        0     1360 2024-03-22 03:44:25.508495 linkwiz-0.2.3/linkwiz/launch.py
--rw-r--r--   0        0        0      864 2024-03-23 07:56:43.483437 linkwiz-0.2.3/linkwiz/match.py
--rw-r--r--   0        0        0      675 2024-03-29 15:06:25.829213 linkwiz-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 linkwiz-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-10 02:50:31.877024 linkwiz-0.2.4/LICENSE
+-rw-r--r--   0        0        0      997 2024-04-10 02:50:31.877024 linkwiz-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 02:50:31.877024 linkwiz-0.2.4/linkwiz/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-10 02:50:31.880357 linkwiz-0.2.4/linkwiz/__main__.py
+-rw-r--r--   0        0        0     1812 2024-04-10 02:54:43.833742 linkwiz-0.2.4/linkwiz/browser.py
+-rw-r--r--   0        0        0     2774 2024-04-10 02:50:31.880357 linkwiz-0.2.4/linkwiz/config.py
+-rw-r--r--   0        0        0     1300 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/core.py
+-rw-r--r--   0        0        0     4007 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/gui.py
+-rw-r--r--   0        0        0     1259 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/install.py
+-rw-r--r--   0        0        0     1360 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/launch.py
+-rw-r--r--   0        0        0      853 2024-04-10 02:52:35.310383 linkwiz-0.2.4/linkwiz/match.py
+-rw-r--r--   0        0        0      676 2024-04-12 09:07:34.567234 linkwiz-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 linkwiz-0.2.4/PKG-INFO
```

### Comparing `linkwiz-0.2.3/LICENSE` & `linkwiz-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/README.md` & `linkwiz-0.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,7 +31,9 @@
 "*.google.com" = "Google Chrome" # This will not match "google.com"
 
 [rules.hostname]
 "example.com" = "Brave Private"
 "github.com" = "Firefox Developer Edition"
 "google.com" = "Google Chrome"
 ```
+## TODO
+- [ ] RIIR
```

### Comparing `linkwiz-0.2.3/linkwiz/__main__.py` & `linkwiz-0.2.4/linkwiz/__main__.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/linkwiz/browser.py` & `linkwiz-0.2.4/linkwiz/browser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from pathlib import Path
 import subprocess
 from typing import Dict, List
 from xdg import DesktopEntry
 from linkwiz.config import config
 
 APPNAME: str = "LinkWiz"
@@ -27,15 +28,16 @@
             own_desktop = f"{APPNAME.lower()}.desktop"
 
             if own_desktop in installed_browsers:
                 installed_browsers.remove(own_desktop)
 
         return get_browser_exec(installed_browsers)
     except subprocess.CalledProcessError:
-        raise ("Error: Unable to retrieve installed browsers.")
+        logging.error("Error getting installed browsers")
+        exit(1)
 
 
 def get_browser_exec(browsers_desktop: List[str]) -> Dict[str, Path]:
     """Get the exec path of installed browsers."""
     installed_browsers: Dict[str, Path] = {}
     for path in DESKTOP_PATHS:
         if not path.exists():
```

### Comparing `linkwiz-0.2.3/linkwiz/config.py` & `linkwiz-0.2.4/linkwiz/config.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/linkwiz/core.py` & `linkwiz-0.2.4/linkwiz/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,10 +33,13 @@
 
     except Exception as e:
         logging.error(f"Error processing URL: {e}")
 
 
 def remove_tracking(url):
     """Remove tracking parameters from the URL."""
-    import unalix
-
-    return unalix.clear_url(url=url)
+    try:
+        import unalix
+        return unalix.clear_url(url=url)
+    except ImportError:
+        logging.warning("The 'unalix' package is not installed. Cannot remove tracking parameters.")
+        return url
```

### Comparing `linkwiz-0.2.3/linkwiz/gui.py` & `linkwiz-0.2.4/linkwiz/gui.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/linkwiz/install.py` & `linkwiz-0.2.4/linkwiz/install.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/linkwiz/launch.py` & `linkwiz-0.2.4/linkwiz/launch.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.3/linkwiz/match.py` & `linkwiz-0.2.4/linkwiz/match.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         for pattern, browser in config.rules_fnmatch.items():
             if fnmatch.fnmatch(hostname, pattern):
                 logging.info(f"Matched {hostname} to {browser}")
                 return browser
         return config.rules_hostname.get(hostname, None)
     except Exception as e:
         logging.warning(f"Error matching {hostname} to {pattern}: {e}")
-    return
 
 
 def find_matching_browser(browsers, url, hostname):
     browser = get_browser_for_url(hostname)
     if browser is None:
         logging.info(f"No match for {url}")
         return
```

### Comparing `linkwiz-0.2.3/pyproject.toml` & `linkwiz-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkwiz"
-version = "0.2.3"
+version = "0.2.4"
 description = "LinkWiz is a Linux tool that lets users select their preferred browser for opening links."
 authors = ["Rin <icealtria+github@gmail.com>"]
 license = "GPL-2.0-only"
 readme = "README.md"
 repository = "https://github.com/icealtria/linkwiz"
 classifiers = [
     "Operating System :: POSIX :: Linux",
@@ -18,8 +18,8 @@
 unalix-rev = "^0.9.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-linkwiz = "linkwiz.__main__:main"
+linkwiz = "linkwiz.__main__:main"
```

### Comparing `linkwiz-0.2.3/PKG-INFO` & `linkwiz-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkwiz
-Version: 0.2.3
+Version: 0.2.4
 Summary: LinkWiz is a Linux tool that lets users select their preferred browser for opening links.
 Home-page: https://github.com/icealtria/linkwiz
 License: GPL-2.0-only
 Author: Rin
 Author-email: icealtria+github@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -51,8 +51,10 @@
 "*.google.com" = "Google Chrome" # This will not match "google.com"
 
 [rules.hostname]
 "example.com" = "Brave Private"
 "github.com" = "Firefox Developer Edition"
 "google.com" = "Google Chrome"
 ```
+## TODO
+- [ ] RIIR
```

