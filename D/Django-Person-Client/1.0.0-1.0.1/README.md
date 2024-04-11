# Comparing `tmp/Django-Person-Client-1.0.0.tar.gz` & `tmp/Django-Person-Client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Django-Person-Client-1.0.0.tar", last modified: Wed Apr 10 18:02:18 2024, max compression
+gzip compressed data, was "Django-Person-Client-1.0.1.tar", last modified: Thu Apr 11 23:47:00 2024, max compression
```

## Comparing `Django-Person-Client-1.0.0.tar` & `Django-Person-Client-1.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.934142 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/Django_Person_Client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.934142 Django-Person-Client-1.0.0/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 18:02:18.000000 Django-Person-Client-1.0.0/uw_person_client/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/adviser.json
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/degree.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/employee.json
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/hold.json
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/major.json
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/person.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/sport.json
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/student.json
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/term.json
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/transcript.json
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/fixtures/transfer.json
--rw-r--r--   0 runner    (1001) docker     (127)    31339 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/test_migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/test_migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 18:02:18.938143 Django-Person-Client-1.0.0/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/test_adviser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/tests/test_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 18:02:09.000000 Django-Person-Client-1.0.0/uw_person_client/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.569223 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-11 23:47:00.000000 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 23:47:00.000000 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:47:00.000000 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 23:47:00.000000 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 23:47:00.000000 Django-Person-Client-1.0.1/Django_Person_Client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.569223 Django-Person-Client-1.0.1/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 23:46:59.000000 Django-Person-Client-1.0.1/uw_person_client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/uw_person_client/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/adviser.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/degree.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/employee.json
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/hold.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/major.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/person.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/sport.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/student.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/term.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/transcript.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/fixtures/transfer.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31983 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/uw_person_client/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    32894 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/test_migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/test_migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:47:00.573223 Django-Person-Client-1.0.1/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/tests/test_adviser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7989 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/tests/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-11 23:46:50.000000 Django-Person-Client-1.0.1/uw_person_client/urls.py
```

### Comparing `Django-Person-Client-1.0.0/Django_Person_Client.egg-info/PKG-INFO` & `Django-Person-Client-1.0.1/Django_Person_Client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-1.0.0/Django_Person_Client.egg-info/SOURCES.txt` & `Django-Person-Client-1.0.1/Django_Person_Client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/LICENSE` & `Django-Person-Client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/PKG-INFO` & `Django-Person-Client-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Person-Client
-Version: 1.0.0
+Version: 1.0.1
 Summary: A UW Person Client Django app
 Home-page: https://github.com/uw-it-aca/django-person-client
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Person-Client-1.0.0/README.md` & `Django-Person-Client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/setup.py` & `Django-Person-Client-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/adviser.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/adviser.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/degree.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/degree.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/employee.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/employee.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/hold.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/hold.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/major.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/major.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/person.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/person.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/sport.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/sport.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/student.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/student.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993359788359788%*

 * *Differences: {'0': "{'fields': {'major_2': 2}}", '1': "{'fields': {'pending_major_1': 1}}"}*

```diff
@@ -64,15 +64,15 @@
             "local_addr_country": null,
             "local_addr_line1": "0100 PRINCETON ST",
             "local_addr_line2": null,
             "local_addr_postal_code": null,
             "local_addr_state": "CA",
             "local_phone_number": "(999) 123-4567",
             "major_1": 1,
-            "major_2": null,
+            "major_2": 2,
             "major_3": null,
             "new_continuing_returning_code": "0",
             "new_continuing_returning_desc": "CONTINUING",
             "parent_name": "Average,Joe",
             "pending_major_1": null,
             "pending_major_2": null,
             "pending_major_3": null,
@@ -201,15 +201,15 @@
             "local_phone_number": "(200) 333-0000",
             "major_1": 2,
             "major_2": null,
             "major_3": null,
             "new_continuing_returning_code": "0",
             "new_continuing_returning_desc": "CONTINUING",
             "parent_name": "Bothell,Joe",
-            "pending_major_1": null,
+            "pending_major_1": 1,
             "pending_major_2": null,
             "pending_major_3": null,
             "perm_addr_4digit_zip": null,
             "perm_addr_5digit_zip": "98052",
             "perm_addr_city": "REDMOND",
             "perm_addr_country": null,
             "perm_addr_line1": "0002 152ND AVE NE APT C505",
```

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/transcript.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/transcript.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/fixtures/transfer.json` & `Django-Person-Client-1.0.1/uw_person_client/fixtures/transfer.json`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/models.py` & `Django-Person-Client-1.0.1/uw_person_client/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,14 +457,36 @@
     hispanic_group_desc = models.TextField(blank=True, null=True)
 
     class Meta:
         db_table = 'student'
         managed = False
 
     @property
+    def majors(self):
+        majors = []
+        if self.major_1:
+            majors.append(self.major_1)
+        if self.major_2:
+            majors.append(self.major_2)
+        if self.major_3:
+            majors.append(self.major_3)
+        return majors
+
+    @property
+    def pending_majors(self):
+        pending_majors = []
+        if self.pending_major_1:
+            pending_majors.append(self.pending_major_1)
+        if self.pending_major_2:
+            pending_majors.append(self.pending_major_2)
+        if self.pending_major_3:
+            pending_majors.append(self.pending_major_3)
+        return pending_majors
+
+    @property
     def transcripts(self):
         try:
             return self._transcripts
         except AttributeError:
             pass
 
     @transcripts.setter
```

### Comparing `Django-Person-Client-1.0.0/uw_person_client/test_migrations/0001_initial.py` & `Django-Person-Client-1.0.1/uw_person_client/test_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/tests/test_adviser.py` & `Django-Person-Client-1.0.1/uw_person_client/tests/test_adviser.py`

 * *Files identical despite different names*

### Comparing `Django-Person-Client-1.0.0/uw_person_client/tests/test_person.py` & `Django-Person-Client-1.0.1/uw_person_client/tests/test_person.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         self.assertEqual(p.employee, None)
         self.assertEqual(p.student.student_number, '1233334')
         self.assertEqual(p.student.academic_term.year, 2013)
         self.assertEqual(p.student.academic_term.quarter, 3)
         self.assertEqual(p.student.major_1.major_name, 'INTERNATIONAL STUDIES')
         self.assertEqual(p.student.major_2, None)
         self.assertEqual(p.student.major_3, None)
+        self.assertEqual(len(p.student.majors), 1)
+        self.assertEqual(len(p.student.pending_majors), 1)
         self.assertEqual(len(p.student.sports.all()), 1)
         self.assertEqual(p.student.sports.all()[0].short_sport_name, 'GLF')
         self.assertEqual(len(p.student.advisers.all()), 1)
         self.assertEqual(p.student.transcripts, None)
         self.assertEqual(p.student.transfers, None)
         self.assertEqual(p.student.holds, None)
         self.assertEqual(p.student.degrees, None)
@@ -144,14 +146,16 @@
     def test_get_student_includes_by_student_number(self):
         p = Person.objects.get_person_by_student_number(
             '1033334',
             include_student=True,
             include_student_transcripts=True)
         self.assertEqual(p.student.student_number, '1033334')
         self.assertEqual(p.student.major_1.major_name, 'PRE SOCIAL SCIENCE')
+        self.assertEqual(len(p.student.majors), 2)
+        self.assertEqual(len(p.student.pending_majors), 0)
         self.assertEqual(len(p.student.transcripts.all()), 2)
 
     def test_person_to_dict(self):
         p1 = Person.objects.get_person_by_uwnetid('javerage')
         data1 = p1.to_dict()
 
         p2 = Person(**data1)
```

