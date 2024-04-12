# Comparing `tmp/nrel_pypsse-1.1.2.tar.gz` & `tmp/nrel_pypsse-1.1.3.tar.gz`

## Comparing `nrel_pypsse-1.1.2.tar` & `nrel_pypsse-1.1.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/__init__.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/channel_map.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/common.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/compile.bat
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/conec.flx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/conet.flx
--rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/contingencies.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/custom_logger.py
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/enumerations.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/exceptions.py
--rw-r--r--   0        0        0    20618 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/helics_interface.py
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/mdao_interface.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/models.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/project.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/result_container.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/simulation_controller.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/simulator.py
--rw-r--r--   0        0        0    18413 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/PSSE.v2.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/common.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/config.yaml
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/app/__init__.py
--rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/app/psse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/web/__init__.py
--rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/api/web/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/__init__.py
--rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/create_profiles.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/create_project.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/explore.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/pypsse.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/run.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/cli/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/fixed_shunt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/machine.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/switched_shunt.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/components/transformer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/__init__.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/csv.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/data_writer.py
--rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/hdf5.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/data_writers/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/__init__.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/export_settings.toml
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/defaults/simulation_settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/__init__.py
--rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/abstract_mode.py
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/constants.py
--rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/dynamic.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/pcm.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/snap.py
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/modes/static.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/__init__.py
--rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/gic_parser.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/parsers/reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/__init__.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/common.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/profile.py
--rw-r--r--   0        0        0    10687 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/profile_manager/profile_store.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/__init__.py
--rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dynamic_utils.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/__init__.py
--rw-r--r--   0        0        0    33318 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/dc_ac_algorithm.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pypsse/utils/dc2ac/helper_functions.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/LICENSE
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/README.md
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/__init__.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/channel_map.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/common.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/compile.bat
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/conec.flx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/conet.flx
+-rw-r--r--   0        0        0     8316 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/contingencies.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/custom_logger.py
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/enumerations.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/exceptions.py
+-rw-r--r--   0        0        0    20618 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/helics_interface.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/mdao_interface.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/models.py
+-rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/project.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/result_container.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/simulation_controller.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/simulator.py
+-rw-r--r--   0        0        0    18413 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/PSSE.v2.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/common.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/config.yaml
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/app/__init__.py
+-rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/app/psse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/web/__init__.py
+-rw-r--r--   0        0        0    11463 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/api/web/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/__init__.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/create_profiles.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/create_project.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/explore.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/pypsse.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/run.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/cli/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/fixed_shunt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/machine.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/switched_shunt.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/system.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/components/transformer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/data_writers/__init__.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/data_writers/csv.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/data_writers/data_writer.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/data_writers/hdf5.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/data_writers/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/defaults/__init__.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/defaults/export_settings.toml
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/defaults/simulation_settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/__init__.py
+-rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/abstract_mode.py
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/constants.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/dynamic.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/pcm.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/snap.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/modes/static.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/parsers/__init__.py
+-rw-r--r--   0        0        0     6416 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/parsers/gic_parser.py
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/parsers/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/profile_manager/__init__.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/profile_manager/common.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/profile_manager/profile.py
+-rw-r--r--   0        0        0    10687 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/profile_manager/profile_store.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/__init__.py
+-rw-r--r--   0        0        0    14515 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/dynamic_utils.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/dc2ac/__init__.py
+-rw-r--r--   0        0        0    33318 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/dc2ac/dc_ac_algorithm.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pypsse/utils/dc2ac/helper_functions.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/README.md
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 nrel_pypsse-1.1.3/PKG-INFO
```

### Comparing `nrel_pypsse-1.1.2/pypsse/channel_map.py` & `nrel_pypsse-1.1.3/pypsse/channel_map.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/common.py` & `nrel_pypsse-1.1.3/pypsse/common.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/compile.bat` & `nrel_pypsse-1.1.3/pypsse/compile.bat`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/contingencies.py` & `nrel_pypsse-1.1.3/pypsse/contingencies.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/custom_logger.py` & `nrel_pypsse-1.1.3/pypsse/custom_logger.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/enumerations.py` & `nrel_pypsse-1.1.3/pypsse/enumerations.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/helics_interface.py` & `nrel_pypsse-1.1.3/pypsse/helics_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/mdao_interface.py` & `nrel_pypsse-1.1.3/pypsse/mdao_interface.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/models.py` & `nrel_pypsse-1.1.3/pypsse/models.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/project.py` & `nrel_pypsse-1.1.3/pypsse/project.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/result_container.py` & `nrel_pypsse-1.1.3/pypsse/result_container.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/simulation_controller.py` & `nrel_pypsse-1.1.3/pypsse/simulation_controller.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/simulator.py` & `nrel_pypsse-1.1.3/pypsse/simulator.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/api/PSSE.v2.json` & `nrel_pypsse-1.1.3/pypsse/api/PSSE.v2.json`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/api/server.py` & `nrel_pypsse-1.1.3/pypsse/api/server.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/api/app/psse.py` & `nrel_pypsse-1.1.3/pypsse/api/app/psse.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/api/web/handler.py` & `nrel_pypsse-1.1.3/pypsse/api/web/handler.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/cli/create_profiles.py` & `nrel_pypsse-1.1.3/pypsse/cli/create_profiles.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/cli/create_project.py` & `nrel_pypsse-1.1.3/pypsse/cli/create_project.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/cli/explore.py` & `nrel_pypsse-1.1.3/pypsse/cli/explore.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/cli/pypsse.py` & `nrel_pypsse-1.1.3/pypsse/cli/pypsse.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/cli/run.py` & `nrel_pypsse-1.1.3/pypsse/cli/run.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/data_writers/csv.py` & `nrel_pypsse-1.1.3/pypsse/data_writers/csv.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/data_writers/data_writer.py` & `nrel_pypsse-1.1.3/pypsse/data_writers/data_writer.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/data_writers/hdf5.py` & `nrel_pypsse-1.1.3/pypsse/data_writers/hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,18 @@
                 self.store_groups[obj_type] = self.store.create_group(obj_type)
                 self.store_datasets[obj_type] = {}
                 for col_name in powerflow_output[obj_type].keys():
                     dtype = data[col_name].dtype
                     if dtype == object:
                         dtype = "S30"
 
-                    self.store_datasets[obj_type][col_name] = self.store_groups[
+                    self.store_datasets[obj_type][self.column_name(col_name)] = self.store_groups[
                         obj_type
                     ].create_dataset(
-                        str(col_name),
+                        self.column_name(col_name),
                         shape=(self.column_length,),
                         maxshape=(None,),
                         chunks=True,
                         compression="gzip",
                         compression_opts=4,
                         shuffle=True,
                         dtype=dtype,
@@ -105,39 +105,42 @@
                         data, ignore_index=True
                     )
 
             if self.step % self.chunkRows == self.chunkRows - 1:
                 si = int(self.step / self.chunkRows) * self.chunkRows
                 ei = si + self.chunkRows
                 for col_name in powerflow_output[obj_type].keys():
-                    r = self.store_datasets[obj_type][col_name].shape[0]
+                    r = self.store_datasets[obj_type][self.column_name(col_name)].shape[0]
                     if ei >= r:
-                        self.store_datasets[obj_type][col_name].resize((ei,))
-                    self.store_datasets[obj_type][col_name][si:ei] = self.dfs[
+                        self.store_datasets[obj_type][self.column_name(col_name)].resize((ei,))
+                    self.store_datasets[obj_type][self.column_name(col_name)][si:ei] = self.dfs[
                         obj_type
                     ][col_name]
                 self.dfs[obj_type] = None
             if self.step >= len(self.Timestamp):
                 self.Timestamp.resize((len(self.Timestamp) + 1,))
                 self.convergence.resize((len(self.convergence) + 1,))
             self.Timestamp[self.step - 1] = np.string_(currenttime.strftime("%Y-%m-%d %H:%M:%S.%f"))
             self.convergence[self.step - 1] = convergence
             # Add object status data to a DataFrame
             self.store.flush()
         self.step += 1
 
+    def column_name(self, column_name:str)-> str:
+        return str(column_name).replace(" ", "")
+
     def close_store(self):
         try:
             k = list(self.dfs.keys())[0]
             if self.dfs[k] is not None:
                 length = len(self.dfs[k])
                 if length > 0:
                     for obj_type in self.dfs.keys():
                         for col_name in self.dfs[k].columns:
-                            self.store_datasets[obj_type][col_name][
+                            self.store_datasets[obj_type][self.column_name(col_name)][
                                 self.column_length - length :
                             ] = self.dfs[obj_type][col_name]
 
             self.store.flush()
             self.store.close()
         except Exception as e:
             logger.info(str(e))
```

### Comparing `nrel_pypsse-1.1.2/pypsse/data_writers/json.py` & `nrel_pypsse-1.1.3/pypsse/data_writers/json.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/defaults/export_settings.toml` & `nrel_pypsse-1.1.3/pypsse/defaults/export_settings.toml`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/defaults/simulation_settings.toml` & `nrel_pypsse-1.1.3/pypsse/defaults/simulation_settings.toml`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/abstract_mode.py` & `nrel_pypsse-1.1.3/pypsse/modes/abstract_mode.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/constants.py` & `nrel_pypsse-1.1.3/pypsse/modes/constants.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/dynamic.py` & `nrel_pypsse-1.1.3/pypsse/modes/dynamic.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/pcm.py` & `nrel_pypsse-1.1.3/pypsse/modes/pcm.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/snap.py` & `nrel_pypsse-1.1.3/pypsse/modes/snap.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/modes/static.py` & `nrel_pypsse-1.1.3/pypsse/modes/static.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/parsers/gic_parser.py` & `nrel_pypsse-1.1.3/pypsse/parsers/gic_parser.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/parsers/reader.py` & `nrel_pypsse-1.1.3/pypsse/parsers/reader.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/profile_manager/common.py` & `nrel_pypsse-1.1.3/pypsse/profile_manager/common.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/profile_manager/profile.py` & `nrel_pypsse-1.1.3/pypsse/profile_manager/profile.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/profile_manager/profile_store.py` & `nrel_pypsse-1.1.3/pypsse/profile_manager/profile_store.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/utils/dynamic_utils.py` & `nrel_pypsse-1.1.3/pypsse/utils/dynamic_utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/utils/utils.py` & `nrel_pypsse-1.1.3/pypsse/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/utils/dc2ac/dc_ac_algorithm.py` & `nrel_pypsse-1.1.3/pypsse/utils/dc2ac/dc_ac_algorithm.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pypsse/utils/dc2ac/helper_functions.py` & `nrel_pypsse-1.1.3/pypsse/utils/dc2ac/helper_functions.py`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/.gitignore` & `nrel_pypsse-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/LICENSE` & `nrel_pypsse-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/README.md` & `nrel_pypsse-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/pyproject.toml` & `nrel_pypsse-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nrel_pypsse-1.1.2/PKG-INFO` & `nrel_pypsse-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NREL-pypsse
-Version: 1.1.2
+Version: 1.1.3
 Summary: A high-level python interface for PSS/E
 Project-URL: Homepage, http://www.github.com/nrel/pypsse
 Author-email: Aadil Latif <Aadil.Latif@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

