# Comparing `tmp/openedx-filters-1.7.0.tar.gz` & `tmp/openedx-filters-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-filters-1.7.0.tar", last modified: Thu Apr 11 22:26:31 2024, max compression
+gzip compressed data, was "openedx-filters-1.8.0.tar", last modified: Thu Apr 11 22:45:10 2024, max compression
```

## Comparing `openedx-filters-1.7.0.tar` & `openedx-filters-1.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24828 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/learning/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/tests/test_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/openedx_filters/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26293 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/learning/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/openedx_filters/learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22219 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/learning/tests/test_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/openedx_filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/openedx_filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/openedx_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 22:45:10.000000 openedx-filters-1.8.0/openedx_filters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 22:45:10.134712 openedx-filters-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-11 22:45:07.000000 openedx-filters-1.8.0/setup.py
```

### Comparing `openedx-filters-1.7.0/CHANGELOG.rst` & `openedx-filters-1.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[1.8.0] - 2024-04-11
+
+Added
+~~~~~
+
+* ORASubmissionViewRenderStarted filter added which can be used to modify the ORA submission view.
+
 [1.7.0] - 2024-04-11
 --------------------
 
 Added
 ~~~~~
 
 * Add Python 3.11 support.
```

### Comparing `openedx-filters-1.7.0/LICENSE.txt` & `openedx-filters-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/PKG-INFO` & `openedx-filters-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.7.0
+Version: 1.8.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-filters-1.7.0/README.rst` & `openedx-filters-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/exceptions.py` & `openedx-filters-1.8.0/openedx_filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/filters.py` & `openedx-filters-1.8.0/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/learning/filters.py` & `openedx-filters-1.8.0/openedx_filters/learning/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """
 Package where filters related to the learning architectural subdomain are implemented.
 """
 
+from typing import Optional
+
 from openedx_filters.exceptions import OpenEdxFilterException
 from openedx_filters.tooling import OpenEdxPublicFilter
 from openedx_filters.utils import SensitiveDataManagementMixin
 
 
 class AccountSettingsRenderStarted(OpenEdxPublicFilter):
     """
@@ -697,7 +699,43 @@
 
         Arguments:
             context (dict): context dictionary for instructor's tab template.
             template_name (str): template name to be rendered by the instructor's tab.
         """
         data = super().run_pipeline(context=context, template_name=template_name)
         return data.get("context"), data.get("template_name")
+
+
+class ORASubmissionViewRenderStarted(OpenEdxPublicFilter):
+    """
+    Custom class used to create ORA submission view filters and its custom methods.
+    """
+
+    filter_type = "org.openedx.learning.ora.submission_view.render.started.v1"
+
+    class RenderInvalidTemplate(OpenEdxFilterException):
+        """
+        Custom class used to stop the submission view render process.
+        """
+
+        def __init__(self, message: str, context: Optional[dict] = None, template_name: str = ""):
+            """
+            Override init that defines specific arguments used in the submission view render process.
+
+            Arguments:
+                message (str): error message for the exception.
+                context (dict): context used to the submission view template.
+                template_name (str): template path rendered instead.
+            """
+            super().__init__(message, context=context, template_name=template_name)
+
+    @classmethod
+    def run_filter(cls, context: dict, template_name: str):
+        """
+        Execute a filter with the signature specified.
+
+        Arguments:
+            context (dict): context dictionary for submission view template.
+            template_name (str): template name to be rendered by the student's dashboard.
+        """
+        data = super().run_pipeline(context=context, template_name=template_name, )
+        return data.get("context"), data.get("template_name")
```

### Comparing `openedx-filters-1.7.0/openedx_filters/learning/tests/test_filters.py` & `openedx-filters-1.8.0/openedx_filters/learning/tests/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     CourseEnrollmentQuerysetRequested,
     CourseEnrollmentStarted,
     CourseHomeUrlCreationStarted,
     CourseRunAPIRenderStarted,
     CourseUnenrollmentStarted,
     DashboardRenderStarted,
     InstructorDashboardRenderStarted,
+    ORASubmissionViewRenderStarted,
     StudentLoginRequested,
     StudentRegistrationRequested,
     VerticalBlockChildRenderStarted,
     VerticalBlockRenderCompleted,
 )
 
 
@@ -542,14 +543,44 @@
         Expected behavior:
             - The exception must have the attributes specified.
         """
         exception = dashboard_exception(message="You can't access the dashboard", **attributes)
 
         self.assertDictContainsSubset(attributes, exception.__dict__)
 
+    def test_ora_submission_view_render_started(self):
+        """
+        Test ORASubmissionViewRenderStarted filter behavior under normal conditions.
+
+        Expected behavior:
+            - The filter must have the signature specified.
+            - The filter should return context and template_name in that order.
+        """
+        result = ORASubmissionViewRenderStarted.run_filter(self.context, self.template_name)
+
+        self.assertTupleEqual((self.context, self.template_name,), result)
+
+    @data(
+        (
+            ORASubmissionViewRenderStarted.RenderInvalidTemplate,
+            {"context": {"course": Mock()}, "template_name": "custom-template.html"},
+        ),
+    )
+    @unpack
+    def test_halt_ora_submission_view_render(self, dashboard_exception, attributes):
+        """
+        Test for the ora submission view exceptions attributes.
+
+        Expected behavior:
+            - The exception must have the attributes specified.
+        """
+        exception = dashboard_exception(message="You can't access the view", **attributes)
+
+        self.assertDictContainsSubset(attributes, exception.__dict__)
+
 
 class TestCohortFilters(TestCase):
     """
     Test class to verify standard behavior of the cohort membership filters.
     You'll find test suites for:
 
     - CohortChangeRequested
```

### Comparing `openedx-filters-1.7.0/openedx_filters/tests/test_exceptions.py` & `openedx-filters-1.8.0/openedx_filters/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/tests/test_filters.py` & `openedx-filters-1.8.0/openedx_filters/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/tests/test_tooling.py` & `openedx-filters-1.8.0/openedx_filters/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/tooling.py` & `openedx-filters-1.8.0/openedx_filters/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters/utils.py` & `openedx-filters-1.8.0/openedx_filters/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/openedx_filters.egg-info/PKG-INFO` & `openedx-filters-1.8.0/openedx_filters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.7.0
+Version: 1.8.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openedx-filters-1.7.0/openedx_filters.egg-info/SOURCES.txt` & `openedx-filters-1.8.0/openedx_filters.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/requirements/constraints.txt` & `openedx-filters-1.8.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.7.0/setup.py` & `openedx-filters-1.8.0/setup.py`

 * *Files identical despite different names*

