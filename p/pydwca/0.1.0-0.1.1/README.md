# Comparing `tmp/pydwca-0.1.0.tar.gz` & `tmp/pydwca-0.1.1.tar.gz`

## Comparing `pydwca-0.1.0.tar` & `pydwca-0.1.1.tar`

### file list

```diff
@@ -1,177 +1,178 @@
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pydwca-0.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydwca-0.1.0/requirements-test.txt
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pydwca-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pydwca-0.1.0/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 pydwca-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/dwca.classes.rst
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/dwca.rst
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/dwca.terms.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/eml.resources.coverage.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/eml.resources.distribution.rst
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/eml.resources.rst
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/eml.rst
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/eml.types.rst
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/install.rst
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/modules.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/requirements.txt
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/usage.dwca.rst
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/usage.eml.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/xml_common.rst
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/xml_common.utils.rst
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydwca-0.1.0/docs/source/_static/_js/pypi-icon.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/base/__init__.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/base/darwincore.py
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/base/darwincore_archive.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/base/simple_darwincore.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/__init__.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/chronometric_age.py
--rw-r--r--   0        0        0    13973 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/data_file.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/event.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/geological_context.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/identification.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/location.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/material_entity.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/material_sample.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/measurement_or_fact.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/occurrence.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/organism.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/outside_class.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/resource_relationship.py
--rw-r--r--   0        0        0    12086 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/classes/taxon.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/__init__.py
--rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/chronometric_age.py
--rw-r--r--   0        0        0    10658 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/event.py
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/field.py
--rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/geological_context.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/identification.py
--rw-r--r--   0        0        0    29913 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/location.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/material_entity.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/material_sample.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/measurement_or_fact.py
--rw-r--r--   0        0        0    15474 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/occurrence.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/organism.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/outside_term.py
--rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/record_level.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/resource_relationship.py
--rw-r--r--   0        0        0    30795 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/dwca/terms/taxon.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/base/__init__.py
--rw-r--r--   0        0        0    17942 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/base/eml.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/base/metadata.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/base/version.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/citation.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/dataset.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/keyword_set.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/licence.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/protocol.py
--rw-r--r--   0        0        0    18330 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/resource.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/resources.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/software.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/coverage/__init__.py
--rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/coverage/coverage.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/coverage/geo_coverage.py
--rw-r--r--   0        0        0    25361 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/coverage/taxa_coverage.py
--rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/coverage/time_coverage.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/distribution/__init__.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/distribution/distribution.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/distribution/inline.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/distribution/offline.py
--rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/resources/distribution/online.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/__init__.py
--rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/access_type.py
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/address.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/eml_object.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/extension_string.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/extension_uri.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/i18n_string.py
--rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/individual_name.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/no_tag_object.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/organization_name.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/phone.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/position_name.py
--rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/responsible_party.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/section.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/semantic_annotation.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/eml/types/text_type.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/xml_object.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/__init__.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/enum.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/establishment_means.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/gpolygon.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/iteratate.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/language.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/length_unit.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 pydwca-0.1.0/src/xml_common/utils/type_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca/__init__.py
--rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca/test_dwca.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca/test_dwca_no_pandas.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca/test_meta.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_classes/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_classes/test_identification.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_classes/test_outside_class.py
--rw-r--r--   0        0        0    16639 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_classes/test_taxon.py
--rw-r--r--   0        0        0     9686 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_classes/test_taxon_no_pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_any_field.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_datetime_field.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_float_field.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_int_field.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_list_str_field.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_outside_term.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_str_field.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_taxon.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_union_datetime_field.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_dwca_terms/test_union_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_access_type.py
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_address.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_annotation.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_citation.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_dataset.py
--rw-r--r--   0        0        0    17788 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_eml.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_extension.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_extension_uri.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_i18n_string.py
--rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_individual_name.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_keyword_set.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_licence.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_metadata.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_organization_name.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_phone.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_position_name.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_protocol.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_responsible_party.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_section.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_semantic_annotation.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_software.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml/test_text_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_coverage/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_coverage/test_coverage.py
--rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_coverage/test_geo_coverage.py
--rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_coverage/test_taxa_coverage.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_coverage/test_time_coverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_distribution/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_distribution/test_distribution.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_distribution/test_inline.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_distribution/test_offline.py
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_eml_distribution/test_online.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_util/__init__.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_util/test_establishment_means.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_util/test_format.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_util/test_unformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_xml/__init__.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_xml/test_simple_xml.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pydwca-0.1.0/tests/test_xml/test_xml.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pydwca-0.1.0/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pydwca-0.1.0/LICENSE
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pydwca-0.1.0/README.md
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pydwca-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 pydwca-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 pydwca-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydwca-0.1.1/requirements-test.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pydwca-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pydwca-0.1.1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 pydwca-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.classes.rst
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.rst
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/dwca.terms.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.coverage.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.distribution.rst
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.resources.rst
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.rst
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/eml.types.rst
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/install.rst
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/modules.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/requirements.txt
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.dwca.rst
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.eml.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/usage.rst
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/xml_common.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/xml_common.utils.rst
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 pydwca-0.1.1/docs/source/_static/_js/pypi-icon.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/__init__.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/darwincore.py
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/darwincore_archive.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/base/simple_darwincore.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/__init__.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/chronometric_age.py
+-rw-r--r--   0        0        0    14151 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/data_file.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/event.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/geological_context.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/identification.py
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/location.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/material_entity.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/material_sample.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/measurement_or_fact.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/occurrence.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/organism.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/outside_class.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/resource_relationship.py
+-rw-r--r--   0        0        0    14149 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/classes/taxon.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/__init__.py
+-rw-r--r--   0        0        0    11804 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/chronometric_age.py
+-rw-r--r--   0        0        0    10658 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/event.py
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/field.py
+-rw-r--r--   0        0        0    12663 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/geological_context.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/identification.py
+-rw-r--r--   0        0        0    29913 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/location.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/material_entity.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/material_sample.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/measurement_or_fact.py
+-rw-r--r--   0        0        0    15474 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/occurrence.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/organism.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/outside_term.py
+-rw-r--r--   0        0        0    12969 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/record_level.py
+-rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/resource_relationship.py
+-rw-r--r--   0        0        0    30795 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/dwca/terms/taxon.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/__init__.py
+-rw-r--r--   0        0        0    17942 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/eml.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/metadata.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/base/version.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/citation.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/dataset.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/keyword_set.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/licence.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/protocol.py
+-rw-r--r--   0        0        0    18330 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/resource.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/resources.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/software.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/__init__.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/coverage.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/geo_coverage.py
+-rw-r--r--   0        0        0    25361 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/taxa_coverage.py
+-rw-r--r--   0        0        0    14438 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/coverage/time_coverage.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/__init__.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/distribution.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/inline.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/offline.py
+-rw-r--r--   0        0        0    23149 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/resources/distribution/online.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/__init__.py
+-rw-r--r--   0        0        0     8044 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/access_type.py
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/address.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/eml_object.py
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/extension_string.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/extension_uri.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/i18n_string.py
+-rw-r--r--   0        0        0     6637 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/individual_name.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/no_tag_object.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/organization_name.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/phone.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/position_name.py
+-rw-r--r--   0        0        0     9980 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/responsible_party.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/section.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/semantic_annotation.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/eml/types/text_type.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/__init__.py
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/xml_object.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/__init__.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/enum.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/establishment_means.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/gpolygon.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/iteratate.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/language.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/length_unit.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 pydwca-0.1.1/src/xml_common/utils/type_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/__init__.py
+-rw-r--r--   0        0        0     6301 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_dwca.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_dwca_no_pandas.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_meta.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca/test_outside_term.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_identification.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_outside_class.py
+-rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_taxon.py
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_classes/test_taxon_no_pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_any_field.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_datetime_field.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_float_field.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_int_field.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_list_str_field.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_outside_term.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_str_field.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_taxon.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_union_datetime_field.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_dwca_terms/test_union_field.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_access_type.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_address.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_annotation.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_citation.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_dataset.py
+-rw-r--r--   0        0        0    17788 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_eml.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_extension.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_extension_uri.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_i18n_string.py
+-rw-r--r--   0        0        0     8325 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_individual_name.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_keyword_set.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_licence.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_metadata.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_organization_name.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_phone.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_position_name.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_protocol.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_responsible_party.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_section.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_semantic_annotation.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_software.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml/test_text_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_coverage.py
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_geo_coverage.py
+-rw-r--r--   0        0        0    17600 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_taxa_coverage.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_coverage/test_time_coverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/__init__.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_distribution.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_inline.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_offline.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_eml_distribution/test_online.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/__init__.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_establishment_means.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_format.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_util/test_unformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/__init__.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/test_simple_xml.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pydwca-0.1.1/tests/test_xml/test_xml.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 pydwca-0.1.1/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pydwca-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 pydwca-0.1.1/README.md
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 pydwca-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 pydwca-0.1.1/PKG-INFO
```

### Comparing `pydwca-0.1.0/.readthedocs.yaml` & `pydwca-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/.github/workflows/publish-pypi.yml` & `pydwca-0.1.1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/.github/workflows/test.yml` & `pydwca-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/Makefile` & `pydwca-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/make.bat` & `pydwca-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/conf.py` & `pydwca-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/dwca.classes.rst` & `pydwca-0.1.1/docs/source/dwca.classes.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/dwca.rst` & `pydwca-0.1.1/docs/source/dwca.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/dwca.terms.rst` & `pydwca-0.1.1/docs/source/dwca.terms.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/eml.resources.coverage.rst` & `pydwca-0.1.1/docs/source/eml.resources.coverage.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/eml.resources.distribution.rst` & `pydwca-0.1.1/docs/source/eml.resources.distribution.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/eml.resources.rst` & `pydwca-0.1.1/docs/source/eml.resources.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/eml.rst` & `pydwca-0.1.1/docs/source/eml.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/eml.types.rst` & `pydwca-0.1.1/docs/source/eml.types.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/index.rst` & `pydwca-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/usage.dwca.rst` & `pydwca-0.1.1/docs/source/usage.dwca.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/usage.eml.rst` & `pydwca-0.1.1/docs/source/usage.eml.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/xml_common.utils.rst` & `pydwca-0.1.1/docs/source/xml_common.utils.rst`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/docs/source/_static/_js/pypi-icon.js` & `pydwca-0.1.1/docs/source/_static/_js/pypi-icon.js`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/base/darwincore.py` & `pydwca-0.1.1/src/dwca/base/darwincore.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/base/darwincore_archive.py` & `pydwca-0.1.1/src/dwca/base/darwincore_archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from warnings import warn
 
 from lxml import etree as et
 
 from dwca.base import DarwinCore
 from dwca.classes import DataFile, Occurrence, Organism, MaterialEntity, MaterialSample, Event, Location, \
     GeologicalContext, Identification, Taxon, ResourceRelationship, MeasurementOrFact, ChronometricAge, OutsideClass
-from xml_common.utils import Language
-from xml_common import XMLObject
 from eml import EML
 from eml.resources import EMLResource
+from xml_common import XMLObject
+from xml_common.utils import Language
 
 
 class DarwinCoreArchive(DarwinCore):
     """
     Represent a Darwin Core Archive file with all its elements.
 
     Parameters
@@ -140,23 +140,23 @@
 
     @core.setter
     def core(self, core: DataFile) -> None:
         self.__meta__.__core__ = core
         try:
             df = self.__meta__.__core__.pandas
             for extension in self.extensions:
-                ext_df = extension.pandas
+                ext_df = extension.as_pandas(_no_interaction=True)
                 mask = ext_df.iloc[:, extension.id].isin(df.iloc[:, core.id])
                 ext_df = ext_df.loc[ext_df[mask].index, :]
                 extension.pandas = ext_df
         except ImportError:
-            core_ids = [getattr(entry, core.__fields__[core.id].name()) for entry in self.core.__entries__]
+            core_ids = [getattr(entry, core.__fields__[core.id].name) for entry in self.core.__entries__]
             for extension in self.extensions:
                 def criteria(entry: DataFile.Entry) -> bool:
-                    entry_id = getattr(entry, extension.__fields__[extension.id].name())
+                    entry_id = getattr(entry, extension.__fields__[extension.id].name)
                     return entry_id in core_ids
                 extension.__entries__ = list(filter(
                     criteria, extension.__entries__
                 ))
         return
 
     @property
```

### Comparing `pydwca-0.1.0/src/dwca/classes/__init__.py` & `pydwca-0.1.1/src/dwca/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/chronometric_age.py` & `pydwca-0.1.1/src/dwca/classes/chronometric_age.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/data_file.py` & `pydwca-0.1.1/src/dwca/classes/data_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 
 from lxml import etree as et
 
 from dwca.terms import Field, DWCType, DWCModified, DWCLanguage, DWCLicense, DWCRightsHolder, DWCAccessRights, \
     DWCBibliographicCitation, DWCReferences, DWCInstitution, DWCCollection, DWCDataset, DWCInstitutionCode, \
     DWCCollectionCode, DWCDatasetName, DWCOwnerInstitutionCode, DWCBasisOfRecord, DWCInformationWithheld, \
     DWCDataGeneralizations, DWCDynamicProperties, OutsideTerm
-from xml_common.utils import iterate_with_bar
 from xml_common import XMLObject
-
+from xml_common.utils import iterate_with_bar
 
 try:
     import pandas as pd
 except Exception:
     pd = None
 
 
@@ -163,15 +162,16 @@
         -------
         Type[Field]
             The Python ``class`` representing the term name.
         """
         for field_class in cls.__field_class__:
             if element.get("term") == field_class.URI:
                 return field_class
-        warn(f"{element.get('term')} not in expected namespace. "
+        warn(f"{element.get('term')} not in expected namespace for "
+             f"{cls.URI} class. "
              f"Some functionalities may not be available.")
         return OutsideTerm
 
     @classmethod
     def parse_kwargs(cls, element: et.Element, nmap: Dict) -> Dict:
         """
         Parse an `lxml.etree.Element` into the DataFile parameters.
@@ -339,58 +339,60 @@
         lines = list(filter(lambda x: x != "", lines))
         for line in iterate_with_bar(
                 lines[self.__ignore_header_lines__:],
                 desc=f"Reading file {self.filename}", unit="entry"
         ):
             kwargs = dict()
             for field, value in zip(self.__fields__, line.split(self.__fields_end__)):
-                kwargs[field.name()] = field.format(value)
+                kwargs[field.name] = field.format(value)
             self.__entries__.append(DataFile.Entry(**kwargs))
         return
 
     def write_file(self) -> str:
         """
         Write the content as a text using format information on this object.
 
         Returns
         -------
         str
             Data File as plain text.
         """
         output_file = ""
-        header = [
-            field.name() for field in self.__fields__
-        ]
+        header = [field.name for field in self.__fields__]
         output_file += f"{self.__fields_end__}".join(header) + self.__lines_end__
         for entry in iterate_with_bar(self.__entries__, desc=f"Writing data {self.uri}", unit="line"):
             line = list()
             for field in self.__fields__:
-                line.append(field.unformat(getattr(entry, field.name())))
+                line.append(field.unformat(getattr(entry, field.name)))
             output_file += f"{self.__fields_end__}".join(line) + self.__lines_end__
         return output_file
 
-    def as_pandas(self) -> pd.DataFrame:
+    def as_pandas(self, _no_interaction: bool = False) -> pd.DataFrame:
         """
         Convert information in this DataFile in a pandas.DataFrame.
 
         Returns
         -------
         DataFrame
             Information as a pandas.DataFrame.
         """
         try:
             import pandas as pd
         except ImportError:
             raise ImportError("Install pandas to use this feature")
         fields = list()
         for field in self.__fields__:
-            fields.append(field.name())
+            fields.append(field.name)
         entries = list()
-        for entry in iterate_with_bar(self.__entries__, desc="Converting to pandas", unit="entry"):
-            entries.append(entry.to_dict())
+        if _no_interaction:
+            for entry in self.__entries__:
+                entries.append(entry.to_dict())
+        else:
+            for entry in iterate_with_bar(self.__entries__, desc="Converting to pandas", unit="entry"):
+                entries.append(entry.to_dict())
         self.__data__ = pd.DataFrame(entries, columns=fields)
         return self.__data__
 
     def __str__(self) -> str:
         role = self.__type__.name.lower().capitalize()
         return (f"{role}:"
                 f"\n\tclass: {self.uri}"
```

### Comparing `pydwca-0.1.0/src/dwca/classes/event.py` & `pydwca-0.1.1/src/dwca/classes/event.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/geological_context.py` & `pydwca-0.1.1/src/dwca/classes/geological_context.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/identification.py` & `pydwca-0.1.1/src/dwca/classes/identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/location.py` & `pydwca-0.1.1/src/dwca/classes/location.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/material_entity.py` & `pydwca-0.1.1/src/dwca/classes/material_entity.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/material_sample.py` & `pydwca-0.1.1/src/dwca/classes/material_sample.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/measurement_or_fact.py` & `pydwca-0.1.1/src/dwca/classes/measurement_or_fact.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/occurrence.py` & `pydwca-0.1.1/src/dwca/classes/occurrence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/organism.py` & `pydwca-0.1.1/src/dwca/classes/organism.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/outside_class.py` & `pydwca-0.1.1/src/dwca/classes/outside_class.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from typing import List, Union, Dict
+from typing import List, Dict, Type
 
 from lxml import etree as et
 
 from dwca.classes import DataFile, DataFileType
-from dwca.terms import Field
+from dwca.terms import Field, OutsideTerm
 
 
 class OutsideClass(DataFile):
     """
     Classes defined outside the Darwin Core specifications.
 
     Parameters
@@ -31,14 +31,15 @@
     fields_terminated_by : str, optional
         Delimiter of the file (cells) on the file, default `","`.
     fields_enclosed_by : str, optional
         Specifies the character used to enclose (mark the start and end of) each field, default empty `""`.
     ignore_header_lines : int, optional
         Ignore headers at the start of document, can be one line or a list of them, default 0 (first line).
     """
+    __field_class__ = DataFile.__field_class__
     def __init__(
             self, _id: int, uri: str,
             files: str,
             fields: List[Field],
             data_file_type: DataFileType = DataFileType.CORE,
             encoding: str = "utf-8",
             lines_terminated_by: str = "\n",
@@ -74,7 +75,27 @@
         if element is None:
             return None
         kwargs = cls.parse_kwargs(element, nmap)
         kwargs["uri"] = element.get("rowType")
         outside = OutsideClass(**kwargs)
         outside.__namespace__ = nmap
         return outside
+
+    @classmethod
+    def get_term_class(cls, element: et.Element) -> Type[Field]:
+        """
+        Extract the Python ``class`` term from an XML element instance.
+
+        Parameters
+        ----------
+        element : lxml.etree.Element
+            XML element instance.
+
+        Returns
+        -------
+        Type[Field]
+            The Python ``class`` representing the term name.
+        """
+        for field_class in cls.__field_class__:
+            if element.get("term") == field_class.URI:
+                return field_class
+        return OutsideTerm
```

### Comparing `pydwca-0.1.0/src/dwca/classes/resource_relationship.py` & `pydwca-0.1.1/src/dwca/classes/resource_relationship.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/classes/taxon.py` & `pydwca-0.1.1/src/dwca/classes/taxon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import re
-from typing import List, Type
+from typing import List, Type, Any, Union, Set, Iterable
+from warnings import warn
 
 from dwca.classes import DataFile, DataFileType
 from dwca.terms import Field, TaxonID, ScientificNameID, AcceptedNameUsageID, ParentNameUsageID, OriginalNameUsageID, \
     NameAccordingToID, NamePublishedInID, TaxonConceptID, ScientificName, AcceptedNameUsage, ParentNameUsage, \
     OriginalNameUsage, NameAccordingTo, NamePublishedIn, NamePublishedInYear, HigherClassification, Kingdom, Phylum, \
     DWCClass, Order, Superfamily, Family, Subfamily, Tribe, Subtribe, Genus, GenericName, Subgenus, \
     InfragenericEpithet, SpecificEpithet, InfraspecificEpithet, CultivarEpithet, TaxonRank, VerbatimTaxonRank, \
     ScientificNameAuthorship, VernacularName, NomenclaturalCode, TaxonomicStatus, NomenclaturalStatus, TaxonRemarks
+from xml_common.utils import iterate_with_bar, OptionalTqdm
 
 try:
     import pandas as pd
 except ImportError:
     pd = None
 
 
@@ -80,55 +82,75 @@
             self,
             taxa_field: Type[Field],
             taxa_name: str,
             taxa: List[str],
             filter_with_rank: bool = True
     ) -> None:
         assert taxa_field.URI in self.fields, f"{taxa_name} must be in fields of this class to use this feature."
-        complete_taxa = set(taxa)
+        tqdm = OptionalTqdm(total=100)
+        tqdm.set_descriptor(desc="Getting Taxon ID")
         try:
             df = self.pandas
-            mask = df[ScientificName.name()].isin(taxa)
+            mask = df[ScientificName.name_cls()].isin(taxa)
             if filter_with_rank:
-                mask &= df[TaxonRank.name()].str.lower() == taxa_name.lower()
-            taxa_id = df[mask][TaxonID.name()]
+                mask &= df[TaxonRank.name_cls()].str.lower() == taxa_name.lower()
+            taxa_id = df[mask][TaxonID.name_cls()]
         except ImportError:
+            tqdm.reset(total=len(taxa))
+            taxa_id = list()
             if filter_with_rank:
-                taxa_id = [
-                    getattr(
-                        self.__get_entry__(**{
-                            ScientificName.name(): taxon,
-                            f"{TaxonRank.name()}__case_insensitive": taxa_name
-                        }), TaxonID.name()
-                    ) for taxon in taxa
-                ]
+                for taxon in taxa:
+                    taxa_id.append(
+                        getattr(
+                            self.__get_entry__(**{
+                                ScientificName.name_cls(): taxon,
+                                f"{TaxonRank.name_cls()}__case_insensitive": taxa_name
+                            }), TaxonID.name_cls()
+                        )
+                    )
+                    tqdm.update()
             else:
-                taxa_id = [
-                    getattr(
-                        self.__get_entry__(**{ScientificName.name(): taxon}),
-                        TaxonID.name()
-                    ) for taxon in taxa
-                ]
-        for taxon in taxa_id:
-            complete_taxa.update(self.all_synonyms(taxon, get_names=True))
-        parents = set()
-        for taxon in taxa_id:
-            parents.update(self.get_parents(taxon))
-        for parent in parents.copy():
-            parents.update(self.all_synonyms(parent))
+                for taxon in taxa:
+                    taxa_id.append(
+                        getattr(
+                            self.__get_entry__(**{ScientificName.name_cls(): taxon}),
+                            TaxonID.name_cls()
+                        )
+                    )
+                    tqdm.update()
+            tqdm.reset(total=100)
+        tqdm.update(n=10)
+        postfix = {"Exact match found": len(taxa_id)}
+        tqdm.set_postfix(ordered_dict=postfix)
+        tqdm.set_descriptor(desc="Getting synonyms")
+        complete_taxa = self.all_synonyms(taxa_id, get_names=True)
+        postfix["Synonyms found"] = len(complete_taxa) - len(taxa_id)
+        tqdm.set_postfix(ordered_dict=postfix)
+        tqdm.update(n=40)
+        tqdm.set_descriptor(desc="Getting parents")
+        parents = self.get_parents(taxa_id)
+        parents.update(self.all_synonyms(parents))
+        postfix["Parents found"] = len(parents)
+        tqdm.set_postfix(ordered_dict=postfix)
+        tqdm.update(n=40)
+        tqdm.set_descriptor(desc=f"Filtering {taxa_name}")
         try:
             df = self.pandas
-            name = taxa_field.name()
-            df = df[df[name].isin(complete_taxa) | df[TaxonID.name()].isin(parents)]
+            name = taxa_field.name_cls()
+            df = df[df[name].isin(complete_taxa) | df[TaxonID.name_cls()].isin(parents)]
             self.pandas = df
         except ImportError:
             def filter_taxa(entry: DataFile.Entry) -> bool:
-                return getattr(entry, taxa_field.name()) in complete_taxa or getattr(entry, TaxonID.name()) in parents
-
+                return (getattr(entry, taxa_field.name_cls()) in complete_taxa or
+                        getattr(entry, TaxonID.name_cls()) in parents)
             self.__entries__ = list(filter(filter_taxa, self.__entries__))
+        postfix["Total filtered"] = len(self)
+        tqdm.set_postfix(ordered_dict=postfix)
+        tqdm.update(n=10)
+        tqdm.close()
         return
 
     def filter_by_kingdom(self, kingdoms: List[str]) -> None:
         """
         Filter data by a valid kingdoms.
 
         Parameters
@@ -207,87 +229,102 @@
         Parameters
         ----------
         species : List[str]
             Scientific Name of species (or rank below) to filter data.
         """
         return self._filter_by_taxa_(ScientificName, "Species", species, filter_with_rank=False)
 
-    def get_parents(self, taxa_id: str) -> List[str]:
+    def get_parents(self, taxa_id: List[str]) -> Set[str]:
         """
-        Get a list of taxa ids of the parent of the taxa.
+        Get a list of taxa ids of the parent of the list taxa id provided.
 
         Parameters
         ----------
-        taxa_id : str
-            A :class:`dwca.terms.taxon.TaxonID` to look for parents.
+        taxa_id : List[str]
+            A list of :class:`dwca.terms.taxon.TaxonID` to look for parents.
 
         Returns
         -------
-        List[str]
-            List of taxa ids.
+        Set[str]
+            Set of taxa ids.
         """
-        parent_taxa = list()
+        parent_taxa = set()
         try:
             df = self.pandas
-            current_taxa = df[df[TaxonID.name()] == taxa_id]
-            if len(current_taxa) != 1:
-                raise ValueError(f"{taxa_id} not found in data file.")
-            while len(current_taxa) == 1:
-                new_parent_found = current_taxa[ParentNameUsageID.name()].iloc[0]
-                if pd.notna(new_parent_found) and new_parent_found != "":
-                    parent_taxa.append(new_parent_found)
-                current_taxa = df[df[TaxonID.name()] == new_parent_found]
+            current_taxa = self.__get_rows__(taxa_id)
+            while len(current_taxa) > 0:
+                new_found_parents = current_taxa[ParentNameUsageID.name_cls()]
+                new_found_parents = new_found_parents[
+                    pd.notna(new_found_parents) &
+                    (new_found_parents != "")
+                ]
+                parent_taxa.update(list(new_found_parents))
+                current_taxa = df[df[TaxonID.name_cls()].isin(new_found_parents)]
         except ImportError:
-            entry = self.__get_entry__(**{TaxonID.name(): taxa_id})
-            if entry is None:
-                raise ValueError(f"{taxa_id} not found in data file.")
-            current = entry
-            while current is not None:
-                new_parent_found = getattr(current, ParentNameUsageID.name())
-                if new_parent_found is not None and new_parent_found != "":
-                    parent_taxa.append(new_parent_found)
-                current = self.__get_entry__(**{TaxonID.name(): new_parent_found})
+            entries = self.__get_rows__(taxa_id)
+            current_taxa = entries.copy()
+            while len(current_taxa) > 0:
+                new_found_parents = [getattr(current, ParentNameUsageID.name_cls()) for current in current_taxa]
+                new_found_parents = list(filter(
+                    lambda current: current != "" and current is not None,
+                    new_found_parents
+                ))
+                parent_taxa.update(new_found_parents)
+                current_taxa = self.__get_entries__(**{f"{TaxonID.name_cls()}__isin": new_found_parents})
         return parent_taxa
 
-    def all_synonyms(self, taxa_id: str, get_names: bool = False) -> List[str]:
+    def all_synonyms(self, taxa_id: Iterable[str], get_names: bool = False) -> List[str]:
         """
-        Get a list of all valid names of a taxon.
+        Get a list of all valid names of a list of taxa.
 
         Parameters
         ----------
-        taxa_id : str
-            A :class:`dwca.terms.taxon.TaxonID` value.
+        taxa_id : Iterable[str]
+            A list (or iterable) of :class:`dwca.terms.taxon.TaxonID` value.
         get_names : bool
             Whether to get :class:`dwca.terms.taxon.ScientificName` or :class:`dwca.terms.taxon.TaxonID`.
 
         Returns
         -------
         List[str]
             A list of :class:`dwca.terms.taxon.TaxonID`.
         """
         try:
             df = self.pandas
-            current_taxa = df[df[TaxonID.name()] == taxa_id]
-            if len(current_taxa) != 1:
-                raise ValueError(f"{taxa_id} not found in data file.")
-            accepted_name = current_taxa.iloc[0][AcceptedNameUsageID.name()]
+            current_taxa = self.__get_rows__(taxa_id)
+            accepted_names = current_taxa[AcceptedNameUsageID.name_cls()]
             return list(
-                df[df[AcceptedNameUsageID.name()] == accepted_name][
-                    ScientificName.name() if get_names else TaxonID.name()
+                df[df[AcceptedNameUsageID.name_cls()].isin(accepted_names)][
+                    ScientificName.name_cls() if get_names else TaxonID.name_cls()
                 ]
             )
         except ImportError:
-            entry = self.__get_entry__(**{TaxonID.name(): taxa_id})
-            if entry is None:
-                raise ValueError(f"{taxa_id} not found in data file.")
-            accepted_name = getattr(entry, AcceptedNameUsageID.name())
-            synonyms = self.__get_entries__(**{AcceptedNameUsageID.name(): accepted_name})
-            field = ScientificName.name() if get_names else TaxonID.name()
+            entries = self.__get_rows__(taxa_id)
+            accepted_names = [getattr(entry, AcceptedNameUsageID.name_cls()) for entry in entries]
+            synonyms = self.__get_entries__(**{f"{AcceptedNameUsageID.name_cls()}__isin": accepted_names})
+            field = ScientificName.name_cls() if get_names else TaxonID.name_cls()
             return [getattr(synonymous, field) for synonymous in synonyms]
 
+    def __get_rows__(self, taxa_id: List[str]) -> Union[pd.DataFrame, List[DataFile.Entry]]:
+        try:
+            df = self.pandas
+            current_taxa = df[df[TaxonID.name_cls()].isin(taxa_id)]
+            if len(current_taxa) != len(taxa_id):
+                candidates = pd.Series(taxa_id)
+                not_present = candidates[~candidates.isin(df[TaxonID.name_cls()])]
+                warn(f"{', '.join(list(not_present))} not found in data file.")
+            return current_taxa
+        except ImportError:
+            entries = self.__get_entries__(**{f"{TaxonID.name_cls()}__isin": taxa_id})
+            if len(entries) != len(taxa_id):
+                found_taxa = [getattr(entry, TaxonID.name_cls()) for entry in entries]
+                not_present = list(filter(lambda candid: candid not in found_taxa, taxa_id))
+                warn(f"{', '.join(not_present)} not found in data file.")
+            return entries
+
     def __get_entry__(self, **kwargs) -> DataFile.Entry | None:
         for candid in self.__entries__:
             found = True
             for key, value in kwargs.items():
                 found &= Taxon.__compare__(candid, key, value)
                 if not found:
                     break
@@ -304,13 +341,15 @@
                 if not found:
                     break
             if found:
                 results.append(candid)
         return results
 
     @staticmethod
-    def __compare__(candid: DataFile.Entry, key: str, value: str) -> bool:
+    def __compare__(candid: DataFile.Entry, key: str, value: Any) -> bool:
         match = re.match(r"(\w+)__case_insensitive$", key)
         if match:
             return getattr(candid, match.group(1)).lower() == value.lower()
-        else:
-            return getattr(candid, key) == value
+        match = re.match(r"(\w+)__isin$", key)
+        if match:
+            return getattr(candid, match.group(1)) in value
+        return getattr(candid, key) == value
```

### Comparing `pydwca-0.1.0/src/dwca/terms/__init__.py` & `pydwca-0.1.1/src/dwca/terms/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/chronometric_age.py` & `pydwca-0.1.1/src/dwca/terms/chronometric_age.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/event.py` & `pydwca-0.1.1/src/dwca/terms/event.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/field.py` & `pydwca-0.1.1/src/dwca/terms/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,31 @@
 
     @property
     def uri(self) -> str:
         """str: An URI for the term represented by this field."""
         return self.URI
 
     @classmethod
-    def name(cls) -> str:
+    def name_cls(cls) -> str:
         """str: The name of the field."""
         names = cls.URI.split("/")
         if len(names) > 1:
             return names[-1]
         else:
             return names[0]
 
+    @property
+    def name(self) -> str:
+        """str: The name of the field."""
+        names = self.uri.split("/")
+        if len(names) > 1:
+            return names[-1]
+        else:
+            return names[0]
+
     def format(self, value: str) -> TYPE:
         """
         Format value in the TYPE of the field.
 
         Parameters
         ----------
         value : str
```

### Comparing `pydwca-0.1.0/src/dwca/terms/geological_context.py` & `pydwca-0.1.1/src/dwca/terms/geological_context.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/identification.py` & `pydwca-0.1.1/src/dwca/terms/identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/location.py` & `pydwca-0.1.1/src/dwca/terms/location.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/material_entity.py` & `pydwca-0.1.1/src/dwca/terms/material_entity.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/material_sample.py` & `pydwca-0.1.1/src/dwca/terms/material_sample.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/measurement_or_fact.py` & `pydwca-0.1.1/src/dwca/terms/measurement_or_fact.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/occurrence.py` & `pydwca-0.1.1/src/dwca/terms/occurrence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/organism.py` & `pydwca-0.1.1/src/dwca/terms/organism.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/outside_term.py` & `pydwca-0.1.1/src/dwca/terms/outside_term.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/record_level.py` & `pydwca-0.1.1/src/dwca/terms/record_level.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/resource_relationship.py` & `pydwca-0.1.1/src/dwca/terms/resource_relationship.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/dwca/terms/taxon.py` & `pydwca-0.1.1/src/dwca/terms/taxon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/base/eml.py` & `pydwca-0.1.1/src/eml/base/eml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/base/metadata.py` & `pydwca-0.1.1/src/eml/base/metadata.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/base/version.py` & `pydwca-0.1.1/src/eml/base/version.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/citation.py` & `pydwca-0.1.1/src/eml/resources/citation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/dataset.py` & `pydwca-0.1.1/src/eml/resources/dataset.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/keyword_set.py` & `pydwca-0.1.1/src/eml/resources/keyword_set.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/licence.py` & `pydwca-0.1.1/src/eml/resources/licence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/protocol.py` & `pydwca-0.1.1/src/eml/resources/protocol.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/resource.py` & `pydwca-0.1.1/src/eml/resources/resource.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/resources.py` & `pydwca-0.1.1/src/eml/resources/resources.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/software.py` & `pydwca-0.1.1/src/eml/resources/software.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/coverage/coverage.py` & `pydwca-0.1.1/src/eml/resources/coverage/coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/coverage/geo_coverage.py` & `pydwca-0.1.1/src/eml/resources/coverage/geo_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/coverage/taxa_coverage.py` & `pydwca-0.1.1/src/eml/resources/coverage/taxa_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/coverage/time_coverage.py` & `pydwca-0.1.1/src/eml/resources/coverage/time_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/distribution/distribution.py` & `pydwca-0.1.1/src/eml/resources/distribution/distribution.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/distribution/inline.py` & `pydwca-0.1.1/src/eml/resources/distribution/inline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/distribution/offline.py` & `pydwca-0.1.1/src/eml/resources/distribution/offline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/resources/distribution/online.py` & `pydwca-0.1.1/src/eml/resources/distribution/online.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/__init__.py` & `pydwca-0.1.1/src/eml/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/access_type.py` & `pydwca-0.1.1/src/eml/types/access_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/address.py` & `pydwca-0.1.1/src/eml/types/address.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/eml_object.py` & `pydwca-0.1.1/src/eml/types/eml_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/extension_string.py` & `pydwca-0.1.1/src/eml/types/extension_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/extension_uri.py` & `pydwca-0.1.1/src/eml/types/extension_uri.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/i18n_string.py` & `pydwca-0.1.1/src/eml/types/i18n_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/individual_name.py` & `pydwca-0.1.1/src/eml/types/individual_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/no_tag_object.py` & `pydwca-0.1.1/src/eml/types/no_tag_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/organization_name.py` & `pydwca-0.1.1/src/eml/types/organization_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/phone.py` & `pydwca-0.1.1/src/eml/types/phone.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/position_name.py` & `pydwca-0.1.1/src/eml/types/position_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/responsible_party.py` & `pydwca-0.1.1/src/eml/types/responsible_party.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/section.py` & `pydwca-0.1.1/src/eml/types/section.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/semantic_annotation.py` & `pydwca-0.1.1/src/eml/types/semantic_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/eml/types/text_type.py` & `pydwca-0.1.1/src/eml/types/text_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/xml_object.py` & `pydwca-0.1.1/src/xml_common/xml_object.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/enum.py` & `pydwca-0.1.1/src/xml_common/utils/enum.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/establishment_means.py` & `pydwca-0.1.1/src/xml_common/utils/establishment_means.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/gpolygon.py` & `pydwca-0.1.1/src/xml_common/utils/gpolygon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/language.py` & `pydwca-0.1.1/src/xml_common/utils/language.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/length_unit.py` & `pydwca-0.1.1/src/xml_common/utils/length_unit.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/src/xml_common/utils/type_functions.py` & `pydwca-0.1.1/src/xml_common/utils/type_functions.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca/test_dwca.py` & `pydwca-0.1.1/tests/test_dwca/test_dwca.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca/test_dwca_no_pandas.py` & `pydwca-0.1.1/tests/test_dwca/test_dwca_no_pandas.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca/test_meta.py` & `pydwca-0.1.1/tests/test_dwca/test_meta.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_classes/test_identification.py` & `pydwca-0.1.1/tests/test_dwca_classes/test_identification.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_classes/test_outside_class.py` & `pydwca-0.1.1/tests/test_dwca_classes/test_outside_class.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_classes/test_taxon.py` & `pydwca-0.1.1/tests/test_dwca_classes/test_taxon.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,61 +47,65 @@
             "Kingdom must be in fields",
             taxon.filter_by_kingdom,
             []
         )
 
     def test_get_parents(self):
         self.read_pandas()
-        parents_set = self.taxon.get_parents("urn:lsid:example.org:taxname:360")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:360"])
         self.assertEqual(11, len(parents_set), "Incorrect number of parents.")
-        parents_set = self.taxon.get_parents("urn:lsid:example.org:taxname:366")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:366"])
+        self.assertEqual(14, len(parents_set), "Incorrect number of parents.")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:360", "urn:lsid:example.org:taxname:366"])
         self.assertEqual(14, len(parents_set), "Incorrect number of parents.")
 
     def test_get_incorrect_parent(self):
         self.read_pandas()
         taxa_id = "urn:lsid:example.org:taxname:300000"
-        self.assertRaisesRegex(
-            ValueError, taxa_id, self.taxon.get_parents, taxa_id
-        )
+        with self.assertWarnsRegex(UserWarning, taxa_id):
+            missing = self.taxon.get_parents([taxa_id])
+            self.assertEqual(0, len(missing), "Parent found of invalid taxon id")
 
     def test_get_synonyms(self):
         self.read_pandas()
-        first_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10000")
+        first_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10000"])
         self.assertEqual(2, len(first_synonyms), "Incorrect number of synonyms.")
-        second_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10001")
+        second_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10001"])
         self.assertEqual(2, len(second_synonyms), "Incorrect number of synonyms.")
         self.assertCountEqual(
             first_synonyms, second_synonyms, "Synonyms do not match"
         )
-        no_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:100005")
-        self.assertEqual(1, len(no_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
-        self.assertEqual("urn:lsid:example.org:taxname:100005", no_synonyms[0], "Incorrect same synonym")
+        two_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10000", "urn:lsid:example.org:taxname:100005"])
+        self.assertEqual(3, len(two_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
+        self.assertTrue("urn:lsid:example.org:taxname:100005" in two_synonyms, "Incorrect same synonym")
 
     def test_get_synonyms_names(self):
         self.read_pandas()
-        first_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10000", get_names=True)
+        first_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10000"], get_names=True)
         self.assertEqual(2, len(first_synonyms), "Incorrect number of synonyms.")
-        second_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10001", get_names=True)
+        second_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10001"], get_names=True)
         self.assertEqual(2, len(second_synonyms), "Incorrect number of synonyms.")
         self.assertCountEqual(
             first_synonyms, second_synonyms, "Synonyms do not match"
         )
-        no_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:100005", get_names=True)
-        self.assertEqual(1, len(no_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
-        self.assertEqual(
-            "Wxjncmbdqbd (Jdhbtbju) oojmaovly var. ushibyxcfc Whhngbhiq",
-            no_synonyms[0], "Incorrect same synonym"
+        two_synonyms = self.taxon.all_synonyms([
+            "urn:lsid:example.org:taxname:10000", "urn:lsid:example.org:taxname:100005"
+        ], get_names=True)
+        self.assertEqual(3, len(two_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
+        self.assertTrue(
+            "Wxjncmbdqbd (Jdhbtbju) oojmaovly var. ushibyxcfc Whhngbhiq" in two_synonyms,
+            "Incorrect same synonym"
         )
 
     def test_get_incorrect_synonyms(self):
         self.read_pandas()
         taxa_id = "urn:lsid:example.org:taxname:300000"
-        self.assertRaisesRegex(
-            ValueError, taxa_id, self.taxon.all_synonyms, taxa_id
-        )
+        with self.assertWarnsRegex(UserWarning, "urn:lsid:example.org:taxname:300000"):
+            synonyms = self.taxon.all_synonyms([taxa_id])
+            self.assertEqual(0, len(synonyms), "Found something of false taxon id.")
 
     def test_filter_kingdom(self):
         self.read_pandas()
         df = self.taxon.pandas
         length_df = len(df)
         kingdom_summary = df.groupby("kingdom").size().to_dict()
         print(f"Kingdom Summary: {kingdom_summary}", file=sys.stderr)
@@ -183,19 +187,16 @@
         print(f"Orders found: {order_names}", file=sys.stderr)
         self.assertEqual(length_df, len(self.taxon), "Original length of dataframe.")
         self.taxon.filter_by_order(orders)
         self.assertEqual(length_df, len(self.taxon), "Filter by all orders.")
         accepted = df[df["scientificName"] == "Rbaliuycliu"]["acceptedNameUsage"].iloc[0]
         with_order = sum(df["order"].isin(["Rbaliuycliu", "Xlhofowltm", accepted]))
         taxa_id = df[df["scientificName"].isin(["Rbaliuycliu", "Xlhofowltm", accepted])]["taxonID"]
-        parents = set()
-        for taxon in taxa_id:
-            parents.update(self.taxon.get_parents(taxon))
-        for parent in parents.copy():
-            parents.update(self.taxon.all_synonyms(parent))
+        parents = self.taxon.get_parents(taxa_id)
+        parents.update(self.taxon.all_synonyms(parents))
         parents = sum(df["taxonID"].isin(parents))
         print("Filtering by orders: Rbaliuycliu, Xlhofowltm", file=sys.stderr)
         print(f"Accepted orders: Rbaliuycliu, {accepted}", file=sys.stderr)
         self.taxon.filter_by_order(["Rbaliuycliu", "Xlhofowltm"])
         print(f"Expected: with order {with_order} and parents {parents}", file=sys.stderr)
         self.assertEqual(with_order + parents, len(self.taxon), "Incorrect filter.")
 
@@ -208,19 +209,16 @@
         print(f"Families found: {family_names}", file=sys.stderr)
         self.assertEqual(length_df, len(self.taxon), "Original length of dataframe.")
         self.taxon.filter_by_family(families)
         self.assertEqual(length_df, len(self.taxon), "Filter by all families.")
         accepted = df[df["scientificName"] == "Dxaougdpy"]["acceptedNameUsage"].iloc[0]
         with_family = sum(df["family"].isin(["Dxaougdpy", "Kvtgqwfmy", accepted]))
         taxa_id = df[df["scientificName"].isin(["Dxaougdpy", "Kvtgqwfmy", accepted])]["taxonID"]
-        parents = set()
-        for taxon in taxa_id:
-            parents.update(self.taxon.get_parents(taxon))
-        for parent in parents.copy():
-            parents.update(self.taxon.all_synonyms(parent))
+        parents = self.taxon.get_parents(taxa_id)
+        parents.update(self.taxon.all_synonyms(parents))
         parents = sum(df["taxonID"].isin(parents))
         print("Filtering by family: Dxaougdpy, Kvtgqwfmy", file=sys.stderr)
         print(f"Accepted families: Kvtgqwfmy, {accepted}", file=sys.stderr)
         self.taxon.filter_by_family(["Dxaougdpy", "Kvtgqwfmy"])
         print(f"Expected: with family {with_family} and parents {parents}", file=sys.stderr)
         self.assertEqual(with_family + parents, len(self.taxon), "Incorrect filter.")
 
@@ -233,19 +231,16 @@
         print(f"Genera found: {genus_names}", file=sys.stderr)
         self.assertEqual(length_df, len(self.taxon), "Original length of dataframe.")
         self.taxon.filter_by_genus(genera)
         self.assertEqual(length_df, len(self.taxon), "Filter by all genera.")
         accepted = df[df["scientificName"] == "Hbqrtfopjuh"]["acceptedNameUsage"].iloc[0]
         with_genus = sum(df["genus"].isin(["Hbqrtfopjuh", "Vbpjkmfqd", accepted]))
         taxa_id = df[df["scientificName"].isin(["Hbqrtfopjuh", "Vbpjkmfqd", accepted])]["taxonID"]
-        parents = set()
-        for taxon in taxa_id:
-            parents.update(self.taxon.get_parents(taxon))
-        for parent in parents.copy():
-            parents.update(self.taxon.all_synonyms(parent))
+        parents = self.taxon.get_parents(taxa_id)
+        parents.update(self.taxon.all_synonyms(parents))
         parents = sum(df["taxonID"].isin(parents))
         print("Filtering by genus: Hbqrtfopjuh, Vbpjkmfqd", file=sys.stderr)
         print(f"Accepted genera: Vbpjkmfqd, {accepted}", file=sys.stderr)
         self.taxon.filter_by_genus(["Hbqrtfopjuh", "Vbpjkmfqd"])
         print(f"Expected: with genus {with_genus} and parents {parents}", file=sys.stderr)
         self.assertEqual(with_genus + parents, len(self.taxon), "Incorrect filter.")
 
@@ -258,26 +253,30 @@
         variety = "Rtfkiaicpdng obzninluz var. cebwyzcqoy Glhnskwn"
         cultivar = "Rtfkiaicpdng (Abifwvxqn) gurqtwpof f. prczacpvtdtu 'xzhgezqpaorp'"
         synonyms = set()
         species_row = df[df["scientificName"] == species_synonym].iloc[0]
         accepted = species_row["acceptedNameUsageID"]
         synonyms.add(accepted)
         synonyms.add(species_row["taxonID"])
-        first_parents = self.taxon.get_parents(accepted)
+        first_parents = self.taxon.get_parents([accepted])
         print(f"For {species_synonym} expected {len(first_parents)} parents, accepted and synonym", file=sys.stderr)
         variety_id = df[df["scientificName"] == variety]["taxonID"].iloc[0]
-        second_parents = self.taxon.get_parents(variety_id)
+        second_parents = self.taxon.get_parents([variety_id])
         synonyms.add(variety_id)
         print(f"For {variety} expected {len(second_parents)} parents and self", file=sys.stderr)
         cultivar_id = df[df["scientificName"] == cultivar]["taxonID"].iloc[0]
-        third_parents = self.taxon.get_parents(cultivar_id)
+        third_parents = self.taxon.get_parents([cultivar_id])
         synonyms.add(cultivar_id)
         print(f"For {cultivar} expected {len(third_parents)} parents", file=sys.stderr)
-        for taxon in list(synonyms.copy()) + first_parents + second_parents + third_parents:
-            synonyms.update(self.taxon.all_synonyms(taxon))
+        synonyms.update(self.taxon.all_synonyms(
+            list(synonyms.copy()) +
+            list(first_parents) +
+            list(second_parents) +
+            list(third_parents)
+        ))
         other_synonyms = synonyms.difference({species_synonym, variety, cultivar})
         other_synonyms = other_synonyms.difference(set(first_parents))
         other_synonyms = other_synonyms.difference(set(second_parents))
         other_synonyms = other_synonyms.difference(set(third_parents))
         print(f"Synonyms found: {len(other_synonyms)}", file=sys.stderr)
         print(f"Total {len(synonyms)}", file=sys.stderr)
         self.taxon.filter_by_species([species_synonym, variety, cultivar])
```

### Comparing `pydwca-0.1.0/tests/test_dwca_classes/test_taxon_no_pandas.py` & `pydwca-0.1.1/tests/test_dwca_classes/test_taxon_no_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,61 +42,66 @@
         self.assertEqual(1, taxon.__ignore_header_lines__, "Ignore header parse incorrectly")
         self.assertEqual(Taxon.URI, taxon.uri, "Row type parse incorrectly")
         self.assertEqual(47, len(taxon.__fields__), "Fields parse incorrectly")
         self.assertEqualTree(self.taxon_xml, taxon.to_element(), "Error on element conversion")
 
     def test_get_parents(self):
         self.read_pandas()
-        parents_set = self.taxon.get_parents("urn:lsid:example.org:taxname:360")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:360"])
         self.assertEqual(11, len(parents_set), "Incorrect number of parents.")
-        parents_set = self.taxon.get_parents("urn:lsid:example.org:taxname:366")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:366"])
+        self.assertEqual(14, len(parents_set), "Incorrect number of parents.")
+        parents_set = self.taxon.get_parents(["urn:lsid:example.org:taxname:360", "urn:lsid:example.org:taxname:366"])
         self.assertEqual(14, len(parents_set), "Incorrect number of parents.")
 
     def test_get_incorrect_parent(self):
         self.read_pandas()
         taxa_id = "urn:lsid:example.org:taxname:300000"
-        self.assertRaisesRegex(
-            ValueError, taxa_id, self.taxon.get_parents, taxa_id
-        )
+        with self.assertWarnsRegex(UserWarning, taxa_id):
+            missing = self.taxon.get_parents([taxa_id])
+            self.assertEqual(0, len(missing), "Parent found of invalid taxon id")
 
     def test_get_synonyms(self):
         self.read_pandas()
-        first_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10000")
+        first_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10000"])
         self.assertEqual(2, len(first_synonyms), "Incorrect number of synonyms.")
-        second_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10001")
+        second_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10001"])
         self.assertEqual(2, len(second_synonyms), "Incorrect number of synonyms.")
         self.assertCountEqual(
             first_synonyms, second_synonyms, "Synonyms do not match"
         )
-        no_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:100005")
-        self.assertEqual(1, len(no_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
-        self.assertEqual("urn:lsid:example.org:taxname:100005", no_synonyms[0], "Incorrect same synonym")
+        two_synonyms = self.taxon.all_synonyms(
+            ["urn:lsid:example.org:taxname:10000", "urn:lsid:example.org:taxname:100005"])
+        self.assertEqual(3, len(two_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
+        self.assertTrue("urn:lsid:example.org:taxname:100005" in two_synonyms, "Incorrect same synonym")
 
     def test_get_synonyms_names(self):
         self.read_pandas()
-        first_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10000", get_names=True)
+        first_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10000"], get_names=True)
         self.assertEqual(2, len(first_synonyms), "Incorrect number of synonyms.")
-        second_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:10001", get_names=True)
+        second_synonyms = self.taxon.all_synonyms(["urn:lsid:example.org:taxname:10001"], get_names=True)
         self.assertEqual(2, len(second_synonyms), "Incorrect number of synonyms.")
         self.assertCountEqual(
             first_synonyms, second_synonyms, "Synonyms do not match"
         )
-        no_synonyms = self.taxon.all_synonyms("urn:lsid:example.org:taxname:100005", get_names=True)
-        self.assertEqual(1, len(no_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
-        self.assertEqual(
-            "Wxjncmbdqbd (Jdhbtbju) oojmaovly var. ushibyxcfc Whhngbhiq",
-            no_synonyms[0], "Incorrect same synonym"
+        two_synonyms = self.taxon.all_synonyms([
+            "urn:lsid:example.org:taxname:10000", "urn:lsid:example.org:taxname:100005"
+        ], get_names=True)
+        self.assertEqual(3, len(two_synonyms), "Incorrect number of synonym with a taxa with no synonymous.")
+        self.assertTrue(
+            "Wxjncmbdqbd (Jdhbtbju) oojmaovly var. ushibyxcfc Whhngbhiq" in two_synonyms,
+            "Incorrect same synonym"
         )
 
     def test_get_incorrect_synonyms(self):
         self.read_pandas()
         taxa_id = "urn:lsid:example.org:taxname:300000"
-        self.assertRaisesRegex(
-            ValueError, taxa_id, self.taxon.all_synonyms, taxa_id
-        )
+        with self.assertWarnsRegex(UserWarning, "urn:lsid:example.org:taxname:300000"):
+            synonyms = self.taxon.all_synonyms([taxa_id])
+            self.assertEqual(0, len(synonyms), "Found something of false taxon id.")
 
     def test_filter_kingdom(self):
         self.read_pandas()
         length = len(self.taxon)
         self.assertEqual(length, len(self.taxon), "Original length of dataframe.")
         self.taxon.filter_by_kingdom(["Ydhxpqku", "Zcmmvusczo"])
         self.assertEqual(length, len(self.taxon), "Filter by all kingdoms.")
```

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_any_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_any_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_datetime_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_datetime_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_float_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_float_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_int_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_int_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_list_str_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_list_str_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_outside_term.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_outside_term.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_str_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_str_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_taxon.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_taxon.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_union_datetime_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_union_datetime_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_dwca_terms/test_union_field.py` & `pydwca-0.1.1/tests/test_dwca_terms/test_union_field.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_access_type.py` & `pydwca-0.1.1/tests/test_eml/test_access_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_address.py` & `pydwca-0.1.1/tests/test_eml/test_address.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_annotation.py` & `pydwca-0.1.1/tests/test_eml/test_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_citation.py` & `pydwca-0.1.1/tests/test_eml/test_citation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_dataset.py` & `pydwca-0.1.1/tests/test_eml/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_eml.py` & `pydwca-0.1.1/tests/test_eml/test_eml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_extension.py` & `pydwca-0.1.1/tests/test_eml/test_extension.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_extension_uri.py` & `pydwca-0.1.1/tests/test_eml/test_extension_uri.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_i18n_string.py` & `pydwca-0.1.1/tests/test_eml/test_i18n_string.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_individual_name.py` & `pydwca-0.1.1/tests/test_eml/test_individual_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_keyword_set.py` & `pydwca-0.1.1/tests/test_eml/test_keyword_set.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_licence.py` & `pydwca-0.1.1/tests/test_eml/test_licence.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_metadata.py` & `pydwca-0.1.1/tests/test_eml/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_organization_name.py` & `pydwca-0.1.1/tests/test_eml/test_organization_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_phone.py` & `pydwca-0.1.1/tests/test_eml/test_phone.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_position_name.py` & `pydwca-0.1.1/tests/test_eml/test_position_name.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_responsible_party.py` & `pydwca-0.1.1/tests/test_eml/test_responsible_party.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_section.py` & `pydwca-0.1.1/tests/test_eml/test_section.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_semantic_annotation.py` & `pydwca-0.1.1/tests/test_eml/test_semantic_annotation.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml/test_text_type.py` & `pydwca-0.1.1/tests/test_eml/test_text_type.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_coverage/test_coverage.py` & `pydwca-0.1.1/tests/test_eml_coverage/test_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_coverage/test_geo_coverage.py` & `pydwca-0.1.1/tests/test_eml_coverage/test_geo_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_coverage/test_taxa_coverage.py` & `pydwca-0.1.1/tests/test_eml_coverage/test_taxa_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_coverage/test_time_coverage.py` & `pydwca-0.1.1/tests/test_eml_coverage/test_time_coverage.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_distribution/test_distribution.py` & `pydwca-0.1.1/tests/test_eml_distribution/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_distribution/test_inline.py` & `pydwca-0.1.1/tests/test_eml_distribution/test_inline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_distribution/test_offline.py` & `pydwca-0.1.1/tests/test_eml_distribution/test_offline.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_eml_distribution/test_online.py` & `pydwca-0.1.1/tests/test_eml_distribution/test_online.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_util/test_establishment_means.py` & `pydwca-0.1.1/tests/test_util/test_establishment_means.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_util/test_format.py` & `pydwca-0.1.1/tests/test_util/test_format.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_util/test_unformat.py` & `pydwca-0.1.1/tests/test_util/test_unformat.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_xml/test_simple_xml.py` & `pydwca-0.1.1/tests/test_xml/test_simple_xml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/tests/test_xml/test_xml.py` & `pydwca-0.1.1/tests/test_xml/test_xml.py`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/.gitignore` & `pydwca-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/LICENSE` & `pydwca-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/README.md` & `pydwca-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydwca-0.1.0/pyproject.toml` & `pydwca-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydwca"
-version = "0.1.0"
+version = "0.1.1"
 dynamic = ["dependencies"]
 description = 'Python library to read, parse and write Darwin Core Archive files'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MPL-2.0"
 license-files = { paths = ["LICENSE"] }
 keywords = []
```

### Comparing `pydwca-0.1.0/PKG-INFO` & `pydwca-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydwca
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library to read, parse and write Darwin Core Archive files
 Project-URL: Documentation, https://pydwca.readthedocs.io/en/latest/index.html
 Project-URL: Issues, https://github.com/IEB-BIODATA/pydwca/issues
 Project-URL: Source, https://github.com/IEB-BIODATA/pydwca
 Author-email: Juan Saez Hidalgo <jmsaez@ieb-chile.cl>
 License-Expression: MPL-2.0
 License-File: LICENSE
```

