# Comparing `tmp/pydantic_numpy-4.2.0.tar.gz` & `tmp/pydantic_numpy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-4.2.0.tar", max compression
+gzip compressed data, was "pydantic_numpy-5.0.0.tar", max compression
```

## Comparing `pydantic_numpy-4.2.0.tar` & `pydantic_numpy-5.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1658 2024-02-24 15:32:23.900048 pydantic_numpy-4.2.0/LICENSE
--rw-r--r--   0        0        0     3224 2024-02-24 15:32:23.900048 pydantic_numpy-4.2.0/README.md
--rw-r--r--   0        0        0      199 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0     8928 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0      163 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/helper/typing.py
--rw-r--r--   0        0        0     3635 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0     9736 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/model.py
--rw-r--r--   0        0        0      474 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     4886 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     4981 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     5076 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     4810 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     4086 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     4176 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     4266 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     4019 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0     1621 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1603 2024-02-24 15:32:23.904048 pydantic_numpy-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 pydantic_numpy-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1658 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/README.md
+-rw-r--r--   0        0        0      199 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0    13321 2024-04-12 07:38:22.484129 pydantic_numpy-5.0.0/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0      168 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/helper/typing.py
+-rw-r--r--   0        0        0     3645 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0     9736 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/model.py
+-rw-r--r--   0        0        0      474 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     4886 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     4981 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     5076 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     4810 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     4086 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     4176 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     4266 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     4019 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1542 2024-04-12 07:38:22.488130 pydantic_numpy-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 pydantic_numpy-5.0.0/PKG-INFO
```

### Comparing `pydantic_numpy-4.2.0/LICENSE` & `pydantic_numpy-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/README.md` & `pydantic_numpy-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 ![Python 3.9-3.12](https://img.shields.io/badge/python-3.9--3.12-blue.svg)
 [![Packaged with Poetry](https://img.shields.io/badge/packaging-poetry-cyan.svg)](https://python-poetry.org/)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)
 ![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)
 
 
+## Usage
+
 Package that integrates NumPy Arrays into Pydantic!
 
 - `pydantic_numpy.typing` provides many typings such as `NpNDArrayFp64`, `Np3DArrayFp64` (float64 that must be 3D)! Works with both `pydantic.BaseModel` and `pydantic.dataclass`
 - `NumpyModel` (derived from `pydantic.BaseModel`) make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
 
 See the [`test.helper.groups`](https://github.com/caniko/pydantic-numpy/blob/trunk/tests/helper/groups.py) to see types that are defined explicitly. Define your own NumPy types with `pydantic_numpy.np_array_pydantic_annotated_typing`.
 
-## Usage
+### Examples
 
 For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
 import numpy as np
 from pydantic import BaseModel
 
@@ -69,14 +71,14 @@
 
 ### Install
 ```shell
 pip install pydantic-numpy
 ```
 
 ## Considerations
-You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only supports Pydantic V1 and will not work with V2.
+The package is designed to work with Pydantic V2 and not V1. You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `<=3.8` and Pydantic V1 support.
 
 ### Licensing notice
 As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
 ### History
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-5.0.0/pydantic_numpy/helper/annotation.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from typing import Any, Callable, ClassVar, Iterable, Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 from pydantic import FilePath, GetJsonSchemaHandler, PositiveInt, validate_call
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
-from typing_extensions import Annotated
+from typing_extensions import Annotated, Final
 
-from pydantic_numpy.helper.typing import NumpyDataDict, SupportedDTypes
+from pydantic_numpy.helper.typing import NumpyArrayTypeData, SupportedDTypes
 from pydantic_numpy.helper.validation import (
     create_array_validator,
     validate_multi_array_numpy_file,
     validate_numpy_array_file,
 )
 from pydantic_numpy.model import MultiArrayNumpyFile
 
 
-def serialize_numpy_array_to_data_dict(array_like: npt.ArrayLike) -> NumpyDataDict:
+def pd_np_native_numpy_array_to_data_dict_serializer(array_like: npt.ArrayLike) -> NumpyArrayTypeData:
     """
     Serialize a NumPy array into a data dictionary format suitable for frontend display or processing.
 
     This function converts a given NumPy array into a dictionary format, which includes the data type
     and the data itself. If the array contains datetime or timedelta objects, it converts them into integer
     representations. Otherwise, the array is converted to a floating-point representation. This is particularly
     useful for preparing NumPy array data for JSON serialization or similar use cases where NumPy's native
@@ -38,64 +38,144 @@
     ----------
     array_like: np.ndarray
                   The NumPy array to be serialized. This can be a standard numerical array or an array
                   of datetime/timedelta objects.
 
     Returns
     -------
-    NumpyDataDict
+    NumpyArrayTypeData
                    A dictionary with two keys: 'data_type', a string representing the data type of the array,
                    and 'data', a list of values converted from the array. The conversion is to integer if the
                    original data type is datetime or timedelta, and to float for other data types.
 
     Example
     -------
     >>> my_array = np.array([1, 2, 3])
-    >>> serialize_numpy_array_to_data_dict(my_array)
+    >>> pd_np_native_numpy_array_to_data_dict_serializer(my_array)
     {'data_type': 'int64', 'data': [1.0, 2.0, 3.0]}
     """
     array = np.array(array_like)
 
     if issubclass(array.dtype.type, np.timedelta64) or issubclass(array.dtype.type, np.datetime64):
-        return NumpyDataDict(data_type=str(array.dtype), data=array.astype(int).tolist())
+        data = array.astype(int).tolist()
+    else:
+        data = array.astype(float).tolist()
 
-    return NumpyDataDict(data_type=str(array.dtype), data=array.astype(float).tolist())
+    return NumpyArrayTypeData(data_type=str(array.dtype), data=data)
+
+
+def pd_np_native_numpy_array_json_schema_from_type_data(
+    _field_core_schema: core_schema.CoreSchema,
+    _handler: GetJsonSchemaHandler,
+    dimensions: Optional[PositiveInt] = None,
+    data_type: Optional[SupportedDTypes] = None,
+) -> JsonSchemaValue:
+    """
+    Generates a JSON schema for a NumPy array field within a Pydantic model.
+
+    This function constructs a JSON schema definition compatible with Pydantic models
+    that are intended to validate NumPy array inputs. It supports specifying the data type
+    and dimensions of the NumPy array, which are used to construct a schema that ensures
+    input data matches the expected structure and type.
+
+    Parameters
+    ----------
+    _field_core_schema : core_schema.CoreSchema
+        The core schema component of the Pydantic model, used for building basic schema structures.
+    _handler : GetJsonSchemaHandler
+        A handler function or object responsible for converting Python types to JSON schema components.
+    dimensions : Optional[PositiveInt], optional
+        The dimensions (shape) of the NumPy array. If specified, the schema will enforce that the
+        input array matches this dimensionality. If `None`, no dimensionality constraint is applied,
+        by default None.
+    data_type : Optional[SupportedDTypes], optional
+        The expected data type of the NumPy array elements. If specified, the schema will enforce
+        that the input array's data type is compatible with this. If `None`, any data type is allowed,
+        by default None.
+
+    Returns
+    -------
+    JsonSchemaValue
+        A dictionary representing the JSON schema for a NumPy array field within a Pydantic model.
+        This schema includes details about the expected array dimensions and data type.
+    """
+    array_shape = _dimensions_to_shape_type[dimensions] if dimensions else "Any"
+
+    if data_type and _data_type_resolver(data_type):
+        array_data_type = data_type.__name__
+        item_schema = core_schema.list_schema(
+            items_schema=core_schema.any_schema(metadata=f"Must be compatible with numpy.dtype: {array_data_type}"),
+        )
+    else:
+        array_data_type = "Any"
+        item_schema = core_schema.list_schema(items_schema=core_schema.any_schema())
+
+    if dimensions:
+        data_schema = core_schema.list_schema(items_schema=item_schema, min_length=dimensions, max_length=dimensions)
+    else:
+        data_schema = item_schema
+
+    return dict(
+        title="Numpy Array",
+        type=f"np.ndarray[{array_shape}, np.dtype[{array_data_type}]]",
+        required=["data_type", "data"],
+        properties=dict(
+            data_type={"title": "dtype", "default": array_data_type, "type": "string"},
+            data=data_schema,
+        ),
+    )
 
 
 class NpArrayPydanticAnnotation:
     dimensions: ClassVar[Optional[PositiveInt]]
-
     data_type: ClassVar[SupportedDTypes]
+
     strict_data_typing: ClassVar[bool]
+
     serialize_numpy_array_to_json: ClassVar[Callable[[npt.ArrayLike], Iterable]]
+    json_schema_from_type_data: ClassVar[
+        Callable[
+            [core_schema.CoreSchema, GetJsonSchemaHandler, Optional[PositiveInt], Optional[SupportedDTypes]],
+            JsonSchemaValue,
+        ]
+    ]
 
     @classmethod
     def factory(
         cls,
         *,
         data_type: Optional[SupportedDTypes] = None,
-        dimensions: Optional[int] = None,
+        dimensions: Optional[PositiveInt] = None,
         strict_data_typing: bool = False,
-        serialize_numpy_array_to_json: Callable[[npt.ArrayLike], Iterable] = serialize_numpy_array_to_data_dict,
+        serialize_numpy_array_to_json: Callable[
+            [npt.ArrayLike], Iterable
+        ] = pd_np_native_numpy_array_to_data_dict_serializer,
+        json_schema_from_type_data: Callable[
+            [core_schema.CoreSchema, GetJsonSchemaHandler, Optional[PositiveInt], Optional[SupportedDTypes]],
+            JsonSchemaValue,
+        ] = pd_np_native_numpy_array_json_schema_from_type_data,
     ) -> type:
         """
         Create an instance NpArrayPydanticAnnotation that is configured for a specific dimension and dtype.
 
         The signature of the function is data_type, dimension and not dimension, data_type to reduce amount of
         code for all the types.
 
         Parameters
         ----------
         data_type: SupportedDTypes
-        dimensions: Optional[int]
-            Number of dimensions determine the depth of the numpy array.
+        dimensions: Optional[PositiveInt]
+            If defined, the number of dimensions determine the depth of the numpy array. Defaults to None,
+            e.g. any number of dimensions
         strict_data_typing: bool
             If True, the dtype of the numpy array must be identical to the data_type. No conversion attempts.
         serialize_numpy_array_to_json: Callable[[npt.ArrayLike], Iterable]
-            Json serialization function to use. Defaults to NumpyDataDict serializer.
+            Json serialization function to use. Defaults to NumpyArrayTypeData serializer.
+        json_schema_from_type_data: Callable
+            Json schema generation function to use. Defaults to NumpyArrayTypeData schema generator.
 
         Returns
         -------
         NpArrayPydanticAnnotation
         """
         if strict_data_typing and not data_type:
             msg = "Strict data typing requires data_type (SupportedDTypes) definition"
@@ -108,14 +188,15 @@
             ),
             (cls,),
             {
                 "dimensions": dimensions,
                 "data_type": data_type,
                 "strict_data_typing": strict_data_typing,
                 "serialize_numpy_array_to_json": serialize_numpy_array_to_json,
+                "json_schema_from_type_data": json_schema_from_type_data,
             },
         )
 
     @classmethod
     def __get_pydantic_core_schema__(
         cls,
         _source_type: Any,
@@ -124,60 +205,65 @@
         np_array_validator = create_array_validator(cls.dimensions, cls.data_type, cls.strict_data_typing)
         np_array_schema = core_schema.no_info_plain_validator_function(np_array_validator)
 
         return core_schema.json_or_python_schema(
             python_schema=core_schema.chain_schema([_common_numpy_array_validator, np_array_schema]),
             json_schema=np_array_schema,
             serialization=core_schema.plain_serializer_function_ser_schema(
-                cls.serialize_numpy_array_to_json, when_used="json-unless-none"
+                cls.serialize_numpy_array_to_json,
+                is_field_serializer=False,
+                when_used="json-unless-none",
             ),
         )
 
     @classmethod
     def __get_pydantic_json_schema__(
-        cls, _core_schema: core_schema.CoreSchema, _handler: GetJsonSchemaHandler
+        cls, field_core_schema: core_schema.CoreSchema, handler: GetJsonSchemaHandler
     ) -> JsonSchemaValue:
-        return dict(
-            type=(
-                f"np.ndarray[{_int_to_dim_type[cls.dimensions] if cls.dimensions else 'Any'}, "
-                f"np.dtype[{cls.data_type.__name__ if _data_type_resolver(cls.data_type) else 'Any'}]"
-            ),
-            strict_data_typing=cls.strict_data_typing,
-        )
+        return cls.json_schema_from_type_data(field_core_schema, handler, cls.dimensions, cls.data_type)
 
 
 def np_array_pydantic_annotated_typing(
     data_type: Optional[SupportedDTypes] = None,
     dimensions: Optional[int] = None,
     strict_data_typing: bool = False,
-    serialize_numpy_array_to_json: Callable[[npt.ArrayLike], Iterable] = serialize_numpy_array_to_data_dict,
+    serialize_numpy_array_to_json: Callable[
+        [npt.ArrayLike], Iterable
+    ] = pd_np_native_numpy_array_to_data_dict_serializer,
 ):
     """
     Generates typing and pydantic annotation of a np.ndarray parametrized with given constraints
 
     Parameters
     ----------
     data_type: SupportedDTypes
     dimensions: Optional[int]
         Number of dimensions determine the depth of the numpy array.
     strict_data_typing: bool
         If True, the dtype of the numpy array must be identical to the data_type. No conversion attempts.
     serialize_numpy_array_to_json: Callable[[npt.ArrayLike], Iterable]
-        Json serialization function to use. Defaults to NumpyDataDict serializer.
+        Json serialization function to use. Defaults to NumpyArrayTypeData serializer.
 
     Returns
     -------
     type-hint for np.ndarray with Pydantic support
+
+    Note
+    ----
+    The function generates the type hints dynamically, and will not work with static type checkers such as mypy
+    or pyright. For that you need to create your types manually.
     """
     return Annotated[
         Union[
             FilePath,
             MultiArrayNumpyFile,
             np.ndarray[  # type: ignore[misc]
-                _int_to_dim_type[dimensions] if dimensions else Any,  # pyright: ignore
+                _dimensions_to_shape_type[dimensions]  # pyright: ignore[reportGeneralTypeIssues]
+                if dimensions
+                else Any,
                 np.dtype[data_type] if _data_type_resolver(data_type) else data_type,  # type: ignore[valid-type]
             ],
         ],
         NpArrayPydanticAnnotation.factory(
             data_type=data_type,
             dimensions=dimensions,
             strict_data_typing=strict_data_typing,
@@ -187,19 +273,35 @@
 
 
 def _data_type_resolver(data_type: Optional[SupportedDTypes]) -> bool:
     return data_type is not None and issubclass(data_type, np.generic)
 
 
 @validate_call
-def _deserialize_numpy_array_from_data_dict(data_dict: NumpyDataDict) -> np.ndarray:
+def _deserialize_numpy_array_from_data_dict(data_dict: NumpyArrayTypeData) -> np.ndarray:
     return np.array(data_dict["data"]).astype(data_dict["data_type"])
 
 
-_int_to_dim_type = {1: tuple[int], 2: tuple[int, int], 3: tuple[int, int, int]}
+# IN_THE_FUTURE: Only works with 3.11 and above
+# @validate_call
+# def _dimension_type_from_depth(depth: PositiveInt) -> type[tuple[int, ...]]:
+#     return tuple[*[int] * depth]  # type: ignore
+
+
+_dimensions_to_shape_type: Final[dict[PositiveInt, type[tuple[int, ...]]]] = {
+    1: tuple[int],  # type: ignore[dict-item]
+    2: tuple[int, int],  # type: ignore[dict-item]
+    3: tuple[int, int, int],  # type: ignore[dict-item]
+    4: tuple[int, int, int, int],  # type: ignore[dict-item]
+    5: tuple[int, int, int, int, int],  # type: ignore[dict-item]
+    6: tuple[int, int, int, int, int, int],  # type: ignore[dict-item]
+    7: tuple[int, int, int, int, int, int, int],  # type: ignore[dict-item]
+}
+
+
 _common_numpy_array_validator = core_schema.union_schema(
     [
         core_schema.chain_schema(
             [
                 core_schema.is_instance_schema(Path),
                 core_schema.no_info_plain_validator_function(validate_numpy_array_file),
             ]
```

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/helper/validation.py` & `pydantic_numpy-5.0.0/pydantic_numpy/helper/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import numpy.typing as npt
 from numpy import floating, integer
 from numpy.lib.npyio import NpzFile
 from pydantic import FilePath
 
-from pydantic_numpy.helper.typing import NumpyDataDict, SupportedDTypes
+from pydantic_numpy.helper.typing import NumpyArrayTypeData, SupportedDTypes
 from pydantic_numpy.model import MultiArrayNumpyFile
 
 
 class PydanticNumpyMultiArrayNumpyFileOnFilePath(Exception):
     pass
 
 
@@ -32,15 +32,15 @@
 
     Returns
     -------
     Callable[[npt.NDArray], npt.NDArray]
     Validator for numpy array
     """
 
-    def array_validator(array_data: Union[npt.NDArray, NumpyDataDict]) -> npt.NDArray:
+    def array_validator(array_data: Union[npt.NDArray, NumpyArrayTypeData]) -> npt.NDArray:
         array: npt.NDArray = (
             np.array(array_data["data"], dtype=array_data.get("dtype", None))
             if isinstance(array_data, dict)
             else array_data
         )
 
         if dimensions and (array_dimensions := len(array.shape)) != dimensions:
```

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/model.py` & `pydantic_numpy-5.0.0/pydantic_numpy/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-5.0.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pydantic_numpy/util.py` & `pydantic_numpy-5.0.0/pydantic_numpy/util.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-4.2.0/pyproject.toml` & `pydantic_numpy-5.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "4.2.0"
+version = "5.0.0"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
 
@@ -25,44 +25,42 @@
 numpy = ">=1.23.0"
 pydantic = "^2.0"
 semver = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 parameterized = "^0.9.0"
-hypothesis = "^6.82.0"
 orjson = "*"
-setuptools = "^68.0.0"
 
 [tool.poetry.group.format.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
-ruff = "^0.0.285"
+ruff = "*"
 
 [tool.poetry.group.typecheck.dependencies]
 mypy = "*"
 pyright = "^1.1.338"
 
 [tool.pytest.ini_options]
 filterwarnings = [
-    "ignore::hypothesis.errors.NonInteractiveExampleWarning",
     "ignore:invalid value encountered in multiply:RuntimeWarning",
 ]
 
 [tool.black]
 line-length = 120
-target-version = ["py311"]
+target-version = ["py312"]
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 line-length = 120
-ignore-init-module-imports = true
-ignore = ["F403", "F405"]
+lint.ignore-init-module-imports = true
+lint.ignore = ["F403", "F405"]
 
 [tool.pyright]
+include = ["pydantic_numpy/**", "tests/**"]
 reportUnsupportedDunderAll = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_numpy-4.2.0/PKG-INFO` & `pydantic_numpy-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_numpy
-Version: 4.2.0
+Version: 5.0.0
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing,validation
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
@@ -30,22 +30,24 @@
 ![Python 3.9-3.12](https://img.shields.io/badge/python-3.9--3.12-blue.svg)
 [![Packaged with Poetry](https://img.shields.io/badge/packaging-poetry-cyan.svg)](https://python-poetry.org/)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)
 ![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)
 
 
+## Usage
+
 Package that integrates NumPy Arrays into Pydantic!
 
 - `pydantic_numpy.typing` provides many typings such as `NpNDArrayFp64`, `Np3DArrayFp64` (float64 that must be 3D)! Works with both `pydantic.BaseModel` and `pydantic.dataclass`
 - `NumpyModel` (derived from `pydantic.BaseModel`) make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
 
 See the [`test.helper.groups`](https://github.com/caniko/pydantic-numpy/blob/trunk/tests/helper/groups.py) to see types that are defined explicitly. Define your own NumPy types with `pydantic_numpy.np_array_pydantic_annotated_typing`.
 
-## Usage
+### Examples
 
 For more examples see [test_ndarray.py](./tests/test_typing.py)
 
 ```python
 import numpy as np
 from pydantic import BaseModel
 
@@ -96,15 +98,15 @@
 
 ### Install
 ```shell
 pip install pydantic-numpy
 ```
 
 ## Considerations
-You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `3.8` support, but this version only supports Pydantic V1 and will not work with V2.
+The package is designed to work with Pydantic V2 and not V1. You can install from [cheind's](https://github.com/cheind/pydantic-numpy) repository if you want Python `<=3.8` and Pydantic V1 support.
 
 ### Licensing notice
 As of version `3.0.0` the license has moved over to BSD-4. The versions prior are under the MIT license.
 
 ### History
 The original idea originates from [this discussion](https://gist.github.com/danielhfrank/00e6b8556eed73fb4053450e602d2434), and forked from [cheind's](https://github.com/cheind/pydantic-numpy) repository.
```

