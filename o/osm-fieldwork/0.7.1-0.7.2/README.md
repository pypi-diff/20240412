# Comparing `tmp/osm-fieldwork-0.7.1.tar.gz` & `tmp/osm-fieldwork-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.7.1.tar", last modified: Thu Apr 11 18:34:52 2024, max compression
+gzip compressed data, was "osm-fieldwork-0.7.2.tar", last modified: Thu Apr 11 18:45:06 2024, max compression
```

## Comparing `osm-fieldwork-0.7.1.tar` & `osm-fieldwork-0.7.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0    34102 2024-04-11 18:34:43.784565 osm-fieldwork-0.7.1/LICENSE.md
--rw-r--r--   0        0        0    14494 2024-04-11 18:34:43.784565 osm-fieldwork-0.7.1/README.md
--rwxr-xr-x   0        0        0    13091 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5037 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     5072 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4919 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    60821 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/OdkCentral.py
--rwxr-xr-x   0        0        0    17428 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/OdkCentralAsync.py
--rw-r--r--   0        0        0       99 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       22 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0    20388 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0    11364 2024-04-11 18:34:43.792565 osm-fieldwork-0.7.1/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      883 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/__init__.py
--rw-r--r--   0        0        0      387 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      348 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      247 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      777 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      126 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      437 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      126 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      490 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0      193 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/highways.yaml
--rw-r--r--   0        0        0       80 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0       90 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0       88 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0       91 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0        0 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/taginfo-db.db
--rw-r--r--   0        0        0      253 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4391 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      415 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      185 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      128 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     8929 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/filter_data.py
--rw-r--r--   0        0        0      798 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/imagery.yaml
--rwxr-xr-x   0        0        0    15977 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0     7371 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/make_data_extract.py
--rw-r--r--   0        0        0     3405 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/models.yaml
--rwxr-xr-x   0        0        0     5416 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4298 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0     5348 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/odk2osm.py
--rwxr-xr-x   0        0        0    17845 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0    23342 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5302 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    15231 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     9381 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     3717 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3795 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0     1151 2024-04-11 18:34:43.796565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2024-04-11 18:34:43.800565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2024-04-11 18:34:43.804565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0      220 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/entities/__init__.py
--rw-r--r--   0        0        0   111104 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/entities/registration_form.xls
--rw-r--r--   0        0        0    69120 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    40448 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/highways.xls
--rw-r--r--   0        0        0    22528 2024-04-11 18:34:43.812565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0   115963 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   265216 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/test.xls
--rw-r--r--   0        0        0   353280 2024-04-11 18:34:43.816565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/thamel.xls
--rw-r--r--   0        0        0   118272 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     5443 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     3547 2024-04-11 18:34:43.820565 osm-fieldwork-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    34102 2024-04-11 18:44:59.129438 osm-fieldwork-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0    14494 2024-04-11 18:44:59.129438 osm-fieldwork-0.7.2/README.md
+-rwxr-xr-x   0        0        0    13091 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5037 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     5072 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4919 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    60821 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/OdkCentral.py
+-rwxr-xr-x   0        0        0    17428 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/OdkCentralAsync.py
+-rw-r--r--   0        0        0       99 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0    20165 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0    11364 2024-04-11 18:44:59.137438 osm-fieldwork-0.7.2/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      883 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      348 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      247 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      777 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      126 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      437 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      126 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      490 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0      193 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/highways.yaml
+-rw-r--r--   0        0        0       80 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0       90 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0       88 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0       91 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0        0 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/taginfo-db.db
+-rw-r--r--   0        0        0      253 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4391 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      415 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      185 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      128 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     8929 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/filter_data.py
+-rw-r--r--   0        0        0      798 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/imagery.yaml
+-rwxr-xr-x   0        0        0    15977 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0     7371 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/make_data_extract.py
+-rw-r--r--   0        0        0     3405 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/models.yaml
+-rwxr-xr-x   0        0        0     5416 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4298 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0     5348 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/odk2osm.py
+-rwxr-xr-x   0        0        0    17845 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0    23342 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5302 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    15231 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     9381 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     3717 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3795 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0     1151 2024-04-11 18:44:59.141438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2024-04-11 18:44:59.145438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2024-04-11 18:44:59.145438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0      220 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/entities/__init__.py
+-rw-r--r--   0        0        0   111104 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/entities/registration_form.xls
+-rw-r--r--   0        0        0    69120 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    40448 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/highways.xls
+-rw-r--r--   0        0        0    22528 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2024-04-11 18:44:59.157438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   265216 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/test.xls
+-rw-r--r--   0        0        0   353280 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/thamel.xls
+-rw-r--r--   0        0        0   118272 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2024-04-11 18:44:59.161438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2024-04-11 18:44:59.165438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2024-04-11 18:44:59.165438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2024-04-11 18:44:59.165438 osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     5443 2024-04-11 18:44:59.165438 osm-fieldwork-0.7.2/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     3547 2024-04-11 18:44:59.165438 osm-fieldwork-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.7.2/PKG-INFO
```

### Comparing `osm-fieldwork-0.7.1/LICENSE.md` & `osm-fieldwork-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/README.md` & `osm-fieldwork-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.7.2/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.7.2/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.7.2/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.7.2/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.7.2/osm_fieldwork/OdkCentral.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/OdkCentralAsync.py` & `osm-fieldwork-0.7.2/osm_fieldwork/OdkCentralAsync.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.7.2/osm_fieldwork/basemapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,28 +327,25 @@
 
         bbox = geometry.bounds
         # left, bottom, right, top
         # minX, minY, maxX, maxY
         return bbox
 
 
-def tileid_from_tms_path(filepath: Union[Path, str]):
+def tileid_from_y_tile(filepath: Union[Path | str]):
     """Helper function to get the tile id from a tile in z/x/y directory structure.
 
     Args:
         filepath (Union[Path, str]): The path to the y tile in /z/x/y.jpg structure.
     """
-    # Extract the final 3 parts from the TMS file path
-    zxy_path = Path(filepath).parts[-3:]
-    # Extract filename without extension
-    y_tile_filename = Path(zxy_path[-1]).stem
-    # If filename contains a dot, take the part before the dot as 'y'
-    y = int(y_tile_filename.split(".")[0]) if "." in y_tile_filename else int(y_tile_filename)
-    # Extract z and x values
-    z, x = map(int, zxy_path[:-1])
+    # Get final two dirs + tile filename
+    parts = list(Path(filepath).parts[-3:])
+    # strip extension from y tile filename
+    parts[-1] = str(Path(parts[-1]).stem)
+    z, x, y = map(int, parts)
     return zxy_to_tileid(z, x, y)
 
 
 def tile_dir_to_pmtiles(outfile: str, tile_dir: str, bbox: tuple, attribution: str):
     """Write PMTiles archive from tiles in the specified directory.
 
     Args:
@@ -378,15 +375,15 @@
 
     # Process tiles
     with open(outfile, "wb") as pmtile_file:
         writer = PMTileWriter(pmtile_file)
 
         for tile_path in tile_dir.rglob("*"):
             if tile_path.is_file():
-                tile_id = tileid_from_tms_path(tile_path)
+                tile_id = tileid_from_y_tile(tile_path)
 
                 with open(tile_path, "rb") as tile:
                     writer.write_tile(tile_id, tile.read())
 
         # Extract bbox values
         min_lon, min_lat, max_lon, max_lat = bbox
 
@@ -414,15 +411,15 @@
     boundary=None,
     tms=None,
     xy=False,
     outfile=None,
     zooms="12-17",
     outdir=None,
     source="esri",
-) -> None:
+):
     """Create a basemap with given parameters.
 
     Args:
         boundary (str, optional): The boundary for the area you want.
         tms (str, optional): Custom TMS URL.
         xy (bool, optional): Swap the X & Y coordinates when using a
             custom TMS if True.
```

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/convert.py` & `osm-fieldwork-0.7.2/osm_fieldwork/convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.7.2/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/data_models/__init__.py` & `osm-fieldwork-0.7.2/osm_fieldwork/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.7.2/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.7.2/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/imagery.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/imagery.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.7.2/osm_fieldwork/json2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.7.2/osm_fieldwork/make_data_extract.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/models.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.7.2/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.7.2/osm_fieldwork/odk2geojson.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/odk2osm.py` & `osm-fieldwork-0.7.2/osm_fieldwork/odk2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.7.2/osm_fieldwork/odk_client.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.7.2/osm_fieldwork/odk_merge.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.7.2/osm_fieldwork/osm2favorities.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.7.2/osm_fieldwork/osmfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.7.2/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.7.2/osm_fieldwork/xforms.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/entities/registration_form.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/entities/registration_form.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/highways.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/highways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/test.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/test.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/thamel.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/thamel.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.7.2/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.7.2/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.7.1/pyproject.toml` & `osm-fieldwork-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.7.1"
+version = "0.7.2"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://hotosm.github.io/osm-fieldwork"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.scripts]
@@ -73,15 +73,15 @@
 testpaths = [
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.1"
+version = "0.7.2"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 update_changelog_on_bump = true
```

### Comparing `osm-fieldwork-0.7.1/PKG-INFO` & `osm-fieldwork-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.7.1
+Version: 0.7.2
 Summary: Processing field data from ODK to OpenStreetMap format.
 License: GPL-3.0-only
 Keywords: hot,odk,openstreetmap,fmtm
 Author-email: Rob Savoye <rob.savoye@hotosm.org>,Sam Woodcock <sam.woodcock@hotosm.org>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.7.1 Summary: Processing
+Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.7.2 Summary: Processing
 field data from ODK to OpenStreetMap format. License: GPL-3.0-only Keywords:
 hot,odk,openstreetmap,fmtm Author-email: Rob Savoye
 hotosm.org>,Sam Woodcock
 hotosm.org> Requires-Python: >=3.10 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

