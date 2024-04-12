# Comparing `tmp/openepd-3.0.0.tar.gz` & `tmp/openepd-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openepd-3.0.0.tar", max compression
+gzip compressed data, was "openepd-3.1.0.tar", max compression
```

## Comparing `openepd-3.0.0.tar` & `openepd-3.1.0.tar`

### file list

```diff
@@ -1,59 +1,95 @@
--rw-r--r--   0        0        0    11357 2023-05-18 14:32:16.267817 openepd-3.0.0/LICENSE
--rw-r--r--   0        0        0     6786 2024-04-05 22:32:16.863523 openepd-3.0.0/README.md
--rw-r--r--   0        0        0     3132 2024-04-05 22:34:29.805796 openepd-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/__init__.py
--rw-r--r--   0        0        0      855 2024-04-05 22:35:07.736448 openepd-3.0.0/src/openepd/__version__.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/__init__.py
--rw-r--r--   0        0        0    21142 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/base_sync_client.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/__init__.py
--rw-r--r--   0        0        0     1067 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/dto.py
--rw-r--r--   0        0        0     1588 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/category/sync_api.py
--rw-r--r--   0        0        0     8681 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/common.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/__init__.py
--rw-r--r--   0        0        0     1250 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/base.py
--rw-r--r--   0        0        0     4705 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/common.py
--rw-r--r--   0        0        0     2377 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/meta.py
--rw-r--r--   0        0        0     2211 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/mf.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/dto/params.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/__init__.py
--rw-r--r--   0        0        0     5091 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/dto.py
--rw-r--r--   0        0        0     4391 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/epd/sync_api.py
--rw-r--r--   0        0        0     2376 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/errors.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/__init__.py
--rw-r--r--   0        0        0     1649 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/dto.py
--rw-r--r--   0        0        0     1805 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/pcr/sync_api.py
--rw-r--r--   0        0        0     2504 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/sync_client.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/api/test/__init__.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.863523 openepd-3.0.0/src/openepd/bundle/__init__.py
--rw-r--r--   0        0        0     7086 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/base.py
--rw-r--r--   0        0        0     2663 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/model.py
--rw-r--r--   0        0        0     6904 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/reader.py
--rw-r--r--   0        0        0     8353 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/bundle/writer.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/compat/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/compat/pydantic.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/__init__.py
--rw-r--r--   0        0        0     9154 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/base.py
--rw-r--r--   0        0        0     1856 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/category.py
--rw-r--r--   0        0        0     5659 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/common.py
--rw-r--r--   0        0        0    14299 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/epd.py
--rw-r--r--   0        0        0     1918 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/factory.py
--rw-r--r--   0        0        0    17165 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/lcia.py
--rw-r--r--   0        0        0     4013 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/org.py
--rw-r--r--   0        0        0     4620 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/pcr.py
--rw-r--r--   0        0        0      862 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/README.md
--rw-r--r--   0        0        0     2315 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/__init__.py
--rw-r--r--   0        0        0     2262 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/aluminium.py
--rw-r--r--   0        0        0     3549 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/asphalt.py
--rw-r--r--   0        0        0     2697 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/base.py
--rw-r--r--   0        0        0    23219 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/concrete.py
--rw-r--r--   0        0        0    14840 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/glass.py
--rw-r--r--   0        0        0     6480 2024-04-05 22:32:16.866857 openepd-3.0.0/src/openepd/model/specs/steel.py
--rw-r--r--   0        0        0     5144 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/specs/wood.py
--rw-r--r--   0        0        0     1535 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/standard.py
--rw-r--r--   0        0        0      837 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/__init__.py
--rw-r--r--   0        0        0     2652 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/common.py
--rw-r--r--   0        0        0     1105 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/numbers.py
--rw-r--r--   0        0        0     5194 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/validation/quantity.py
--rw-r--r--   0        0        0     4690 2024-04-05 22:32:16.870190 openepd-3.0.0/src/openepd/model/versioning.py
--rw-r--r--   0        0        0        0 2023-06-15 10:11:54.308584 openepd-3.0.0/src/openepd/py.typed
--rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 openepd-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 18:47:11.289607 openepd-3.1.0/LICENSE
+-rw-r--r--   0        0        0     6786 2024-04-12 18:47:11.289607 openepd-3.1.0/README.md
+-rw-r--r--   0        0        0     3132 2024-04-12 18:47:11.289607 openepd-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/__version__.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/__init__.py
+-rw-r--r--   0        0        0    21142 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/base_sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/category/__init__.py
+-rw-r--r--   0        0        0     1067 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/category/dto.py
+-rw-r--r--   0        0        0     1588 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/category/sync_api.py
+-rw-r--r--   0        0        0     8681 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/common.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/__init__.py
+-rw-r--r--   0        0        0     1250 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/base.py
+-rw-r--r--   0        0        0     4705 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/common.py
+-rw-r--r--   0        0        0     2377 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/meta.py
+-rw-r--r--   0        0        0     2211 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/mf.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/dto/params.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/epd/__init__.py
+-rw-r--r--   0        0        0     5091 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/epd/dto.py
+-rw-r--r--   0        0        0     4391 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/epd/sync_api.py
+-rw-r--r--   0        0        0     2376 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/errors.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/pcr/__init__.py
+-rw-r--r--   0        0        0     1649 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/pcr/dto.py
+-rw-r--r--   0        0        0     1805 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/pcr/sync_api.py
+-rw-r--r--   0        0        0     2504 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/sync_client.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/api/test/__init__.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/bundle/__init__.py
+-rw-r--r--   0        0        0     7086 2024-04-12 18:47:11.289607 openepd-3.1.0/src/openepd/bundle/base.py
+-rw-r--r--   0        0        0     2663 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/bundle/model.py
+-rw-r--r--   0        0        0     6904 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/bundle/reader.py
+-rw-r--r--   0        0        0     8353 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/bundle/writer.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/compat/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/compat/pydantic.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/__init__.py
+-rw-r--r--   0        0        0     9154 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/base.py
+-rw-r--r--   0        0        0     1856 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/category.py
+-rw-r--r--   0        0        0     5659 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/common.py
+-rw-r--r--   0        0        0    14299 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/epd.py
+-rw-r--r--   0        0        0     1918 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/factory.py
+-rw-r--r--   0        0        0    17165 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/lcia.py
+-rw-r--r--   0        0        0     4013 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/org.py
+-rw-r--r--   0        0        0     4620 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/pcr.py
+-rw-r--r--   0        0        0      862 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/README.md
+-rw-r--r--   0        0        0     5176 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/__init__.py
+-rw-r--r--   0        0        0     2271 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/aluminium.py
+-rw-r--r--   0        0        0     3549 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/asphalt.py
+-rw-r--r--   0        0        0     2697 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/base.py
+-rw-r--r--   0        0        0    15655 2024-04-12 18:47:11.293607 openepd-3.1.0/src/openepd/model/specs/concrete.py
+-rw-r--r--   0        0        0     1934 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/accessories.py
+-rw-r--r--   0        0        0     3161 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/aggregates.py
+-rw-r--r--   0        0        0     2440 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/aluminium.py
+-rw-r--r--   0        0        0     3837 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/asphalt.py
+-rw-r--r--   0        0        0     1034 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/bulk_materials.py
+-rw-r--r--   0        0        0     1058 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/cast_decks_and_underlayment.py
+-rw-r--r--   0        0        0     6939 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/cladding.py
+-rw-r--r--   0        0        0     2324 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/cmu.py
+-rw-r--r--   0        0        0     1117 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/common.py
+-rw-r--r--   0        0        0     6617 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/concrete.py
+-rw-r--r--   0        0        0     2422 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/conveying_equipment.py
+-rw-r--r--   0        0        0    10457 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/electrical.py
+-rw-r--r--   0        0        0     2117 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/electrical_transmission_and_distribution_equipment.py
+-rw-r--r--   0        0        0     1029 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/electricity.py
+-rw-r--r--   0        0        0    57079 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/enums.py
+-rw-r--r--   0        0        0    22337 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/finishes.py
+-rw-r--r--   0        0        0     2801 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/fire_and_smoke_protection.py
+-rw-r--r--   0        0        0     3076 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/furnishings.py
+-rw-r--r--   0        0        0     1023 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/grouting.py
+-rw-r--r--   0        0        0     4599 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/manufacturing_inputs.py
+-rw-r--r--   0        0        0     3177 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/masonry.py
+-rw-r--r--   0        0        0     1225 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/material_handling.py
+-rw-r--r--   0        0        0    11561 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/mechanical.py
+-rw-r--r--   0        0        0     1900 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/mechanical_insulation.py
+-rw-r--r--   0        0        0     8644 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/network_infrastructure.py
+-rw-r--r--   0        0        0    17100 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/openings.py
+-rw-r--r--   0        0        0     1057 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/other_electrical_equipment.py
+-rw-r--r--   0        0        0     3453 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/other_materials.py
+-rw-r--r--   0        0        0     5439 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/plumbing.py
+-rw-r--r--   0        0        0     2690 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/precast_concrete.py
+-rw-r--r--   0        0        0     3516 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/sheathing.py
+-rw-r--r--   0        0        0     8102 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/steel.py
+-rw-r--r--   0        0        0     7963 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/thermal_moisture_protection.py
+-rw-r--r--   0        0        0     2768 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/utility_piping.py
+-rw-r--r--   0        0        0     6199 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/wood.py
+-rw-r--r--   0        0        0     1880 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/generated/wood_joists.py
+-rw-r--r--   0        0        0    13664 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/glass.py
+-rw-r--r--   0        0        0     6367 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/steel.py
+-rw-r--r--   0        0        0     5144 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/specs/wood.py
+-rw-r--r--   0        0        0     1535 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/standard.py
+-rw-r--r--   0        0        0      837 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/validation/__init__.py
+-rw-r--r--   0        0        0     2652 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/validation/common.py
+-rw-r--r--   0        0        0     1105 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/validation/numbers.py
+-rw-r--r--   0        0        0     5287 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/validation/quantity.py
+-rw-r--r--   0        0        0     4690 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/model/versioning.py
+-rw-r--r--   0        0        0        0 2024-04-12 18:47:11.297608 openepd-3.1.0/src/openepd/py.typed
+-rw-r--r--   0        0        0     7762 1970-01-01 00:00:00.000000 openepd-3.1.0/PKG-INFO
```

### Comparing `openepd-3.0.0/LICENSE` & `openepd-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/README.md` & `openepd-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/pyproject.toml` & `openepd-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openepd"
-version = "3.0.0"
+version = "3.1.0"
 license = "Apache-2.0"
 description = "Python library to work with OpenEPD format"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/openepd"
 keywords = []
 classifiers = [
```

### Comparing `openepd-3.0.0/src/openepd/__init__.py` & `openepd-3.1.0/src/openepd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/__version__.py` & `openepd-3.1.0/src/openepd/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-VERSION = "3.0.0"
+VERSION = "3.1.0"
```

### Comparing `openepd-3.0.0/src/openepd/api/__init__.py` & `openepd-3.1.0/src/openepd/api/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/base_sync_client.py` & `openepd-3.1.0/src/openepd/api/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/category/__init__.py` & `openepd-3.1.0/src/openepd/api/category/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/category/dto.py` & `openepd-3.1.0/src/openepd/api/category/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/category/sync_api.py` & `openepd-3.1.0/src/openepd/api/category/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/common.py` & `openepd-3.1.0/src/openepd/api/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/__init__.py` & `openepd-3.1.0/src/openepd/api/dto/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/base.py` & `openepd-3.1.0/src/openepd/api/dto/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/common.py` & `openepd-3.1.0/src/openepd/api/dto/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/meta.py` & `openepd-3.1.0/src/openepd/api/dto/meta.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/mf.py` & `openepd-3.1.0/src/openepd/api/dto/mf.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/dto/params.py` & `openepd-3.1.0/src/openepd/api/dto/params.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/epd/__init__.py` & `openepd-3.1.0/src/openepd/api/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/epd/dto.py` & `openepd-3.1.0/src/openepd/api/epd/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/epd/sync_api.py` & `openepd-3.1.0/src/openepd/api/epd/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/errors.py` & `openepd-3.1.0/src/openepd/api/errors.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/pcr/__init__.py` & `openepd-3.1.0/src/openepd/api/pcr/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/pcr/dto.py` & `openepd-3.1.0/src/openepd/api/pcr/dto.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/pcr/sync_api.py` & `openepd-3.1.0/src/openepd/api/pcr/sync_api.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/sync_client.py` & `openepd-3.1.0/src/openepd/api/sync_client.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/api/test/__init__.py` & `openepd-3.1.0/src/openepd/api/test/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/bundle/__init__.py` & `openepd-3.1.0/src/openepd/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/bundle/base.py` & `openepd-3.1.0/src/openepd/bundle/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/bundle/model.py` & `openepd-3.1.0/src/openepd/bundle/model.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/bundle/reader.py` & `openepd-3.1.0/src/openepd/bundle/reader.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/bundle/writer.py` & `openepd-3.1.0/src/openepd/bundle/writer.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/compat/__init__.py` & `openepd-3.1.0/src/openepd/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/compat/pydantic.py` & `openepd-3.1.0/src/openepd/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/__init__.py` & `openepd-3.1.0/src/openepd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/base.py` & `openepd-3.1.0/src/openepd/model/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/category.py` & `openepd-3.1.0/src/openepd/model/category.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/common.py` & `openepd-3.1.0/src/openepd/model/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/epd.py` & `openepd-3.1.0/src/openepd/model/epd.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/factory.py` & `openepd-3.1.0/src/openepd/model/factory.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/lcia.py` & `openepd-3.1.0/src/openepd/model/lcia.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/org.py` & `openepd-3.1.0/src/openepd/model/org.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/pcr.py` & `openepd-3.1.0/src/openepd/model/pcr.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/specs/README.md` & `openepd-3.1.0/src/openepd/model/specs/README.md`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/specs/__init__.py` & `openepd-3.1.0/src/openepd/model/specs/generated/cmu.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,33 +13,34 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
-
 from openepd.compat.pydantic import pyd
-from openepd.model.base import BaseOpenEpdSchema
-from openepd.model.specs import concrete, steel
-from openepd.model.specs.aluminium import AluminiumV1
-from openepd.model.specs.asphalt import AsphaltV1
-from openepd.model.specs.glass import GlazingV1
-from openepd.model.specs.wood import TimberV1
+from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from openepd.model.specs.generated.enums import CmuBlockType, CmuWeightClassification
+from openepd.model.validation.quantity import GwpKgCo2eStr, PressureMPaStr, validate_unit_factory
+
+
+class CMUV1(BaseOpenEpdHierarchicalSpec):
+    """CMU performance specification."""
 
+    _EXT_VERSION = "1.0"
 
-class Specs(BaseOpenEpdSchema):
-    """Material specific specs."""
+    # Own fields:
+    white_cement: bool | None = pyd.Field(default=None, description="", example=True)
+    strength_28d: PressureMPaStr | None = pyd.Field(default=None, description="", example="1 MPa")
+    weight_classification: CmuWeightClassification | None = pyd.Field(default=None, description="", example="Normal")
+    block_type: CmuBlockType | None = pyd.Field(default=None, description="", example="Gray")
+    insulated: bool | None = pyd.Field(default=None, description="", example=True)
+    sound_performance: bool | None = pyd.Field(default=None, description="", example=True)
+    b1_recarbonation: GwpKgCo2eStr | None = pyd.Field(default=None, description="", example="1 kgCO2e")
+    b1_recarbonation_z: float | None = pyd.Field(default=None, description="", example=2.3)
 
-    cmu: concrete.CmuSpec | None = pyd.Field(default=None, description="Concrete Masonry Unit-specific (CMU) specs")
-    CMU: concrete.CmuSpec | None = pyd.Field(default=None, description="Concrete Masonry Unit-specific (CMU) specs")
-    Concrete: concrete.ConcreteV1 | None = pyd.Field(
-        default=None, title="ConcreteV1", description="Concrete-specific specs"
+    _concrete_compressive_strength_28d_is_quantity_validator = pyd.validator("strength_28d", allow_reuse=True)(
+        validate_unit_factory("MPa")
     )
-    PrecastConcrete: concrete.PrecastConcreteV1 | None = pyd.Field(
-        default=None, title="PrecastConcreteV1", description="Precast Concrete-specific specs"
+    _b1_recarbonation_is_quantity_validator = pyd.validator("b1_recarbonation", allow_reuse=True)(
+        validate_unit_factory("kgCO2e")
     )
-    Steel: steel.SteelV1 | None = pyd.Field(default=None, title="SteelV1", description="Steel-specific specs")
-    Asphalt: AsphaltV1 | None = pyd.Field(default=None, title="AsphaltV1")
-    Aluminium: AluminiumV1 | None = pyd.Field(default=None, title="AluminiumV1", description="Aluminium-specific specs")
-    Timber: TimberV1 | None = pyd.Field(default=None, title="TimberV1", description="Timber-specific specs")
-    Glazing: GlazingV1 | None = pyd.Field(default=None, title="GlazingV1", description="Glazing-specific specs")
```

### Comparing `openepd-3.0.0/src/openepd/model/specs/aluminium.py` & `openepd-3.1.0/src/openepd/model/specs/aluminium.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,12 @@
 
 class AluminiumV1(BaseOpenEpdHierarchicalSpec):
     """Aluminium V1 spec."""
 
     _EXT_VERSION = "1.0"
     recycled_content: RatioFloat | None = pyd.Field(default=None, description="Recycled content")
 
-    alloy: AluminiumAlloy | None = pyd.Field(default=None, description="Alloy")
+    alloy: AluminiumAlloy | None = pyd.Field(default=None, description="AluminiumAlloy")
     anodized: bool | None = None
     painted: bool | None = None
 
     AluminiumExtrusions: AluminiumExtrusionsV1 | None = pyd.Field(title="AluminiumExtrusionsV1", default=None)
```

### Comparing `openepd-3.0.0/src/openepd/model/specs/asphalt.py` & `openepd-3.1.0/src/openepd/model/specs/asphalt.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/specs/base.py` & `openepd-3.1.0/src/openepd/model/specs/base.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/specs/glass.py` & `openepd-3.1.0/src/openepd/model/specs/glass.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #  Find out more at www.BuildingTransparency.org
 #
 from enum import StrEnum
 
 from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from openepd.model.specs.generated.enums import NAFSPerformanceGrade
 from openepd.model.validation.numbers import PositiveInt, RatioFloat
 from openepd.model.validation.quantity import HeatConductanceUCIStr, LengthMmStr, PressureMPaStr, QuantityStr
 
 
 class SolarHeatGainMixin(BaseOpenEpdSchema):
     """Solar heat gain mixin."""
 
@@ -175,59 +176,14 @@
     """Hurricane resistant mixin."""
 
     hurricane_resistant: bool | None = pyd.Field(
         default=None, description="The product has been designed to resist windborne debris."
     )
 
 
-class NAFSPerformanceGrade(StrEnum):
-    """NAFS Performance Grade enum."""
-
-    GRADE_15_PSF = "15 psf"
-    GRADE_20_PSF = "20 psf"
-    GRADE_25_PSF = "25 psf"
-    GRADE_30_PSF = "30 psf"
-    GRADE_35_PSF = "35 psf"
-    GRADE_40_PSF = "40 psf"
-    GRADE_45_PSF = "45 psf"
-    GRADE_50_PSF = "50 psf"
-    GRADE_55_PSF = "55 psf"
-    GRADE_60_PSF = "60 psf"
-    GRADE_65_PSF = "65 psf"
-    GRADE_70_PSF = "70 psf"
-    GRADE_75_PSF = "75 psf"
-    GRADE_80_PSF = "80 psf"
-    GRADE_85_PSF = "85 psf"
-    GRADE_90_PSF = "90 psf"
-    GRADE_95_PSF = "95 psf"
-    GRADE_100_PSF = "100 psf"
-    GRADE_105_PSF = "105 psf"
-    GRADE_110_PSF = "110 psf"
-    GRADE_115_PSF = "115 psf"
-    GRADE_120_PSF = "120 psf"
-    GRADE_125_PSF = "125 psf"
-    GRADE_130_PSF = "130 psf"
-    GRADE_135_PSF = "135 psf"
-    GRADE_140_PSF = "140 psf"
-    GRADE_145_PSF = "145 psf"
-    GRADE_150_PSF = "150 psf"
-    GRADE_155_PSF = "155 psf"
-    GRADE_160_PSF = "160 psf"
-    GRADE_165_PSF = "165 psf"
-    GRADE_170_PSF = "170 psf"
-    GRADE_175_PSF = "175 psf"
-    GRADE_180_PSF = "180 psf"
-    GRADE_185_PSF = "185 psf"
-    GRADE_190_PSF = "190 psf"
-    GRADE_195_PSF = "195 psf"
-    GRADE_200_PSF = "200 psf"
-    GRADE_205_PSF = "205 psf"
-    GRADE_210_PSF = "210 psf"
-
-
 class SpacerEnum(StrEnum):
     """Spacer enum."""
 
     ALUMINIUM = "Aluminium"
     STAINLESS_STEEL = "Stainless steel"
     PLASTIC_AND_STAINLESS_STEEL = "Plastic and stainless steel"
     THERMOPLASTIC = "Thermoplastic"
```

### Comparing `openepd-3.0.0/src/openepd/model/specs/steel.py` & `openepd-3.1.0/src/openepd/model/specs/steel.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,28 @@
 #
 from enum import StrEnum
 
 from openepd.compat.pydantic import pyd
 from openepd.model.base import BaseOpenEpdSchema
 from openepd.model.common import OpenEPDUnit
 from openepd.model.specs.base import BaseOpenEpdHierarchicalSpec
+from openepd.model.specs.generated.enums import SteelComposition
 from openepd.model.standard import Standard
 from openepd.model.validation.numbers import RatioFloat
 from openepd.model.validation.quantity import LengthMmStr, validate_unit_factory
 
 
 class SteelMakingRoute(BaseOpenEpdSchema):
     """Steel making route."""
 
     bof: bool | None = pyd.Field(default=None, description="Basic oxygen furnace")
     eaf: bool | None = pyd.Field(default=None, description="Electric arc furnace")
     ohf: bool | None = pyd.Field(default=None, description="Open hearth furnace")
 
 
-class SteelComposition(StrEnum):
-    """Steel composition enum."""
-
-    CARBON = "Carbon"
-    ALLOY = "Alloy"
-    STAINLESS = "Stainless"
-    TOOL = "Tool"
-    OTHER = "Other"
-
-
 class FabricatedOptionsMixin(pyd.BaseModel):
     """Fabricated options mixin."""
 
     _EXT_VERSION = "1.0"
 
     fabricated: bool | None = pyd.Field(default=None, description="Fabricated")
```

### Comparing `openepd-3.0.0/src/openepd/model/specs/wood.py` & `openepd-3.1.0/src/openepd/model/specs/wood.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/standard.py` & `openepd-3.1.0/src/openepd/model/standard.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/validation/__init__.py` & `openepd-3.1.0/src/openepd/model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/validation/common.py` & `openepd-3.1.0/src/openepd/model/validation/common.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/validation/numbers.py` & `openepd-3.1.0/src/openepd/model/validation/numbers.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/src/openepd/model/validation/quantity.py` & `openepd-3.1.0/src/openepd/model/validation/quantity.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,13 +119,14 @@
 # todo with the migration to Pydantic 2 we will be able to use pydantic.funcational_validators.AfterDecorator
 # this will let us bind the validator not to the model or the field, but to the type itself.
 
 # for abitrary non-standard quantity
 QuantityStr: TypeAlias = Annotated[str, pyd.Field()]
 PressureMPaStr: TypeAlias = Annotated[str, pyd.Field(example="30 MPa")]
 MassKgStr: TypeAlias = Annotated[str, pyd.Field(example="30 kg")]
-LengthMmStr: TypeAlias = Annotated[str, pyd.Field(example="30 mm")]
-AreaM2Str: TypeAlias = Annotated[str, pyd.Field(example="12 m2")]
-LengthMStr: TypeAlias = Annotated[str, pyd.Field(example="30 m")]
+AreaM2Str: TypeAlias = Annotated[str, pyd.Field(example="12 m2", gt=0)]
+LengthMStr: TypeAlias = Annotated[str, pyd.Field(example="30 m", gt=0)]
+LengthMmStr: TypeAlias = Annotated[str, pyd.Field(example="30 mm", gt=0)]
+LengthInchStr: TypeAlias = Annotated[str, pyd.Field(example="30 m", gt=0)]
 TemperatureCStr: TypeAlias = Annotated[str, pyd.Field(example="45 C")]
 HeatConductanceUCIStr: TypeAlias = Annotated[str, pyd.Field(example="0.3 U")]
 GwpKgCo2eStr: TypeAlias = Annotated[str, pyd.Field(example="300 kgCO2e")]
```

### Comparing `openepd-3.0.0/src/openepd/model/versioning.py` & `openepd-3.1.0/src/openepd/model/versioning.py`

 * *Files identical despite different names*

### Comparing `openepd-3.0.0/PKG-INFO` & `openepd-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openepd
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python library to work with OpenEPD format
 Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openepd Version: 3.0.0 Summary: Python library to
+Metadata-Version: 2.1 Name: openepd Version: 3.1.0 Summary: Python library to
 work with OpenEPD format Home-page: https://github.com/cchangelabs/openepd
 License: Apache-2.0 Author: C-Change Labs Author-email: support@c-change-
 labs.com Maintainer: C-Change Labs Maintainer-email: open-source@c-change-
 labs.com Requires-Python: >=3.11,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

