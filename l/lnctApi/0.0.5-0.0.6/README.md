# Comparing `tmp/lnctApi-0.0.5.tar.gz` & `tmp/lnctApi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnctApi-0.0.5.tar", last modified: Fri Feb  9 19:40:36 2024, max compression
+gzip compressed data, was "lnctApi-0.0.6.tar", last modified: Fri Apr 12 07:14:05 2024, max compression
```

## Comparing `lnctApi-0.0.5.tar` & `lnctApi-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-02-09 19:40:36.509260 lnctApi-0.0.5/
--rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.5/LICENSE.txt
--rw-r--r--   0 cro        (501) staff       (20)      891 2024-02-09 19:40:36.509138 lnctApi-0.0.5/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.5/README.md
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-02-09 19:40:36.507987 lnctApi-0.0.5/lnctApi/
--rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.5/lnctApi/__init__.py
--rw-r--r--   0 cro        (501) staff       (20)    23468 2024-02-09 19:09:53.000000 lnctApi-0.0.5/lnctApi/accsoft_api.py
-drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-02-09 19:40:36.508948 lnctApi-0.0.5/lnctApi.egg-info/
--rw-r--r--   0 cro        (501) staff       (20)      891 2024-02-09 19:40:36.000000 lnctApi-0.0.5/lnctApi.egg-info/PKG-INFO
--rw-r--r--   0 cro        (501) staff       (20)      227 2024-02-09 19:40:36.000000 lnctApi-0.0.5/lnctApi.egg-info/SOURCES.txt
--rw-r--r--   0 cro        (501) staff       (20)        1 2024-02-09 19:40:36.000000 lnctApi-0.0.5/lnctApi.egg-info/dependency_links.txt
--rw-r--r--   0 cro        (501) staff       (20)       37 2024-02-09 19:40:36.000000 lnctApi-0.0.5/lnctApi.egg-info/requires.txt
--rw-r--r--   0 cro        (501) staff       (20)        8 2024-02-09 19:40:36.000000 lnctApi-0.0.5/lnctApi.egg-info/top_level.txt
--rw-r--r--   0 cro        (501) staff       (20)       38 2024-02-09 19:40:36.509308 lnctApi-0.0.5/setup.cfg
--rw-r--r--   0 cro        (501) staff       (20)      868 2024-02-09 19:27:18.000000 lnctApi-0.0.5/setup.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-04-12 07:14:05.036937 lnctApi-0.0.6/
+-rw-r--r--   0 cro        (501) staff       (20)    35148 2023-07-26 12:21:56.000000 lnctApi-0.0.6/LICENSE.txt
+-rw-r--r--   0 cro        (501) staff       (20)      891 2024-04-12 07:14:05.036766 lnctApi-0.0.6/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      336 2023-08-05 18:56:59.000000 lnctApi-0.0.6/README.md
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-04-12 07:14:05.035216 lnctApi-0.0.6/lnctApi/
+-rw-r--r--   0 cro        (501) staff       (20)       32 2023-08-04 19:28:06.000000 lnctApi-0.0.6/lnctApi/__init__.py
+-rw-r--r--   0 cro        (501) staff       (20)    23469 2024-04-12 06:58:45.000000 lnctApi-0.0.6/lnctApi/accsoft_api.py
+drwxr-xr-x   0 cro        (501) staff       (20)        0 2024-04-12 07:14:05.036530 lnctApi-0.0.6/lnctApi.egg-info/
+-rw-r--r--   0 cro        (501) staff       (20)      891 2024-04-12 07:14:04.000000 lnctApi-0.0.6/lnctApi.egg-info/PKG-INFO
+-rw-r--r--   0 cro        (501) staff       (20)      227 2024-04-12 07:14:05.000000 lnctApi-0.0.6/lnctApi.egg-info/SOURCES.txt
+-rw-r--r--   0 cro        (501) staff       (20)        1 2024-04-12 07:14:04.000000 lnctApi-0.0.6/lnctApi.egg-info/dependency_links.txt
+-rw-r--r--   0 cro        (501) staff       (20)       37 2024-04-12 07:14:04.000000 lnctApi-0.0.6/lnctApi.egg-info/requires.txt
+-rw-r--r--   0 cro        (501) staff       (20)        8 2024-04-12 07:14:04.000000 lnctApi-0.0.6/lnctApi.egg-info/top_level.txt
+-rw-r--r--   0 cro        (501) staff       (20)       38 2024-04-12 07:14:05.036996 lnctApi-0.0.6/setup.cfg
+-rw-r--r--   0 cro        (501) staff       (20)      868 2024-04-12 07:12:05.000000 lnctApi-0.0.6/setup.py
```

### Comparing `lnctApi-0.0.5/LICENSE.txt` & `lnctApi-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lnctApi-0.0.5/PKG-INFO` & `lnctApi-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.5
+Version: 0.0.6
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documentation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lnctApi-0.0.5/lnctApi/accsoft_api.py` & `lnctApi-0.0.6/lnctApi/accsoft_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             return show
         response = self.session.get('https://portal.lnct.ac.in/Accsoft2/Parents/StuAttendanceStatus.aspx')
         soup = BeautifulSoup(response.text, 'html.parser')
         name = soup.find(id='ctl00_ContentPlaceHolder1_txtStudentName')['value']
         table = soup.find(id="ctl00_ContentPlaceHolder1_Gridview1")
         if table.find("td").get_text() == "Record Not Found":
             return json.dumps({"name": name, "totalLectures": 0, "present": 0, "absent": 0, "percentage": 0})
-        TotalLectures = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotperiod11')[0].get_text()))
+        TotalLectures = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotperiod111')[0].get_text()))
         present = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotalp11')[0].get_text()))
         absent = int(re.sub('\D', '', soup.find_all(id='ctl00_ContentPlaceHolder1_lbltotala11')[0].get_text()))
         if TotalLectures != 0:
             percentage = (present * 100 )/ TotalLectures
             percentage = round(percentage, 2)
         else:
             percentage = 0
```

### Comparing `lnctApi-0.0.5/lnctApi.egg-info/PKG-INFO` & `lnctApi-0.0.6/lnctApi.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnctApi
-Version: 0.0.5
+Version: 0.0.6
 Summary: LNCT API wrapper, written in Python.
 Home-page: https://github.com/cro2003/lnctApi
 Author: cro2003
 Author-email: cro@chirag.software
 License: MIT
 Project-URL: Documentation, https://cro2003.github.io/lnctApi/
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `lnctApi-0.0.5/setup.py` & `lnctApi-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lnctApi",
-    version="0.0.5",
+    version="0.0.6",
     description="LNCT API wrapper, written in Python.",
     packages=['lnctApi'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cro2003/lnctApi",
     project_urls = {
     'Documentation': 'https://cro2003.github.io/lnctApi/',
```

