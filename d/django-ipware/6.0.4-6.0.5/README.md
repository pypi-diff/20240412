# Comparing `tmp/django-ipware-6.0.4.tar.gz` & `tmp/django-ipware-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipware-6.0.4.tar", last modified: Sun Feb  4 19:30:38 2024, max compression
+gzip compressed data, was "django-ipware-6.0.5.tar", last modified: Thu Apr 11 23:38:35 2024, max compression
```

## Comparing `django-ipware-6.0.4.tar` & `django-ipware-6.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-02-04 19:30:38.840431 django-ipware-6.0.4/
--rw-r--r--   0 val        (501) staff       (20)     1103 2023-10-02 23:45:14.000000 django-ipware-6.0.4/LICENSE
--rw-r--r--   0 val        (501) staff       (20)     8972 2024-02-04 19:30:38.840504 django-ipware-6.0.4/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)     8119 2023-11-29 16:43:30.000000 django-ipware-6.0.4/README.md
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-02-04 19:30:38.839613 django-ipware-6.0.4/django_ipware.egg-info/
--rw-r--r--   0 val        (501) staff       (20)     8972 2024-02-04 19:30:38.000000 django-ipware-6.0.4/django_ipware.egg-info/PKG-INFO
--rw-r--r--   0 val        (501) staff       (20)      340 2024-02-04 19:30:38.000000 django-ipware-6.0.4/django_ipware.egg-info/SOURCES.txt
--rw-r--r--   0 val        (501) staff       (20)        1 2024-02-04 19:30:38.000000 django-ipware-6.0.4/django_ipware.egg-info/dependency_links.txt
--rw-r--r--   0 val        (501) staff       (20)        1 2023-11-23 00:20:32.000000 django-ipware-6.0.4/django_ipware.egg-info/not-zip-safe
--rw-r--r--   0 val        (501) staff       (20)       21 2024-02-04 19:30:38.000000 django-ipware-6.0.4/django_ipware.egg-info/requires.txt
--rw-r--r--   0 val        (501) staff       (20)        7 2024-02-04 19:30:38.000000 django-ipware-6.0.4/django_ipware.egg-info/top_level.txt
-drwxr-xr-x   0 val        (501) staff       (20)        0 2024-02-04 19:30:38.840239 django-ipware-6.0.4/ipware/
--rw-r--r--   0 val        (501) staff       (20)       87 2023-10-02 23:45:14.000000 django-ipware-6.0.4/ipware/__init__.py
--rw-r--r--   0 val        (501) staff       (20)      319 2024-02-04 19:26:02.000000 django-ipware-6.0.4/ipware/__version__.py
--rw-r--r--   0 val        (501) staff       (20)      250 2023-10-02 23:45:14.000000 django-ipware-6.0.4/ipware/apps.py
--rw-r--r--   0 val        (501) staff       (20)     1205 2024-02-04 19:26:02.000000 django-ipware-6.0.4/ipware/ip.py
--rw-r--r--   0 val        (501) staff       (20)      502 2023-11-23 00:20:01.000000 django-ipware-6.0.4/pyproject.toml
--rw-r--r--   0 val        (501) staff       (20)       73 2024-02-04 19:30:38.840833 django-ipware-6.0.4/setup.cfg
--rw-r--r--   0 val        (501) staff       (20)     2344 2024-02-04 18:02:08.000000 django-ipware-6.0.4/setup.py
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.411474 django-ipware-6.0.5/
+-rw-r--r--   0 val        (501) staff       (20)     1103 2023-10-02 23:45:14.000000 django-ipware-6.0.5/LICENSE
+-rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-11 23:38:35.411549 django-ipware-6.0.5/PKG-INFO
+-rw-r--r--   0 val        (501) staff       (20)     8160 2024-04-11 23:36:17.000000 django-ipware-6.0.5/README.md
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.410925 django-ipware-6.0.5/django_ipware.egg-info/
+-rw-r--r--   0 val        (501) staff       (20)     9013 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/PKG-INFO
+-rw-r--r--   0 val        (501) staff       (20)      340 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/SOURCES.txt
+-rw-r--r--   0 val        (501) staff       (20)        1 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/dependency_links.txt
+-rw-r--r--   0 val        (501) staff       (20)        1 2023-11-23 00:20:32.000000 django-ipware-6.0.5/django_ipware.egg-info/not-zip-safe
+-rw-r--r--   0 val        (501) staff       (20)       21 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/requires.txt
+-rw-r--r--   0 val        (501) staff       (20)        7 2024-04-11 23:38:35.000000 django-ipware-6.0.5/django_ipware.egg-info/top_level.txt
+drwxr-xr-x   0 val        (501) staff       (20)        0 2024-04-11 23:38:35.411375 django-ipware-6.0.5/ipware/
+-rw-r--r--   0 val        (501) staff       (20)       87 2023-10-02 23:45:14.000000 django-ipware-6.0.5/ipware/__init__.py
+-rw-r--r--   0 val        (501) staff       (20)      319 2024-04-11 23:36:17.000000 django-ipware-6.0.5/ipware/__version__.py
+-rw-r--r--   0 val        (501) staff       (20)      250 2023-10-02 23:45:14.000000 django-ipware-6.0.5/ipware/apps.py
+-rw-r--r--   0 val        (501) staff       (20)     1205 2024-02-04 19:26:02.000000 django-ipware-6.0.5/ipware/ip.py
+-rw-r--r--   0 val        (501) staff       (20)      502 2023-11-23 00:20:01.000000 django-ipware-6.0.5/pyproject.toml
+-rw-r--r--   0 val        (501) staff       (20)       73 2024-04-11 23:38:35.411854 django-ipware-6.0.5/setup.cfg
+-rw-r--r--   0 val        (501) staff       (20)     2344 2024-04-11 23:36:17.000000 django-ipware-6.0.5/setup.py
```

### Comparing `django-ipware-6.0.4/LICENSE` & `django-ipware-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipware-6.0.4/PKG-INFO` & `django-ipware-6.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipware
-Version: 6.0.4
+Version: 6.0.5
 Summary: A Django application to retrieve user's IP address
 Home-page: https://github.com/un33k/django-ipware
 Author: Val Neekman
 Author-email: info@neekware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -83,23 +83,23 @@
 
   The default meta precedence order is top to bottom. You may customize the order
   by providing your own `IPWARE_META_PRECEDENCE_ORDER` by adding it to your project's settings.py
 
   ```python
    # The default meta precedence order (update as needed)
    IPWARE_META_PRECEDENCE_ORDER = (
-        "X_FORWARDED_FOR",  # AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
+        "X_FORWARDED_FOR",  # Load balancers or proxies such as AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
         "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
         "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_FORWARDED",  # Squid and others
         "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
         "HTTP_FORWARDED_FOR",  # RFC 7239
         "HTTP_FORWARDED",  # RFC 7239
-        "HTTP_VIA",  # Squid and others
+        "HTTP_CF_CONNECTING_IP",  # CloudFlare
         "X-CLIENT-IP",  # Microsoft Azure
         "X-REAL-IP",  # NGINX
         "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
         "X_FORWARDED",  # Squid
         "FORWARDED_FOR",  # RFC 7239
         "CF-CONNECTING-IP",  # CloudFlare
         "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `django-ipware-6.0.4/README.md` & `django-ipware-6.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,23 +60,23 @@
 
   The default meta precedence order is top to bottom. You may customize the order
   by providing your own `IPWARE_META_PRECEDENCE_ORDER` by adding it to your project's settings.py
 
   ```python
    # The default meta precedence order (update as needed)
    IPWARE_META_PRECEDENCE_ORDER = (
-        "X_FORWARDED_FOR",  # AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
+        "X_FORWARDED_FOR",  # Load balancers or proxies such as AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
         "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
         "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_FORWARDED",  # Squid and others
         "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
         "HTTP_FORWARDED_FOR",  # RFC 7239
         "HTTP_FORWARDED",  # RFC 7239
-        "HTTP_VIA",  # Squid and others
+        "HTTP_CF_CONNECTING_IP",  # CloudFlare
         "X-CLIENT-IP",  # Microsoft Azure
         "X-REAL-IP",  # NGINX
         "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
         "X_FORWARDED",  # Squid
         "FORWARDED_FOR",  # RFC 7239
         "CF-CONNECTING-IP",  # CloudFlare
         "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `django-ipware-6.0.4/django_ipware.egg-info/PKG-INFO` & `django-ipware-6.0.5/django_ipware.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipware
-Version: 6.0.4
+Version: 6.0.5
 Summary: A Django application to retrieve user's IP address
 Home-page: https://github.com/un33k/django-ipware
 Author: Val Neekman
 Author-email: info@neekware.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -83,23 +83,23 @@
 
   The default meta precedence order is top to bottom. You may customize the order
   by providing your own `IPWARE_META_PRECEDENCE_ORDER` by adding it to your project's settings.py
 
   ```python
    # The default meta precedence order (update as needed)
    IPWARE_META_PRECEDENCE_ORDER = (
-        "X_FORWARDED_FOR",  # AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
+        "X_FORWARDED_FOR",  # Load balancers or proxies such as AWS ELB (default client is `left-most` [`<client>, <proxy1>, <proxy2>`])
         "HTTP_X_FORWARDED_FOR",  # Similar to X_FORWARDED_TO
         "HTTP_CLIENT_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_REAL_IP",  # Standard headers used by providers such as Amazon EC2, Heroku etc.
         "HTTP_X_FORWARDED",  # Squid and others
         "HTTP_X_CLUSTER_CLIENT_IP",  # Rackspace LB and Riverbed Stingray
         "HTTP_FORWARDED_FOR",  # RFC 7239
         "HTTP_FORWARDED",  # RFC 7239
-        "HTTP_VIA",  # Squid and others
+        "HTTP_CF_CONNECTING_IP",  # CloudFlare
         "X-CLIENT-IP",  # Microsoft Azure
         "X-REAL-IP",  # NGINX
         "X-CLUSTER-CLIENT-IP",  # Rackspace Cloud Load Balancers
         "X_FORWARDED",  # Squid
         "FORWARDED_FOR",  # RFC 7239
         "CF-CONNECTING-IP",  # CloudFlare
         "TRUE-CLIENT-IP",  # CloudFlare Enterprise,
```

### Comparing `django-ipware-6.0.4/ipware/ip.py` & `django-ipware-6.0.5/ipware/ip.py`

 * *Files identical despite different names*

### Comparing `django-ipware-6.0.4/setup.py` & `django-ipware-6.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import setup
 
 package = 'ipware'
 python_requires = ">=3.8"
 here = os.path.abspath(os.path.dirname(__file__))
 
-requires = ['python-ipware>=2.0.0']
+requires = ['python-ipware>=2.0.3']
 test_requirements = []
 
 about = {}
 with open(os.path.join(here, package, '__version__.py'), 'r', 'utf-8') as f:
     exec(f.read(), about)
 
 with open('README.md', 'r', 'utf-8') as f:
```

