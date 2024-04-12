# Comparing `tmp/geoh5py-0.9.0a2.tar.gz` & `tmp/geoh5py-0.9.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoh5py-0.9.0a2.tar", max compression
+gzip compressed data, was "geoh5py-0.9.0a3.tar", max compression
```

## Comparing `geoh5py-0.9.0a2.tar` & `geoh5py-0.9.0a3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0      841 2024-02-27 21:35:13.324040 geoh5py-0.9.0a2/geoh5py/__init__.py
--rw-r--r--   0        0        0     1574 2024-01-31 17:10:26.210995 geoh5py-0.9.0a2/geoh5py/data/__init__.py
--rw-r--r--   0        0        0     1311 2024-01-31 17:10:26.210995 geoh5py-0.9.0a2/geoh5py/data/blob_data.py
--rw-r--r--   0        0        0     2005 2024-02-27 21:35:13.325039 geoh5py-0.9.0a2/geoh5py/data/boolean_data.py
--rw-r--r--   0        0        0     3948 2024-01-31 17:10:26.211988 geoh5py-0.9.0a2/geoh5py/data/color_map.py
--rw-r--r--   0        0        0     8843 2024-02-27 21:35:13.325039 geoh5py-0.9.0a2/geoh5py/data/data.py
--rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.212998 geoh5py-0.9.0a2/geoh5py/data/data_association_enum.py
--rw-r--r--   0        0        0    12241 2024-02-27 21:35:13.326039 geoh5py-0.9.0a2/geoh5py/data/data_type.py
--rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.213988 geoh5py-0.9.0a2/geoh5py/data/data_unit.py
--rw-r--r--   0        0        0     1340 2024-01-31 17:10:26.213988 geoh5py-0.9.0a2/geoh5py/data/datetime_data.py
--rw-r--r--   0        0        0     3690 2024-01-31 17:10:26.213988 geoh5py-0.9.0a2/geoh5py/data/filename_data.py
--rw-r--r--   0        0        0     1787 2024-01-31 17:10:26.214988 geoh5py-0.9.0a2/geoh5py/data/float_data.py
--rw-r--r--   0        0        0     1625 2024-01-31 17:10:26.214988 geoh5py-0.9.0a2/geoh5py/data/geometric_data_constants.py
--rw-r--r--   0        0        0     1709 2024-01-31 17:10:26.214988 geoh5py-0.9.0a2/geoh5py/data/integer_data.py
--rw-r--r--   0        0        0     4001 2024-01-31 17:10:26.215988 geoh5py-0.9.0a2/geoh5py/data/numeric_data.py
--rw-r--r--   0        0        0     1121 2024-01-31 17:10:26.215988 geoh5py-0.9.0a2/geoh5py/data/primitive_type_enum.py
--rw-r--r--   0        0        0     2914 2024-02-27 21:35:13.326039 geoh5py-0.9.0a2/geoh5py/data/reference_value_map.py
--rw-r--r--   0        0        0     1531 2024-01-31 17:10:26.216996 geoh5py-0.9.0a2/geoh5py/data/referenced_data.py
--rw-r--r--   0        0        0     5093 2024-01-31 17:10:26.216996 geoh5py-0.9.0a2/geoh5py/data/text_data.py
--rw-r--r--   0        0        0     1573 2024-01-31 17:10:26.216996 geoh5py-0.9.0a2/geoh5py/data/unknown_data.py
--rw-r--r--   0        0        0     4559 2024-01-31 17:10:26.217996 geoh5py-0.9.0a2/geoh5py/data/visual_parameters.py
--rw-r--r--   0        0        0     1587 2024-01-31 17:10:26.217996 geoh5py-0.9.0a2/geoh5py/groups/__init__.py
--rw-r--r--   0        0        0     1441 2024-02-27 21:35:13.327038 geoh5py-0.9.0a2/geoh5py/groups/container_group.py
--rw-r--r--   0        0        0     1395 2024-02-27 21:35:13.328038 geoh5py-0.9.0a2/geoh5py/groups/custom_group.py
--rw-r--r--   0        0        0     1797 2024-02-27 21:35:13.328038 geoh5py-0.9.0a2/geoh5py/groups/drillhole_group.py
--rw-r--r--   0        0        0     1444 2024-02-27 21:35:13.329038 geoh5py-0.9.0a2/geoh5py/groups/giftools_group.py
--rw-r--r--   0        0        0     6409 2024-02-27 21:35:13.329038 geoh5py-0.9.0a2/geoh5py/groups/group.py
--rw-r--r--   0        0        0     3656 2024-02-27 21:35:13.330039 geoh5py-0.9.0a2/geoh5py/groups/group_type.py
--rw-r--r--   0        0        0     6714 2024-02-27 21:35:13.330039 geoh5py-0.9.0a2/geoh5py/groups/integrator_group.py
--rw-r--r--   0        0        0     1295 2024-02-27 21:35:13.330039 geoh5py-0.9.0a2/geoh5py/groups/maps_group.py
--rw-r--r--   0        0        0     1414 2024-02-27 21:35:13.331038 geoh5py-0.9.0a2/geoh5py/groups/notype_group.py
--rw-r--r--   0        0        0     8138 2024-02-27 21:35:13.331038 geoh5py-0.9.0a2/geoh5py/groups/property_group.py
--rw-r--r--   0        0        0     1593 2024-01-31 17:10:26.221995 geoh5py-0.9.0a2/geoh5py/groups/root_group.py
--rw-r--r--   0        0        0     2053 2024-02-27 21:35:13.332040 geoh5py-0.9.0a2/geoh5py/groups/simpeg_group.py
--rw-r--r--   0        0        0     1322 2024-02-27 21:35:13.332040 geoh5py-0.9.0a2/geoh5py/groups/survey_group.py
--rw-r--r--   0        0        0      866 2024-01-31 17:10:26.228996 geoh5py-0.9.0a2/geoh5py/io/__init__.py
--rw-r--r--   0        0        0    17088 2024-01-31 17:10:26.228996 geoh5py-0.9.0a2/geoh5py/io/h5_reader.py
--rw-r--r--   0        0        0    34668 2024-02-27 21:35:13.334054 geoh5py-0.9.0a2/geoh5py/io/h5_writer.py
--rw-r--r--   0        0        0     2403 2024-01-31 17:10:26.229997 geoh5py-0.9.0a2/geoh5py/objects/__init__.py
--rw-r--r--   0        0        0     9440 2024-02-27 21:35:13.334054 geoh5py-0.9.0a2/geoh5py/objects/block_model.py
--rw-r--r--   0        0        0     7874 2024-01-31 17:10:26.230995 geoh5py-0.9.0a2/geoh5py/objects/cell_object.py
--rw-r--r--   0        0        0     6283 2024-01-31 17:10:26.230995 geoh5py-0.9.0a2/geoh5py/objects/curve.py
--rw-r--r--   0        0        0     6204 2024-02-27 21:35:13.335556 geoh5py-0.9.0a2/geoh5py/objects/drape_model.py
--rw-r--r--   0        0        0    26674 2024-02-27 21:35:13.335556 geoh5py-0.9.0a2/geoh5py/objects/drillhole.py
--rw-r--r--   0        0        0    21664 2024-02-27 21:35:13.336599 geoh5py-0.9.0a2/geoh5py/objects/geo_image.py
--rw-r--r--   0        0        0    14054 2024-02-27 21:35:13.337607 geoh5py-0.9.0a2/geoh5py/objects/grid2d.py
--rw-r--r--   0        0        0     4879 2024-01-31 17:10:26.233995 geoh5py-0.9.0a2/geoh5py/objects/grid_object.py
--rw-r--r--   0        0        0     1957 2024-01-31 17:10:26.233995 geoh5py-0.9.0a2/geoh5py/objects/integrator.py
--rw-r--r--   0        0        0     2921 2024-02-27 21:35:13.337607 geoh5py-0.9.0a2/geoh5py/objects/label.py
--rw-r--r--   0        0        0     2686 2024-02-27 21:35:13.338599 geoh5py-0.9.0a2/geoh5py/objects/notype_object.py
--rw-r--r--   0        0        0    21547 2024-02-27 21:35:13.338599 geoh5py-0.9.0a2/geoh5py/objects/object_base.py
--rw-r--r--   0        0        0     2706 2024-02-27 21:35:13.339599 geoh5py-0.9.0a2/geoh5py/objects/object_type.py
--rw-r--r--   0        0        0    13293 2024-02-27 21:35:13.339599 geoh5py-0.9.0a2/geoh5py/objects/octree.py
--rw-r--r--   0        0        0     5354 2024-02-27 21:35:13.339599 geoh5py-0.9.0a2/geoh5py/objects/points.py
--rw-r--r--   0        0        0     2588 2024-01-31 17:10:26.236988 geoh5py-0.9.0a2/geoh5py/objects/surface.py
--rw-r--r--   0        0        0      747 2024-01-31 17:10:26.236988 geoh5py-0.9.0a2/geoh5py/objects/surveys/__init__.py
--rw-r--r--   0        0        0    14521 2024-02-27 21:35:13.340599 geoh5py-0.9.0a2/geoh5py/objects/surveys/direct_current.py
--rw-r--r--   0        0        0      747 2024-01-31 17:10:26.237995 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py
--rw-r--r--   0        0        0     3660 2024-01-31 17:10:26.238995 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
--rw-r--r--   0        0        0     3629 2024-01-31 17:10:26.238995 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
--rw-r--r--   0        0        0    36522 2024-02-27 21:35:13.341599 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/base.py
--rw-r--r--   0        0        0     6925 2024-01-31 17:10:26.239995 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py
--rw-r--r--   0        0        0     6937 2024-01-31 17:10:26.240997 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py
--rw-r--r--   0        0        0     2615 2024-01-31 17:10:26.240997 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
--rw-r--r--   0        0        0     6605 2024-02-27 21:35:13.341599 geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py
--rw-r--r--   0        0        0     1247 2024-01-31 17:10:26.241996 geoh5py-0.9.0a2/geoh5py/objects/surveys/magnetics.py
--rw-r--r--   0        0        0        0 2023-05-16 13:39:30.036442 geoh5py-0.9.0a2/geoh5py/py.typed
--rw-r--r--   0        0        0     1013 2024-01-31 17:10:26.242995 geoh5py-0.9.0a2/geoh5py/shared/__init__.py
--rw-r--r--   0        0        0     1057 2024-02-27 21:35:13.342599 geoh5py-0.9.0a2/geoh5py/shared/concatenation/__init__.py
--rw-r--r--   0        0        0     1847 2024-02-27 21:35:13.343599 geoh5py-0.9.0a2/geoh5py/shared/concatenation/concatenated.py
--rw-r--r--   0        0        0    24482 2024-02-27 21:35:13.343599 geoh5py-0.9.0a2/geoh5py/shared/concatenation/concatenator.py
--rw-r--r--   0        0        0     3029 2024-01-31 17:10:26.243995 geoh5py-0.9.0a2/geoh5py/shared/concatenation/data.py
--rw-r--r--   0        0        0    14314 2024-02-27 21:35:13.344598 geoh5py-0.9.0a2/geoh5py/shared/concatenation/drillhole.py
--rw-r--r--   0        0        0    15588 2024-02-27 21:35:13.344598 geoh5py-0.9.0a2/geoh5py/shared/concatenation/drillholes_group_table.py
--rw-r--r--   0        0        0     6455 2024-02-27 21:35:13.345598 geoh5py-0.9.0a2/geoh5py/shared/concatenation/object.py
--rw-r--r--   0        0        0     4054 2024-01-31 17:10:26.244995 geoh5py-0.9.0a2/geoh5py/shared/concatenation/property_group.py
--rw-r--r--   0        0        0      937 2024-01-31 17:10:26.245988 geoh5py-0.9.0a2/geoh5py/shared/conversion/__init__.py
--rw-r--r--   0        0        0     4426 2024-01-31 17:10:26.247000 geoh5py-0.9.0a2/geoh5py/shared/conversion/base.py
--rw-r--r--   0        0        0     5694 2024-01-31 17:10:26.247000 geoh5py-0.9.0a2/geoh5py/shared/conversion/geo_image.py
--rw-r--r--   0        0        0    10840 2024-01-31 17:10:26.247996 geoh5py-0.9.0a2/geoh5py/shared/conversion/grid2d.py
--rw-r--r--   0        0        0    10949 2024-02-27 21:35:13.345598 geoh5py-0.9.0a2/geoh5py/shared/entity.py
--rw-r--r--   0        0        0     8227 2024-02-27 21:35:13.346598 geoh5py-0.9.0a2/geoh5py/shared/entity_container.py
--rw-r--r--   0        0        0     4902 2024-02-27 21:35:13.346598 geoh5py-0.9.0a2/geoh5py/shared/entity_type.py
--rw-r--r--   0        0        0     8353 2024-01-31 17:10:26.248996 geoh5py-0.9.0a2/geoh5py/shared/exceptions.py
--rw-r--r--   0        0        0      923 2024-01-31 17:10:26.248996 geoh5py-0.9.0a2/geoh5py/shared/merging/__init__.py
--rw-r--r--   0        0        0     7734 2024-01-31 17:10:26.249988 geoh5py-0.9.0a2/geoh5py/shared/merging/base.py
--rw-r--r--   0        0        0     2336 2024-01-31 17:10:26.249988 geoh5py-0.9.0a2/geoh5py/shared/merging/cell.py
--rw-r--r--   0        0        0     6105 2024-01-31 17:10:26.249988 geoh5py-0.9.0a2/geoh5py/shared/merging/drape_model.py
--rw-r--r--   0        0        0     1845 2024-01-31 17:10:26.250990 geoh5py-0.9.0a2/geoh5py/shared/merging/points.py
--rw-r--r--   0        0        0    20399 2024-02-27 21:35:13.347598 geoh5py-0.9.0a2/geoh5py/shared/utils.py
--rw-r--r--   0        0        0     8847 2024-01-31 17:10:26.252006 geoh5py-0.9.0a2/geoh5py/shared/validators.py
--rw-r--r--   0        0        0     2647 2024-01-31 17:10:26.252997 geoh5py-0.9.0a2/geoh5py/shared/weakref_utils.py
--rw-r--r--   0        0        0      959 2024-01-31 17:10:26.252997 geoh5py-0.9.0a2/geoh5py/ui_json/__init__.py
--rw-r--r--   0        0        0     2991 2024-01-31 17:10:26.253990 geoh5py-0.9.0a2/geoh5py/ui_json/constants.py
--rw-r--r--   0        0        0     1983 2024-01-31 17:10:26.255001 geoh5py-0.9.0a2/geoh5py/ui_json/descriptors.py
--rw-r--r--   0        0        0    11461 2024-01-31 17:10:26.255001 geoh5py-0.9.0a2/geoh5py/ui_json/enforcers.py
--rw-r--r--   0        0        0    18309 2024-01-31 17:10:26.255001 geoh5py-0.9.0a2/geoh5py/ui_json/forms.py
--rw-r--r--   0        0        0    18470 2024-01-31 17:10:26.256568 geoh5py-0.9.0a2/geoh5py/ui_json/input_file.py
--rw-r--r--   0        0        0     4945 2024-01-31 17:10:26.256568 geoh5py-0.9.0a2/geoh5py/ui_json/parameters.py
--rw-r--r--   0        0        0    13401 2024-02-27 21:35:13.347598 geoh5py-0.9.0a2/geoh5py/ui_json/templates.py
--rw-r--r--   0        0        0     5076 2024-01-31 17:10:26.257592 geoh5py-0.9.0a2/geoh5py/ui_json/ui_json.py
--rw-r--r--   0        0        0    11335 2024-02-27 21:35:13.348599 geoh5py-0.9.0a2/geoh5py/ui_json/utils.py
--rw-r--r--   0        0        0    11275 2024-02-27 21:35:13.349598 geoh5py-0.9.0a2/geoh5py/ui_json/validation.py
--rw-r--r--   0        0        0      852 2024-01-31 17:10:26.258592 geoh5py-0.9.0a2/geoh5py/workspace/__init__.py
--rw-r--r--   0        0        0    50862 2024-02-27 21:35:13.349691 geoh5py-0.9.0a2/geoh5py/workspace/workspace.py
--rw-r--r--   0        0        0     2111 2024-01-31 17:10:26.259585 geoh5py-0.9.0a2/package.rst
--rw-r--r--   0        0        0     2212 2024-02-27 21:35:13.350853 geoh5py-0.9.0a2/pyproject.toml
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 geoh5py-0.9.0a2/PKG-INFO
+-rw-r--r--   0        0        0      841 2024-04-12 18:06:37.656160 geoh5py-0.9.0a3/geoh5py/__init__.py
+-rw-r--r--   0        0        0     1574 2024-01-31 17:10:26.210995 geoh5py-0.9.0a3/geoh5py/data/__init__.py
+-rw-r--r--   0        0        0     1311 2024-01-31 17:10:26.210995 geoh5py-0.9.0a3/geoh5py/data/blob_data.py
+-rw-r--r--   0        0        0     2005 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/data/boolean_data.py
+-rw-r--r--   0        0        0     3756 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/color_map.py
+-rw-r--r--   0        0        0     8914 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/data.py
+-rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.212998 geoh5py-0.9.0a3/geoh5py/data/data_association_enum.py
+-rw-r--r--   0        0        0    13377 2024-04-12 17:42:35.137291 geoh5py-0.9.0a3/geoh5py/data/data_type.py
+-rw-r--r--   0        0        0     1138 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/data_unit.py
+-rw-r--r--   0        0        0     1340 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/datetime_data.py
+-rw-r--r--   0        0        0     3690 2024-01-31 17:10:26.213988 geoh5py-0.9.0a3/geoh5py/data/filename_data.py
+-rw-r--r--   0        0        0     1787 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/float_data.py
+-rw-r--r--   0        0        0     1625 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/geometric_data_constants.py
+-rw-r--r--   0        0        0     1709 2024-01-31 17:10:26.214988 geoh5py-0.9.0a3/geoh5py/data/integer_data.py
+-rw-r--r--   0        0        0     4001 2024-01-31 17:10:26.215988 geoh5py-0.9.0a3/geoh5py/data/numeric_data.py
+-rw-r--r--   0        0        0     1121 2024-01-31 17:10:26.215988 geoh5py-0.9.0a3/geoh5py/data/primitive_type_enum.py
+-rw-r--r--   0        0        0     2896 2024-04-12 17:42:35.138630 geoh5py-0.9.0a3/geoh5py/data/reference_value_map.py
+-rw-r--r--   0        0        0     1531 2024-01-31 17:10:26.216996 geoh5py-0.9.0a3/geoh5py/data/referenced_data.py
+-rw-r--r--   0        0        0     5093 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/data/text_data.py
+-rw-r--r--   0        0        0     1573 2024-01-31 17:10:26.216996 geoh5py-0.9.0a3/geoh5py/data/unknown_data.py
+-rw-r--r--   0        0        0     4559 2024-01-31 17:10:26.217996 geoh5py-0.9.0a3/geoh5py/data/visual_parameters.py
+-rw-r--r--   0        0        0     1587 2024-01-31 17:10:26.217996 geoh5py-0.9.0a3/geoh5py/groups/__init__.py
+-rw-r--r--   0        0        0     1441 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/container_group.py
+-rw-r--r--   0        0        0     1474 2024-04-12 17:42:35.139243 geoh5py-0.9.0a3/geoh5py/groups/custom_group.py
+-rw-r--r--   0        0        0     1797 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/drillhole_group.py
+-rw-r--r--   0        0        0     1444 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/giftools_group.py
+-rw-r--r--   0        0        0     7068 2024-04-12 17:42:35.139513 geoh5py-0.9.0a3/geoh5py/groups/group.py
+-rw-r--r--   0        0        0     2517 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/groups/group_type.py
+-rw-r--r--   0        0        0     6714 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/integrator_group.py
+-rw-r--r--   0        0        0     1295 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/maps_group.py
+-rw-r--r--   0        0        0     1414 2024-04-12 17:41:26.545326 geoh5py-0.9.0a3/geoh5py/groups/notype_group.py
+-rw-r--r--   0        0        0     7843 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/groups/property_group.py
+-rw-r--r--   0        0        0     1593 2024-01-31 17:10:26.221995 geoh5py-0.9.0a3/geoh5py/groups/root_group.py
+-rw-r--r--   0        0        0     2053 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/groups/simpeg_group.py
+-rw-r--r--   0        0        0     1322 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/groups/survey_group.py
+-rw-r--r--   0        0        0      866 2024-01-31 17:10:26.228996 geoh5py-0.9.0a3/geoh5py/io/__init__.py
+-rw-r--r--   0        0        0    17355 2024-04-12 17:42:35.139932 geoh5py-0.9.0a3/geoh5py/io/h5_reader.py
+-rw-r--r--   0        0        0    34866 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/io/h5_writer.py
+-rw-r--r--   0        0        0     2403 2024-01-31 17:10:26.229997 geoh5py-0.9.0a3/geoh5py/objects/__init__.py
+-rw-r--r--   0        0        0     9440 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/block_model.py
+-rw-r--r--   0        0        0     7874 2024-01-31 17:10:26.230995 geoh5py-0.9.0a3/geoh5py/objects/cell_object.py
+-rw-r--r--   0        0        0     6300 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/objects/curve.py
+-rw-r--r--   0        0        0     6204 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/drape_model.py
+-rw-r--r--   0        0        0    26674 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/drillhole.py
+-rw-r--r--   0        0        0    21664 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/geo_image.py
+-rw-r--r--   0        0        0    14054 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/grid2d.py
+-rw-r--r--   0        0        0     4879 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/grid_object.py
+-rw-r--r--   0        0        0     1957 2024-01-31 17:10:26.233995 geoh5py-0.9.0a3/geoh5py/objects/integrator.py
+-rw-r--r--   0        0        0     2921 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/label.py
+-rw-r--r--   0        0        0     2686 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/notype_object.py
+-rw-r--r--   0        0        0    21773 2024-04-12 17:42:35.141445 geoh5py-0.9.0a3/geoh5py/objects/object_base.py
+-rw-r--r--   0        0        0     1098 2024-04-12 17:42:35.142822 geoh5py-0.9.0a3/geoh5py/objects/object_type.py
+-rw-r--r--   0        0        0    13455 2024-04-12 17:42:35.142822 geoh5py-0.9.0a3/geoh5py/objects/octree.py
+-rw-r--r--   0        0        0     5354 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/points.py
+-rw-r--r--   0        0        0     2588 2024-01-31 17:10:26.236988 geoh5py-0.9.0a3/geoh5py/objects/surface.py
+-rw-r--r--   0        0        0      747 2024-01-31 17:10:26.236988 geoh5py-0.9.0a3/geoh5py/objects/surveys/__init__.py
+-rw-r--r--   0        0        0    14521 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/direct_current.py
+-rw-r--r--   0        0        0      747 2024-01-31 17:10:26.237995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py
+-rw-r--r--   0        0        0     3660 2024-01-31 17:10:26.238995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py
+-rw-r--r--   0        0        0     3629 2024-01-31 17:10:26.238995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py
+-rw-r--r--   0        0        0    36522 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/base.py
+-rw-r--r--   0        0        0     6925 2024-01-31 17:10:26.239995 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py
+-rw-r--r--   0        0        0     6937 2024-01-31 17:10:26.240997 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py
+-rw-r--r--   0        0        0     2615 2024-01-31 17:10:26.240997 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py
+-rw-r--r--   0        0        0     6605 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py
+-rw-r--r--   0        0        0     1247 2024-01-31 17:10:26.241996 geoh5py-0.9.0a3/geoh5py/objects/surveys/magnetics.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:39:30.036442 geoh5py-0.9.0a3/geoh5py/py.typed
+-rw-r--r--   0        0        0     1013 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/__init__.py
+-rw-r--r--   0        0        0     1057 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/__init__.py
+-rw-r--r--   0        0        0     1847 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenated.py
+-rw-r--r--   0        0        0    25972 2024-04-12 17:42:35.144031 geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenator.py
+-rw-r--r--   0        0        0     3029 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/concatenation/data.py
+-rw-r--r--   0        0        0    14282 2024-04-12 17:42:35.144031 geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillhole.py
+-rw-r--r--   0        0        0    15847 2024-04-12 17:42:35.144771 geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillholes_group_table.py
+-rw-r--r--   0        0        0     6729 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/concatenation/object.py
+-rw-r--r--   0        0        0     5193 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/concatenation/property_group.py
+-rw-r--r--   0        0        0      937 2024-01-31 17:10:26.245988 geoh5py-0.9.0a3/geoh5py/shared/conversion/__init__.py
+-rw-r--r--   0        0        0     4426 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/conversion/base.py
+-rw-r--r--   0        0        0     5694 2024-01-31 17:10:26.247000 geoh5py-0.9.0a3/geoh5py/shared/conversion/geo_image.py
+-rw-r--r--   0        0        0    10840 2024-01-31 17:10:26.247996 geoh5py-0.9.0a3/geoh5py/shared/conversion/grid2d.py
+-rw-r--r--   0        0        0    10730 2024-04-12 17:42:35.145267 geoh5py-0.9.0a3/geoh5py/shared/entity.py
+-rw-r--r--   0        0        0     7630 2024-04-12 17:42:35.146468 geoh5py-0.9.0a3/geoh5py/shared/entity_container.py
+-rw-r--r--   0        0        0     8632 2024-04-12 17:42:35.146468 geoh5py-0.9.0a3/geoh5py/shared/entity_type.py
+-rw-r--r--   0        0        0     8353 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/exceptions.py
+-rw-r--r--   0        0        0      923 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/merging/__init__.py
+-rw-r--r--   0        0        0     7734 2024-04-12 17:41:26.560944 geoh5py-0.9.0a3/geoh5py/shared/merging/base.py
+-rw-r--r--   0        0        0     2336 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/cell.py
+-rw-r--r--   0        0        0     6105 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/drape_model.py
+-rw-r--r--   0        0        0     1845 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/merging/points.py
+-rw-r--r--   0        0        0    21424 2024-04-12 17:42:35.147275 geoh5py-0.9.0a3/geoh5py/shared/utils.py
+-rw-r--r--   0        0        0     8847 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/shared/validators.py
+-rw-r--r--   0        0        0     2647 2024-01-31 17:10:26.252997 geoh5py-0.9.0a3/geoh5py/shared/weakref_utils.py
+-rw-r--r--   0        0        0      959 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/__init__.py
+-rw-r--r--   0        0        0     2991 2024-01-31 17:10:26.253990 geoh5py-0.9.0a3/geoh5py/ui_json/constants.py
+-rw-r--r--   0        0        0     1983 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/descriptors.py
+-rw-r--r--   0        0        0    11461 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/enforcers.py
+-rw-r--r--   0        0        0    18309 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/forms.py
+-rw-r--r--   0        0        0    18789 2024-04-12 17:42:35.147275 geoh5py-0.9.0a3/geoh5py/ui_json/input_file.py
+-rw-r--r--   0        0        0     4945 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/parameters.py
+-rw-r--r--   0        0        0    15250 2024-04-12 17:42:35.148339 geoh5py-0.9.0a3/geoh5py/ui_json/templates.py
+-rw-r--r--   0        0        0     5076 2024-04-12 17:41:26.576578 geoh5py-0.9.0a3/geoh5py/ui_json/ui_json.py
+-rw-r--r--   0        0        0    11199 2024-04-12 17:42:35.148922 geoh5py-0.9.0a3/geoh5py/ui_json/utils.py
+-rw-r--r--   0        0        0    11408 2024-04-12 17:42:35.148922 geoh5py-0.9.0a3/geoh5py/ui_json/validation.py
+-rw-r--r--   0        0        0      852 2024-01-31 17:10:26.258592 geoh5py-0.9.0a3/geoh5py/workspace/__init__.py
+-rw-r--r--   0        0        0    50970 2024-04-12 17:42:35.150153 geoh5py-0.9.0a3/geoh5py/workspace/workspace.py
+-rw-r--r--   0        0        0     2111 2024-01-31 17:10:26.259585 geoh5py-0.9.0a3/package.rst
+-rw-r--r--   0        0        0     2211 2024-04-12 18:06:37.656160 geoh5py-0.9.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3412 1970-01-01 00:00:00.000000 geoh5py-0.9.0a3/PKG-INFO
```

### Comparing `geoh5py-0.9.0a2/geoh5py/__init__.py` & `geoh5py-0.9.0a3/geoh5py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # flake8: noqa
 
-__version__ = "0.9.0-alpha.2"
+__version__ = "0.9.0-alpha.3"
 
 from geoh5py.workspace import Workspace
```

### Comparing `geoh5py-0.9.0a2/geoh5py/data/__init__.py` & `geoh5py-0.9.0a3/geoh5py/data/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/blob_data.py` & `geoh5py-0.9.0a3/geoh5py/data/blob_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/boolean_data.py` & `geoh5py-0.9.0a3/geoh5py/data/boolean_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/color_map.py` & `geoh5py-0.9.0a3/geoh5py/data/color_map.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from geoh5py.shared.exceptions import ShapeValidationError
+from ..shared.exceptions import ShapeValidationError
+from ..shared.utils import map_attributes
 
 if TYPE_CHECKING:
     from .data_type import DataType
 
 
 class ColorMap:
     """Records colors assigned to value ranges (where Value is the start of the range)."""
@@ -34,21 +35,15 @@
     _formats = ["<f8", "u1", "u1", "u1", "u1"]
 
     def __init__(self, **kwargs):
         self._values = np.empty((0, 5))
         self._name = "geoh5py_custom.TBL"
         self._parent = None
 
-        for attr, item in kwargs.items():
-            try:
-                if attr in self._attribute_map:
-                    attr = self._attribute_map[attr]
-                setattr(self, attr, item)
-            except AttributeError:
-                continue
+        map_attributes(self, **kwargs)
 
     @property
     def values(self) -> np.ndarray | None:
         """
         :obj:`numpy.array`: Colormap defined by values and corresponding RGBA:
 
         .. code-block:: python
```

### Comparing `geoh5py-0.9.0a2/geoh5py/data/data.py` & `geoh5py-0.9.0a3/geoh5py/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,18 @@
     _attribute_map = Entity._attribute_map.copy()
     _attribute_map.update({"Association": "association", "Modifiable": "modifiable"})
     _visible = False
 
     def __init__(
         self,
         data_type: DataType,
+        association: DataAssociationEnum = DataAssociationEnum.OBJECT,
         **kwargs,
     ):
-        self._association = None
+        self.association = association
         self._on_file = False
         self._modifiable = True
 
         if (
             not isinstance(data_type, DataType)
             or data_type.primitive_type != self.primitive_type()
         ):
@@ -177,15 +178,15 @@
     def values(self):
         """
         Data values
         """
         return self._values
 
     @property
-    def association(self) -> DataAssociationEnum | None:
+    def association(self) -> DataAssociationEnum:
         """
         :obj:`~geoh5py.data.data_association_enum.DataAssociationEnum`:
         Relationship made between the
         :func:`~geoh5py.data.data.Data.values` and elements of the
         :obj:`~geoh5py.shared.entity.Entity.parent` object.
         Association can be set from a :obj:`str` chosen from the list of available
         :obj:`~geoh5py.data.data_association_enum.DataAssociationEnum` options.
```

### Comparing `geoh5py-0.9.0a2/geoh5py/data/data_association_enum.py` & `geoh5py-0.9.0a3/geoh5py/data/data_association_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/data_type.py` & `geoh5py-0.9.0a3/geoh5py/data/data_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,309 +14,292 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import uuid
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING, Literal, cast, get_args
 
 import numpy as np
 
 from ..shared import EntityType
 from .color_map import ColorMap
 from .geometric_data_constants import GeometricDataConstants
 from .primitive_type_enum import PrimitiveTypeEnum
 from .reference_value_map import ReferenceValueMap
 
 if TYPE_CHECKING:
     from ..workspace import Workspace
     from .data import Data  # noqa: F401
 
 
+ColorMapping = Literal["linear", "equal_area", "logarithmic", "cdf", "missing"]
+
+
 class DataType(EntityType):
+    # pylint: disable=too-many-arguments
     """
-    DataType class
+    DataType class.
+
+    Controls all the attributes of the data type for displays in Geoscience ANALYST.
+
+    :param workspace: An active Workspace.
+    :param primitive_type: The primitive type of the data.
+    :param color_map: The colormap used for plotting.
+    :param hidden: If the data are hidden or not.
+    :param mapping: The type of color stretching to plot the colormap.
+    :param number_of_bins: The number of bins used by the histogram.
+    :param transparent_no_data: If the no data values are displayed as transparent or not.
+    :param units: The type of the units of the data.
+    :param value_map: Reference value map for to map index with description.
+    :param kwargs: Additional keyword arguments to set as attributes
+        (see :obj:`...shared.entity_type.EntityType`).
     """
 
     _attribute_map = EntityType._attribute_map.copy()
     _attribute_map.update(
         {
             "Hidden": "hidden",
             "Mapping": "mapping",
             "Number of bins": "number_of_bins",
             "Primitive type": "primitive_type",
             "Transparent no data": "transparent_no_data",
         }
     )
 
-    _primitive_type: PrimitiveTypeEnum | None = None
-    _value_map: ReferenceValueMap | None = None
-    _color_map: ColorMap | None = None
-    _units: str | None = None
-    _number_of_bins: int = 50
-    _transparent_no_data = True
-    _mapping: str = "equal_area"
-    _hidden: bool = False
-
-    def __init__(self, workspace: Workspace, **kwargs):
-        assert workspace is not None
+    def __init__(
+        self,
+        workspace: Workspace,
+        primitive_type: type[Data] | PrimitiveTypeEnum | str | None = None,
+        color_map: ColorMap | None = None,
+        hidden: bool = False,
+        mapping: ColorMapping = "equal_area",
+        number_of_bins: int | None = None,
+        transparent_no_data: bool = True,
+        units: str | None = None,
+        value_map: dict[int, str] | ReferenceValueMap | None = None,
+        **kwargs,
+    ):
         super().__init__(workspace, **kwargs)
+        self.color_map = color_map
+        self.hidden = hidden
+        self.mapping = mapping
+        self.number_of_bins = number_of_bins
+        self.primitive_type = primitive_type  # type: ignore
+        self.transparent_no_data = transparent_no_data
+        self.units = units
+        self.value_map = value_map  # type: ignore
 
-    @staticmethod
-    def _is_abstract() -> bool:
-        return False
+    @classmethod
+    def _for_geometric_data(cls, workspace: Workspace, uid: uuid.UUID) -> DataType:
+        """
+        Get the data type for geometric data.
+
+        :param workspace: An active Workspace.
+        :param uid: The uid of the existing data type to get.
+
+        :return: A new instance of DataType.
+        """
+        geom_primitive_type = GeometricDataConstants.primitive_type()
+        data_type = cast(DataType, workspace.find_type(uid, DataType))
+        if data_type is not None:
+            if not data_type.primitive_type == geom_primitive_type:
+                raise ValueError(
+                    f"Data type with uid {uid} is not of type {geom_primitive_type}"
+                )
+            return data_type
+        return cls(workspace, uid=uid, primitive_type=geom_primitive_type)
 
     @property
     def color_map(self) -> ColorMap | None:
         r"""
-        :obj:`~geoh5py.data.color_map.ColorMap`: Colormap used for plotting
+        The Colormap used for plotting
 
-        The colormap can be set from a :obj:`dict` of sorted values with
+        The colormap can be set from a dictionary of sorted values with
         corresponding RGBA color.
+        Or from a numpy array containing the RGBA values.
 
         .. code-block:: python
 
             color_map = {
                 val_1: [r_1, g_1, b_1, a_1],
                 ...,
                 val_i: [r_i, g_i, b_i, a_i]
             }
 
+        It can be set to None if non-existing.
         """
         return self._color_map
 
     @color_map.setter
-    def color_map(self, color_map: ColorMap | dict | np.ndarray):
+    def color_map(self, color_map: ColorMap | dict | np.ndarray | None):
         if isinstance(color_map, dict):
             color_map = ColorMap(**color_map)
 
         elif isinstance(color_map, np.ndarray):
             color_map = ColorMap(values=color_map)
 
-        elif not isinstance(color_map, ColorMap):
+        if not isinstance(color_map, (ColorMap, type(None))):
             raise TypeError(
                 f"Input value for 'color_map' must be of type {ColorMap},"
                 f"numpy.ndarray or dict with 'values'."
             )
 
-        color_map.parent = self
-        self._color_map = color_map
-        self.workspace.update_attribute(self, "color_map")
-
-    @property
-    def value_map(self) -> ReferenceValueMap | None:
-        r"""
-        :obj:`~geoh5py.data.reference_value_map.ReferenceValueMap`:
-        Reference value map for :obj:`~geoh5py.data.reference_data.ReferenceData`
-
-        The value_map can be set from a :obj:`dict` of sorted values with
-        corresponding :obj:`str` description.
+        if isinstance(color_map, ColorMap):
+            color_map.parent = self
 
-        .. code-block:: python
+        self._color_map: ColorMap | None = color_map
 
-            value_map = {
-                val_1: str_1,
-                ...,
-                val_i: str_i
-            }
+        self.workspace.update_attribute(self, "color_map")
 
+    @classmethod
+    def for_x_data(cls, workspace: Workspace) -> DataType:
         """
-        return self._value_map
-
-    @value_map.setter
-    def value_map(self, value_map: dict | ReferenceValueMap):
-        if isinstance(value_map, dict):
-            value_map = ReferenceValueMap(value_map)
-        if not isinstance(value_map, ReferenceValueMap):
-            raise TypeError(f"'value_map' must be a {dict} or {ReferenceValueMap}.")
+        Get the data type for x data.
 
-        self._value_map = value_map
-        self.workspace.update_attribute(self, "value_map")
+        :param workspace: An active Workspace.
 
-    @property
-    def units(self) -> str | None:
+        :return: A new instance of DataType.
         """
-        :obj:`str`: Data units
+        return cls._for_geometric_data(
+            workspace, GeometricDataConstants.x_datatype_uid()
+        )
+
+    @classmethod
+    def for_y_data(cls, workspace: Workspace) -> DataType:
         """
-        return self._units
+        Get the data type for y data.
 
-    @units.setter
-    def units(self, unit: str):
-        self._units = unit
-        self.workspace.update_attribute(self, "attributes")
+        :param workspace: An active Workspace.
 
-    @property
-    def number_of_bins(self) -> int | None:
+        :return: A new instance of DataType.
         """
-        :obj:`int`: Number of bins used by the histogram [50]
+        return cls._for_geometric_data(
+            workspace, GeometricDataConstants.y_datatype_uid()
+        )
+
+    @classmethod
+    def for_z_data(cls, workspace: Workspace) -> DataType:
         """
-        return self._number_of_bins
+        Get the data type for z data.
 
-    @number_of_bins.setter
-    def number_of_bins(self, n_bins: int):
-        self._number_of_bins = n_bins
-        self.workspace.update_attribute(self, "attributes")
+        :param workspace: An active Workspace.
 
-    @property
-    def transparent_no_data(self) -> bool:
-        """
-        :obj:`bool`: Use transparent for no-data-value [True]
+        :return: A new instance of DataType.
         """
-        return self._transparent_no_data
-
-    @transparent_no_data.setter
-    def transparent_no_data(self, value: bool):
-        self._transparent_no_data = value
-        self.workspace.update_attribute(self, "attributes")
+        return cls._for_geometric_data(
+            workspace, GeometricDataConstants.z_datatype_uid()
+        )
 
     @property
     def hidden(self) -> bool:
         """
-        :obj:`bool`: Hidden data [False]
+        If the data are hidden or not.
         """
         return self._hidden
 
     @hidden.setter
     def hidden(self, value: bool):
-        self._hidden = value
+        if not isinstance(value, bool) and value != 1 and value != 0:
+            raise TypeError(f"hidden must be a bool, not {type(value)}")
+
+        self._hidden: bool = bool(value)
+
         self.workspace.update_attribute(self, "attributes")
 
     @property
     def mapping(self) -> str:
         """
-        :obj:`str`: Color stretching type chosen from:
-        'linear', ['equal_area'], 'logarithmic', 'cdf', 'missing'
+        The type of color stretching to plot the colormap.
+        It chan be one of the following:
+        'linear', 'equal_area', 'logarithmic', 'cdf', 'missing'
         """
         return self._mapping
 
     @mapping.setter
-    def mapping(self, value: str):
-        mappings = ["linear", "equal_area", "logarithmic", "cdf", "missing"]
-        assert (
-            value in mappings
-        ), f"Mapping {value} was provided but should be one of {mappings}"
-        self._mapping = value
+    def mapping(self, value: ColorMapping):
+        if value not in get_args(ColorMapping):
+            raise ValueError(
+                f"Mapping {value} was provided but should be one of {get_args(ColorMapping)}"
+            )
+        self._mapping: str = value
+
         self.workspace.update_attribute(self, "attributes")
 
     @property
-    def primitive_type(self) -> PrimitiveTypeEnum | None:
+    def number_of_bins(self) -> int | None:
         """
-        :obj:`~geoh5py.data.primitive_type_enum.PrimitiveTypeEnum`
+        The number of bins used by the histogram.
+        It can be None if no histogram is used.
         """
-        return self._primitive_type
+        return self._number_of_bins
 
-    @primitive_type.setter
-    def primitive_type(self, value):
-        if isinstance(value, str):
-            self._primitive_type = getattr(
-                PrimitiveTypeEnum, value.replace("-", "_").upper()
+    @number_of_bins.setter
+    def number_of_bins(self, n_bins: int | None):
+        if n_bins is None:
+            pass
+        elif not isinstance(n_bins, (int, np.integer)) or n_bins < 1:
+            raise ValueError(
+                f"Number of bins should be an integer greater than 0 or None, not {n_bins}"
             )
-        else:
-            assert isinstance(
-                value, PrimitiveTypeEnum
-            ), f"Primitive type value must be of type {PrimitiveTypeEnum}"
-            self._primitive_type = value
-
-    @classmethod
-    def create(cls, workspace: Workspace, data_class: type[Data]) -> DataType:
-        """Creates a new instance of :obj:`~geoh5py.data.data_type.DataType` with
-        corresponding :obj:`~geoh5py.data.primitive_type_enum.PrimitiveTypeEnum`.
-
-        :param workspace: An active Workspace.
-        :param data_class: A :obj:`~geoh5py.data.data.Data` implementation class.
-
-        :return: A new instance of :obj:`~geoh5py.data.data_type.DataType`.
-        """
-        uid = uuid.uuid4()
-        primitive_type = data_class.primitive_type()
-        return cls(workspace, uid=uid, primitive_type=primitive_type)
 
-    @classmethod
-    def find_or_create(cls, workspace: Workspace, **kwargs) -> DataType:
-        """Find or creates an EntityType with given UUID that matches the given
-        Group implementation class.
+        self._number_of_bins: int | None = n_bins
 
-        :param workspace: An active Workspace class
+        self.workspace.update_attribute(self, "attributes")
 
-        :return: A new instance of DataType.
+    @property
+    def primitive_type(self) -> PrimitiveTypeEnum | None:
         """
-        uid = uuid.uuid4()
-
-        for key, val in kwargs.items():
-            if key.lower() in ["id", "uid"]:
-                if isinstance(val, uuid.UUID):
-                    uid = val
-                else:
-                    uid = uuid.UUID(val)
-
-        entity_type = cls.find(workspace, uid)
-
-        if entity_type is not None:
-            return entity_type
-
-        kwargs["uid"] = uid
-
-        return cls(workspace, **kwargs)
-
-    @classmethod
-    def _for_geometric_data(cls, workspace: Workspace, uid: uuid.UUID) -> DataType:
+        The primitive type of the data.
         """
-        Get the data type for geometric data.
+        return self._primitive_type
 
-        :param workspace: An active Workspace.
-        :param uid: The uid of the existing data type to get.
+    @primitive_type.setter
+    def primitive_type(self, value: str | type[Data] | PrimitiveTypeEnum | None):
+        if isinstance(value, str):
+            value = getattr(PrimitiveTypeEnum, value.replace("-", "_").upper())
+        elif hasattr(value, "primitive_type"):
+            value = getattr(value, "primitive_type")()
+        if not isinstance(value, (PrimitiveTypeEnum, type(None))):
+            raise ValueError(
+                f"Primitive type value must be of type {PrimitiveTypeEnum}, find {type(value)}"
+            )
 
-        :return: A new instance of DataType.
-        """
-        geom_primitive_type = GeometricDataConstants.primitive_type()
-        data_type = cast(DataType, workspace.find_type(uid, DataType))
-        if data_type is not None:
-            assert data_type.primitive_type == geom_primitive_type
-            return data_type
-        return cls(workspace, uid=uid, primitive_type=geom_primitive_type)
+        self._primitive_type = value
 
-    @classmethod
-    def for_x_data(cls, workspace: Workspace) -> DataType:
+    @property
+    def transparent_no_data(self) -> bool:
         """
-        Get the data type for x data.
-
-        :param workspace: An active Workspace.
-
-        :return: A new instance of DataType.
+        If the no data values are displayed as transparent or not.
         """
-        return cls._for_geometric_data(
-            workspace, GeometricDataConstants.x_datatype_uid()
-        )
+        return self._transparent_no_data
 
-    @classmethod
-    def for_y_data(cls, workspace: Workspace) -> DataType:
-        """
-        Get the data type for y data.
+    @transparent_no_data.setter
+    def transparent_no_data(self, value: bool):
+        if not isinstance(value, bool) and value != 1 and value != 0:
+            raise TypeError(f"transparent_no_data must be a bool, not {type(value)}")
+        self._transparent_no_data = bool(value)
 
-        :param workspace: An active Workspace.
+        self.workspace.update_attribute(self, "attributes")
 
-        :return: A new instance of DataType.
+    @property
+    def units(self) -> str | None:
         """
-        return cls._for_geometric_data(
-            workspace, GeometricDataConstants.y_datatype_uid()
-        )
-
-    @classmethod
-    def for_z_data(cls, workspace: Workspace) -> DataType:
+        The type of the units of the data.
         """
-        Get the data type for z data.
+        return self._units
 
-        :param workspace: An active Workspace.
+    @units.setter
+    def units(self, unit: str | None):
+        if not isinstance(unit, (str, type(None))):
+            raise TypeError(f"units must be a string, not {type(unit)}")
+        self._units = unit
 
-        :return: A new instance of DataType.
-        """
-        return cls._for_geometric_data(
-            workspace, GeometricDataConstants.z_datatype_uid()
-        )
+        self.workspace.update_attribute(self, "attributes")
 
     @staticmethod
     def validate_data_type(workspace: Workspace, attribute_dict: dict):
         """
         Get a dictionary of attributes and validate the type of data.
 
         :param workspace: An active Workspace.
@@ -333,20 +316,22 @@
                     primitive_type.upper() in PrimitiveTypeEnum.__members__
                 ), f"Data 'type' should be one of {PrimitiveTypeEnum.__members__}"
                 entity_type = {"primitive_type": primitive_type.upper()}
             else:
                 values = attribute_dict.get("values")
                 if values is None or (
                     isinstance(values, np.ndarray)
-                    and (values.dtype in [np.float32, np.float64])
+                    and np.issubdtype(values.dtype, np.floating)
                 ):
                     entity_type = {"primitive_type": "FLOAT"}
+
                 elif isinstance(values, np.ndarray) and (
-                    values.dtype in [np.uint32, np.int32]
+                    np.issubdtype(values.dtype, np.integer)
                 ):
+
                     entity_type = {"primitive_type": "INTEGER"}
                 elif isinstance(values, str) or (
                     isinstance(values, np.ndarray) and values.dtype.kind in ["U", "S"]
                 ):
                     entity_type = {"primitive_type": "TEXT"}
                 elif isinstance(values, np.ndarray) and (values.dtype == bool):
                     entity_type = {"primitive_type": "BOOLEAN"}
@@ -358,7 +343,39 @@
         elif isinstance(entity_type, EntityType) and (
             (entity_type.uid not in getattr(workspace, "_types"))
             or (entity_type.workspace != workspace)
         ):
             return entity_type.copy(workspace=workspace)
 
         return entity_type
+
+    @property
+    def value_map(self) -> ReferenceValueMap | None:
+        r"""
+        Reference value map for to map index with description.
+
+        The value_map can be set from a dictionary of sorted values int
+        values with text description.
+
+        .. code-block:: python
+
+            value_map = {
+                val_1: str_1,
+                ...,
+                val_i: str_i
+            }
+
+        """
+        return self._value_map
+
+    @value_map.setter
+    def value_map(self, value_map: dict[int, str] | ReferenceValueMap | None):
+        if isinstance(value_map, dict):
+            value_map = ReferenceValueMap(value_map)
+        if not isinstance(value_map, (ReferenceValueMap, type(None))):
+            raise TypeError(
+                f"'value_map' must be a {dict} or {ReferenceValueMap} or {type(None)}."
+            )
+
+        self._value_map: ReferenceValueMap | None = value_map
+
+        self.workspace.update_attribute(self, "value_map")
```

### Comparing `geoh5py-0.9.0a2/geoh5py/data/data_unit.py` & `geoh5py-0.9.0a3/geoh5py/data/data_unit.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/datetime_data.py` & `geoh5py-0.9.0a3/geoh5py/data/datetime_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/filename_data.py` & `geoh5py-0.9.0a3/geoh5py/data/filename_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/float_data.py` & `geoh5py-0.9.0a3/geoh5py/data/float_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/geometric_data_constants.py` & `geoh5py-0.9.0a3/geoh5py/data/geometric_data_constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/integer_data.py` & `geoh5py-0.9.0a3/geoh5py/data/integer_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/numeric_data.py` & `geoh5py-0.9.0a3/geoh5py/data/numeric_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/primitive_type_enum.py` & `geoh5py-0.9.0a3/geoh5py/data/primitive_type_enum.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/reference_value_map.py` & `geoh5py-0.9.0a3/geoh5py/data/reference_value_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         """
         Verify that the key and value are valid.
         It raises errors if there is an issue
 
         :param key: The key to verify.
         :param value: The value to verify.
         """
-        if not isinstance(key, (int, np.int16, np.int32, np.int64)) or key < 0:
+        if not isinstance(key, (int, np.integer)) or key < 0:
             raise KeyError("Key must be an positive integer")
         if not isinstance(value, str):
             raise TypeError("Value must be a string")
 
         if key == 0 and value != "Unknown":
             raise ValueError("Value for key 0 must be 'Unknown'")
```

### Comparing `geoh5py-0.9.0a2/geoh5py/data/referenced_data.py` & `geoh5py-0.9.0a3/geoh5py/data/referenced_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/text_data.py` & `geoh5py-0.9.0a3/geoh5py/data/text_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/unknown_data.py` & `geoh5py-0.9.0a3/geoh5py/data/unknown_data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/data/visual_parameters.py` & `geoh5py-0.9.0a3/geoh5py/data/visual_parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/__init__.py` & `geoh5py-0.9.0a3/geoh5py/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/container_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/container_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/custom_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/custom_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,9 +33,12 @@
         super().__init__(group_type, **kwargs)
 
         if self.entity_type.name == "Entity":
             self.entity_type.name = "Custom Group"
 
     @classmethod
     def default_type_uid(cls) -> uuid.UUID | None:
-        # raise RuntimeError(f"No predefined static type UUID for {cls}.")
-        return None
+        """
+        Mock the default type uid for the custom group.
+        It returns a new UUID every time this class is called.
+        """
+        return uuid.uuid4()
```

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/drillhole_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/drillhole_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/giftools_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/giftools_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/group.py` & `geoh5py-0.9.0a3/geoh5py/groups/group.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 from abc import abstractmethod
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from ..data import CommentsData, Data
+from ..shared.entity import Entity
 from ..shared.entity_container import EntityContainer
 from .group_type import GroupType
 
 if TYPE_CHECKING:
-    from .. import workspace
+    from ..workspace import Workspace
 
 
 class Group(EntityContainer):
     """Base Group class"""
 
     def __init__(self, group_type: GroupType, **kwargs):
         assert group_type is not None
@@ -41,14 +42,30 @@
         super().__init__(**kwargs)
 
     @classmethod
     @abstractmethod
     def default_type_uid(cls) -> uuid.UUID | None:
         """Abstract method to return the default type uid for the class."""
 
+    def add_children(self, children: list[Entity]):
+        """
+        :param children: Add a list of entities as
+            :obj:`~geoh5py.shared.entity.Entity.children`
+        """
+        if not isinstance(children, list):
+            children = [children]
+
+        for child in children:
+            if child not in self._children:
+                if not isinstance(child, Entity):
+                    raise TypeError(
+                        f"Child must be an instance of Entity, not {type(child)}"
+                    )
+                self._children.append(child)
+
     def add_comment(self, comment: str, author: str | None = None):
         """
         Add text comment to an object.
 
         :param comment: Text to be added as comment.
         :param author: Author's name or :obj:`~geoh5py.workspace.workspace.Workspace.contributors`.
         """
@@ -195,9 +212,10 @@
                     np.max(extents, axis=0),
                 ]
             )
 
         return None
 
     @classmethod
-    def find_or_create_type(cls, workspace: workspace.Workspace, **kwargs) -> GroupType:
-        return GroupType.find_or_create(workspace, cls, **kwargs)
+    def find_or_create_type(cls, workspace: Workspace, **kwargs) -> GroupType:
+        kwargs["entity_class"] = cls
+        return GroupType.find_or_create(workspace, **kwargs)
```

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/integrator_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/integrator_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/maps_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/maps_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/notype_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/notype_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/property_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/property_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 from __future__ import annotations
 
 import uuid
 from abc import ABC
 from collections.abc import Iterable
 from typing import TYPE_CHECKING
 
-from geoh5py.data import Data, DataAssociationEnum
+from ..data import Data, DataAssociationEnum
+from ..shared.utils import map_attributes
 
 if TYPE_CHECKING:
-    from geoh5py.objects import ObjectBase
+    from ..objects import ObjectBase
 
 
 class PropertyGroup(ABC):
     """
     Property group listing data children of an object.
     This group is not registered to the workspace and only visible to the parent object.
     """
@@ -66,21 +67,15 @@
 
         self._parent: ObjectBase = parent
         self._properties: list[uuid.UUID] | None = None
         self._property_group_type = property_group_type
 
         parent.add_children([self])
 
-        for attr, item in kwargs.items():
-            try:
-                if attr in self._attribute_map:
-                    attr = self._attribute_map[attr]
-                setattr(self, attr, item)
-            except AttributeError:
-                continue
+        map_attributes(self, **kwargs)
 
         self.parent.workspace.register(self)
 
     def add_properties(self, data: Data | list[Data | uuid.UUID] | uuid.UUID):
         """
         Remove data from the properties.
         """
@@ -233,23 +228,24 @@
         if isinstance(data, (Data, uuid.UUID)):
             data = [data]
 
         if self._properties is None:
             return
 
         for elem in data:
-            if isinstance(elem, uuid.UUID):
-                entity = self.parent.get_entity(elem)[0]
-            elif isinstance(elem, Data) and elem in self.parent.children:
-                entity = elem
-            else:
-                continue
 
-            if entity is not None and entity.uid in self._properties:
-                self._properties.remove(entity.uid)
+            if isinstance(elem, Data):
+                elem = elem.uid
+
+            if elem in self._properties:
+                self._properties.remove(elem)
+
+        if len(self._properties) == 0:
+            self.parent.workspace.remove_entity(self)
+            return
 
         self.parent.workspace.add_or_update_property_group(self)
 
     @property
     def uid(self) -> uuid.UUID:
         """
         :obj:`uuid.UUID` Unique identifier
```

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/root_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/root_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/simpeg_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/simpeg_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/groups/survey_group.py` & `geoh5py-0.9.0a3/geoh5py/groups/survey_group.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/io/__init__.py` & `geoh5py-0.9.0a3/geoh5py/io/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/io/h5_reader.py` & `geoh5py-0.9.0a3/geoh5py/io/h5_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         -------
         attributes: :obj:`dict` of attributes for the :obj:`~geoh5py.shared.entity.Entity`
         type_attributes: :obj:`dict` of attributes for the :obj:`~geoh5py.shared.entity.EntityType`
         property_groups: :obj:`dict` of data :obj:`uuid.UUID`
         """
         with fetch_h5_handle(file) as h5file:
             name = list(h5file)[0]
+
             entity_type = cls.format_type_string(entity_type)
 
             if entity_type == "Root":
                 entity = h5file[name].get(entity_type)
             else:
                 entity = h5file[name][entity_type].get(as_str_if_uuid(uid))
 
@@ -177,26 +178,31 @@
             entity_type = cls.format_type_string(entity_type)
             label = KEY_MAP.get(label, label)
 
             try:
                 group = h5file[name][entity_type][as_str_if_uuid(uid)][
                     "Concatenated Data"
                 ]
-                if label not in group["Index"]:
+                indices = group["Index"].get(label.replace("/", "\u2044"))
+                if indices is None:
                     return None
 
-                if label in group["Data"]:
-                    attribute = group["Data"][label][:]
-                else:
-                    attribute = group[label][:]
+                array = group["Data"].get(label.replace("/", "\u2044"))
+                if array is None:
+                    array = group.get(label.replace("/", "\u2044"))
+
+                attribute = array[:]
 
                 if attribute.dtype in [float, "float64", "float32"]:
                     attribute[attribute == FLOAT_NDV] = np.nan
 
-                return attribute, group["Index"][label][:]
+                if attribute.dtype == object and isinstance(attribute[0], bytes):
+                    attribute = np.char.decode(attribute.astype(np.bytes_), "UTF-8")
+
+                return attribute, indices[:]
 
             except KeyError:
                 return None
 
     @classmethod
     def fetch_concatenated_attributes(
         cls,
```

### Comparing `geoh5py-0.9.0a2/geoh5py/io/h5_writer.py` & `geoh5py-0.9.0a3/geoh5py/io/h5_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,25 +275,26 @@
                 del attr_handle[name]
                 entity.workspace.repack = True
             except KeyError:
                 pass
 
             dict_values = getattr(entity, attribute)
 
-            if channel in dict_values:
+            if channel in dict_values and len(dict_values[channel]) > 0:
+
                 values = dict_values[channel].copy()
 
-                if isinstance(values, np.ndarray) and values.dtype in (
-                    np.float64,
-                    np.float32,
-                ):
-                    values[np.isnan(values)] = FLOAT_NDV
-                    values = values.astype(np.float32)
-                if np.issubdtype(values.dtype, np.str_):
-                    values = values.astype(h5py.special_dtype(vlen=str))
+                if isinstance(values, np.ndarray):
+
+                    if np.issubdtype(values.dtype, np.floating):
+                        values[np.isnan(values)] = FLOAT_NDV
+                        values = values.astype(np.float32)
+
+                    if np.issubdtype(values.dtype, np.str_):
+                        values = values.astype(h5py.special_dtype(vlen=str))
 
                 attr_handle.create_dataset(
                     name,
                     data=values,
                     compression="gzip",
                     compression_opts=9,
                 )
@@ -535,15 +536,19 @@
 
             try:
                 del entity_handle[KEY_MAP[attribute]]
                 entity.workspace.repack = True
             except KeyError:
                 pass
 
+            if isinstance(values, np.ndarray) and np.issubdtype(values.dtype, np.str_):
+                values = values.astype(h5py.special_dtype(vlen=str))
+
             if values is not None:
+
                 entity_handle.create_dataset(
                     KEY_MAP[attribute],
                     data=values,
                     compression="gzip",
                     compression_opts=9,
                     **kwargs,
                 )
@@ -633,15 +638,15 @@
                 if isinstance(entity, BooleanData):
                     out_values = np.round(out_values).astype("int8")
 
                 elif isinstance(entity, IntegerData):
                     out_values = np.round(out_values).astype("int32")
 
                 elif isinstance(entity, TextData) and not isinstance(values[0], bytes):
-                    out_values = [val.encode() for val in values]
+                    out_values = np.char.encode(values, encoding="utf-8").astype("O")
 
                 if getattr(entity, "ndv", None) is not None:
                     out_values[np.isnan(out_values)] = entity.ndv
 
                 entity_handle.create_dataset(
                     name_map,
                     data=out_values,
```

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/__init__.py` & `geoh5py-0.9.0a3/geoh5py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/block_model.py` & `geoh5py-0.9.0a3/geoh5py/objects/block_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/cell_object.py` & `geoh5py-0.9.0a3/geoh5py/objects/cell_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/curve.py` & `geoh5py-0.9.0a3/geoh5py/objects/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         :obj:`~geoh5py.objects.curve.Curve.parts` if set by the user.
         """
         if getattr(self, "_cells", None) is None:
             if self._parts is not None:
                 cells = []
                 for part_id in self.unique_parts:
                     ind = np.where(self.parts == part_id)[0]
-                    cells.append(np.c_[ind[:-1], ind[1:]])
+                    cells.append(np.sort(np.c_[ind[:-1], ind[1:]], axis=0))
                 self.cells = np.vstack(cells)
 
             elif self.on_file:
                 self._cells = self.workspace.fetch_array_attribute(self)
 
             if self._cells is None and self.vertices is not None:
                 n_segments = self.vertices.shape[0]
```

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/drape_model.py` & `geoh5py-0.9.0a3/geoh5py/objects/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/drillhole.py` & `geoh5py-0.9.0a3/geoh5py/objects/drillhole.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/geo_image.py` & `geoh5py-0.9.0a3/geoh5py/objects/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/grid2d.py` & `geoh5py-0.9.0a3/geoh5py/objects/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/grid_object.py` & `geoh5py-0.9.0a3/geoh5py/objects/grid_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/integrator.py` & `geoh5py-0.9.0a3/geoh5py/objects/integrator.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/label.py` & `geoh5py-0.9.0a3/geoh5py/objects/label.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/notype_object.py` & `geoh5py-0.9.0a3/geoh5py/objects/notype_object.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/object_base.py` & `geoh5py-0.9.0a3/geoh5py/objects/object_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # pylint: disable=R0904
 
 from __future__ import annotations
 
 import uuid
+import warnings
 from abc import abstractmethod
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from ..data import CommentsData, Data, DataAssociationEnum, DataType, VisualParameters
@@ -61,30 +62,39 @@
             kwargs["name"] = type(self).__name__
 
         super().__init__(**kwargs)
 
         if self.entity_type.name == "Entity":
             self.entity_type.name = type(self).__name__
 
-    def add_children(self, children: list[Entity] | list[PropertyGroup]):
+    def add_children(self, children: list[Entity | PropertyGroup]):
         """
         :param children: Add a list of entities as
             :obj:`~geoh5py.shared.entity.Entity.children`
         """
         property_groups = self._property_groups or []
 
+        prop_group_uids = {prop_group.uid: prop_group for prop_group in property_groups}
+        children_uids = {child.uid: child for child in self._children}
+
         for child in children:
-            if child not in self._children and isinstance(child, (Data, PropertyGroup)):
+            if child.uid not in children_uids and isinstance(
+                child, (Data, PropertyGroup)
+            ):
                 self._children.append(child)
+                if (
+                    isinstance(child, PropertyGroup)
+                    and child.uid not in prop_group_uids
+                ):
+                    property_groups.append(child)
+            else:
+                warnings.warn(f"Child {child} is not valid or already exists.")
 
-            if isinstance(child, PropertyGroup) and child not in property_groups:
-                property_groups.append(child)
-
-            if property_groups:
-                self._property_groups = property_groups
+        if property_groups:
+            self._property_groups = property_groups
 
     def add_comment(self, comment: str, author: str | None = None):
         """
         Add text comment to an object.
 
         :param comment: Text to be added as comment.
         :param author: Name of author or defaults to
@@ -340,15 +350,16 @@
         """
         Find or create a type instance for a given object class.
 
         :param workspace: Target :obj:`~geoh5py.workspace.workspace.Workspace`.
 
         :return: The ObjectType instance for the given object class.
         """
-        return ObjectType.find_or_create(workspace, cls, **kwargs)
+        kwargs["entity_class"] = cls
+        return ObjectType.find_or_create(workspace, **kwargs)
 
     def get_property_group(self, name: uuid.UUID | str) -> list:
         """
         Get a child :obj:`~geoh5py.groups.property_group.PropertyGroup` by name.
         :param name: the reference of the property group to get.
         :return: A list of children Data objects
         """
@@ -424,20 +435,17 @@
 
         :param name: Name of the target child data
 
         :return: A list of children Data objects
         """
         entity_list = []
 
-        for child in self.children:
+        for child in self.get_entity(name):
             if isinstance(child, Data):
-                if (
-                    isinstance(name, uuid.UUID) and child.uid == name
-                ) or child.name == name:
-                    entity_list.append(child)
+                entity_list.append(child)
 
         return entity_list
 
     def get_data_list(self, attribute="name") -> list[str]:
         """
         Get a list of names of all children :obj:`~geoh5py.data.data.Data`.
 
@@ -481,15 +489,15 @@
     @property
     def property_groups(self) -> list[PropertyGroup] | None:
         """
         List of :obj:`~geoh5py.groups.property_group.PropertyGroup`.
         """
         return self._property_groups
 
-    def remove_children(self, children: list[Entity] | list[PropertyGroup]):
+    def remove_children(self, children: list[Entity | PropertyGroup]):
         """
         Remove children from the list of children entities.
 
         :param children: List of entities
 
         .. warning::
             Removing a child entity without re-assigning it to a different
@@ -500,24 +508,21 @@
         if not isinstance(children, list):
             children = [children]
 
         for child in children:
             if child not in self._children:
                 continue
 
-            self._children.remove(child)
-
-            if not self._property_groups:
-                continue
-
-            if isinstance(child, PropertyGroup):
+            if isinstance(child, PropertyGroup) and self._property_groups:
                 self._property_groups.remove(child)
             elif isinstance(child, Data):
                 self.remove_data_from_groups(child)
 
+            self._children.remove(child)
+
         self.workspace.remove_children(self, children)
 
     def remove_children_values(
         self,
         indices: list[int] | np.ndarray,
         association: str,
         clear_cache: bool = False,
```

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/object_type.py` & `geoh5py-0.9.0a3/geoh5py/shared/merging/cell.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,73 +10,58 @@
 #  geoh5py is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
-
 from __future__ import annotations
 
-import uuid
-from typing import TYPE_CHECKING
+import numpy as np
 
-from ..shared import EntityType
+from ...objects import CellObject, Curve, ObjectBase, Surface
+from ...workspace import Workspace
+from .points import PointsMerger
 
-if TYPE_CHECKING:
-    from .. import workspace
 
+class CellMerger(PointsMerger):
+    _type: type = CellObject
 
-class ObjectType(EntityType):
-    """
-    Object type class
-    """
+    @classmethod
+    def create_object(
+        cls, workspace: Workspace, input_entities: list[ObjectBase], **kwargs
+    ) -> CellObject:
+        """
+        Create a new object of type cls._type from a list of input entities.
+        It merges the cells together and create a new object with the merged cells.
 
-    def __init__(self, workspace: workspace.Workspace, **kwargs):
-        assert workspace is not None
-        super().__init__(workspace, **kwargs)
+        :param workspace: The workspace to create the object in.
+        :param input_entities: The list of input entities to merge together.
+        :param kwargs: The kwargs to pass to the object creation.
 
-    @staticmethod
-    def _is_abstract() -> bool:
-        return False
+        :return: The newly created object merged from input_entities.
+        """
+        # create the vertices
+        vertices = np.vstack([input_entity.vertices for input_entity in input_entities])
 
-    @staticmethod
-    def create_custom(workspace: workspace.Workspace) -> ObjectType:
-        """Creates a new instance of ObjectType for an unlisted custom Object type with a
-        new auto-generated UUID.
+        # merge the simplices
+        cells: list = []
+        previous: int = 0
+        for entity in input_entities:
+            temp_cells = entity.cells + previous
+            cells.append(temp_cells)
+            previous = np.nanmax(temp_cells) + 1
 
-        :param workspace: An active Workspace class
-        """
-        return ObjectType(workspace)
+        # create an object of type
+        output = cls._type.create(  # type: ignore
+            workspace, vertices=vertices, cells=np.vstack(cells).tolist(), **kwargs
+        )
 
-    @classmethod
-    def find_or_create(
-        cls, workspace: workspace.Workspace, entity_class, **kwargs
-    ) -> ObjectType:
-        """Find or creates an EntityType with given :obj:`uuid.UUID` that matches the given
-        Group implementation class.
+        return output
 
-        It is expected to have a single instance of EntityType in the Workspace
-        for each concrete Entity class.
 
-        :param workspace: An active Workspace class
-        :param entity_class: An Group implementation class.
+class CurveMerger(CellMerger):
+    _type = Curve
 
-        :return: A new instance of GroupType.
-        """
-        uid = uuid.uuid4()
-        if getattr(entity_class, "default_type_uid", None) is not None:
-            uid = entity_class.default_type_uid()
-            if "ID" in kwargs:
-                kwargs["ID"] = uid
-            else:
-                kwargs["uid"] = uid
-        else:
-            for key, val in kwargs.items():
-                if key.lower() in ["id", "uid"]:
-                    uid = uuid.UUID(val)
-
-        entity_type = cls.find(workspace, uid)
-        if entity_type is not None:
-            return entity_type
 
-        return cls(workspace, **kwargs)
+class SurfaceMerger(CellMerger):
+    _type = Surface
```

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/octree.py` & `geoh5py-0.9.0a3/geoh5py/objects/octree.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,15 +303,18 @@
         """
         return self._u_count
 
     @u_count.setter
     def u_count(self, value: int):
         value = np.int32(value).item()
 
-        if not isinstance(value, (float, np.int32, int)) or np.log2(value) % 1.0 != 0:
+        if (
+            not isinstance(value, (float, np.floating, np.integer, int))
+            or np.log2(value) % 1.0 != 0
+        ):
             raise TypeError("Attribute 'u_count' must be type(int) in power of 2.")
 
         self._centroids = None
 
         self._u_count = np.int32(value).item()
         self.workspace.update_attribute(self, "attributes")
 
@@ -342,15 +345,18 @@
         """
         return self._v_count
 
     @v_count.setter
     def v_count(self, value: int):
         value = np.int32(value).item()
 
-        if not isinstance(value, (float, np.int32, int)) or np.log2(value) % 1.0 != 0:
+        if (
+            not isinstance(value, (float, np.floating, np.integer, int))
+            or np.log2(value) % 1.0 != 0
+        ):
             raise TypeError("Attribute 'v_count' must be type(int) in power of 2.")
         self._centroids = None
         self._v_count = np.int32(value).item()
         self.workspace.update_attribute(self, "attributes")
 
     @property
     def w_cell_size(self) -> float | None:
@@ -379,12 +385,15 @@
         """
         return self._w_count
 
     @w_count.setter
     def w_count(self, value: int):
         value = np.int32(value).item()
 
-        if not isinstance(value, (float, np.int32, int)) or np.log2(value) % 1.0 != 0:
+        if (
+            not isinstance(value, (float, np.floating, np.integer, int))
+            or np.log2(value) % 1.0 != 0
+        ):
             raise TypeError("Attribute 'w_count' must be type(int) in power of 2.")
         self._centroids = None
         self._w_count = np.int32(value).item()
         self.workspace.update_attribute(self, "attributes")
```

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/points.py` & `geoh5py-0.9.0a3/geoh5py/objects/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surface.py` & `geoh5py-0.9.0a3/geoh5py/objects/surface.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/__init__.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/direct_current.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/direct_current.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/__init__.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/airborne_fem.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/airborne_tem.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/airborne_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/base.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/ground_fem.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_fem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/ground_tem.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/ground_tem.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/magnetotellurics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/electromagnetics/tipper.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/electromagnetics/tipper.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/objects/surveys/magnetics.py` & `geoh5py-0.9.0a3/geoh5py/objects/surveys/magnetics.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/__init__.py` & `geoh5py-0.9.0a3/geoh5py/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/__init__.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/concatenated.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenated.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/concatenator.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/concatenator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from ...groups import Group
 from ..entity import Entity
 from ..utils import INV_KEY_MAP, KEY_MAP, as_str_if_utf8_bytes, as_str_if_uuid, str2uuid
 from .concatenated import Concatenated
 from .data import ConcatenatedData
 from .drillholes_group_table import DrillholesGroupTable
 from .object import ConcatenatedObject
+from .property_group import ConcatenatedPropertyGroup
 
 if TYPE_CHECKING:
     from ...groups import GroupType
 
 
 PROPERTY_KWARGS = {
     "trace": {"maxshape": (None,)},
@@ -165,14 +166,15 @@
     def concatenated_attributes(self, concatenated_attributes: dict):
         if not isinstance(concatenated_attributes, (dict, type(None))):
             raise ValueError(
                 "Input 'concatenated_attributes' must be a dictionary or None"
             )
 
         self._concatenated_attributes = concatenated_attributes
+        self.workspace.update_attribute(self, "concatenated_attributes")
 
     @property
     def concatenated_object_ids(self) -> list[bytes] | None:
         """Dictionary of concatenated objects and data concatenated_object_ids."""
         if getattr(self, "_concatenated_object_ids", None) is None:
             concatenated_object_ids = self.workspace.fetch_array_attribute(
                 self, "concatenated_object_ids"
@@ -254,14 +256,17 @@
                     )
                     data_type = DataType.find_or_create(
                         new_entity.workspace, **attr_type
                     )
                     new_entity.workspace.save_entity_type(data_type)
 
             new_entity.workspace.fetch_children(new_entity)
+            for child in self.children:
+                if not isinstance(child, Concatenated):
+                    child.copy(parent=new_entity)
         else:
             for child in self.children:
                 child.copy(
                     parent=new_entity, clear_cache=clear_cache, omit_list=["_uid"]
                 )
 
         return new_entity
@@ -449,41 +454,75 @@
             )
 
             if property_groups_ids is not None:
                 self._property_group_ids = property_groups_ids[0].tolist()
 
         return self._property_group_ids
 
-    def remove_entity(self, entity: Concatenated):
+    def remove_children(self, children: list | Concatenated):
+        """
+        Remove children from object.
+
+        This method calls the ObjectBase parent class to remove children from the
+        object children, but also deletes the children from the workspace.
+
+        :param children: List of children to remove.
+        """
+        if not isinstance(children, list):
+            children = [children]
+
+        for child in children:
+            if child not in self._children:
+                continue
+
+            self.remove_entity(child)
+
+    def remove_entity(self, entity: Concatenated | ConcatenatedPropertyGroup):
         """Remove a concatenated entity."""
 
+        parent = entity.parent
         if isinstance(entity, ConcatenatedData):
             # Remove the rows of data and index
             self.update_array_attribute(entity, entity.name, remove=True)
+            # Remove the data from the group
+
+            if entity.property_group is not None:
+                entity.property_group.remove_properties([entity])
+
             # Remove from the concatenated Attributes
-            parent_attr = self.get_concatenated_attributes(entity.parent.uid)
+            parent_attr = self.get_concatenated_attributes(parent.uid)
             name = entity.name
             del parent_attr[f"Property:{name}"]
-        elif isinstance(entity, ConcatenatedObject):
-            if entity.property_groups is not None:  # type: ignore
-                self.update_array_attribute(entity, "property_groups", remove=True)
 
+        elif isinstance(entity, ConcatenatedObject):
+            # First remove the children
+            entity.remove_children(entity.children.copy())
             object_ids = self.concatenated_object_ids
 
             if object_ids is not None:
                 object_ids.remove(as_str_if_uuid(entity.uid).encode())
                 self.concatenated_object_ids = object_ids
 
-        if self.concatenated_attributes is not None:
+        elif isinstance(entity, ConcatenatedPropertyGroup):
+            # Remove all data within the group
+            if entity.properties is not None and len(entity.properties) > 0:
+                data = [entity.parent.get_entity(uid)[0] for uid in entity.properties]
+                entity.parent.remove_children(data)
+
+            self.update_array_attribute(parent, "property_groups", remove=True)
+
+        if (
+            self.concatenated_attributes is not None
+            and self.attributes_keys is not None
+        ):
             attr_handle = self.get_concatenated_attributes(entity.uid)
+            self.attributes_keys.remove(as_str_if_uuid(entity.uid))
             self.concatenated_attributes["Attributes"].remove(attr_handle)
             self.workspace.repack = True
 
-        entity.parent._children.remove(entity)  # pylint: disable=protected-access
-
     def save_attribute(self, field: str):
         """
         Save a concatenated attribute.
 
         :param field: Name of the attribute
         """
         field = INV_KEY_MAP.get(field, field)
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/data.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/data.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/drillhole.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillhole.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,15 @@
                         f"assign to a new property group."
                     )
                 return out_group
 
         else:
             out_group = property_group
 
-        _ = getattr(self, "add_data")(
+        self.add_data(
             {
                 f"DEPTH{label}": {
                     "association": "DEPTH",
                     "values": depth,
                     "entity_type": {"primitive_type": "FLOAT"},
                     "parent": self,
                     "allow_move": False,
@@ -346,15 +346,15 @@
                     f"Input values with shape({values.shape[0]}) "
                     f"do not match the from-to intervals of the group '{out_group}' "
                     f"with shape({out_group.from_.values.shape[0]}). Check values or "
                     f"assign to a new property group."
                 )
             return out_group
 
-        _ = getattr(self, "add_data")(
+        self.add_data(
             {
                 f"FROM{label}": {
                     "association": "DEPTH",
                     "values": from_to[:, 0],
                     "entity_type": {"primitive_type": "FLOAT"},
                     "parent": self,
                     "allow_move": False,
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/drillholes_group_table.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/drillholes_group_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from abc import ABC
 from typing import TYPE_CHECKING, Any
 from uuid import UUID
 
 import numpy as np
 
+from ...data import DataType
 from ..utils import str2uuid, to_tuple
 from .property_group import ConcatenatedPropertyGroup
 
 if TYPE_CHECKING:
     from .concatenator import Concatenator
     from .data import ConcatenatedData
     from .drillhole import ConcatenatedDrillhole
@@ -181,37 +182,39 @@
             else:
                 padded_array = array
             padded_arrays.append(padded_array)
 
         return padded_arrays
 
     def add_values_to_property_group(
-        self, name: str, values: np.ndarray, value_map: dict[int, str] | None = None
+        self, name: str, values: np.ndarray, data_type: DataType | None = None
     ):
         """
         Push the values to each drillhole of the property group based on association.
 
         :param name: The name of the data to push.
         :param values: The values to push.
-        :param value_map: The value map associating the index and the description
-            in the case of referenced data
+        :param data_type: The data type associated to description;
+            useful especially for referenced data.
         """
         if not isinstance(name, str) or name in self.parent.data:
             raise KeyError("The name must be a string not present in data.")
 
         # ensure the length of the values is the same as the length of the template
         if values.shape != self.parent.data[self.association[0]].shape:
             raise ValueError(
                 "The length of the values must be the same as the association "
                 f"({self.parent.data[self.association[0]].shape})."
             )
 
-        attributes = {}
-        if isinstance(value_map, dict):
-            attributes.update({"type": "referenced", "value_map": value_map})
+        if not isinstance(data_type, DataType):
+            primitive_type = DataType.validate_data_type(
+                self.parent.workspace, {"values": values}
+            )["primitive_type"]
+            data_type = DataType(self.parent.workspace, primitive_type, name=name)
 
         for drillhole_uid, indices in self.index_by_drillhole.items():
             # get the drillhole
             drillhole: ConcatenatedDrillhole = self.parent.workspace.get_entity(  # type: ignore
                 str2uuid(drillhole_uid)
             )[
                 0
@@ -225,15 +228,15 @@
                             "values": values[
                                 indices[self.association[0]][0] : indices[
                                     self.association[0]
                                 ][0]
                                 + indices[self.association[0]][1]
                             ]
                         },
-                        **attributes,
+                        "entity_type": data_type,
                     },
                 },
                 property_group=self.property_groups[drillhole.uid],
             )
 
         self._update_drillholes_group_table(name)
 
@@ -412,17 +415,18 @@
     def _update_drillholes_group_table(self, name):
         """
         Update the drillholes group table with a new property group.
 
         :param name: The name of the property group to update.
         """
         self.parent.update_data_index()
+        self.parent.workspace.update_attribute(self.parent, "concatenated_attributes")
         self._property_groups = self._get_property_groups(self.parent, self.name)
 
         if self._properties is not None:
             self._properties += (name,)
         else:
-            self._properties = (name,)
+            self._properties = ((name,),)
 
         if self._index_by_drillhole is not None:
             for value in self._index_by_drillhole.values():
                 value[name] = value[self.association[0]]
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/object.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 import uuid
-import warnings
 from typing import TYPE_CHECKING
 
 from ...data import Data
 from ...objects import ObjectBase
 from .concatenated import Concatenated
 from .data import ConcatenatedData
 from .property_group import ConcatenatedPropertyGroup
 
 if TYPE_CHECKING:
+    from ..entity import Entity
     from .concatenator import Concatenator
 
 
 class ConcatenatedObject(Concatenated, ObjectBase):
     _parent: Concatenator
 
     def __init__(self, entity_type, **kwargs):
@@ -41,39 +41,14 @@
                 "of type Concatenator."
             )
 
         self._property_groups: list | None = None
 
         super().__init__(entity_type, **kwargs)
 
-    def add_children(
-        self,
-        children,
-    ):
-        """
-        :param children: Add a list of entities as
-            :obj:`~geoh5py.shared.entity.Entity.children`
-        """
-        property_groups = self._property_groups or []
-
-        for child in children:
-            if child not in self._children and isinstance(
-                child, (ConcatenatedData, ConcatenatedPropertyGroup)
-            ):
-                self._children.append(child)
-
-            if (
-                isinstance(child, ConcatenatedPropertyGroup)
-                and child not in property_groups
-            ):
-                property_groups.append(child)
-
-            if property_groups:
-                self._property_groups = property_groups
-
     def create_property_group(
         self, name=None, on_file=False, uid=None, **kwargs
     ) -> ConcatenatedPropertyGroup:
         """
         Create a new :obj:`~geoh5py.groups.property_group.PropertyGroup`.
 
         :param name: Name of the property group.
@@ -94,52 +69,56 @@
 
         prop_group = ConcatenatedPropertyGroup(
             self, name=name, on_file=on_file, **kwargs
         )
 
         return prop_group
 
-    def get_data(self, name: str | uuid.UUID) -> list[Data]:
+    def _fetch_concatenated_children(self):
         """
-        Generic function to get data values from object.
+        Method to generate concatenated children.
         """
-        entity_list = []
-        attr = self.concatenator.get_concatenated_attributes(
-            getattr(self, "uid")
-        ).copy()
+        attr = self.concatenator.get_concatenated_attributes(self.uid).copy()
 
         for key, value in attr.items():
             if "Property:" in key:
                 child_data = self.workspace.get_entity(uuid.UUID(value))[0]
                 if child_data is None:
                     attributes: dict = self.concatenator.get_concatenated_attributes(
                         value
                     ).copy()
                     attributes["parent"] = self
                     self.workspace.create_from_concatenation(attributes)
                 elif not isinstance(child_data, ConcatenatedPropertyGroup):
                     self.add_children([child_data])
-                else:
-                    warnings.warn(f"Failed: '{name}' is a property group, not a Data.")
 
-        for child in getattr(self, "children"):
-            if (
-                isinstance(name, str) and hasattr(child, "name") and child.name == name
-            ) or (
-                isinstance(name, uuid.UUID)
-                and hasattr(child, "uid")
-                and child.uid == name
-            ):
-                entity_list.append(child)
+    def get_entity(self, name: str | uuid.UUID) -> list[Entity | None]:
+        """
+        Get a child :obj:`~geoh5py.data.data.Data` by name.
+
+        :param name: Name of the target child data
+        :param entity_type: Sub-select entities based on type.
+        :return: A list of children Data objects
+        """
+        if not any(child for child in self.children if isinstance(child, Data)):
+            self._fetch_concatenated_children()
+
+        if isinstance(name, uuid.UUID):
+            entity_list = [child for child in self.children if child.uid == name]
+        else:
+            entity_list = [child for child in self.children if child.name == name]
+
+        if not entity_list:
+            return [None]
 
         return entity_list
 
     def get_data_list(self, attribute="name"):
         """
-        Get list of data names.
+        Lazy loading of data names from concatenated attributes.
         """
         data_list = [
             attr.replace("Property:", "").replace("\u2044", "/")
             for attr in self.concatenator.get_concatenated_attributes(self.uid)
             if "Property:" in attr
         ]
 
@@ -178,7 +157,32 @@
                 if isinstance(child, ConcatenatedPropertyGroup)
             ]
 
             if len(property_groups) > 0:
                 self._property_groups = property_groups
 
         return self._property_groups
+
+    def remove_children(
+        self, children: list | Concatenated | ConcatenatedPropertyGroup
+    ):
+        """
+        Remove children from object.
+
+        This method calls the ObjectBase parent class to remove children from the
+        object children, but also deletes the children from the workspace.
+
+        :param children: List of children to remove.
+        """
+        if not isinstance(children, list):
+            children = [children]
+
+        for child in children:
+            if child not in self._children:
+                continue
+
+            self.concatenator.remove_entity(child)
+
+            if isinstance(child, ConcatenatedPropertyGroup) and self._property_groups:
+                self._property_groups.remove(child)
+
+            self._children.remove(child)
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/concatenation/property_group.py` & `geoh5py-0.9.0a3/geoh5py/shared/concatenation/property_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,31 +13,40 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
+import uuid
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from geoh5py.data import Data
 from geoh5py.groups import PropertyGroup
 
 if TYPE_CHECKING:
+    from .concatenator import Concatenator
     from .object import ConcatenatedObject
 
 
 class ConcatenatedPropertyGroup(PropertyGroup):
     _parent: ConcatenatedObject
 
     def __init__(self, parent: ConcatenatedObject, **kwargs):
         super().__init__(parent, **kwargs)
 
+    @property
+    def concatenator(self) -> Concatenator:
+        """
+        Parental Concatenator entity.
+        """
+        return self._parent.concatenator
+
     def is_collocated(
         self,
         locations: np.ndarray,
         collocation_distance: float,
     ) -> bool:
         """
         True if locations are collocated with property group.
@@ -71,48 +80,48 @@
     @property
     def depth_(self):
         if self.properties is None or len(self.properties) < 1:
             return None
 
         data = self.parent.get_data(  # pylint: disable=no-value-for-parameter
             self.properties[0]
-        )[0]
+        )
 
-        if isinstance(data, Data) and "depth" in data.name.lower():
-            return data
+        if any(data) and isinstance(data[0], Data) and "depth" in data[0].name.lower():
+            return data[0]
 
         return None
 
     @property
     def from_(self):
         """Return the data entities defined the 'from' depth intervals."""
         if self.properties is None or len(self.properties) < 1:
             return None
 
         data = self.parent.get_data(  # pylint: disable=no-value-for-parameter
             self.properties[0]
-        )[0]
+        )
 
-        if isinstance(data, Data) and "from" in data.name.lower():
-            return data
+        if any(data) and isinstance(data[0], Data) and "from" in data[0].name.lower():
+            return data[0]
 
         return None
 
     @property
     def to_(self):
         """Return the data entities defined the 'to' depth intervals."""
         if self.properties is None or len(self.properties) < 2:
             return None
 
         data = self.parent.get_data(  # pylint: disable=no-value-for-parameter
             self.properties[1]
-        )[0]
+        )
 
-        if isinstance(data, Data) and "to" in data.name.lower():
-            return data
+        if any(data) and isinstance(data[0], Data) and "to" in data[0].name.lower():
+            return data[0]
 
         return None
 
     @property
     def parent(self) -> ConcatenatedObject:
         return self._parent
 
@@ -126,7 +135,33 @@
                 "The 'parent' of a concatenated data must have an 'add_children' method."
             )
 
         parent.add_children([self])
         self._parent: ConcatenatedObject = parent
 
         parent.workspace.add_or_update_property_group(self)
+
+    def remove_properties(self, data: Data | list[Data | uuid.UUID] | uuid.UUID):
+        """
+        Remove data from the properties.
+
+        The property group is removed if only the depth or from/to data are left.
+        """
+        super().remove_properties(data)
+
+        if (
+            self._properties is not None
+            and len(self._properties) == 1
+            and self.depth_ is not None
+        ):
+            self.depth_.allow_delete = True
+            self.parent.remove_children(self)
+
+        elif (
+            self._properties is not None
+            and len(self._properties) == 2
+            and self.from_ is not None
+            and self.to_ is not None
+        ):
+            self.from_.allow_delete = True
+            self.to_.allow_delete = True
+            self.parent.remove_children(self)
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/conversion/__init__.py` & `geoh5py-0.9.0a3/geoh5py/shared/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/conversion/base.py` & `geoh5py-0.9.0a3/geoh5py/shared/conversion/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/conversion/geo_image.py` & `geoh5py-0.9.0a3/geoh5py/shared/conversion/geo_image.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/conversion/grid2d.py` & `geoh5py-0.9.0a3/geoh5py/shared/conversion/grid2d.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/entity.py` & `geoh5py-0.9.0a3/geoh5py/shared/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import uuid
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from geoh5py.shared.utils import str2uuid
+from ..shared.utils import map_attributes, str2uuid
 
 if TYPE_CHECKING:
     from .. import shared
     from ..workspace import Workspace
 
 DEFAULT_CRS = {"Code": "Unknown", "Name": "Unknown"}
 
@@ -64,21 +64,15 @@
         self._metadata: dict | None = None
         self._name = name
         self._on_file = False
         self._parent: Entity | None = None
         self._partially_hidden = False
         self._public = True
 
-        for attr, item in kwargs.items():
-            try:
-                if attr in self._attribute_map:
-                    attr = self._attribute_map[attr]
-                setattr(self, attr, item)
-            except AttributeError:
-                continue
+        map_attributes(self, **kwargs)
 
         self.workspace.register(self)
 
     @property
     def allow_delete(self) -> bool:
         """
         :obj:`bool` Entity can be deleted from the workspace.
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/entity_container.py` & `geoh5py-0.9.0a3/geoh5py/shared/entity_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,30 +46,14 @@
         self._uid = (
             str2uuid(uid) if isinstance(str2uuid(uid), uuid.UUID) else uuid.uuid4()
         )
         self._children: list = []
 
         super().__init__(uid, name, **kwargs)
 
-    def add_children(self, children: list[Entity]):
-        """
-        :param children: Add a list of entities as
-            :obj:`~geoh5py.shared.entity.Entity.children`
-        """
-        if not isinstance(children, list):
-            children = [children]
-
-        for child in children:
-            if child not in self._children:
-                if not isinstance(child, Entity):
-                    raise TypeError(
-                        f"Child must be an instance of Entity, not {type(child)}"
-                    )
-                self._children.append(child)
-
     def add_file(self, file: str):
         """
         Add a file to the object or group stored as bytes on a FilenameData
 
         :param file: File name with path to import.
         """
         if not Path(file).is_file():
@@ -218,15 +202,15 @@
                 if (obj is not None) and (obj.uid in children_uid)
             ]
         elif isinstance(value, uuid.UUID):
             uid = [value]
 
         return uid
 
-    def remove_children(self, children: list[shared.Entity] | list[PropertyGroup]):
+    def remove_children(self, children: list[shared.Entity | PropertyGroup]):
         """
         Remove children from the list of children entities.
 
         :param children: List of entities
 
         .. warning::
             Removing a child entity without re-assigning it to a different
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/exceptions.py` & `geoh5py-0.9.0a3/geoh5py/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/merging/__init__.py` & `geoh5py-0.9.0a3/geoh5py/shared/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/merging/base.py` & `geoh5py-0.9.0a3/geoh5py/shared/merging/base.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/merging/drape_model.py` & `geoh5py-0.9.0a3/geoh5py/shared/merging/drape_model.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/merging/points.py` & `geoh5py-0.9.0a3/geoh5py/shared/merging/points.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/utils.py` & `geoh5py-0.9.0a3/geoh5py/shared/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -308,21 +308,24 @@
 def compare_entities(
     object_a, object_b, ignore: list[str] | None = None, decimal: int = 6
 ) -> None:
     if isinstance(object_a, bytes):
         compare_bytes(object_a, object_b)
         return
 
-    base_ignore = ["_workspace", "_children", "_visual_parameters"]
+    base_ignore = ["_workspace", "_children", "_visual_parameters", "_entity_class"]
     ignore_list = base_ignore + ignore if ignore else base_ignore
 
     for attr in [k for k in object_a.__dict__.keys() if k not in ignore_list]:
         if isinstance(getattr(object_a, attr[1:]), ABC):
             compare_entities(
-                getattr(object_a, attr[1:]), getattr(object_b, attr[1:]), ignore=ignore
+                getattr(object_a, attr[1:]),
+                getattr(object_b, attr[1:]),
+                ignore=ignore,
+                decimal=decimal,
             )
         else:
             if isinstance(getattr(object_a, attr[1:]), np.ndarray):
                 compare_arrays(object_a, object_b, attr[1:], decimal=decimal)
             elif isinstance(getattr(object_a, attr[1:]), float):
                 compare_floats(object_a, object_b, attr[1:], decimal=decimal)
             elif isinstance(getattr(object_a, attr[1:]), list):
@@ -406,17 +409,14 @@
 
 
 def str2uuid(value: Any) -> UUID | Any:
     """Convert string to UUID"""
     if isinstance(value, bytes):
         value = value.decode("utf-8")
 
-    if isinstance(value, str) and not (value.startswith("{") and value.endswith("}")):
-        value = value.strip("{}")
-
     if is_uuid(value):
         # TODO insert validation
         return UUID(str(value))
     return value
 
 
 def as_str_if_uuid(value: UUID | Any) -> str | Any:
@@ -434,14 +434,32 @@
 def as_str_if_utf8_bytes(value) -> str:
     """Convert bytes to string"""
     if isinstance(value, bytes):
         value = value.decode("utf-8")
     return value
 
 
+def ensure_uuid(value: UUID | str) -> UUID:
+    """
+    Ensure that the value is a UUID.
+
+    If not, it raises a type error.
+
+    :param value: The value to ensure is a UUID.
+
+    :return: The verified UUID.
+    """
+    value = str2uuid(value)
+
+    if not isinstance(value, UUID):
+        raise TypeError(f"Value {value} is not a UUID but a {type(value)}.")
+
+    return value
+
+
 def dict_mapper(val, string_funcs: list[Callable], *args, omit: dict | None = None):
     """
     Recursion through nested dictionaries and applies mapping functions to values.
 
     :param val: Value (could be another dictionary) to apply transform functions.
     :param string_funcs: Functions to apply on values within the input dictionary.
     :param omit: Dictionary of functions to omit.
@@ -601,14 +619,34 @@
 
     # Rotate back the points to initial orientation
     points = xy_rotation_matrix(rotation) @ points
 
     return points.T
 
 
+def map_attributes(object_, **kwargs):
+    """
+    Map attributes to an object. The object must have an '_attribute_map'.
+
+    :param object_: The object to map the attributes to.
+    :param kwargs: The kwargs to map to the object.
+    """
+    if not hasattr(object_, "_attribute_map"):
+        warnings.warn(f"Object {object_} does not have an attribute map.")
+        return
+
+    for attr, item in kwargs.items():
+        try:
+            if attr in getattr(object_, "_attribute_map"):
+                attr = getattr(object_, "_attribute_map")[attr]
+            setattr(object_, attr, item)
+        except AttributeError:
+            continue
+
+
 def to_tuple(value: Any) -> tuple:
     """
     Convert value to a tuple.
 
     :param value: The value to convert.
 
     :return: A tuple
```

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/validators.py` & `geoh5py-0.9.0a3/geoh5py/shared/validators.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/shared/weakref_utils.py` & `geoh5py-0.9.0a3/geoh5py/shared/weakref_utils.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/__init__.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/constants.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/constants.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/descriptors.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/descriptors.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/enforcers.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/enforcers.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/forms.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/forms.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/input_file.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/input_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,16 +103,22 @@
         self.validations = validations
         self.promotion = promotion
         self.ui_json = ui_json
         self.data = data
 
     @property
     def data(self) -> dict[str, Any] | None:
+        """
+        Dictionary representing the input data for the ui.json file.
+        """
         if self._data is None and self.ui_json is not None:
+            original = self.validation_options.get("update_enabled", True)
+            self.validation_options["update_enabled"] = False
             self.data = flatten(self.ui_json)
+            self.validation_options["update_enabled"] = original
 
         return self._data
 
     @data.setter
     def data(self, value: dict[str, Any] | None):
         if value is not None:
             if not isinstance(value, dict):
@@ -268,15 +274,14 @@
                     else:
                         self.ui_json[key]["isValue"] = True
 
                 if (value is None) and (not self.ui_json[key].get("enabled", False)):
                     continue
 
                 self.ui_json[key][member] = value
-
             else:
                 self.ui_json[key] = value
 
     @property
     def validate(self):
         """Option to run validations."""
         return self._validate
@@ -299,15 +304,15 @@
             If True, the enabled status of the ui_json will be updated based on the
             value provided. Default is True.
         - ignore_list: tuple
             List of keys to ignore when validating the ui_json. Default is empty tuple.
 
         """
         if self._validation_options is None:
-            return {
+            self._validation_options = {
                 "update_enabled": True,
                 "ignore_list": (),
             }
 
         return self._validation_options
 
     @validation_options.setter
```

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/parameters.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/parameters.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/templates.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  along with geoh5py.  If not, see <https://www.gnu.org/licenses/>.
 
 # pylint: disable=R0913
 
 from __future__ import annotations
 
 import inspect
+import uuid
 from uuid import UUID
 
 from .. import groups, objects
 from ..shared import Entity
 
 known_object_types = [
     member.default_type_uid()
@@ -444,7 +445,62 @@
         "enabled": enabled,
         "tooltip": tooltip,
     }
 
     if optional is not None:
         form.update(optional_parameter(optional))
     return form
+
+
+def range_label_template(
+    main: bool = True,
+    label: str = "Range",
+    allow_complement: bool = False,
+    is_complement: bool = False,
+    parent: str = "",
+    property_: str | uuid.UUID = "",
+    association: str = "Vertex",
+    data_type: list[str] | str = "Float",
+    value: list[float | int] | None = None,
+    range_label: str = "Values",
+    enabled: bool = True,
+    optional: str | None = None,
+) -> dict:
+    """
+    Template for range label.
+
+    Or it is a multiselect data on a property group if referenced data.
+    Or they are 2 values, an upper and lower bound as float values.
+    In the second scenario, is_complement allows to invert the range.
+
+    :param main: Show form in main.
+    :param label: The label identifier.
+    :param allow_complement: If users can invert the range.
+    :param is_complement: If the range is inverted.
+    :param parent: The parent object.
+    :param property_: The property uid associated with the range.
+    :param association: The association type.
+    :param data_type: The data type of the range.
+    :param value: The value of the range.
+    :param range_label: The label of the range.
+    :param enabled: The state of the form.
+    :param optional: Make optional if not None. Initial state provided by not None.
+
+    :return: The form dictionary.
+    """
+    form = {
+        "main": main,
+        "label": label,
+        "allowComplement": allow_complement,
+        "isComplement": is_complement,
+        "parent": parent,
+        "property": property_,
+        "association": association,
+        "dataType": data_type,
+        "value": value,
+        "rangeLabel": range_label,
+        "enabled": enabled,
+    }
+    if optional is not None:
+        form.update(optional_parameter(optional))
+
+    return form
```

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/ui_json.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/ui_json.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/utils.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,20 +38,15 @@
     for name, value in ui_json.items():
         if isinstance(value, dict):
             if is_form(value):
                 field = "value" if truth(ui_json, name, "isValue") else "property"
                 if not truth(ui_json, name, "enabled"):
                     data[name] = None
                 else:
-                    temp_value = value[field]
-
-                    if value.get("groupValue"):
-                        temp_value = {"group": value["groupValue"], "value": temp_value}
-
-                    data[name] = temp_value
+                    data[name] = value[field]
         else:
             data[name] = value
 
     return data
 
 
 def collect(ui_json: dict[str, dict], member: str, value: Any = None) -> dict[str, Any]:
@@ -192,16 +187,17 @@
     is_group_optional = False
     group_name = ui_json[parameter].get("group", False)
     if group_name:
         group = collect(ui_json, "group", group_name)
         parameters = find_all(group, "groupOptional")
         if parameters:
             is_group_optional = True
-            for form in group.values():
-                form["enabled"] = value
+            if parameters[0] == parameter:
+                for form in group.values():
+                    form["enabled"] = value
 
     if not is_group_optional and "dependency" in ui_json[parameter]:
         is_group_optional = not dependency_requires_value(ui_json, parameter)
 
     if (not value) and not (
         ui_json[parameter].get("optional", False) or is_group_optional
     ):
```

### Comparing `geoh5py-0.9.0a2/geoh5py/ui_json/validation.py` & `geoh5py-0.9.0a3/geoh5py/ui_json/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,21 @@
                 try:
                     validations[key]["association"] = item["parent"]
                     validations[key]["uuid"] = None
                 except KeyError as error:
                     warn(
                         f"Failed to set association for {key}. {error}",
                     )
+            elif "rangeLabel" in item:
+                validations[key] = {
+                    "types": [list],
+                }
             elif "groupValue" in item and "value" in item:
                 validations[key] = {
-                    "types": [dict],
+                    "types": [list],
                 }
             elif "choiceList" in item:
                 validations[key] = {
                     "types": [str],
                     "values": item["choiceList"],
                 }
             elif "fileType" in item:
@@ -255,15 +259,14 @@
             val = str(validator.validator_type)
             if (
                 val not in validations
                 or (val == "required" and self.ignore_requirements)
                 or name in self.ignore_list
             ):
                 continue
-
             self.validators[val](name, value, validations[val])
 
     def validate_data(self, data: dict[str, Any]) -> None:
         """
         Calls validate method on ui.json data structure for cross-dependencies.
 
         Individual key, value pairs are validated for expected type.
```

### Comparing `geoh5py-0.9.0a2/geoh5py/workspace/__init__.py` & `geoh5py-0.9.0a3/geoh5py/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/geoh5py/workspace/workspace.py` & `geoh5py-0.9.0a3/geoh5py/workspace/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             for entity in self.groups:
                 if isinstance(entity, Concatenator) and self.repack:
                     self.update_attribute(entity, "concatenated_attributes")
 
             self._io_call(H5Writer.save_entity, self.root, add_children=True, mode="r+")
 
         self.geoh5.close()
-        self._data = {}
+
         if (
             self.repack
             and not isinstance(self._h5file, BytesIO)
             and self._h5file is not None
         ):
             temp_file = Path(tempfile.gettempdir()) / Path(self._h5file).name
             try:
@@ -343,32 +343,34 @@
         """Create a named blank workspace and save to disk."""
         return cls(**kwargs).save_as(path)
 
     def create_from_concatenation(self, attributes):
         if "Name" in attributes:
             attributes["Name"] = attributes["Name"].replace("\u2044", "/")
 
+        recovered_entity = None
+
         if "Object Type ID" in attributes:
             recovered_entity = self.create_entity(
                 ObjectBase,
                 save_on_creation=False,
                 **{
                     "entity": attributes,
-                    "entity_type": {"uid": attributes["Object Type ID"]},
+                    "entity_type": {"uid": attributes.pop("Object Type ID")},
                 },
             )
 
-        else:
+        elif "Type ID" in attributes:
             recovered_entity = self.create_entity(
                 Data,
                 save_on_creation=False,
                 **{
                     "entity": attributes,
                     "entity_type": self.fetch_type(
-                        uuid.UUID(attributes["Type ID"]), "Data"
+                        uuid.UUID(attributes.pop("Type ID")), "Data"
                     ),
                 },
             )
 
         if recovered_entity is not None:
             recovered_entity.on_file = True
             recovered_entity.entity_type.on_file = True
@@ -441,14 +443,15 @@
 
         :param entity_class: Type of entity to be created
         :param save_on_creation: Save the entity to geoh5 immediately
         :param compression: Compression level for data.
 
         :return entity: Newly created entity registered to the workspace
         """
+
         entity_kwargs: dict = kwargs.get("entity", {})
         entity_type_kwargs: dict = kwargs.get("entity_type", {})
 
         if entity_class is not RootGroup and (
             "parent" not in entity_kwargs or entity_kwargs["parent"] is None
         ):
             entity_kwargs["parent"] = self.root
@@ -503,14 +506,15 @@
             :obj:`~geoh5py.groups.group.Group` class.
         :param entity_kwargs: Attributes of the entity.
         :param entity_type_kwargs: Attributes of the entity_type.
 
         :return: A new Object or Group.
         """
         entity_type_uid = None
+
         for key, val in entity_type_kwargs.items():
             if key.lower() in ["id", "uid"]:
                 entity_type_uid = uuid.UUID(str(val))
 
         if entity_type_uid is None:
             if hasattr(entity_class, "default_type_uid"):
                 entity_type_uid = entity_class.default_type_uid()
@@ -593,40 +597,42 @@
                 )
             else:
                 ref_type = self.str_from_type(child)
                 self._io_call(
                     H5Writer.remove_child, child.uid, ref_type, parent, mode="r+"
                 )
 
-    def remove_entity(self, entity: Entity):
+    def remove_entity(self, entity: Entity | PropertyGroup):
         """
         Function to remove an entity and its children from the workspace.
         """
         if not entity.allow_delete:
             raise UserWarning(
                 f"The 'allow_delete' property of entity {entity} prevents it from "
                 "being removed. Please revise."
             )
 
-        if not isinstance(entity, Concatenated):
-            self.workspace.remove_recursively(entity)
-
-        if isinstance(entity, Concatenated):
+        if isinstance(entity, (Concatenated, ConcatenatedPropertyGroup)):
             entity.concatenator.remove_entity(entity)
-        else:
+            return
+
+        self.workspace.remove_recursively(entity)
+
+        if not isinstance(entity, PropertyGroup):
             ref_type = self.str_from_type(entity)
             self._io_call(
                 H5Writer.remove_entity,
                 entity.uid,
                 ref_type,
                 mode="r+",
             )
-            del entity
-            collect()
-            self.remove_none_referents(self._types, "Types")
+
+        del entity
+        collect()
+        self.remove_none_referents(self._types, "Types")
 
     def remove_none_referents(
         self,
         referents: dict[uuid.UUID, ReferenceType],
         rtype: str,
     ):
         """
@@ -639,23 +645,23 @@
                 self._io_call(
                     H5Writer.remove_entity, key, rtype, parent=self, mode="r+"
                 )
 
         for key in rem_list:
             del referents[key]
 
-    def remove_recursively(self, entity: Entity):
+    def remove_recursively(self, entity: Entity | PropertyGroup):
         """Delete an entity and its children from the workspace and geoh5 recursively"""
         parent = entity.parent
 
         if hasattr(entity, "children"):
             for child in entity.children:
                 self.remove_entity(child)
 
-        parent.remove_children(entity)
+        parent.remove_children([entity])
 
     def deactivate(self):
         """Deactivate this workspace if it was the active one, else does nothing."""
         if Workspace._active_ref() is self:
             Workspace._active_ref = type(None)
 
     @property
@@ -708,29 +714,28 @@
         if isinstance(entity, Group):
             entity_type = "group"
         elif isinstance(entity, ObjectBase):
             entity_type = "object"
 
         if isinstance(entity, RootGroup) and not entity.on_file:
             children_list = {child.uid: "" for child in entity.children}
-        else:
-            children_list = self._io_call(
-                H5Reader.fetch_children, entity.uid, entity_type, mode="r"
-            )
 
-        if isinstance(entity, Concatenator):
+        elif isinstance(entity, Concatenator):
             if any(entity.children):
                 return entity.children
 
             cat_children = entity.fetch_concatenated_objects()
-            children_list.update(
-                {
-                    str2uuid(as_str_if_utf8_bytes(uid)): attr
-                    for uid, attr in cat_children.items()
-                }
+            children_list = {
+                str2uuid(as_str_if_utf8_bytes(uid)): attr
+                for uid, attr in cat_children.items()
+            }
+
+        else:
+            children_list = self._io_call(
+                H5Reader.fetch_children, entity.uid, entity_type, mode="r"
             )
 
         family_tree = []
         for uid, child_type in children_list.items():
             recovered_object = self.get_entity(uid)[0]
             if recovered_object is None and not isinstance(entity, PropertyGroup):
                 recovered_object = self.load_entity(uid, child_type, parent=entity)
@@ -1109,14 +1114,15 @@
         :obj:`dict` of :obj:`uuid.UUID` keys and name values for all registered Objects.
         """
         objects_name = {}
         for key, val in self._objects.items():
             entity = val()
             if entity is not None:
                 objects_name[key] = entity.name
+                objects_name[key] = entity.name
         return objects_name
 
     def load_entity(
         self,
         uid: uuid.UUID,
         entity_type: str,
         parent: Entity | None = None,
```

### Comparing `geoh5py-0.9.0a2/package.rst` & `geoh5py-0.9.0a3/package.rst`

 * *Files identical despite different names*

### Comparing `geoh5py-0.9.0a2/pyproject.toml` & `geoh5py-0.9.0a3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoh5py"
-version = "0.9.0-alpha.2"
+version = "0.9.0-alpha.3"
 license = "LGPL-3.0-or-later"
 description = "Python API for geoh5, an open file format for geoscientific data"
 authors = ["Mira Geoscience <support@mirageoscience.com>"]
 repository = "https://github.com/MiraGeoscience/geoh5py"
 documentation = "https://geoh5py.readthedocs.io/en/latest/"
 homepage = "https://mirageoscience.com"
 readme = "package.rst"
@@ -20,15 +20,15 @@
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 exclude = ["geoh5py/handlers/*", "geoh5py/interfaces/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
-Pillow = "^10.0.1"
+Pillow = "10.1.0"
 h5py = "^3.2.1"
 numpy = "!=1.19.4, ~1.23.5"
 
 
 [tool.poetry.group.dev.dependencies]
 lockfile = "^0.12.2"
 pylint = "*"
```

### Comparing `geoh5py-0.9.0a2/PKG-INFO` & `geoh5py-0.9.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoh5py
-Version: 0.9.0a2
+Version: 0.9.0a3
 Summary: Python API for geoh5, an open file format for geoscientific data
 Home-page: https://mirageoscience.com
 License: LGPL-3.0-or-later
 Keywords: geology,geophysics,data,interoperability
 Author: Mira Geoscience
 Author-email: support@mirageoscience.com
 Requires-Python: >=3.8,<3.11
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: Pillow (>=10.0.1,<11.0.0)
+Requires-Dist: Pillow (==10.1.0)
 Requires-Dist: h5py (>=3.2.1,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Project-URL: Documentation, https://geoh5py.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/MiraGeoscience/geoh5py
 Description-Content-Type: text/x-rst
 
 geoh5py: Python API for geoh5. An open file format for geoscientific data
```

