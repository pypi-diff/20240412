# Comparing `tmp/firecrawl-py-0.0.3.tar.gz` & `tmp/firecrawl-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.3.tar", last modified: Fri Apr 12 01:00:52 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.4.tar", last modified: Fri Apr 12 01:21:34 2024, max compression
```

## Comparing `firecrawl-py-0.0.3.tar` & `firecrawl-py-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.241577 firecrawl-py-0.0.3/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:00:52.241478 firecrawl-py-0.0.3/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3318 2024-04-12 00:43:37.000000 firecrawl-py-0.0.3/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.240793 firecrawl-py-0.0.3/firecrawl/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-12 01:00:36.000000 firecrawl-py-0.0.3/firecrawl/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3365 2024-04-12 00:57:26.000000 firecrawl-py-0.0.3/firecrawl/firecrawl.py
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.241333 firecrawl-py-0.0.3/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/top_level.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 01:00:52.241618 firecrawl-py-0.0.3/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 01:00:45.000000 firecrawl-py-0.0.3/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:21:34.456833 firecrawl-py-0.0.4/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:21:34.456717 firecrawl-py-0.0.4/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3419 2024-04-12 01:21:09.000000 firecrawl-py-0.0.4/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:21:34.455871 firecrawl-py-0.0.4/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-12 01:00:36.000000 firecrawl-py-0.0.4/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3743 2024-04-12 01:11:28.000000 firecrawl-py-0.0.4/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:21:34.456566 firecrawl-py-0.0.4/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:21:34.000000 firecrawl-py-0.0.4/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 01:21:34.000000 firecrawl-py-0.0.4/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 01:21:34.000000 firecrawl-py-0.0.4/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 01:21:34.000000 firecrawl-py-0.0.4/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 01:21:34.000000 firecrawl-py-0.0.4/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 01:21:34.456874 firecrawl-py-0.0.4/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 01:12:45.000000 firecrawl-py-0.0.4/setup.py
```

### Comparing `firecrawl-py-0.0.3/firecrawl/firecrawl.py` & `firecrawl-py-0.0.4/firecrawl/firecrawl.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,39 +3,47 @@
 
 class FirecrawlApp:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('FIRECRAWL_API_KEY')
         if self.api_key is None:
             raise ValueError('No API key provided')
     
-    def scrape_url(self, url, params):
+    def scrape_url(self, url, params=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Bearer {self.api_key}'
         }
+        json_data = {'url': url}
+        if params:
+            json_data.update(params)
         response = requests.post(
             'https://api.firecrawl.dev/v0/scrape',
             headers=headers,
-            json={'url': url, **params}
+            json=json_data
         )
         if response.status_code == 200:
             return response.json()
         elif response.status_code in [402, 409, 500]:
             error_message = response.json().get('error', 'Unknown error occurred')
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}. Error: {error_message}')
         else:
             raise Exception(f'Failed to scrape URL. Status code: {response.status_code}')
 
-    def crawl_url(self, url, params):
-        import time
+    def crawl_url(self, url, params=None, wait_until_done=True, timeout=2):
         headers = self._prepare_headers()
-        response = self._post_request('https://api.firecrawl.dev/v0/crawl', {'url': url, **params}, headers)
+        json_data = {'url': url}
+        if params:
+            json_data.update(params)
+        response = self._post_request('https://api.firecrawl.dev/v0/crawl', json_data, headers)
         if response.status_code == 200:
             job_id = response.json().get('jobId')
-            return self._monitor_job_status(job_id, headers)
+            if wait_until_done:
+                return self._monitor_job_status(job_id, headers, timeout)
+            else:
+                return {'jobId': job_id}
         else:
             self._handle_error(response, 'start crawl job')
 
     def check_crawl_status(self, job_id):
         headers = self._prepare_headers()
         response = self._get_request(f'https://api.firecrawl.dev/v0/crawl/status/{job_id}', headers)
         if response.status_code == 200:
@@ -51,24 +59,26 @@
 
     def _post_request(self, url, data, headers):
         return requests.post(url, headers=headers, json=data)
 
     def _get_request(self, url, headers):
         return requests.get(url, headers=headers)
 
-    def _monitor_job_status(self, job_id, headers):
+    def _monitor_job_status(self, job_id, headers, timeout):
         import time
         while True:
             status_response = self._get_request(f'https://api.firecrawl.dev/v0/crawl/status/{job_id}', headers)
             if status_response.status_code == 200:
                 status_data = status_response.json()
                 if status_data['status'] == 'completed':
                     return status_data
                 elif status_data['status'] in ['active', 'paused', 'pending', 'queued']:
-                    time.sleep(2)  # Wait for 2 seconds before checking again
+                    if timeout < 2:
+                        timeout = 2
+                    time.sleep(timeout)  # Wait for the specified timeout before checking again
                 else:
                     raise Exception(f'Crawl job failed or was stopped. Status: {status_data["status"]}')
             else:
                 self._handle_error(status_response, 'check crawl status')
 
     def _handle_error(self, response, action):
         if response.status_code in [402, 409, 500]:
```

