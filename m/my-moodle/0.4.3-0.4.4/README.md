# Comparing `tmp/my-moodle-0.4.3.tar.gz` & `tmp/my-moodle-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-moodle-0.4.3.tar", last modified: Mon Apr  1 01:44:42 2024, max compression
+gzip compressed data, was "my-moodle-0.4.4.tar", last modified: Fri Apr 12 12:52:51 2024, max compression
```

## Comparing `my-moodle-0.4.3.tar` & `my-moodle-0.4.4.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 01:44:42.849100 my-moodle-0.4.3/
--rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my-moodle-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1842 2024-04-01 01:44:42.848100 my-moodle-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my-moodle-0.4.3/license
-drwxrwxrwx   0        0        0        0 2024-04-01 01:44:42.817347 my-moodle-0.4.3/my_moodle/
--rw-rw-rw-   0        0        0     1306 2024-03-31 18:49:59.000000 my-moodle-0.4.3/my_moodle/__init__.py
--rw-rw-rw-   0        0        0      322 2024-03-01 22:18:35.000000 my-moodle-0.4.3/my_moodle/__main__.py
--rw-rw-rw-   0        0        0     4133 2024-03-31 18:50:22.000000 my-moodle-0.4.3/my_moodle/api.py
--rw-rw-rw-   0        0        0      437 2024-03-31 18:05:47.000000 my-moodle-0.4.3/my_moodle/api_functions.py
--rw-rw-rw-   0        0        0     2825 2024-03-31 01:09:50.000000 my-moodle-0.4.3/my_moodle/config_utility.py
--rw-rw-rw-   0        0        0    10541 2024-03-31 20:13:23.000000 my-moodle-0.4.3/my_moodle/course_markdown_builder.py
--rw-rw-rw-   0        0        0      340 2024-03-31 18:28:26.000000 my-moodle-0.4.3/my_moodle/course_status.py
--rw-rw-rw-   0        0        0     1572 2024-03-31 20:29:52.000000 my-moodle-0.4.3/my_moodle/csv_utility.py
--rw-rw-rw-   0        0        0     8887 2024-04-01 01:07:40.000000 my-moodle-0.4.3/my_moodle/data_utility.py
--rw-rw-rw-   0        0        0     1393 2024-03-31 10:33:22.000000 my-moodle-0.4.3/my_moodle/enrolled_users_fields.py
--rw-rw-rw-   0        0        0     1254 2024-03-31 21:14:09.000000 my-moodle-0.4.3/my_moodle/json_utility.py
--rw-rw-rw-   0        0        0     6848 2024-03-31 11:21:10.000000 my-moodle-0.4.3/my_moodle/markdown_document.py
--rw-rw-rw-   0        0        0     3596 2024-03-31 17:05:15.000000 my-moodle-0.4.3/my_moodle/markdown_methods.py
--rw-rw-rw-   0        0        0     7734 2024-04-01 00:25:25.000000 my-moodle-0.4.3/my_moodle/moodle_data_downloader.py
--rw-rw-rw-   0        0        0     5904 2024-03-31 20:12:54.000000 my-moodle-0.4.3/my_moodle/moodle_json_downloader.py
--rw-rw-rw-   0        0        0     4803 2024-03-31 19:36:21.000000 my-moodle-0.4.3/my_moodle/program_markdown_builder.py
--rw-rw-rw-   0        0        0     3874 2024-03-31 21:25:59.000000 my-moodle-0.4.3/my_moodle/project_structure.py
--rw-rw-rw-   0        0        0      311 2024-04-01 01:42:45.000000 my-moodle-0.4.3/my_moodle/resource.json
--rw-rw-rw-   0        0        0      157 2024-04-01 01:43:26.000000 my-moodle-0.4.3/my_moodle/version.py
--rw-rw-rw-   0        0        0     8987 2024-03-31 20:15:05.000000 my-moodle-0.4.3/my_moodle/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-01 01:44:42.845830 my-moodle-0.4.3/my_moodle.egg-info/
--rw-rw-rw-   0        0        0     1842 2024-04-01 01:44:42.000000 my-moodle-0.4.3/my_moodle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1037 2024-04-01 01:44:42.000000 my-moodle-0.4.3/my_moodle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 01:44:42.000000 my-moodle-0.4.3/my_moodle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-01 01:44:42.000000 my-moodle-0.4.3/my_moodle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-01 01:44:42.000000 my-moodle-0.4.3/my_moodle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1243 2024-03-31 22:19:42.000000 my-moodle-0.4.3/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-01 01:44:42.849100 my-moodle-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      996 2024-04-01 01:43:26.000000 my-moodle-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 01:44:42.844493 my-moodle-0.4.3/tests/
--rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my-moodle-0.4.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1015 2024-03-28 07:15:10.000000 my-moodle-0.4.3/tests/config_parser_test.py
--rw-rw-rw-   0        0        0     2061 2024-03-31 20:26:08.000000 my-moodle-0.4.3/tests/course_markdown_builder_test.py
--rw-rw-rw-   0        0        0     1630 2024-03-31 21:38:20.000000 my-moodle-0.4.3/tests/moodle_data_downloader_test.py
--rw-rw-rw-   0        0        0     1243 2024-03-31 20:27:00.000000 my-moodle-0.4.3/tests/moodle_data_utility_test.py
--rw-rw-rw-   0        0        0     1408 2024-03-30 17:59:07.000000 my-moodle-0.4.3/tests/moodle_json_downloader_test.py
--rw-rw-rw-   0        0        0     1476 2024-03-31 15:44:24.000000 my-moodle-0.4.3/tests/package_test.py
--rw-rw-rw-   0        0        0     1013 2024-03-30 20:11:27.000000 my-moodle-0.4.3/tests/program_markdown_builder_test.py
--rw-rw-rw-   0        0        0      659 2024-04-01 01:43:26.000000 my-moodle-0.4.3/tests/version_test.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.195171 my-moodle-0.4.4/
+-rw-rw-rw-   0        0        0       36 2024-03-01 17:54:38.000000 my-moodle-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1842 2024-04-12 12:52:51.193046 my-moodle-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       88 2024-03-01 02:03:47.000000 my-moodle-0.4.4/license
+drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.151948 my-moodle-0.4.4/my_moodle/
+-rw-rw-rw-   0        0        0     1306 2024-03-31 18:49:59.000000 my-moodle-0.4.4/my_moodle/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-03-01 22:18:35.000000 my-moodle-0.4.4/my_moodle/__main__.py
+-rw-rw-rw-   0        0        0     5053 2024-04-09 00:23:45.000000 my-moodle-0.4.4/my_moodle/api.py
+-rw-rw-rw-   0        0        0      555 2024-04-01 03:19:50.000000 my-moodle-0.4.4/my_moodle/api_functions.py
+-rw-rw-rw-   0        0        0     2825 2024-03-31 01:09:50.000000 my-moodle-0.4.4/my_moodle/config_utility.py
+-rw-rw-rw-   0        0        0    12286 2024-04-03 02:33:59.000000 my-moodle-0.4.4/my_moodle/course_markdown_builder.py
+-rw-rw-rw-   0        0        0      340 2024-03-31 18:28:26.000000 my-moodle-0.4.4/my_moodle/course_status.py
+-rw-rw-rw-   0        0        0     1572 2024-03-31 20:29:52.000000 my-moodle-0.4.4/my_moodle/csv_utility.py
+-rw-rw-rw-   0        0        0    10814 2024-04-08 19:04:03.000000 my-moodle-0.4.4/my_moodle/data_utility.py
+-rw-rw-rw-   0        0        0     1393 2024-03-31 10:33:22.000000 my-moodle-0.4.4/my_moodle/enrolled_users_fields.py
+-rw-rw-rw-   0        0        0     1254 2024-03-31 21:14:09.000000 my-moodle-0.4.4/my_moodle/json_utility.py
+-rw-rw-rw-   0        0        0     6848 2024-03-31 11:21:10.000000 my-moodle-0.4.4/my_moodle/markdown_document.py
+-rw-rw-rw-   0        0        0     3596 2024-03-31 17:05:15.000000 my-moodle-0.4.4/my_moodle/markdown_methods.py
+-rw-rw-rw-   0        0        0     8545 2024-04-04 17:26:47.000000 my-moodle-0.4.4/my_moodle/moodle_data_downloader.py
+-rw-rw-rw-   0        0        0     5969 2024-04-09 00:22:43.000000 my-moodle-0.4.4/my_moodle/moodle_json_downloader.py
+-rw-rw-rw-   0        0        0     4896 2024-04-04 23:02:57.000000 my-moodle-0.4.4/my_moodle/program_markdown_builder.py
+-rw-rw-rw-   0        0        0     4470 2024-04-09 01:00:41.000000 my-moodle-0.4.4/my_moodle/project_structure.py
+-rw-rw-rw-   0        0        0      311 2024-04-01 01:42:45.000000 my-moodle-0.4.4/my_moodle/resource.json
+-rw-rw-rw-   0        0        0      157 2024-04-12 12:48:56.000000 my-moodle-0.4.4/my_moodle/version.py
+-rw-rw-rw-   0        0        0     8987 2024-03-31 20:15:05.000000 my-moodle-0.4.4/my_moodle/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.192038 my-moodle-0.4.4/my_moodle.egg-info/
+-rw-rw-rw-   0        0        0     1842 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1066 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 12:52:51.000000 my-moodle-0.4.4/my_moodle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1243 2024-03-31 22:19:42.000000 my-moodle-0.4.4/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 12:52:51.195171 my-moodle-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      996 2024-04-12 12:48:56.000000 my-moodle-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 12:52:51.190160 my-moodle-0.4.4/tests/
+-rw-rw-rw-   0        0        0     1531 2024-04-12 12:51:27.000000 my-moodle-0.4.4/tests/_.py
+-rw-rw-rw-   0        0        0        0 2024-03-01 02:03:47.000000 my-moodle-0.4.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     2876 2024-04-12 12:51:34.000000 my-moodle-0.4.4/tests/api_test.py
+-rw-rw-rw-   0        0        0     1015 2024-03-28 07:15:10.000000 my-moodle-0.4.4/tests/config_parser_test.py
+-rw-rw-rw-   0        0        0     2104 2024-04-04 16:34:12.000000 my-moodle-0.4.4/tests/course_markdown_builder_test.py
+-rw-rw-rw-   0        0        0     1630 2024-03-31 21:38:20.000000 my-moodle-0.4.4/tests/moodle_data_downloader_test.py
+-rw-rw-rw-   0        0        0     1243 2024-03-31 20:27:00.000000 my-moodle-0.4.4/tests/moodle_data_utility_test.py
+-rw-rw-rw-   0        0        0     1408 2024-03-30 17:59:07.000000 my-moodle-0.4.4/tests/moodle_json_downloader_test.py
+-rw-rw-rw-   0        0        0     1476 2024-03-31 15:44:24.000000 my-moodle-0.4.4/tests/package_test.py
+-rw-rw-rw-   0        0        0     1013 2024-03-30 20:11:27.000000 my-moodle-0.4.4/tests/program_markdown_builder_test.py
+-rw-rw-rw-   0        0        0      659 2024-04-12 12:48:56.000000 my-moodle-0.4.4/tests/version_test.py
```

### Comparing `my-moodle-0.4.3/PKG-INFO` & `my-moodle-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.3
+Version: 0.4.4
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `my-moodle-0.4.3/my_moodle/__init__.py` & `my-moodle-0.4.4/my_moodle/__init__.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/api.py` & `my-moodle-0.4.4/my_moodle/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from json import loads
 from requests import post, Response
 from .api_functions import (
     CORE_COURSE_GET_CONTENTS,
     CORE_COURSE_GET_ENROLLED_COURSES_BY_TIMELINE_CLASSIFICATION,
     CORE_ENROL_GET_ENROLLED_USERS,
+    MOD_ASSIGN_GET_ASSIGNMENTS,
+    MOD_ASSIGN_GET_SUBMISSIONS,
 )
 
 
 class Api:
     """This class is responsible for calling endpoints of the Moodle API."""
 
     WEB_SERVICE_PATH: str = "webservice/rest/server.php"
@@ -72,14 +74,40 @@
         Returns:
             dict: The result
         """
         url = f"{self.moodle_url}&wsfunction={function_name}"
         response: Response = post(url, params=params, timeout=self.timeout)
         return loads(response.content)
 
+    def get_assignment_submissions(self, assignment_id: str) -> dict:
+        """Get assignment submissions.
+
+        Args:
+            assignment_id (str): The assignment id.
+
+        Returns:
+            dict: A dictionaries containing submission information.
+        """
+        params = {"assignmentids[0]": assignment_id}
+        json = self.call_moodle_api(MOD_ASSIGN_GET_SUBMISSIONS, params)
+        return self.__get_dict(json)
+
+    def get_course_assignments(self, course_id: str) -> dict:
+        """Get assignments from a course
+
+        Args:
+            course_id (str): The course id
+
+        Returns:
+            list: A json list of assignments
+        """
+        params = {"courseids[0]": course_id}
+        json = self.call_moodle_api(MOD_ASSIGN_GET_ASSIGNMENTS, params)
+        return self.__get_dict(json)
+
     def get_course_contents(self, course_id: str) -> list[dict]:
         """Get contents from a course
 
         Args:
             course_id (str): The course id
 
         Returns:
```

### Comparing `my-moodle-0.4.3/my_moodle/config_utility.py` & `my-moodle-0.4.4/my_moodle/config_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/course_markdown_builder.py` & `my-moodle-0.4.4/my_moodle/course_markdown_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 CourseMarkdownBuilder Class
 """
 
 from html import unescape
 from os import makedirs
 from pathlib import Path
-from typing import Optional
 
 from my_moodle.wrapper import MoodleFile
 
 from .data_utility import FileData, content_course_filename
 from .markdown_document import MarkdownDocument
 from .markdown_methods import MarkdownLink
 
@@ -157,16 +156,27 @@
                     local_link = MarkdownLink(content_name, local_uri, content_name)
                     moodle_link = MarkdownLink(
                         _MOODLE_LINK_TEXT, moodle_content_url, content_name
                     )
                     self._markdown_document.write_bullet_line(
                         f"**{local_link}**: original at {moodle_link}"
                     )
-                    file_url = self.get_file_url(module_contents)
-                    self.__add_file(FileData(course_file_number, local_uri, file_url))
+                    file_url, file_size, file_created, file_modified = (
+                        self.get_file_data(module_contents)
+                    )
+                    self.__add_file(
+                        FileData(
+                            course_file_number,
+                            local_uri,
+                            file_url,
+                            file_size,
+                            file_created,
+                            file_modified,
+                        )
+                    )
                     course_file_number += 1
 
             else:
                 if is_link:
                     moodle_link = MarkdownLink(
                         f"`{content_name}`", moodle_content_url, content_name
                     )
@@ -182,16 +192,27 @@
                     local_link = MarkdownLink(content_name, local_uri, content_name)
                     moodle_link = MarkdownLink(
                         _MOODLE_LINK_TEXT, moodle_content_url, content_name
                     )
                     self._markdown_document.write_bullet_line(
                         f"**{local_link}**: original at {moodle_link}"
                     )
-                    file_url = self.get_file_url(module_contents)
-                    self.__add_file(FileData(course_file_number, local_uri, file_url))
+                    file_url, file_size, file_created, file_modified = (
+                        self.get_file_data(module_contents)
+                    )
+                    self.__add_file(
+                        FileData(
+                            course_file_number,
+                            local_uri,
+                            file_url,
+                            file_size,
+                            file_created,
+                            file_modified,
+                        )
+                    )
                     course_file_number += 1
             self._markdown_document.write_line()
         return course_file_number
 
     def get_file_url(self, module_contents: list) -> str:
         """Get the file URL
 
@@ -203,14 +224,34 @@
         """
         for module_content in module_contents:
             moodle_file = MoodleFile(module_content)
             if moodle_file.is_file() and "fileurl" in module_content:
                 return moodle_file.file_url
         return ""
 
+    def get_file_data(self, module_contents: list) -> tuple[str, int, int, int]:
+        """Get the file URL
+
+        Args:
+            module_contents (list): The module contents
+
+        Returns:
+            str: The file URL
+        """
+        for module_content in module_contents:
+            moodle_file = MoodleFile(module_content)
+            if moodle_file.is_file() and "fileurl" in module_content:
+                return (
+                    moodle_file.file_url,
+                    moodle_file.file_size,
+                    moodle_file.time_created,
+                    moodle_file.time_modified,
+                )
+        return "", 0, 0, 0
+
     def process_module_folder_contents(
         self, module_contents: list, course_file_number: int
     ) -> int:
         """_summary_
 
         Args:
             module_contents (list): _description_
@@ -230,17 +271,27 @@
                 local_link = MarkdownLink(content_name, local_uri, content_name)
                 moodle_link = MarkdownLink(
                     _MOODLE_LINK_TEXT, moodle_content_url, content_name
                 )
                 self._markdown_document.write_bullet_line(
                     f"**{local_link}**: original at {moodle_link}", 1
                 )
-                file_url = self.get_file_url(module_contents)
-
-                self.__add_file(FileData(course_file_number, local_uri, file_url))
+                file_url, file_size, file_created, file_modified = self.get_file_data(
+                    module_contents
+                )
+                self.__add_file(
+                    FileData(
+                        course_file_number,
+                        local_uri,
+                        file_url,
+                        file_size,
+                        file_created,
+                        file_modified,
+                    )
+                )
                 course_file_number += 1
             elif moodle_file.is_url():
                 moodle_link = MarkdownLink(
                     _MOODLE_LINK_TEXT, moodle_content_url, content_name
                 )
                 self._markdown_document.write_bullet_line(
                     f"**{local_link}**: original at {moodle_link}"
```

### Comparing `my-moodle-0.4.3/my_moodle/csv_utility.py` & `my-moodle-0.4.4/my_moodle/csv_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/enrolled_users_fields.py` & `my-moodle-0.4.4/my_moodle/enrolled_users_fields.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/json_utility.py` & `my-moodle-0.4.4/my_moodle/json_utility.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/markdown_document.py` & `my-moodle-0.4.4/my_moodle/markdown_document.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/markdown_methods.py` & `my-moodle-0.4.4/my_moodle/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle/moodle_data_downloader.py` & `my-moodle-0.4.4/my_moodle/moodle_data_downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 Moodle data downloader Class
 """
 
 import logging
-from os import makedirs
+from os import makedirs, utime
 from pathlib import Path
 from requests import get, RequestException
 from .api import Api
 from .course_markdown_builder import CourseMarkdownBuilder
-from .data_utility import FileData, get_courses_favoured
+from .data_utility import N_TUTORR, FileData, get_courses_favoured, is_file_a_copy
 from .json_utility import load_json_from_file, load_json_list_from_file
 from .moodle_json_downloader import MoodleJsonDownloader
 from .program_markdown_builder import ProgramMarkdownBuilder
 from .project_structure import clean_course_name, course_directory
 from .version import __version__
 
 
@@ -82,16 +82,16 @@
             courses (list): The courses
         """
         program_builder = ProgramMarkdownBuilder(self.program_name)
         program_builder.process_courses_json(courses)
         program_builder.save_to_directory(self.data_dir)
 
         for course in courses:
-            if course.get("coursecategory") == "N-TUTORR":
-                break
+            if course.get("coursecategory") == N_TUTORR:
+                continue
 
             course_name: str = clean_course_name(course.get("fullname", ""))
             directory_path: str = self.create_directory(course_directory(course))
             course_url: str = course.get("viewurl", "")
 
             course_markdown_builder = CourseMarkdownBuilder(
                 self.program_name, course_name, course_url
@@ -137,16 +137,16 @@
     def download_courses_contents(self, courses: list) -> None:
         """Download courses contents
 
         Args:
             courses (list): The courses
         """
         for course in courses:
-            if course.get("coursecategory") == "N-TUTORR":
-                break
+            if course.get("coursecategory") == N_TUTORR:
+                continue
             course_name: str = clean_course_name(course.get("fullname", ""))
             directory_path: str = self.create_directory(course_directory(course))
 
             self.download_course_contents(directory_path, course_name)
 
     def download_course_contents(self, directory_path: str, course_name: str) -> None:
         """Download all files from a course
@@ -168,42 +168,72 @@
         """Download files to a directory
 
         Args:
             directory_path (str): The directory path
             files (list): The files
         """
         for file in files:
-            message = f"Filename: {file.name} , URL: {file.url}"
-            print(message)
+            logging.info("Filename: %s , URL: %s", file.name, file.url)
             file_path = str(Path(directory_path, file.name).absolute())
-            # url contains forcedownload=1&token= so we can download the file directly
-            file_url: str = (
-                f"{file.url}&token={self.api.token}"
-                if file.url.find("&token=") == -1
-                else f"{file.url}?forcedownload=1&token={self.api.token}"
+
+            if is_file_a_copy(file, file_path):
+                logging.info("File already exists: %s", file_path)
+                continue
+
+            file_url: str = file.get_download_url(self.api.token)
+            self.download_file(
+                file_url,
+                file_path,
+                file.date_created,
+                file.date_modified,
+                self.api.timeout,
             )
-            self.download_file(file_url, file_path, self.api.timeout)
 
     @staticmethod
-    def download_file(file_url: str, save_path: str, timeout: float) -> None:
+    def download_file(
+        file_url: str,
+        save_path: str,
+        date_created: int,
+        date_modified: int,
+        timeout: float,
+    ) -> None:
         """Download a file from Moodle"""
         try:
             response = get(file_url, stream=True, timeout=timeout)
             response.raise_for_status()
 
             if response.status_code == 200:
                 with open(save_path, "wb") as file:
                     for chunk in response.iter_content(chunk_size=1024):
                         file.write(chunk)
+
+                MoodleDataDownloader.set_file_timestamps(
+                    save_path, date_created, date_modified
+                )
                 logging.info("Saved to: %s", save_path)
             else:
                 logging.warning("Download refused: %s", response.status_code)
         except RequestException as e:
             logging.error("Failed to download file: %s\n", str(e))
 
+    @staticmethod
+    def set_file_timestamps(save_path: str, date_created: int, date_modified: int):
+        """Set the file timestamps
+
+        Args:
+            save_path (str): The file path
+            date_created (int): The date created
+            date_modified (int): The date modified
+        """
+        if date_modified:
+            if date_created:
+                utime(save_path, (date_created, date_modified))
+            else:
+                utime(save_path, (date_modified, date_modified))
+
     def download_favorite_courses_contents(self) -> None:
         """Download favorite courses
 
         Returns:
             list: The favorite courses data
         """
         program = load_json_from_file(self._json_downloader.program_filepath)
```

### Comparing `my-moodle-0.4.3/my_moodle/moodle_json_downloader.py` & `my-moodle-0.4.4/my_moodle/moodle_json_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import logging
 from os import makedirs
 from pathlib import Path
 from .api import Api
 from .csv_utility import save_json_fields_list_to_csv
-from .data_utility import preprocess_enrolled_users, process_courses
+from .data_utility import N_TUTORR, preprocess_enrolled_users, process_courses
 from .enrolled_users_fields import EnrolledUsersFields
 from .json_utility import save_json_to_file
 from .project_structure import (
     clean_course_name,
     course_contents_filename,
     get_enrolled_filename,
     make_slug,
@@ -87,40 +87,43 @@
         """Download courses
 
         Args:
             courses_json (dict): The courses json
         """
 
         for course_json in courses_json.get("courses", []):
-            if course_json.get("coursecategory") == "N-TUTORR":
-                break
+            if course_json.get("coursecategory") == N_TUTORR:
+                continue
 
             self.download_course_contents(course_json)
             # self.download_json_course_private_files(course_json)
             self.download_students_by_course(course_json)
 
     def download_course_contents(self, course_json: dict) -> None:
         """Download course contents json
         Args:
             course_json (dict): The course json
         """
         course_id = course_json.get("id", "")
         name = clean_course_name(course_json.get("fullname", ""))
         self.download_course_contents_by_id(course_id, name)
 
-    def download_course_contents_by_id(self, course_id: str, course_name: str) -> None:
+    def download_course_contents_by_id(
+        self, course_id: str, course_name: str
+    ) -> list[dict]:
         """Download course contents json
 
         Args:
             course_id (str): The course id
             course_name (str): The course name
         """
         course_contents = self.api.get_course_contents(course_id)
         path = self.get_course_content_filepath(course_name)
         save_json_to_file(course_contents, path)
+        return course_contents
 
     def download_students_by_course(self, course_json: dict) -> None:
         """Download enrolled students
 
         Args:
             course_json (dict): The course json
         """
```

### Comparing `my-moodle-0.4.3/my_moodle/program_markdown_builder.py` & `my-moodle-0.4.4/my_moodle/program_markdown_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
-CourseMarkdownBuilder Class
+ProgramMarkdownBuilder Class
 """
 
+import logging
 from os import makedirs
 from os.path import dirname, join
 from pathlib import Path
 
 from my_moodle.json_utility import load_json_from_file
-from .data_utility import group_courses_by_category
+from .data_utility import N_TUTORR, group_courses_by_category
 from .markdown_document import MarkdownDocument
 from .markdown_methods import MarkdownLink
 from .project_structure import course_directory, clean_course_name
 
 class ProgramMarkdownBuilder:
     """Program Markdown Builder"""
 
@@ -122,15 +123,16 @@
             courses_json (dict): The courses json.
         """
 
         self.add_program(self._program_name)
         self.add_template_notice()
         courses_by_category = group_courses_by_category(courses_json)
         for category, courses in courses_by_category.items():
-            if category == "N-TUTORR":
+            if category == N_TUTORR:
+                logging.warning("Skipping category: %s", category)
                 continue
             self.add_category(category)
             courses = sorted(courses, key=lambda x: x.get("fullname", ""))
             for course in courses:
                 name =  clean_course_name(course.get("fullname", ""))
                 dir_path = course_directory(course)
```

### Comparing `my-moodle-0.4.3/my_moodle/project_structure.py` & `my-moodle-0.4.4/my_moodle/project_structure.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,14 +112,38 @@
 
     Returns:
         str: The filename
     """
     return f"enrolled-users-{clean_course_slug(course_name)}.{file_type}"
 
 
+def get_assignments_filename(course_name: str) -> str:
+    """Create an assignments filename
+
+    Args:
+        course_name (str): The course name
+
+    Returns:
+        str: The filename
+    """
+    return f"{clean_course_slug(course_name)}-assignments.json"
+
+
+def get_submissions_filename(course_name: str, assignment_name: str) -> str:
+    """Create an submissions filename
+
+    Args:
+        course_name (str): The course name
+
+    Returns:
+        str: The filename
+    """
+    return f"{clean_course_slug(course_name)}-submission-{make_slug(assignment_name)}.json"
+
+
 def make_slug(filename: str) -> str:
     """Generate a clean filename slug.
     Removes illegal characters and replaces spaces with dashes.
     Collapses multiple dashes into one.
 
     Args:
         filename (str): The filename
```

### Comparing `my-moodle-0.4.3/my_moodle/wrapper.py` & `my-moodle-0.4.4/my_moodle/wrapper.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/my_moodle.egg-info/PKG-INFO` & `my-moodle-0.4.4/my_moodle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my-moodle
-Version: 0.4.3
+Version: 0.4.4
 Summary: Download Moodle Course content.
 Home-page: https://github.com/marcocrowe/my-moodle-py-pi/
 Author: Mark Crowe
 Author-email: 66536097+marcocrowe@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/marcocrowe/my-moodle-py-pi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `my-moodle-0.4.3/my_moodle.egg-info/SOURCES.txt` & `my-moodle-0.4.4/my_moodle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 my_moodle/version.py
 my_moodle/wrapper.py
 my_moodle.egg-info/PKG-INFO
 my_moodle.egg-info/SOURCES.txt
 my_moodle.egg-info/dependency_links.txt
 my_moodle.egg-info/requires.txt
 my_moodle.egg-info/top_level.txt
+tests/_.py
 tests/__init__.py
+tests/api_test.py
 tests/config_parser_test.py
 tests/course_markdown_builder_test.py
 tests/moodle_data_downloader_test.py
 tests/moodle_data_utility_test.py
 tests/moodle_json_downloader_test.py
 tests/package_test.py
 tests/program_markdown_builder_test.py
```

### Comparing `my-moodle-0.4.3/readme.md` & `my-moodle-0.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/setup.py` & `my-moodle-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Setuptools configuration for my-moodle package.
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="my-moodle",
-    version="0.4.3",
+    version="0.4.4",
     author="Mark Crowe",
     author_email="66536097+marcocrowe@users.noreply.github.com",
     description="Download Moodle Course content.",
     long_description=open("readme.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/marcocrowe/my-moodle-py-pi/",
     project_urls={
```

### Comparing `my-moodle-0.4.3/tests/config_parser_test.py` & `my-moodle-0.4.4/tests/config_parser_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/course_markdown_builder_test.py` & `my-moodle-0.4.4/tests/course_markdown_builder_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Test cases for the project.
 Copyright © 2024 Mark Crowe <https://github.com/marcocrowe>. All rights reserved.
 """
 
 import unittest
 from pathlib import Path
 from my_moodle import CourseMarkdownBuilder
+from my_moodle.data_utility import N_TUTORR
 from my_moodle.json_utility import load_json_from_file, load_json_list_from_file
 from my_moodle.project_structure import (
     clean_course_name,
     course_contents_filename,
     course_directory,
 )
 
@@ -24,15 +25,15 @@
         data_directory = "_data"
         test_file = "program-business-with-computing-courses.json"
         test_file_path = str(Path(data_directory, test_file).absolute())
         courses_json = load_json_from_file(test_file_path).get("courses", [])
         program_name = "Business with Computing"
 
         for course in courses_json:
-            if course.get("coursecategory") == "N-TUTORR":
+            if course.get("coursecategory") == N_TUTORR:
                 continue
 
             self.__process_course(directory, data_directory, program_name, course)
 
     def __process_course(self, directory, data_directory, program_name, course):
         course_name: str = clean_course_name(course.get("fullname", ""))
         course_dir = course_directory(course)
```

### Comparing `my-moodle-0.4.3/tests/moodle_data_downloader_test.py` & `my-moodle-0.4.4/tests/moodle_data_downloader_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/moodle_data_utility_test.py` & `my-moodle-0.4.4/tests/moodle_data_utility_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/moodle_json_downloader_test.py` & `my-moodle-0.4.4/tests/moodle_json_downloader_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/package_test.py` & `my-moodle-0.4.4/tests/package_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/program_markdown_builder_test.py` & `my-moodle-0.4.4/tests/program_markdown_builder_test.py`

 * *Files identical despite different names*

### Comparing `my-moodle-0.4.3/tests/version_test.py` & `my-moodle-0.4.4/tests/version_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class TestVersion(unittest.TestCase):
     """Test case for version"""
 
     def test_version(self) -> None:
         """Test the version of the package"""
-        expected_version: str = "0.4.3"  # Update this value when the version changes
+        expected_version: str = "0.4.4"  # Update this value when the version changes
         self.assertEqual(
             __version__,
             expected_version,
             f"Expected version: {expected_version}, Actual version: {__version__}",
         )
```

