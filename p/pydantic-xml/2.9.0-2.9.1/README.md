# Comparing `tmp/pydantic_xml-2.9.0.tar.gz` & `tmp/pydantic_xml-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-2.9.0.tar", max compression
+gzip compressed data, was "pydantic_xml-2.9.1.tar", max compression
```

## Comparing `pydantic_xml-2.9.0.tar` & `pydantic_xml-2.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2024-02-03 17:00:11.477938 pydantic_xml-2.9.0/LICENSE
--rw-r--r--   0        0        0     3218 2024-02-03 17:00:11.477938 pydantic_xml-2.9.0/README.rst
--rw-r--r--   0        0        0      453 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/config.py
--rw-r--r--   0        0        0      134 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    17277 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      394 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1948 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1322 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      413 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/element/utils.py
--rw-r--r--   0        0        0      712 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/errors.py
--rw-r--r--   0        0        0    15171 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/model.py
--rw-r--r--   0        0        0     3702 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/mypy.py
--rw-r--r--   0        0        0        0 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/py.typed
--rw-r--r--   0        0        0       36 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0      151 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     4121 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4486 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0      460 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/is_instance.py
--rw-r--r--   0        0        0     5761 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0    15611 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     6731 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     2858 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/raw.py
--rw-r--r--   0        0        0     5287 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/tagged_union.py
--rw-r--r--   0        0        0     1047 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/tuple.py
--rw-r--r--   0        0        0     1428 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/typed_mapping.py
--rw-r--r--   0        0        0     5880 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2996 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0    10819 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0      375 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     3978 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pydantic_xml/utils.py
--rw-r--r--   0        0        0     2149 2024-02-03 17:00:11.481938 pydantic_xml-2.9.0/pyproject.toml
--rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 pydantic_xml-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-12 14:01:50.246366 pydantic_xml-2.9.1/LICENSE
+-rw-r--r--   0        0        0     3218 2024-04-12 14:01:50.246366 pydantic_xml-2.9.1/README.rst
+-rw-r--r--   0        0        0      453 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/config.py
+-rw-r--r--   0        0        0      134 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    17277 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      394 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1948 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1322 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      413 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/element/utils.py
+-rw-r--r--   0        0        0      712 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    15400 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/model.py
+-rw-r--r--   0        0        0     3702 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/mypy.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     4121 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4486 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0      460 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/is_instance.py
+-rw-r--r--   0        0        0     5761 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    15611 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     6731 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     2858 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/raw.py
+-rw-r--r--   0        0        0     5287 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tagged_union.py
+-rw-r--r--   0        0        0     1047 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tuple.py
+-rw-r--r--   0        0        0     1428 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     5880 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2996 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0    10871 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      375 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     3978 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     2149 2024-04-12 14:01:50.250366 pydantic_xml-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5010 1970-01-01 00:00:00.000000 pydantic_xml-2.9.1/PKG-INFO
```

### Comparing `pydantic_xml-2.9.0/LICENSE` & `pydantic_xml-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/README.rst` & `pydantic_xml-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/element/element.py` & `pydantic_xml-2.9.1/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.9.1/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/element/native/std.py` & `pydantic_xml-2.9.1/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/errors.py` & `pydantic_xml-2.9.1/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/model.py` & `pydantic_xml-2.9.1/pydantic_xml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses as dc
 import typing
 from typing import Any, Callable, ClassVar, Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 
 import pydantic as pd
 import pydantic_core as pdc
+import typing_extensions as te
 from pydantic import BaseModel, RootModel
 from pydantic._internal._model_construction import ModelMetaclass  # noqa
 from pydantic.root_model import _RootModelMetaclass as RootModelMetaclass  # noqa
 
 from . import config, errors, utils
 from .element import SearchMode
 from .element.native import ElementT, XmlElement, etree
@@ -245,14 +246,15 @@
     return XmlEntityInfo(
         EntityLocation.WRAPPED,
         path=path, ns=ns, nsmap=nsmap, wrapped=entity, default=default, default_factory=default_factory,
         **kwargs,
     )
 
 
+@te.dataclass_transform(kw_only_default=True, field_specifiers=(attr, element, wrapped, pd.Field))
 class XmlModelMeta(ModelMetaclass):
     """
     Xml model metaclass.
     """
 
     def __new__(
             mcls,
@@ -430,14 +432,15 @@
         :param kwargs: additional xml serialization arguments
         :return: object xml representation
         """
 
         return etree.tostring(self.to_xml_tree(skip_empty=skip_empty), **kwargs)
 
 
+@te.dataclass_transform(kw_only_default=True, field_specifiers=(attr, element, wrapped, pd.Field))
 class RootXmlModelMeta(XmlModelMeta, RootModelMetaclass):
     pass
 
 
 RootModelRootType = TypeVar('RootModelRootType')
```

### Comparing `pydantic_xml-2.9.0/pydantic_xml/mypy.py` & `pydantic_xml-2.9.1/pydantic_xml/mypy.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/raw.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/raw.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/tagged_union.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tagged_union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/tuple.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/tuple.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/typed_mapping.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/typed_mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pydantic_xml/serializers/serializer.py` & `pydantic_xml-2.9.1/pydantic_xml/serializers/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 TYPE_FAMILY = {
     'none':             SchemaTypeFamily.PRIMITIVE,
     'bool':             SchemaTypeFamily.PRIMITIVE,
     'int':              SchemaTypeFamily.PRIMITIVE,
     'float':            SchemaTypeFamily.PRIMITIVE,
     'str':              SchemaTypeFamily.PRIMITIVE,
     'bytes':            SchemaTypeFamily.PRIMITIVE,
+    'enum':             SchemaTypeFamily.PRIMITIVE,
     'date':             SchemaTypeFamily.PRIMITIVE,
     'time':             SchemaTypeFamily.PRIMITIVE,
     'datetime':         SchemaTypeFamily.PRIMITIVE,
     'timedelta':        SchemaTypeFamily.PRIMITIVE,
     'uuid':             SchemaTypeFamily.PRIMITIVE,
     'decimal':          SchemaTypeFamily.PRIMITIVE,
     'url':              SchemaTypeFamily.PRIMITIVE,
```

### Comparing `pydantic_xml-2.9.0/pydantic_xml/utils.py` & `pydantic_xml-2.9.1/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.9.0/pyproject.toml` & `pydantic_xml-2.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "2.9.0"
+version = "2.9.1"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://pydantic-xml.readthedocs.io"
```

### Comparing `pydantic_xml-2.9.0/PKG-INFO` & `pydantic_xml-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 2.9.0
+Version: 2.9.1
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8
```

