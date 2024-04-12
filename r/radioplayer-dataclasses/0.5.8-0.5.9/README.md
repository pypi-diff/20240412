# Comparing `tmp/radioplayer_dataclasses-0.5.8.tar.gz` & `tmp/radioplayer_dataclasses-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.5.8.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.5.9.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.5.8.tar` & `radioplayer_dataclasses-0.5.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34520 2024-02-20 06:57:46.888537 radioplayer_dataclasses-0.5.8/LICENSE
--rw-r--r--   0        0        0     3627 2024-02-20 06:57:46.888537 radioplayer_dataclasses-0.5.8/README.md
--rw-r--r--   0        0        0     2220 2024-02-20 06:58:07.288531 radioplayer_dataclasses-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     2351 2024-02-20 06:57:46.888537 radioplayer_dataclasses-0.5.8/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    57445 2024-02-20 06:57:46.888537 radioplayer_dataclasses-0.5.8/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2024-02-20 06:57:46.888537 radioplayer_dataclasses-0.5.8/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-03-10 12:07:15.519234 radioplayer_dataclasses-0.5.9/LICENSE
+-rw-r--r--   0        0        0     3627 2024-03-10 12:07:15.519234 radioplayer_dataclasses-0.5.9/README.md
+-rw-r--r--   0        0        0     2160 2024-03-10 12:07:32.638979 radioplayer_dataclasses-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     2443 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    58103 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2024-03-10 12:07:15.523234 radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.9/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.5.8/LICENSE` & `radioplayer_dataclasses-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.8/README.md` & `radioplayer_dataclasses-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.5.8/pyproject.toml` & `radioplayer_dataclasses-0.5.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.5.8" # 0.0.0 placeholder is replaced on release
+version = "v0.5.9" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -60,15 +60,14 @@
 # C0116 = missing-function-docstring
 disable = ["C0114","C0116"]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=radioplayer.dataclasses --cov-fail-under=100 --pylint --mypy --ignore=docs/"
 filterwarnings = [
-    "ignore::pytest.PytestRemovedIn8Warning:pytest_pylint",
     "ignore::DeprecationWarning:pytest_pylint",
     "ignore::DeprecationWarning:pylint",
     "ignore::DeprecationWarning:pkg_resources",
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `radioplayer_dataclasses-0.5.8/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 from radioplayer.dataclasses.dataclasses import (
-    Catype,
-    CatypeType,
     AlternateSourceType,
     AlternateSourceTypeProtocol,
     AlternateSourceTypeType,
     AudioStreamGroupType,
     AudioStreamType,
     BitRateType,
     BroadcastType,
+    Catype,
+    CatypeType,
     EnsembleType,
     Epg,
     EpgLanguageType,
     FormatType,
     FrequencyType,
     FrequencyTypeType,
     GenreType,
     GenreTypeType,
+    GeoFootprintType,
+    GeoLocationsType,
     KeywordsType,
     LangValue,
     LinkType,
     ListenliveGroupType,
     LocationType,
     LongDescriptionType,
     LongNameType,
     MediaCreditType,
     MediaDescriptionType,
     MediumNameType,
     MemberOfType,
     MessageType,
     MultimediaType,
     OndemandType,
+    ProgrammeGroupsType,
     ProgrammeGroupType,
     ProgrammeGroupTypeType,
-    ProgrammeGroupsType,
     ProgrammeType,
+    RadioplayerIdType,
     RecommendationType,
+    RestrictionRelationship,
     RestrictionType,
     RestrictionTypeRelationship,
-    RestrictionRelationship,
     ScheduleType,
     ServiceGroupIdHead,
     ServiceGroupType,
     ServiceIdType,
     ServiceIdTypeAttr,
-    RadioplayerIdType,
     ServiceInformation,
     ServiceType,
     ShortDescriptionType,
     ShortNameType,
     SimulcastType,
     SocialIdentifierType,
     SystemType,
@@ -67,14 +69,16 @@
     "Epg",
     "EpgLanguageType",
     "FormatType",
     "FrequencyType",
     "FrequencyTypeType",
     "GenreType",
     "GenreTypeType",
+    "GeoFootprintType",
+    "GeoLocationsType",
     "KeywordsType",
     "LangValue",
     "LinkType",
     "ListenliveGroupType",
     "LocationType",
     "LongDescriptionType",
     "LongNameType",
```

### Comparing `radioplayer_dataclasses-0.5.8/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.5.9/radioplayer/dataclasses/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,14 +259,46 @@
         metadata={
             "type": "Attribute",
         },
     )
 
 
 @dataclass
+class GeoFootprintType:
+    class Meta:
+        name = "geoFootprintType"
+        target_namespace = (
+            "http://www.radioplayer.co.uk/schemas/11/rpDataTypes"
+        )
+
+    value: str = field(
+        default="",
+        metadata={
+            "required": True,
+        },
+    )
+
+
+@dataclass
+class GeoLocationsType:
+    class Meta:
+        name = "geoLocationsType"
+        target_namespace = (
+            "http://www.radioplayer.co.uk/schemas/11/rpDataTypes"
+        )
+
+    value: str = field(
+        default="",
+        metadata={
+            "required": True,
+        },
+    )
+
+
+@dataclass
 class MediaCreditType:
     class Meta:
         name = "mediaCreditType"
         target_namespace = (
             "http://www.radioplayer.co.uk/schemas/11/rpDataTypes"
         )
 
@@ -1055,22 +1087,22 @@
             default=None,
             metadata={
                 "type": "Element",
                 "namespace": "http://www.radioplayer.co.uk/schemas/11/rpDataTypes",
                 "required": True,
             },
         )
-        restriction: Optional[
-            "ListenliveGroupType.Listenlive.Restriction"
-        ] = field(
-            default=None,
-            metadata={
-                "type": "Element",
-                "namespace": "http://www.radioplayer.co.uk/schemas/11/rpDataTypes",
-            },
+        restriction: Optional["ListenliveGroupType.Listenlive.Restriction"] = (
+            field(
+                default=None,
+                metadata={
+                    "type": "Element",
+                    "namespace": "http://www.radioplayer.co.uk/schemas/11/rpDataTypes",
+                },
+            )
         )
         audio_stream_group: Optional[AudioStreamGroupType] = field(
             default=None,
             metadata={
                 "name": "audioStreamGroup",
                 "type": "Element",
                 "namespace": "http://www.radioplayer.co.uk/schemas/11/rpDataTypes",
@@ -1715,24 +1747,24 @@
         metadata={
             "name": "listenliveGroup",
             "type": "Element",
             "namespace": "http://www.radioplayer.co.uk/schemas/11/epgSI",
             "required": True,
         },
     )
-    geo_locations: Optional[str] = field(
+    geo_locations: Optional[GeoLocationsType] = field(
         default=None,
         metadata={
             "name": "geoLocations",
             "type": "Element",
             "namespace": "http://www.radioplayer.co.uk/schemas/11/epgSI",
             "required": True,
         },
     )
-    geo_footprint: Optional[str] = field(
+    geo_footprint: Optional[GeoFootprintType] = field(
         default=None,
         metadata={
             "name": "geoFootprint",
             "type": "Element",
             "namespace": "http://www.radioplayer.co.uk/schemas/11/epgSI",
             "required": True,
         },
```

### Comparing `radioplayer_dataclasses-0.5.8/PKG-INFO` & `radioplayer_dataclasses-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioplayer-dataclasses
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python dataclasses for radioplayer generated from XSD
 Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

