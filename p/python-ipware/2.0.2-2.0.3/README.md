# Comparing `tmp/python-ipware-2.0.2.tar.gz` & `tmp/python-ipware-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ipware-2.0.2.tar", last modified: Thu Feb 29 15:45:42 2024, max compression
+gzip compressed data, was "python-ipware-2.0.3.tar", last modified: Thu Apr 11 23:10:05 2024, max compression
```

## Comparing `python-ipware-2.0.2.tar` & `python-ipware-2.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:42.293990 python-ipware-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-29 15:45:34.000000 python-ipware-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14809 2024-02-29 15:45:42.293990 python-ipware-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13507 2024-02-29 15:45:34.000000 python-ipware-2.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-29 15:45:34.000000 python-ipware-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:42.293990 python-ipware-2.0.2/python_ipware/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-29 15:45:34.000000 python-ipware-2.0.2/python_ipware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 15:45:34.000000 python-ipware-2.0.2/python_ipware/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:34.000000 python-ipware-2.0.2/python_ipware/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-02-29 15:45:34.000000 python-ipware-2.0.2/python_ipware/python_ipware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:42.293990 python-ipware-2.0.2/python_ipware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14809 2024-02-29 15:45:42.000000 python-ipware-2.0.2/python_ipware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-29 15:45:42.000000 python-ipware-2.0.2/python_ipware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 15:45:42.000000 python-ipware-2.0.2/python_ipware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-29 15:45:42.000000 python-ipware-2.0.2/python_ipware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-29 15:45:42.000000 python-ipware-2.0.2/python_ipware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 15:45:42.293990 python-ipware-2.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:45:42.293990 python-ipware-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-02-29 15:45:34.000000 python-ipware-2.0.2/tests/tests_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-02-29 15:45:34.000000 python-ipware-2.0.2/tests/tests_ipv6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-11 23:09:55.000000 python-ipware-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-11 23:10:05.723339 python-ipware-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13550 2024-04-11 23:09:55.000000 python-ipware-2.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-11 23:09:55.000000 python-ipware-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/python_ipware/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-11 23:09:55.000000 python-ipware-2.0.3/python_ipware/python_ipware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/python_ipware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14852 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 23:10:05.000000 python-ipware-2.0.3/python_ipware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:10:05.723339 python-ipware-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:05.723339 python-ipware-2.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14756 2024-04-11 23:09:55.000000 python-ipware-2.0.3/tests/tests_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-11 23:09:55.000000 python-ipware-2.0.3/tests/tests_ipv6.py
```

### Comparing `python-ipware-2.0.2/LICENSE` & `python-ipware-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ipware-2.0.2/PKG-INFO` & `python-ipware-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
@@ -130,14 +130,15 @@
     "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
     "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_FORWARDED",  # Squid and others
     "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
     "HTTP_FORWARDED_FOR",  # RFC 7239
     "HTTP_FORWARDED",  # RFC 7239
+    "HTTP_CF_CONNECTING_IP",  # CloudFlare
     "X-CLIENT-IP",  # Microsoft Azure
     "X-REAL-IP",  # NGINX
     "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
     "X_FORWARDED",  # Squid
     "FORWARDED_FOR",  # RFC 7239
     "CF-CONNECTING-IP",  # CloudFlare
     "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `python-ipware-2.0.2/README.md` & `python-ipware-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
     "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_FORWARDED",  # Squid and others
     "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
     "HTTP_FORWARDED_FOR",  # RFC 7239
     "HTTP_FORWARDED",  # RFC 7239
+    "HTTP_CF_CONNECTING_IP",  # CloudFlare
     "X-CLIENT-IP",  # Microsoft Azure
     "X-REAL-IP",  # NGINX
     "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
     "X_FORWARDED",  # Squid
     "FORWARDED_FOR",  # RFC 7239
     "CF-CONNECTING-IP",  # CloudFlare
     "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `python-ipware-2.0.2/pyproject.toml` & `python-ipware-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-ipware-2.0.2/python_ipware/python_ipware.py` & `python-ipware-2.0.3/python_ipware/python_ipware.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
             "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
             "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
             "HTTP_X_FORWARDED",  # Squid and others
             "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
             "HTTP_FORWARDED_FOR",  # RFC 7239
             "HTTP_FORWARDED",  # RFC 7239
+            "HTTP_CF_CONNECTING_IP",  # CloudFlare
             "X-CLIENT-IP",  # Microsoft Azure
             "X-REAL-IP",  # NGINX
             "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
             "X_FORWARDED",  # Squid
             "FORWARDED_FOR",  # RFC 7239
             "CF-CONNECTING-IP",  # CloudFlare
             "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `python-ipware-2.0.2/python_ipware.egg-info/PKG-INFO` & `python-ipware-2.0.3/python_ipware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ipware
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python package to retrieve user's IP address
 Author-email: Val Neekman <info@neekware.com>
 License: MIT
 Project-URL: Documentation, https://github.com/un33k/python-ipware#readme
 Project-URL: Issues, https://github.com/un33k/python-ipware/issues
 Project-URL: Source, https://github.com/un33k/python-ipware
 Project-URL: Changelog, https://github.com/un33k/python-ipware/blob/main/CHANGELOG.md
@@ -130,14 +130,15 @@
     "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
     "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
     "HTTP_X_FORWARDED",  # Squid and others
     "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
     "HTTP_FORWARDED_FOR",  # RFC 7239
     "HTTP_FORWARDED",  # RFC 7239
+    "HTTP_CF_CONNECTING_IP",  # CloudFlare
     "X-CLIENT-IP",  # Microsoft Azure
     "X-REAL-IP",  # NGINX
     "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
     "X_FORWARDED",  # Squid
     "FORWARDED_FOR",  # RFC 7239
     "CF-CONNECTING-IP",  # CloudFlare
     "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `python-ipware-2.0.2/tests/tests_ipv4.py` & `python-ipware-2.0.3/tests/tests_ipv4.py`

 * *Files identical despite different names*

### Comparing `python-ipware-2.0.2/tests/tests_ipv6.py` & `python-ipware-2.0.3/tests/tests_ipv6.py`

 * *Files identical despite different names*

