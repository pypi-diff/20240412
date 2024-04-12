# Comparing `tmp/wagtail_bynder-0.2.0.tar.gz` & `tmp/wagtail_bynder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_bynder-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtail_bynder-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtail_bynder-0.2.0.tar` & `wagtail_bynder-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
--rw-r--r--   0        0        0     2643 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1495 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/LICENSE
--rw-r--r--   0        0        0     8720 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/README.md
--rw-r--r--   0        0        0     1836 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      916 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/__init__.py
--rw-r--r--   0        0        0       22 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/__version__.py
--rw-r--r--   0        0        0      149 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/apps.py
--rw-r--r--   0        0        0      516 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/blocks.py
--rw-r--r--   0        0        0     5839 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/management/commands/base.py
--rw-r--r--   0        0        0      228 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/management/commands/update_stale_documents.py
--rw-r--r--   0        0        0      803 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/management/commands/update_stale_images.py
--rw-r--r--   0        0        0      216 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/management/commands/update_stale_videos.py
--rw-r--r--   0        0        0     1791 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/middleware.py
--rw-r--r--   0        0        0    13782 2024-02-25 16:58:34.001032 wagtail_bynder-0.2.0/src/wagtail_bynder/models.py
--rw-r--r--   0        0        0   976618 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js
--rw-r--r--   0        0        0     1190 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js
--rw-r--r--   0        0        0     1289 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js
--rw-r--r--   0        0        0      171 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/video-chooser.js
--rw-r--r--   0        0        0     2563 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js
--rw-r--r--   0        0        0     1214 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js
--rw-r--r--   0        0        0     1190 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js
--rw-r--r--   0        0        0      532 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html
--rw-r--r--   0        0        0      515 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html
--rw-r--r--   0        0        0        0 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/templatetags/__init__.py
--rw-r--r--   0        0        0      311 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/templatetags/bynder_tags.py
--rw-r--r--   0        0        0     2215 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/utils.py
--rw-r--r--   0        0        0        0 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/views/__init__.py
--rw-r--r--   0        0        0     2472 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/views/document.py
--rw-r--r--   0        0        0     2372 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/views/image.py
--rw-r--r--   0        0        0     1845 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/views/mixins.py
--rw-r--r--   0        0        0     2186 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/views/video.py
--rw-r--r--   0        0        0     2333 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/wagtail_hooks.py
--rw-r--r--   0        0        0     1535 2024-02-25 16:58:34.009032 wagtail_bynder-0.2.0/src/wagtail_bynder/widgets.py
--rw-r--r--   0        0        0    10331 1970-01-01 00:00:00.000000 wagtail_bynder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2643 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1495 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/LICENSE
+-rw-r--r--   0        0        0    13052 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/README.md
+-rw-r--r--   0        0        0     1836 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      916 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/__version__.py
+-rw-r--r--   0        0        0      149 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/apps.py
+-rw-r--r--   0        0        0      516 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/blocks.py
+-rw-r--r--   0        0        0      161 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/exceptions.py
+-rw-r--r--   0        0        0     9277 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/base.py
+-rw-r--r--   0        0        0      336 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_documents.py
+-rw-r--r--   0        0        0      324 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_images.py
+-rw-r--r--   0        0        0      325 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/refresh_bynder_videos.py
+-rw-r--r--   0        0        0      400 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_documents.py
+-rw-r--r--   0        0        0     1033 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_images.py
+-rw-r--r--   0        0        0      386 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/management/commands/update_stale_videos.py
+-rw-r--r--   0        0        0     1791 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/middleware.py
+-rw-r--r--   0        0        0    15692 2024-04-12 15:41:32.454192 wagtail_bynder-0.3.0/src/wagtail_bynder/models.py
+-rw-r--r--   0        0        0   976618 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js
+-rw-r--r--   0        0        0     1190 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js
+-rw-r--r--   0        0        0     1289 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js
+-rw-r--r--   0        0        0      171 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser.js
+-rw-r--r--   0        0        0     2563 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js
+-rw-r--r--   0        0        0     1214 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js
+-rw-r--r--   0        0        0     1190 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js
+-rw-r--r--   0        0        0      532 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html
+-rw-r--r--   0        0        0      515 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html
+-rw-r--r--   0        0        0        0 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templatetags/__init__.py
+-rw-r--r--   0        0        0      311 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/templatetags/bynder_tags.py
+-rw-r--r--   0        0        0     1971 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/__init__.py
+-rw-r--r--   0        0        0     2472 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/document.py
+-rw-r--r--   0        0        0     2372 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/image.py
+-rw-r--r--   0        0        0     1845 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/mixins.py
+-rw-r--r--   0        0        0     2186 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/views/video.py
+-rw-r--r--   0        0        0     2333 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/wagtail_hooks.py
+-rw-r--r--   0        0        0     1535 2024-04-12 15:41:32.458192 wagtail_bynder-0.3.0/src/wagtail_bynder/widgets.py
+-rw-r--r--   0        0        0    14663 1970-01-01 00:00:00.000000 wagtail_bynder-0.3.0/PKG-INFO
```

### Comparing `wagtail_bynder-0.2.0/CONTRIBUTING.md` & `wagtail_bynder-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/LICENSE` & `wagtail_bynder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/pyproject.toml` & `wagtail_bynder-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/__init__.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/blocks.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/middleware.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/middleware.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/models.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,95 +1,78 @@
 import logging
 import math
-import os
 
 from datetime import datetime
 from mimetypes import guess_type
 from typing import Any
 
 from django.conf import settings
-from django.core.exceptions import ImproperlyConfigured
-from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 from django.utils.functional import cached_property
 from django.utils.translation import gettext_lazy as _
 from wagtail.admin.panels import FieldPanel, MultiFieldPanel
 from wagtail.documents.models import AbstractDocument, Document
 from wagtail.images.models import AbstractImage, Image
 from wagtail.models import Collection, CollectionMember
 from wagtail.search import index
 
 from wagtail_bynder import utils
 
+from .exceptions import BynderAssetDataError
+
 
 logger = logging.getLogger("wagtail.images")
 
 
 class BynderAssetMixin(models.Model):
     # Fields relevant to the Bynder integration only
     bynder_id = models.CharField(
         verbose_name=_("Bynder asset ID"),
         max_length=36,
         blank=True,
         unique=True,
         editable=False,
         db_index=True,
-    )
-    bynder_id_hash = models.CharField(max_length=100, blank=True, editable=False)
-    bynder_original_filename = models.CharField(
-        max_length=255, blank=True, editable=False
+        null=True,
     )
     bynder_last_modified = models.DateTimeField(
         null=True, editable=False, db_index=True
     )
+    source_filename = models.CharField(
+        verbose_name=_("source filename"),
+        max_length=255,
+        blank=True,
+        editable=False,
+    )
+    original_filesize = models.IntegerField(
+        verbose_name=_("original filesize"), editable=False, null=True
+    )
 
     # Fields for broader use
     description = models.TextField(verbose_name=_("description"), blank=True)
     copyright = models.TextField(verbose_name=_("copyright info"), blank=True)
     is_archived = models.BooleanField(
         verbose_name=_("asset is archived"), default=False
     )
     is_limited_use = models.BooleanField(
         verbose_name=_("asset is marked as 'limited use'"),
         default=False,
     )
     is_public = models.BooleanField(
         verbose_name=_("asset is marked as public"), default=False
     )
-    metadata = models.JSONField(
-        verbose_name=_("additional metadata"),
-        default=dict,
-        encoder=DjangoJSONEncoder,
-        blank=True,
-    )
 
     extra_admin_form_fields = (
         "description",
         "copyright",
-        "metadata",
         "is_archived",
         "is_limited_use",
         "is_public",
     )
 
-    directly_mapped_bynder_fields = (
-        "id",
-        "name",
-        "copyright",
-        "description",
-        "idHash",
-        "dateModified",
-        "archive",
-        "limited",
-        "isPublic",
-        "extension",
-        "original",
-        "type",
-    )
-
     extra_search_fields = [
         index.SearchField("bynder_id", boost=3),
         index.SearchField("description"),
         index.SearchField("copyright"),
         index.AutocompleteField("bynder_id"),
         index.AutocompleteField("description"),
         index.AutocompleteField("copyright"),
@@ -117,68 +100,86 @@
         Update this object (without saving) to reflect values in `asset_data`,
         which is a representation of the related asset from the Bynder API.
         """
         self.title = asset_data.get("name", self.title)
         self.copyright = asset_data.get("copyright", self.copyright)
         self.description = asset_data.get("description", self.description)
         self.collection = self.get_target_collection(asset_data)
-        self.bynder_id_hash = asset_data["idHash"]
         self.bynder_last_modified = asset_data["dateModified"]
-        self.metadata = self.extract_relevant_metadata(asset_data)
         self.is_archived = bool(asset_data.get("archive", 0))
         self.is_limited_use = bool(asset_data.get("limited", 0))
         self.is_public = bool(asset_data.get("isPublic", 0))
 
     def get_target_collection(self, asset_data: dict[str, Any]) -> Collection:
         return utils.get_default_collection()
 
-    def extract_relevant_metadata(self, asset_data: dict[str, Any]) -> dict[str, Any]:
-        directly_mapped = set(self.directly_mapped_bynder_fields)
-        return {k: v for k, v in asset_data.items() if k not in directly_mapped}
-
 
 class BynderAssetWithFileMixin(BynderAssetMixin):
     extra_search_fields = BynderAssetMixin.extra_search_fields + [
         index.SearchField("file", boost=1),
         index.AutocompleteField("file"),
     ]
 
     class Meta:
         abstract = True
 
+    @staticmethod
+    def extract_file_source(asset_data: dict[str, Any]) -> str:
+        raise NotImplementedError
+
     def update_from_asset_data(self, asset_data: dict[str, Any]) -> None:
         super().update_from_asset_data(asset_data)
-        if self.asset_file_has_changed(asset_data):
-            self.bynder_original_filename = os.path.basename(asset_data["original"])
-            self.file = self.download_asset_file(asset_data)
+        if not self.file or self.asset_file_has_changed(asset_data):
+            self.update_file(asset_data)
 
     def asset_file_has_changed(self, asset_data: dict[str, Any]) -> bool:
-        filename = os.path.basename(asset_data["original"])
-        return self.bynder_original_filename != filename
+        source_url = self.extract_file_source(asset_data)
+        filename = utils.filename_from_url(source_url)
+        return (
+            self.source_filename != filename
+            or self.original_filesize is None
+            or self.original_filesize != int(asset_data["fileSize"])
+        )
 
-    def download_asset_file(self, asset_data: dict[str, Any]) -> utils.DownloadedFile:
-        raise NotImplementedError
+    def update_file(self, asset_data: dict[str, Any]) -> None:
+        source_url = self.extract_file_source(asset_data)
+        self.file = utils.download_asset(source_url)
+
+        # Used to trigger additional updates on save()
+        self._file_changed = True
+
+        # Update supplementary field values
+        self.source_filename = utils.filename_from_url(source_url)
+        self.original_filesize = int(asset_data["fileSize"])
 
 
 class BynderSyncedImage(BynderAssetWithFileMixin, AbstractImage):
     admin_form_fields = (
         Image.admin_form_fields + BynderAssetMixin.extra_admin_form_fields
     )
 
-    directly_mapped_bynder_fields = BynderAssetMixin.directly_mapped_bynder_fields + (
-        "activeOriginalFocusPoint",
+    original_width = models.IntegerField(
+        verbose_name=_("original width"), null=True, editable=False
+    )
+    original_height = models.IntegerField(
+        verbose_name=_("original height"), null=True, editable=False
     )
 
     search_fields = (
         AbstractImage.search_fields + BynderAssetWithFileMixin.extra_search_fields
     )
 
-    class Meta:
+    class Meta(AbstractImage.Meta):
         abstract = True
 
+    def save(self, *args, **kwargs):
+        if getattr(self, "_file_changed", False):
+            self._set_image_file_metadata()
+        super().save(*args, **kwargs)
+
     def update_from_asset_data(
         self,
         asset_data: dict[str, Any],
     ) -> None:
         # Update the file and other field values without saving the changes
         super().update_from_asset_data(asset_data)
 
@@ -188,14 +189,26 @@
             self.set_focal_area_from_focus_point(
                 int(focus_point["x"]),
                 int(focus_point["y"]),
                 int(asset_data["height"]),
                 int(asset_data["width"]),
             )
 
+    def asset_file_has_changed(self, asset_data: dict[str, Any]) -> bool:
+        return (
+            super().asset_file_has_changed(asset_data)
+            or (self.original_height or 0) != int(asset_data["height"])
+            or (self.original_width or 0) != int(asset_data["width"])
+        )
+
+    def update_file(self, asset_data: dict[str, Any]) -> None:
+        self.original_width = int(asset_data["width"])
+        self.original_height = int(asset_data["height"])
+        return super().update_file(asset_data)
+
     def set_focal_area_from_focus_point(
         self, x: int, y: int, original_height: int, original_width: int
     ) -> None:
         """
         Using the provided center-point coordinates, generate a
         2D focal area for the downloaded image.
         """
@@ -217,58 +230,78 @@
 
         # For the width, span outwards until we hit the left or right bounds
         self.focal_point_width = min(x, self.width - x) * 2
 
         # For the height, span outwards until we hit the top or bottom bounds
         self.focal_point_height = min(y, self.height - y) * 2
 
-    def download_asset_file(self, asset_data: dict[str, Any]) -> utils.DownloadedFile:
-        # Use the thumbnail specified in settings as the source image for
-        # Wagtail. NOTE: This should still be a high quality image. We just
-        # don't need a print quality original to generate renditions from.
-        key = getattr(settings, "BYNDER_IMAGE_SOURCE_THUMBNAIL_NAME", "webimage")
+    @staticmethod
+    def extract_file_source(asset_data: dict[str, Any]) -> str:
+        # For images, we store and use the source derivative filename,
+        # because the 'original' isn't always present
+        asset_id = asset_data["id"]
+        key = getattr(settings, "BYNDER_IMAGE_SOURCE_THUMBNAIL_NAME", "WagtailSource")
         thumbnails = asset_data["thumbnails"]
         try:
-            source_url = thumbnails[key]
+            return thumbnails[key]
         except KeyError as e:
-            raise ImproperlyConfigured(
-                f"The '{key}' derivative is missing from 'thumbnails' for image asset '{self.bynder_id}'. "
+            raise BynderAssetDataError(
+                f"The '{key}' derivative is missing from 'thumbnails' for image asset '{asset_id}'. "
                 "You might need to update the 'BYNDER_IMAGE_SOURCE_THUMBNAIL_NAME' setting value to reflect "
-                "derivative names used in your Bynder instance. The available derivative for this asset "
-                f"are: {thumbnails.keys()}"
+                "derivative names used in your Bynder instance. The available derivatives for this asset "
+                f"are: {list(thumbnails.keys())}"
             ) from e
-        return utils.download_image(source_url)
 
 
 class BynderSyncedDocument(BynderAssetWithFileMixin, AbstractDocument):
     admin_form_fields = (
         Document.admin_form_fields + BynderAssetMixin.extra_admin_form_fields
     )
 
     search_fields = (
         AbstractDocument.search_fields + BynderAssetWithFileMixin.extra_search_fields
     )
 
-    class Meta:
+    class Meta(AbstractDocument.Meta):
         abstract = True
 
-    def download_asset_file(self, asset_data: dict[str, Any]) -> utils.DownloadedFile:
-        return utils.download_document(asset_data["original"])
+    def save(self, *args, **kwargs):
+        if getattr(self, "_file_changed", False):
+            self._set_document_file_metadata()
+        super().save(*args, **kwargs)
+
+    @staticmethod
+    def extract_file_source(asset_data: dict[str, Any]) -> str:
+        asset_id = asset_data["id"]
+        try:
+            return asset_data["original"]
+        except KeyError as e:
+            raise BynderAssetDataError(
+                f"'original' is missing from the API representation for document asset '{asset_id}'. "
+                "This is likely because the asset is marked as 'private' in Bynder. Wagtail needs the "
+                "'original' asset URL in order to download and save its own copy."
+            ) from e
 
 
 class BynderSyncedVideo(
     BynderAssetMixin, CollectionMember, index.Indexed, models.Model
 ):
     title = models.CharField(max_length=255, verbose_name=_("title"))
     created_at = models.DateTimeField(
         verbose_name=_("created at"), auto_now_add=True, db_index=True
     )
     updated_at = models.DateTimeField(
         verbose_name=_("last updated at"), auto_now=True, db_index=True
     )
+    original_width = models.IntegerField(
+        verbose_name=_("original width"), null=True, editable=False
+    )
+    original_height = models.IntegerField(
+        verbose_name=_("original height"), null=True, editable=False
+    )
     primary_source_url = models.URLField(
         verbose_name=_("primary source URL"),
         help_text=_(
             "A derivative using a WebM container using the VP9 codec for video and the Opus codec "
             "for audio. These are all open, royalty-free formats which are generally "
             "well-supported, although only in quite recent browsers, which is why a fallback is a "
             "good idea."
@@ -304,19 +337,28 @@
             heading=_("Status flags"),
             children=[
                 FieldPanel("is_archived", read_only=True),
                 FieldPanel("is_limited_use", read_only=True),
                 FieldPanel("is_public", read_only=True),
             ],
         ),
-        FieldPanel("metadata", read_only=True),
+        MultiFieldPanel(
+            heading=_("Further information"),
+            children=[
+                FieldPanel("original_filesize", read_only=True),
+                FieldPanel("original_height", read_only=True),
+                FieldPanel("original_width", read_only=True),
+            ],
+        ),
     ]
 
     class Meta:
         abstract = True
+        verbose_name = _("video")
+        verbose_name_plural = _("videos")
 
     def __str__(self):
         return self.title
 
     @cached_property
     def primary_source_mimetype(self) -> str:
         if not self.primary_source_url:
@@ -329,44 +371,50 @@
             return ""
         return guess_type(self.fallback_source_url)[0]
 
     def update_from_asset_data(
         self,
         asset_data: dict[str, Any],
     ) -> None:
-        super().update_from_asset_data(asset_data)
-
         primary_derivative_name = getattr(
-            settings, "BYNDER_VIDEO_PRIMARY_DERIVATIVE_NAME", "Web-Primary"
+            settings, "BYNDER_VIDEO_PRIMARY_DERIVATIVE_NAME", "WebPrimary"
         )
         fallback_derivative_name = getattr(
-            settings, "BYNDER_VIDEO_FALLBACK_DERIVATIVE_NAME", "Web-Fallback"
+            settings, "BYNDER_VIDEO_FALLBACK_DERIVATIVE_NAME", "WebFallback"
         )
         poster_image_derivative_name = getattr(
             settings, "BYNDER_VIDEO_POSTER_IMAGE_DERIVATIVE_NAME", "webimage"
         )
 
         derivatives = {v.split("/")[-2]: v for v in asset_data["videoPreviewURLs"]}
         try:
             self.primary_source_url = derivatives[primary_derivative_name]
-        except KeyError:
-            raise ImproperlyConfigured(
+        except KeyError as e:
+            raise BynderAssetDataError(
                 "'videoPreviewURLs' does not contain a URL matching the derivative name "
                 f"'{primary_derivative_name}'. You might need to update the "
                 "'BYNDER_VIDEO_PRIMARY_DERIVATIVE_NAME' setting value to reflect the derivative "
                 "names set by Bynder for your instance. The available derivatives for this "
-                f"asset are: {derivatives}"
-            ) from None
+                f"asset are: {list(derivatives.keys())}"
+            ) from e
+        else:
+            self.source_filename = utils.filename_from_url(self.primary_source_url)
 
         self.fallback_source_url = derivatives.get(fallback_derivative_name)
 
         thumbnails = asset_data["thumbnails"]
         try:
             self.poster_image_url = thumbnails[poster_image_derivative_name]
         except KeyError as e:
-            raise ImproperlyConfigured(
+            raise BynderAssetDataError(
                 f"The '{poster_image_derivative_name}' derivative is missing from 'thumbnails' for "
                 f"video asset '{self.bynder_id}'. You might need to update the "
                 "'BYNDER_VIDEO_POSTER_IMAGE_DERIVATIVE_NAME' setting value to reflect the "
                 "derivative names set by Bynder for you instance. The available derivative names "
-                f"for this asset are: {thumbnails.keys()}"
+                f"for this asset are: {list(thumbnails.keys())}"
             ) from e
+
+        self.original_filesize = int(asset_data["fileSize"])
+        self.original_width = int(asset_data["width"])
+        self.original_height = int(asset_data["height"])
+
+        super().update_from_asset_data(asset_data)
```

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/compactview-v4.0.0.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/bynder/js/video-chooser-telepath.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailadmin/js/chooser-modal-handler-factory.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtaildocs/js/document-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js` & `wagtail_bynder-0.3.0/src/wagtail_bynder/static/wagtailimages/js/image-chooser-modal.js`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html` & `wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/admin_base.html`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html` & `wagtail_bynder-0.3.0/src/wagtail_bynder/templates/wagtailadmin/chooser/chooser-bynder.html`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/utils.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,52 +13,42 @@
 
 
 _DEFAULT_COLLECTION = Local()
 
 
 class DownloadedFile(BytesIO):
     name: str
-    content_type: str
-    charset: str
     size: int
+    content_type: str | None
+    charset: str | None
 
 
 def download_file(url: str) -> DownloadedFile:
     raw_bytes = requests.get(url, timeout=20).content
     f = DownloadedFile(raw_bytes)
     f.name = os.path.basename(url)
     f.size = len(raw_bytes)
     f.content_type, f.charset = mimetypes.guess_type(f.name)
     return f
 
 
-def download_document(url: str) -> InMemoryUploadedFile:
+def download_asset(url: str) -> InMemoryUploadedFile:
     f = download_file(url)
-    uploadedfile = InMemoryUploadedFile(
+    return InMemoryUploadedFile(
         f,
         name=f.name,
         field_name="file",
         size=f.size,
         charset=f.charset,
         content_type=f.content_type,
     )
-    return uploadedfile
 
 
-def download_image(url: str) -> InMemoryUploadedFile:
-    f = download_file(url)
-    uploadedfile = InMemoryUploadedFile(
-        f,
-        name=f.name,
-        field_name="file",
-        size=f.size,
-        charset=f.charset,
-        content_type=f.content_type,
-    )
-    return uploadedfile
+def filename_from_url(url: str) -> str:
+    return os.path.basename(url)
 
 
 def get_bynder_client() -> BynderClient:
     return BynderClient(
         domain=getattr(settings, "BYNDER_DOMAIN", ""),
         permanent_token=getattr(settings, "BYNDER_API_TOKEN", ""),
     )
```

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/views/document.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/views/document.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/views/image.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/views/image.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/views/mixins.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/views/mixins.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/views/video.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/views/video.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/wagtail_hooks.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/src/wagtail_bynder/widgets.py` & `wagtail_bynder-0.3.0/src/wagtail_bynder/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail_bynder-0.2.0/PKG-INFO` & `wagtail_bynder-0.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: wagtail-bynder
-Version: 0.2.0
-Summary: Wagtail integration with Bynder, a Digital Asset Management System
-Keywords: Wagtail,Django,Bynder,DAMS,digital asset management
-Author-email: Andy Babic  <andy.babic@torchbox.com>
-Maintainer-email: Andy Babic <andy.babic@torchbox.com>, Dan Braghis <dan.braghis@torchbox.com>
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Django :: 5.0
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
-Requires-Dist: Django>=3.2
-Requires-Dist: Wagtail>=4.1
-Requires-Dist: bynder-sdk>=1.1.5,<2.0
-Requires-Dist: dj-database-url>=2.1.0,<3.0 ; extra == "testing"
-Requires-Dist: wagtail_factories>=4.1.0,<5.0 ; extra == "testing"
-Requires-Dist: responses>=0.24,<1 ; extra == "testing"
-Requires-Dist: coverage>=7.0,<8.0 ; extra == "testing"
-Requires-Dist: freezegun>=1.1,<2 ; extra == "testing"
-Project-URL: Changelog, https://github.com/torchbox/wagtail-bynder/blob/main/CHANGELOG.md
-Project-URL: Source, https://github.com/torchbox/wagtail-bynder
-Provides-Extra: testing
-
 # Bynder integration for Wagtail
 
 [![License: BSD-3-Clause](https://img.shields.io/badge/License-BSD--3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![PyPI version](https://img.shields.io/pypi/v/wagtail-bynder.svg?style=flat)](https://pypi.org/project/wagtail-bynder)
 [![Build status](https://img.shields.io/github/actions/workflow/status/torchbox/wagtail-bynder/test.yml?branch=main)](https://github.com/torchbox/wagtail-bynder/actions)
 
@@ -88,14 +52,70 @@
 
 To sync images updated within the last three days:
 
 ```sh
 $ python manage.py update_stale_images --days=3
 ```
 
+## What to ask of Bynder
+
+When communicating with Bynder about configuring a new instance for compatibility with Wagtail, there are a few things you'll want to be clear about:
+
+1. Document assets should be fully enabled
+2. A custom derivative must to be configured for image assets
+3. A couple of custom derivatives must be configured for video assets
+
+
+### Why are custom derivatives needed?
+
+It is common for assets to be uploaded to a DAMS in formats that preserve as much quality as possible. For example, high-resolution uncompressed TIFF images are common for digital photography. While great for print and other media, such formats are simply overkill for most websites. Not only are images likely to be shown at much smaller dimensions in a web browser, but they are also likely to be converted to more web-friendly formats like AVIF or WebP by Wagtail, where the image quality of an uncompressed TIFF is unlikely to shine through.
+
+Over time, unnecessarily large source images will have a compounding impact on website performance. Editors will need to wait longer for Wagtail to download the images from Bynder. And, every time a new rendition is needed, the original must be loaded into memory from wherever it is stored, consuming more precious system memory than necessary, and blocking system I/O operations for longer whilst the file is read from storage.
+
+#### 'WagtailSource' derivative for images
+
+What Wagtail really needs is a reliable, high quality derivative, which it can use as a 'source' to generate renditions from. This should strike the right balance between:
+
+- Being large enough to use in most website contexts (Think full-width hero images that need to look decent on a large high-resolution display). A maximum width or height of **3500 pixels** is usually enough for this.
+- Retaining as much visual quality as possible, whilst keeping file sizes reasonable. Individual images will naturally vary, but somewhere **between 4MB and 6MB** is a reasonable target.
+
+In most cases, `JPG` will probably the best option. But, for fine art images with lots of uniform colour and sharp edges, `PNG` might be a better fit.
+
+Once configured, URLs for the new derivative should appear under `"thumbnails"` in the API representation for image assets, like so:
+
+```json
+"thumbnails": {
+  "mini": "https://orgname.bynder.com/m/3ece125489f192fa/YourGroovyImage.png",
+  "thul": "https://orgname.bynder.com/m/3ece125489f192fa/thul-YourGroovyImage.png",
+  "webimage": "https://orgname.bynder.com/m/3ece125489f192fa/webimage-YourGroovyImage.png",
+  "WagtailSource": "https://orgname.bynder.com/m/3ece125489f192fa/WagtailSource-YourGroovyImage.jpg",
+}
+```
+
+### 'WebPrimary' and 'WebFallback' derivatives for videos
+
+The goal here is to ensure video can be seen by the widest possibly audience (Wagtail doesn't take a copy of video media like it does for image - as it isn't well equipped for re-encoding it).
+
+Support for media container formats, video and audio codecs has become more consistant over the years. The general consensus is that video on the web should be provided in two different formats in order to work for the widest audience. So, we recommend that Bynder generate **two** custom derivatives for videos:
+
+**WebPrimary**: A derivative using a WebM container, the VP9 codec for video and the Opus codec for audio. These are all open, royalty-free formats which are generally well-supported, although only in quite recent browsers, which is why a fallback is a good idea.
+
+**WebFallback**: A derivative using an MP4 container and the AVC (H.264) video codec, ideally with the AAC codec for audio. This combination has great support in every major browser, and the quality is typically good for most use cases.
+
+Once configured, URLs for the new derivatives should appear under `"videoPreviewURLs"` in the API representation for video assets, like so:
+
+```json
+"videoPreviewURLs": [
+  "https://orgname.bynder.com/asset/52477218-06f5-4e55-ad55-049bf33b105f/WebPrimary/WebPrimary-YourGroovyVideo.web",
+  "https://orgname.bynder.com/asset/52477218-06f5-4e55-ad55-049bf33b105f/WebFallback/WebFallback-YourGroovyVideo.mp4",
+]
+```
+
+NOTE: The proposed 'WebPrimary' and 'WebFallback' names do not include 'Wagtail' in the name, because there really isn't anything Wagtail-specific about them. They should be useful in any 'web' context.
+
 ## Installation
 
 In your project's Django settings, add the app your `INSTALLED_APPS` list (at the end is fine):
 
 ```python
 INSTALLED_APPS = [
   # ...
@@ -220,17 +240,15 @@
 
 An API token for Bynder's JavaScript 'compact view' to use. The value is injected into the `admin_base.html` template for Wagtail
 for the JavaScript to pick up, exposing it to Wagtail users. Because of this, it should be different to `BYNDER_API_TOKEN`
 and only needs to have basic read permissions.
 
 ### `BYNDER_IMAGE_SOURCE_THUMBNAIL_NAME`
 
-Example: `"WagtailSource"`
-
-Default: `"webimage"`
+Default: `"WagtailSource"`
 
 The name of the automatically generated derivative that should be downloaded and used as the `file` value for the
 representative Wagtail image (as it appears in `thumbnails` in the API representation).
 
 WARNING: It's important to get this right, because if the specified derivative is NOT present in the response for an
 image for any reason, the ORIGINAL will be downloaded - which will lead to slow chooser response times and higher memory
 usage when generating renditions.
@@ -239,19 +257,19 @@
 
 Example: `"video.Video"`
 
 Default: `None`
 
 ### `BYNDER_VIDEO_PRIMARY_DERIVATIVE_NAME`
 
-Default: `"Web-Primary"`
+Default: `"WebPrimary"`
 
 ### `BYNDER_VIDEO_FALLBACK_DERIVATIVE_NAME`
 
-Default: `"Web-Fallback"`
+Default: `"WebFallback"`
 
 ### `BYNDER_VIDEO_POSTER_IMAGE_DERIVATIVE_NAME`
 
 Default: `"webimage"`
 
 ### `BYNDER_SYNC_EXISTING_IMAGES_ON_CHOOSE`
 
@@ -296,8 +314,7 @@
 All contributions are welcome! See [CONTRIBUTING.md](https://github.com/torchbox/wagtail-bynder/blob/main/CONTRIBUTING.md)
 
 Supported versions:
 
 - Python 3.11, 3.12
 - Django 3.2, 4.2, 5.0
 - Wagtail 4.1 (LTS), 5.1, 5.2 (LTS)
-
```

