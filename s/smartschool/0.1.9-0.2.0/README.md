# Comparing `tmp/smartschool-0.1.9.tar.gz` & `tmp/smartschool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartschool-0.1.9.tar", max compression
+gzip compressed data, was "smartschool-0.2.0.tar", max compression
```

## Comparing `smartschool-0.1.9.tar` & `smartschool-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-11-17 13:53:05.752129 smartschool-0.1.9/LICENSE
--rw-r--r--   0        0        0     1666 2023-11-17 14:07:23.659646 smartschool-0.1.9/README.md
--rw-r--r--   0        0        0     3555 2023-12-01 18:25:25.467053 smartschool-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0     3755 2023-11-17 13:53:05.756130 smartschool-0.1.9/scripts/smartschool_report_on_future_tasks
--rwxr-xr-x   0        0        0     4472 2023-12-01 18:25:25.471053 smartschool-0.1.9/scripts/smartschool_report_on_results
--rw-r--r--   0        0        0     1225 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/__init__.py
--rw-r--r--   0        0        0     4255 2023-11-17 18:04:21.099316 smartschool-0.1.9/src/smartschool/_xml_interface.py
--rw-r--r--   0        0        0     5015 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/agenda.py
--rw-r--r--   0        0        0     7197 2023-11-17 14:07:23.663646 smartschool-0.1.9/src/smartschool/common.py
--rw-r--r--   0        0        0     1371 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/courses.py
--rw-r--r--   0        0        0     1527 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/credentials.py
--rw-r--r--   0        0        0      452 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/logger.py
--rw-r--r--   0        0        0     7680 2023-11-17 17:34:42.548921 smartschool-0.1.9/src/smartschool/messages.py
--rw-r--r--   0        0        0     9456 2023-11-20 17:23:00.462382 smartschool-0.1.9/src/smartschool/objects.py
--rw-r--r--   0        0        0      540 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/periods.py
--rw-r--r--   0        0        0     1095 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/results.py
--rw-r--r--   0        0        0     4086 2023-11-17 18:04:21.099316 smartschool-0.1.9/src/smartschool/session.py
--rw-r--r--   0        0        0      669 2023-11-17 13:53:05.756130 smartschool-0.1.9/src/smartschool/student_support.py
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 smartschool-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-11-17 13:53:05.752129 smartschool-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1666 2023-11-17 14:07:23.659646 smartschool-0.2.0/README.md
+-rw-r--r--   0        0        0     3555 2024-04-12 06:27:51.125157 smartschool-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     3755 2023-11-17 13:53:05.756130 smartschool-0.2.0/scripts/smartschool_report_on_future_tasks
+-rwxr-xr-x   0        0        0     4472 2023-12-01 18:25:25.471053 smartschool-0.2.0/scripts/smartschool_report_on_results
+-rw-r--r--   0        0        0     1225 2023-11-17 13:53:05.756130 smartschool-0.2.0/src/smartschool/__init__.py
+-rw-r--r--   0        0        0     4255 2023-11-17 18:04:21.099316 smartschool-0.2.0/src/smartschool/_xml_interface.py
+-rw-r--r--   0        0        0     5015 2023-11-17 13:53:05.756130 smartschool-0.2.0/src/smartschool/agenda.py
+-rw-r--r--   0        0        0     7197 2023-11-17 14:07:23.663646 smartschool-0.2.0/src/smartschool/common.py
+-rw-r--r--   0        0        0     1373 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/courses.py
+-rw-r--r--   0        0        0     1527 2023-11-17 13:53:05.756130 smartschool-0.2.0/src/smartschool/credentials.py
+-rw-r--r--   0        0        0      452 2023-11-17 13:53:05.756130 smartschool-0.2.0/src/smartschool/logger.py
+-rw-r--r--   0        0        0     7683 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/messages.py
+-rw-r--r--   0        0        0     9457 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/objects.py
+-rw-r--r--   0        0        0      541 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/periods.py
+-rw-r--r--   0        0        0     1096 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/results.py
+-rw-r--r--   0        0        0     4086 2023-11-17 18:04:21.099316 smartschool-0.2.0/src/smartschool/session.py
+-rw-r--r--   0        0        0      670 2024-04-12 06:27:51.133157 smartschool-0.2.0/src/smartschool/student_support.py
+-rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 smartschool-0.2.0/PKG-INFO
```

### Comparing `smartschool-0.1.9/LICENSE` & `smartschool-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/README.md` & `smartschool-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/pyproject.toml` & `smartschool-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartschool"
-version = "0.1.9"
+version = "0.2.0"
 description = "Unofficial API interface to the smartschool system."
 authors = ["Steven 'KaReL' Van Ingelgem <steven@vaningelgem.be>"]
 readme = "README.md"
 homepage = "https://github.com/svaningelgem/smartschool"
 license = "GPL-3.0"
 packages = [{include = "smartschool", from = "src"}]
```

### Comparing `smartschool-0.1.9/scripts/smartschool_report_on_future_tasks` & `smartschool-0.2.0/scripts/smartschool_report_on_future_tasks`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/scripts/smartschool_report_on_results` & `smartschool-0.2.0/scripts/smartschool_report_on_results`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/__init__.py` & `smartschool-0.2.0/src/smartschool/__init__.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/_xml_interface.py` & `smartschool-0.2.0/src/smartschool/_xml_interface.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/agenda.py` & `smartschool-0.2.0/src/smartschool/agenda.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/common.py` & `smartschool-0.2.0/src/smartschool/common.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/courses.py` & `smartschool-0.2.0/src/smartschool/courses.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     Example:
     -------
     >>> for course in TopNavCourses():
     >>>     print(course.name)
     Aardrijkskunde_3_LOP_2023-2024
     bibliotheek
+
     """
 
     @cached_property
     def _list(self) -> list[CourseCondensed]:
         return [CourseCondensed(**course) for course in session.json("/Topnav/getCourseConfig", method="post")["own"]]
 
     def __iter__(self) -> Iterator[CourseCondensed]:
@@ -41,14 +42,15 @@
 
     Example:
     -------
     >>> for course in Courses():
     >>>     print(course.name)
     Aardrijkskunde
     Biologie
+
     """
 
     @cached_property
     def _list(self) -> list[Course]:
         return [Course(**course) for course in session.json("/results/api/v1/courses/")]
 
     def __iter__(self) -> Iterator[Course]:
```

### Comparing `smartschool-0.1.9/src/smartschool/credentials.py` & `smartschool-0.2.0/src/smartschool/credentials.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/messages.py` & `smartschool-0.2.0/src/smartschool/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
     Example:
     -------
     >>> for message in MessageHeaders():
     >>>     print(message.subject)
     Re: LO les
     Frans
+
     """
 
     def __init__(
         self,
         box_type: BoxType = BoxType.INBOX,
         sort_by: SortField = SortField.DATE,
         sort_order: SortOrder = SortOrder.DESC,
@@ -147,14 +148,15 @@
     To reproduce: just go to a message and click it.
 
     Example:
     -------
     >>> message: FullMessage = list(Message(123))[0]
     >>> message.subject
     Griezelfestijn
+
     """
 
     @property
     def _action(self) -> str:
         return "show message"
 
     @property
@@ -185,14 +187,15 @@
 
     Example:
     -------
     >>> for attachment in Attachments(123):
     >>>     print(attachment.name)
     Oproep figuranten en helpers.pdf
     Poster griezelfestijn.pdf
+
     """
 
     @property
     def _action(self) -> str:
         return "attachment list"
 
     @property
```

### Comparing `smartschool-0.1.9/src/smartschool/objects.py` & `smartschool-0.2.0/src/smartschool/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     >>> for day in FutureTasks().days:
     >>>     for course in day.courses:
     >>>         print("Course:", course.course_title)
     >>>         for task in course.items.tasks:
     >>>             print("Task:", task.description)
     Course: 2 - AAR1, Lotte Peeters
     Task: Toets 3. De koolstofcyclus in het systeem aarde pagina 42 - 47
+
     """
 
     days: list[FutureTaskOneDay] = Field(default_factory=list)
     last_assignment_id: int = 0
     last_date: Date = Field(default_factory=date.today)
 
     def __post_init__(self):
```

### Comparing `smartschool-0.1.9/src/smartschool/periods.py` & `smartschool-0.2.0/src/smartschool/periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 
     Example:
     -------
     >>> for period in Periods():
     >>>     print(period.name)
     1 september - 24 oktober
     25 oktober - 19 december
+
     """
 
     def __iter__(self) -> Iterator[Period]:
         for period in session.json("/results/api/v1/periods/"):
             yield Period(**period)
```

### Comparing `smartschool-0.1.9/src/smartschool/results.py` & `smartschool-0.2.0/src/smartschool/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     To reproduce: "Ga naar" > "Resultaten", it'll be one of the XHR calls then.
 
     Example:
     -------
     >>> for result in Results():
     >>>     print(result.name)
     Repetitie hoofdstuk 1
+
     """
 
     def __iter__(self) -> Iterator[Result]:
         for page_nr in count(start=1):  # pragma: no branch
             json = session.json(f"/results/api/v1/evaluations/?pageNumber={page_nr}&itemsOnPage={RESULTS_PER_PAGE}")
             for result in json:
                 yield Result(**result)
```

### Comparing `smartschool-0.1.9/src/smartschool/session.py` & `smartschool-0.2.0/src/smartschool/session.py`

 * *Files identical despite different names*

### Comparing `smartschool-0.1.9/src/smartschool/student_support.py` & `smartschool-0.2.0/src/smartschool/student_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 
     Example:
     -------
     >>> for link in StudentSupportLinks():
     >>>     print(link.name)
     1712
     Autisme chat
+
     """
 
     def __iter__(self) -> Iterator[StudentSupportLink]:
         json = session.json("/student-support/api/v1/")
         for result in json:
             yield StudentSupportLink(**result)
```

### Comparing `smartschool-0.1.9/PKG-INFO` & `smartschool-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartschool
-Version: 0.1.9
+Version: 0.2.0
 Summary: Unofficial API interface to the smartschool system.
 Home-page: https://github.com/svaningelgem/smartschool
 License: GPL-3.0
 Author: Steven 'KaReL' Van Ingelgem
 Author-email: steven@vaningelgem.be
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

