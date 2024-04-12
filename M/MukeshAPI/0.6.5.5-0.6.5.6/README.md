# Comparing `tmp/MukeshAPI-0.6.5.5.tar.gz` & `tmp/MukeshAPI-0.6.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MukeshAPI-0.6.5.5.tar", last modified: Tue Apr  9 16:58:53 2024, max compression
+gzip compressed data, was "MukeshAPI-0.6.5.6.tar", last modified: Fri Apr 12 15:07:14 2024, max compression
```

## Comparing `MukeshAPI-0.6.5.5.tar` & `MukeshAPI-0.6.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.325052 MukeshAPI-0.6.5.5/
--rw-rw-rw-   0        0        0     1106 2024-03-20 19:28:38.000000 MukeshAPI-0.6.5.5/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.209178 MukeshAPI-0.6.5.5/MukeshAPI/
--rw-rw-rw-   0        0        0    28369 2024-04-09 16:53:56.000000 MukeshAPI-0.6.5.5/MukeshAPI/__init__.py
--rw-rw-rw-   0        0        0    12815 2024-03-13 07:52:51.000000 MukeshAPI-0.6.5.5/MukeshAPI/func.py
--rw-rw-rw-   0        0        0    44002 2024-03-28 05:19:20.000000 MukeshAPI-0.6.5.5/MukeshAPI/truth_dare.py
--rw-rw-rw-   0        0        0  6825608 2024-03-14 16:26:42.000000 MukeshAPI-0.6.5.5/MukeshAPI/words.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:58:53.316739 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/
--rw-rw-rw-   0        0        0     6157 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-04-09 16:58:53.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 16:58:52.000000 MukeshAPI-0.6.5.5/MukeshAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6157 2024-04-09 16:58:53.320307 MukeshAPI-0.6.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     4338 2024-03-13 03:51:40.000000 MukeshAPI-0.6.5.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 16:58:53.326050 MukeshAPI-0.6.5.5/setup.cfg
--rw-rw-rw-   0        0        0     2426 2024-03-14 17:55:27.000000 MukeshAPI-0.6.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:07:14.143957 MukeshAPI-0.6.5.6/
+-rw-rw-rw-   0        0        0     1106 2024-03-20 19:28:38.000000 MukeshAPI-0.6.5.6/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-12 15:07:14.045704 MukeshAPI-0.6.5.6/MukeshAPI/
+-rw-rw-rw-   0        0        0    29880 2024-04-12 15:07:08.000000 MukeshAPI-0.6.5.6/MukeshAPI/__init__.py
+-rw-rw-rw-   0        0        0    12815 2024-03-13 07:52:51.000000 MukeshAPI-0.6.5.6/MukeshAPI/func.py
+-rw-rw-rw-   0        0        0    44002 2024-03-28 05:19:20.000000 MukeshAPI-0.6.5.6/MukeshAPI/truth_dare.py
+-rw-rw-rw-   0        0        0  6825608 2024-03-14 16:26:42.000000 MukeshAPI-0.6.5.6/MukeshAPI/words.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:07:14.132711 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/
+-rw-rw-rw-   0        0        0     6189 2024-04-12 15:07:13.000000 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-04-12 15:07:13.000000 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:07:13.000000 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-12 15:07:13.000000 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 15:07:13.000000 MukeshAPI-0.6.5.6/MukeshAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6189 2024-04-12 15:07:14.132711 MukeshAPI-0.6.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4338 2024-03-13 03:51:40.000000 MukeshAPI-0.6.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:07:14.145774 MukeshAPI-0.6.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     2444 2024-04-12 14:43:25.000000 MukeshAPI-0.6.5.6/setup.py
```

### Comparing `MukeshAPI-0.6.5.5/LICENSE` & `MukeshAPI-0.6.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.5/MukeshAPI/__init__.py` & `MukeshAPI-0.6.5.6/MukeshAPI/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import random
 import requests
 import string,re,os
-import base64,json
+import base64,json,time
+from bs4 import BeautifulSoup
+from urllib.request import urlopen
 from bs4 import BeautifulSoup
-from requests_html import HTMLSession
 import urllib
+from requests_html import HTMLSession
 from MukeshAPI.func import (MORSE_CODE_DICT,payloads_response,gpt_4_mode,payload8)
 from base64 import b64decode as m,b64encode as n
 from MukeshAPI.words import wordshub
 from PIL import Image, ImageDraw, ImageFont
 from MukeshAPI.truth_dare import TRUTH,DARE
-__version__ = "0.6.5.5"
+__version__ = "0.6.5.6"
 
 __all__ = ["api"]
 
 
 class MukeshAPI:
     
     def __init__(self)->None:
@@ -779,14 +781,19 @@
 
     Args:
         image_url (str, optional): The URL of the image to upload.
         image_file (file, optional): The file object of the image to upload.
 
     Returns:
         str: The URL of the uploaded image.
+        
+    Example usage:
+        >>> from MukeshAPI import api
+        >>> upload_image = api.upload_image(image_url="url-of-img.jpg")
+        >>> print(upload_image)
     """
 
         if image_url is None and image_file is None:
             raise ValueError("Either image_url or image_file must be provided.")
 
         if image_url is not None:
             image =image_url
@@ -803,11 +810,49 @@
     def truth():
         truth_string=random.choice(TRUTH)
         return truth_string
     
     @staticmethod
     def dare():
         dare_string=random.choice(DARE)
-        return truth_string
+        return dare_string
+    
+    @staticmethod
+    def ai_image(prompt: str) -> bytes:
+        """Generates an AI-generated image based on the provided prompt.
+
+        Args:
+            prompt (str): The input prompt for generating the image.
+
+        Returns:
+            bytes: The generated image in bytes format.
+            
+        Example usage:
+        >>> from MukeshAPI import api
+        >>> generated_image= api.ai_image("boy image")
+        >>> print(generated_image)
+        """
+        url = base64.b64decode('aHR0cHM6Ly9haS1hcGkubWFnaWNzdHVkaW8uY29tL2FwaS9haS1hcnQtZ2VuZXJhdG9y').decode("utf-8")
+
+        form_data = {
+            'prompt': prompt,
+            'output_format': 'bytes',
+            'request_timestamp': str(int(time.time())),
+            'user_is_subscribed': 'false',
+        }
+
+        response = requests.post(url, data=form_data)
+        if response.status_code == 200:
+            try:
+                if response.content:
+                    return response.content
+                else:
+                    raise Exception("Failed to get image from the server.")
+            except Exception as e:
+                raise e
+        else:
+            raise Exception("Error:", response.status_code)
+
         
+            
 api=MukeshAPI()
```

### Comparing `MukeshAPI-0.6.5.5/MukeshAPI/func.py` & `MukeshAPI-0.6.5.6/MukeshAPI/func.py`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.5/MukeshAPI/truth_dare.py` & `MukeshAPI-0.6.5.6/MukeshAPI/truth_dare.py`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.5/MukeshAPI/words.py` & `MukeshAPI-0.6.5.6/MukeshAPI/words.py`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.5/MukeshAPI.egg-info/PKG-INFO` & `MukeshAPI-0.6.5.6/MukeshAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MukeshAPI
-Version: 0.6.5.5
+Version: 0.6.5.6
 Summary: python api hub | MukeshAPI
 Home-page: https://github.com/noob-mukesh/MukeshAPI
 Download-URL: https://github.com/Noob-mukesh/MukeshAPI/blob/main/README.md
 Author: Mukesh | noob-mukesh
 Author-email: itzcodermukesh@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/noob-mukesh/MukeshAPI/issues
@@ -34,14 +34,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests-html
 Requires-Dist: pillow
+Requires-Dist: lxml_html_clean
 
 # MukeshAPI 🚀
 
 ## Chatgpt AI 🤖
 
 ```
 from MukeshAPI import api
```

### Comparing `MukeshAPI-0.6.5.5/PKG-INFO` & `MukeshAPI-0.6.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MukeshAPI
-Version: 0.6.5.5
+Version: 0.6.5.6
 Summary: python api hub | MukeshAPI
 Home-page: https://github.com/noob-mukesh/MukeshAPI
 Download-URL: https://github.com/Noob-mukesh/MukeshAPI/blob/main/README.md
 Author: Mukesh | noob-mukesh
 Author-email: itzcodermukesh@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/noob-mukesh/MukeshAPI/issues
@@ -34,14 +34,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pytz>=2023.3
 Requires-Dist: requests-html
 Requires-Dist: pillow
+Requires-Dist: lxml_html_clean
 
 # MukeshAPI 🚀
 
 ## Chatgpt AI 🤖
 
 ```
 from MukeshAPI import api
```

### Comparing `MukeshAPI-0.6.5.5/README.md` & `MukeshAPI-0.6.5.6/README.md`

 * *Files identical despite different names*

### Comparing `MukeshAPI-0.6.5.5/setup.py` & `MukeshAPI-0.6.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     description="python api hub | MukeshAPI",
     long_description_content_type="text/markdown",
     long_description=long_desc,
     packages=find_packages(),
     license="MIT",
     url="https://github.com/noob-mukesh/MukeshAPI",
     download_url="https://github.com/Noob-mukesh/MukeshAPI/blob/main/README.md",
-    install_requires=["pytz>=2023.3","requests-html","pillow"],
+    install_requires=["pytz>=2023.3","requests-html","pillow","lxml_html_clean"],
     keywords=['python', "MukeshAPI","flask"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

