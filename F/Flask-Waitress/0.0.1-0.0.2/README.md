# Comparing `tmp/Flask-Waitress-0.0.1.tar.gz` & `tmp/Flask-Waitress-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Waitress-0.0.1.tar", last modified: Tue May 28 22:30:03 2019, max compression
+gzip compressed data, was "Flask-Waitress-0.0.2.tar", last modified: Fri Apr 12 10:01:03 2024, max compression
```

## Comparing `Flask-Waitress-0.0.1.tar` & `Flask-Waitress-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/
-drwxr-xr-x   0 c         (1000) c         (1000)        0 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/
--rw-r--r--   0 c         (1000) c         (1000)      339 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/PKG-INFO
--rw-r--r--   0 c         (1000) c         (1000)      226 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/SOURCES.txt
--rw-r--r--   0 c         (1000) c         (1000)        1 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/dependency_links.txt
--rw-r--r--   0 c         (1000) c         (1000)       31 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/requires.txt
--rw-r--r--   0 c         (1000) c         (1000)       15 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/Flask_Waitress.egg-info/top_level.txt
--rw-r--r--   0 c         (1000) c         (1000)      339 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/PKG-INFO
--rw-r--r--   0 c         (1000) c         (1000)       64 2019-05-28 22:26:05.000000 Flask-Waitress-0.0.1/README.txt
--rw-r--r--   0 c         (1000) c         (1000)      863 2019-05-28 22:26:30.000000 Flask-Waitress-0.0.1/flask_waitress.py
--rw-r--r--   0 c         (1000) c         (1000)       38 2019-05-28 22:30:03.000000 Flask-Waitress-0.0.1/setup.cfg
--rw-r--r--   0 c         (1000) c         (1000)      475 2019-05-28 22:23:41.000000 Flask-Waitress-0.0.1/setup.py
+drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-12 10:01:03.528963 Flask-Waitress-0.0.2/
+drwxr-xr-x   0 c         (1000) c         (1000)        0 2024-04-12 10:01:03.528963 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/
+-rw-r--r--   0 c         (1000) c         (1000)      365 2024-04-12 10:01:03.000000 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/PKG-INFO
+-rw-r--r--   0 c         (1000) c         (1000)      238 2024-04-12 10:01:03.000000 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/SOURCES.txt
+-rw-r--r--   0 c         (1000) c         (1000)        1 2024-04-12 10:01:03.000000 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/dependency_links.txt
+-rw-r--r--   0 c         (1000) c         (1000)       31 2024-04-12 10:01:03.000000 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/requires.txt
+-rw-r--r--   0 c         (1000) c         (1000)       15 2024-04-12 10:01:03.000000 Flask-Waitress-0.0.2/Flask_Waitress.egg-info/top_level.txt
+-rw-r--r--   0 c         (1000) c         (1000)     1831 2024-04-12 00:48:10.000000 Flask-Waitress-0.0.2/LICENSE.txt
+-rw-r--r--   0 c         (1000) c         (1000)      365 2024-04-12 10:01:03.528963 Flask-Waitress-0.0.2/PKG-INFO
+-rw-r--r--   0 c         (1000) c         (1000)       64 2024-04-12 00:48:10.000000 Flask-Waitress-0.0.2/README.txt
+-rw-r--r--   0 c         (1000) c         (1000)      900 2024-04-12 00:50:49.000000 Flask-Waitress-0.0.2/flask_waitress.py
+-rw-r--r--   0 c         (1000) c         (1000)       38 2024-04-12 10:01:03.528963 Flask-Waitress-0.0.2/setup.cfg
+-rw-r--r--   0 c         (1000) c         (1000)      476 2024-04-12 00:50:59.000000 Flask-Waitress-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-Waitress-0.0.1/flask_waitress.py` & `Flask-Waitress-0.0.2/flask_waitress.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,8 +19,8 @@
                            self.waitress_serve)
         app.cli.command()(command_func)
 
     def waitress_serve(self, app):
         port = current_app.config['PORT']
         address = current_app.config['SERVER_ADDRESS']
         bind = '{address}:{port}'.format(address=address, port=port)
-        return waitress.serve(TransLogger(app), listen=bind)
+        return waitress.serve(TransLogger(app), listen=bind, clear_untrusted_proxy_headers=False)
```

