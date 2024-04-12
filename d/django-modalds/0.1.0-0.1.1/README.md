# Comparing `tmp/django_modalds-0.1.0.tar.gz` & `tmp/django_modalds-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_modalds-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_modalds-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_modalds-0.1.0.tar` & `django_modalds-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,34 @@
--rw-r--r--   0        0        0     6148 2024-03-20 06:31:46.234580 django_modalds-0.1.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.1.0/.gitattributes
--rw-r--r--   0        0        0        7 2024-03-20 06:42:27.733546 django_modalds-0.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.1.0/LICENSE
--rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.1.0/__init__.py
--rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.1.0/django_modalds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.1.0/django_modalds/__init__.py
--rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.1.0/django_modalds/admin.py
--rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.1.0/django_modalds/apps.py
--rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.1.0/django_modalds/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.1.0/django_modalds/migrations/__init__.py
--rw-r--r--   0        0        0     5597 2024-03-20 04:58:30.866086 django_modalds-0.1.0/django_modalds/models.py
--rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.1.0/django_modalds/static/popupds/.DS_Store
--rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.1.0/django_modalds/static/popupds/js/jquery-3.6.0.min.js
--rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.1.0/django_modalds/static/popupds/js/jquery.cookie.js
--rw-r--r--   0        0        0     2736 2024-03-20 06:39:56.521967 django_modalds-0.1.0/django_modalds/templates/django_modalds/modalds.html
--rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.1.0/django_modalds/templates/django_modalds/type1.html
--rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.1.0/django_modalds/templates/django_modalds/type2.html
--rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.1.0/django_modalds/templates/django_modalds/type3.html
--rw-r--r--   0        0        0     2501 2024-03-18 03:18:17.561054 django_modalds-0.1.0/django_modalds/templates/django_modalds/type4.html
--rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.1.0/django_modalds/templates/django_modalds/type5.html
--rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.1.0/django_modalds/templatetags/__init__.py
--rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.1.0/django_modalds/templatetags/django_modalds_tags.py
--rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.1.0/django_modalds/tests.py
--rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.1.0/django_modalds/views.py
--rw-r--r--   0        0        0      684 2024-03-20 06:26:59.749784 django_modalds-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 django_modalds-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-03-20 06:31:46.234580 django_modalds-0.1.1/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-20 06:31:24.352716 django_modalds-0.1.1/.gitattributes
+-rw-r--r--   0        0        0        7 2024-03-20 06:42:27.733546 django_modalds-0.1.1/.gitignore
+-rw-r--r--   0        0        0      561 2024-03-20 06:42:46.246240 django_modalds-0.1.1/.idea/django-modalds.iml
+-rw-r--r--   0        0        0      174 2024-03-20 06:42:46.266987 django_modalds-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      419 2024-03-20 06:42:46.257139 django_modalds-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2024-03-20 06:42:46.249379 django_modalds-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-20 06:42:46.269904 django_modalds-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     3349 2024-04-12 05:19:57.446364 django_modalds-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     1079 2024-03-17 02:01:04.369747 django_modalds-0.1.1/LICENSE
+-rw-r--r--   0        0        0      986 2024-03-20 06:37:57.974200 django_modalds-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 12:26:04.845135 django_modalds-0.1.1/__init__.py
+-rw-r--r--   0        0        0     6148 2024-03-20 04:57:42.962921 django_modalds-0.1.1/django_modalds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.425896 django_modalds-0.1.1/django_modalds/__init__.py
+-rw-r--r--   0        0        0      673 2024-03-20 04:58:10.906719 django_modalds-0.1.1/django_modalds/admin.py
+-rw-r--r--   0        0        0      159 2024-03-20 06:34:50.496883 django_modalds-0.1.1/django_modalds/apps.py
+-rw-r--r--   0        0        0     5451 2024-03-20 05:16:29.358222 django_modalds-0.1.1/django_modalds/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-03-20 04:56:14.427712 django_modalds-0.1.1/django_modalds/migrations/__init__.py
+-rw-r--r--   0        0        0     5597 2024-03-20 04:58:30.866086 django_modalds-0.1.1/django_modalds/models.py
+-rw-r--r--   0        0        0     6148 2024-03-17 02:26:18.949539 django_modalds-0.1.1/django_modalds/static/popupds/.DS_Store
+-rw-r--r--   0        0        0    89501 2023-03-21 07:33:49.921877 django_modalds-0.1.1/django_modalds/static/popupds/js/jquery-3.6.0.min.js
+-rw-r--r--   0        0        0     3252 2023-03-21 07:33:49.693764 django_modalds-0.1.1/django_modalds/static/popupds/js/jquery.cookie.js
+-rw-r--r--   0        0        0     2515 2024-04-12 05:18:38.250197 django_modalds-0.1.1/django_modalds/templates/django_modalds/modalds.html
+-rw-r--r--   0        0        0     3154 2024-03-18 03:18:17.556824 django_modalds-0.1.1/django_modalds/templates/django_modalds/type1.html
+-rw-r--r--   0        0        0     3319 2024-03-18 03:18:17.567128 django_modalds-0.1.1/django_modalds/templates/django_modalds/type2.html
+-rw-r--r--   0        0        0     3069 2024-03-18 03:18:17.563552 django_modalds-0.1.1/django_modalds/templates/django_modalds/type3.html
+-rw-r--r--   0        0        0     2501 2024-03-18 03:18:17.561054 django_modalds-0.1.1/django_modalds/templates/django_modalds/type4.html
+-rw-r--r--   0        0        0      632 2024-03-18 03:18:17.565436 django_modalds-0.1.1/django_modalds/templates/django_modalds/type5.html
+-rw-r--r--   0        0        0        0 2024-03-15 04:56:10.557033 django_modalds-0.1.1/django_modalds/templatetags/__init__.py
+-rw-r--r--   0        0        0     1759 2024-03-20 06:37:57.977861 django_modalds-0.1.1/django_modalds/templatetags/django_modalds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-20 04:56:14.427567 django_modalds-0.1.1/django_modalds/tests.py
+-rw-r--r--   0        0        0       63 2024-03-20 04:56:14.426329 django_modalds-0.1.1/django_modalds/views.py
+-rw-r--r--   0        0        0      684 2024-04-12 07:06:23.609744 django_modalds-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 django_modalds-0.1.1/PKG-INFO
```

### Comparing `django_modalds-0.1.0/.DS_Store` & `django_modalds-0.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/LICENSE` & `django_modalds-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/README.md` & `django_modalds-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/.DS_Store` & `django_modalds-0.1.1/django_modalds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/admin.py` & `django_modalds-0.1.1/django_modalds/admin.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/migrations/0001_initial.py` & `django_modalds-0.1.1/django_modalds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/models.py` & `django_modalds-0.1.1/django_modalds/models.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/static/popupds/.DS_Store` & `django_modalds-0.1.1/django_modalds/static/popupds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/static/popupds/js/jquery-3.6.0.min.js` & `django_modalds-0.1.1/django_modalds/static/popupds/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/static/popupds/js/jquery.cookie.js` & `django_modalds-0.1.1/django_modalds/static/popupds/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/modalds.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/modalds.html`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 .modal-body {
   padding: 0;
 }
 </style>
 
 
 <!-- Modal -->
-<div class="modal fade" id="calendarModal" tabindex="-1" aria-labelledby="popupModal" aria-hidden="true">
+<div class="modal fade" id="popupModal" tabindex="-1" aria-labelledby="popupModal" aria-hidden="true">
   <div class="modal-dialog modal-lg">
     <div class="modal-content">
       <div class="modal-header">
-        <h5 class="modal-title" id="calendarModalLabel">{{ popup.modal_title }}</h5>
+        <h5 class="modal-title" id="popupModalLabel">{{ popup.modal_title }}</h5>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
       </div>
       <div class="modal-body">
         {% if type == 'Type1' %}
           {% include 'django_modalds/type1.html' %}
         {% elif type == 'Type2' %}
           {% include 'django_modalds/type2.html' %}
@@ -58,30 +58,24 @@
 
 <!-- 창이 열리자마자 모달을 뜨게하고 쿠키를 통해 다시 열기 방지 체크 및 창 오픈시 모달창 실행 스크립트 -->
 <script src="https://code.jquery.com/jquery-3.7.1.min.js" crossorigin="anonymous"></script>
 <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-cookie/1.4.1/jquery.cookie.min.js" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 
 <script>
   jQuery(document).ready(function($) {
-    if ($.cookie("ecacher-modal_calendarModal")) {
-      $("#demianModal").remove();
+    if ($.cookie("ecacher-modal_popupModal")) {
+      $("#popupModal").remove();
     } else {
-      {% if type == 'Calendar' %}
-        demian_modal = $("#calendarModal").modal()
-        demian_modal.on('shown.bs.modal', function () {
-          calendar.render();
-        })
-      {% endif %}
-      $("#calendarModal").modal("show");
+      $("#popupModal").modal("show");
     }
 
     $("#epopup_suppress").click(function() {
       if ($(this).is(":checked")) {
-          $("#calendarModal").modal("hide");
-          $.cookie("ecacher-modal_calendarModal", true);
+          $("#popupModal").modal("hide");
+          $.cookie("ecacher-modal_popupModal", true);
       } else {
-        $.cookie("ecacher-modal_calendarModal", false);
+        $.cookie("ecacher-modal_popupModal", false);
       }
     })
   });
 </script>
 {% endif %}
```

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/type1.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/type1.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/type2.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/type2.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/type3.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/type3.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/type4.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/type4.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templates/django_modalds/type5.html` & `django_modalds-0.1.1/django_modalds/templates/django_modalds/type5.html`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/django_modalds/templatetags/django_modalds_tags.py` & `django_modalds-0.1.1/django_modalds/templatetags/django_modalds_tags.py`

 * *Files identical despite different names*

### Comparing `django_modalds-0.1.0/pyproject.toml` & `django_modalds-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-modalds"
-version = "0.1.0"
+version = "0.1.1"
 description = "One of the my demiansoft apps"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 5.0.3",
```

### Comparing `django_modalds-0.1.0/PKG-INFO` & `django_modalds-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-modalds
-Version: 0.1.0
+Version: 0.1.1
 Summary: One of the my demiansoft apps
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 5.0.3
 Requires-Dist: pillow >= 10.2.0
 Project-URL: Home, https://www.demiansoft.com
```

