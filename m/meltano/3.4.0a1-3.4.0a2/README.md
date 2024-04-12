# Comparing `tmp/meltano-3.4.0a1.tar.gz` & `tmp/meltano-3.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltano-3.4.0a1.tar", max compression
+gzip compressed data, was "meltano-3.4.0a2.tar", max compression
```

## Comparing `meltano-3.4.0a1.tar` & `meltano-3.4.0a2.tar`

### file list

```diff
@@ -1,298 +1,298 @@
--rw-r--r--   0        0        0     1048 2024-04-03 20:47:33.568166 meltano-3.4.0a1/LICENSE
--rw-r--r--   0        0        0     5237 2024-04-03 20:47:33.568166 meltano-3.4.0a1/README.md
--rw-r--r--   0        0        0    19356 2024-04-03 20:47:33.704166 meltano-3.4.0a1/pyproject.toml
--rw-r--r--   0        0        0      100 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/__init__.py
--rw-r--r--   0        0        0     3631 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/__init__.py
--rw-r--r--   0        0        0       73 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/__main__.py
--rw-r--r--   0        0        0     6770 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/add.py
--rw-r--r--   0        0        0     6006 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/cli.py
--rw-r--r--   0        0        0     3806 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/compile.py
--rw-r--r--   0        0        0    14489 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/config.py
--rw-r--r--   0        0        0      406 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/docs.py
--rw-r--r--   0        0        0      507 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/dragon.py
--rw-r--r--   0        0        0    17244 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/elt.py
--rw-r--r--   0        0        0     2548 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/environment.py
--rw-r--r--   0        0        0     1671 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/hub.py
--rw-r--r--   0        0        0     2221 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/initialize.py
--rw-r--r--   0        0        0     4100 2024-04-03 20:47:33.704166 meltano-3.4.0a1/src/meltano/cli/install.py
--rw-r--r--   0        0        0      181 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/__init__.py
--rw-r--r--   0        0        0    16395 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/config.py
--rw-r--r--   0        0        0      241 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/interactive/utils.py
--rw-r--r--   0        0        0     6275 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/invoke.py
--rw-r--r--   0        0        0    10060 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/job.py
--rw-r--r--   0        0        0     3804 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/lock.py
--rw-r--r--   0        0        0     2242 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/params.py
--rw-r--r--   0        0        0     2789 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/remove.py
--rw-r--r--   0        0        0     7299 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/run.py
--rw-r--r--   0        0        0    12993 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/schedule.py
--rw-r--r--   0        0        0      770 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/schema.py
--rw-r--r--   0        0        0     4446 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/select.py
--rw-r--r--   0        0        0    10590 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/state.py
--rw-r--r--   0        0        0     4344 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/upgrade.py
--rw-r--r--   0        0        0    23965 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/utils.py
--rw-r--r--   0        0        0     4185 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/cli/validate.py
--rw-r--r--   0        0        0        0 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/__init__.py
--rw-r--r--   0        0        0       64 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/__init__.py
--rw-r--r--   0        0        0    13060 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/canonical.py
--rw-r--r--   0        0        0     3962 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/hookable.py
--rw-r--r--   0        0        0      192 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/name_eq.py
--rw-r--r--   0        0        0     1187 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/versioned.py
--rw-r--r--   0        0        0      406 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/behavior/visitor.py
--rw-r--r--   0        0        0      117 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/__init__.py
--rw-r--r--   0        0        0     1582 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/blockset.py
--rw-r--r--   0        0        0    29706 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/extract_load.py
--rw-r--r--   0        0        0     2705 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/future_utils.py
--rw-r--r--   0        0        0     3946 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/ioblock.py
--rw-r--r--   0        0        0    11236 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/parser.py
--rw-r--r--   0        0        0     5745 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/plugin_command.py
--rw-r--r--   0        0        0    12176 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/block/singer.py
--rw-r--r--   0        0        0      128 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/__init__.py
--rw-r--r--   0        0        0      460 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/initialize.yml
--rw-r--r--   0        0        0     2625 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/bundle/settings.yml
--rw-r--r--   0        0        0    10326 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/cli_messages.py
--rw-r--r--   0        0        0     3094 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/config_service.py
--rw-r--r--   0        0        0       81 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/__init__.py
--rw-r--r--   0        0        0     2130 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/container_service.py
--rw-r--r--   0        0        0     2997 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/container/container_spec.py
--rw-r--r--   0        0        0     7391 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/db.py
--rw-r--r--   0        0        0    14930 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/elt_context.py
--rw-r--r--   0        0        0     6924 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/environment.py
--rw-r--r--   0        0        0     2797 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/environment_service.py
--rw-r--r--   0        0        0     3747 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/error.py
--rw-r--r--   0        0        0      181 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/__init__.py
--rw-r--r--   0        0        0    11085 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/client.py
--rw-r--r--   0        0        0      896 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/hub/schema.py
--rw-r--r--   0        0        0      103 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/__init__.py
--rw-r--r--   0        0        0     5940 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/finder.py
--rw-r--r--   0        0        0    11544 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/job.py
--rw-r--r--   0        0        0     1036 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job/stale_job_failer.py
--rw-r--r--   0        0        0     6015 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/job_state.py
--rw-r--r--   0        0        0     2974 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/locked_definition_service.py
--rw-r--r--   0        0        0      699 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/__init__.py
--rw-r--r--   0        0        0     4530 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/formatters.py
--rw-r--r--   0        0        0     5573 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/job_logging_service.py
--rw-r--r--   0        0        0     7367 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/output_logger.py
--rw-r--r--   0        0        0     7084 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/logging/utils.py
--rw-r--r--   0        0        0     3453 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/__init__.py
--rw-r--r--   0        0        0      365 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/cache.py
--rw-r--r--   0        0        0     4835 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/contexts.py
--rw-r--r--   0        0        0     4867 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/jsonschema.py
--rw-r--r--   0        0        0    18190 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/manifest/manifest.py
--rw-r--r--   0        0        0     5137 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/meltano_file.py
--rw-r--r--   0        0        0     2679 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/meltano_invoker.py
--rw-r--r--   0        0        0     3665 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/migration_service.py
--rw-r--r--   0        0        0      481 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/models.py
--rw-r--r--   0        0        0      188 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/__init__.py
--rw-r--r--   0        0        0     5707 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/airflow.py
--rw-r--r--   0        0        0    27344 2024-04-03 20:47:33.708166 meltano-3.4.0a1/src/meltano/core/plugin/base.py
--rw-r--r--   0        0        0     3638 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/command.py
--rw-r--r--   0        0        0     1422 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/config_service.py
--rw-r--r--   0        0        0      139 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/dbt/__init__.py
--rw-r--r--   0        0        0     4072 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/dbt/base.py
--rw-r--r--   0        0        0     2703 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/error.py
--rw-r--r--   0        0        0     1849 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/factory.py
--rw-r--r--   0        0        0     9890 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/file.py
--rw-r--r--   0        0        0     2708 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/meltano_file.py
--rw-r--r--   0        0        0    14822 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/project_plugin.py
--rw-r--r--   0        0        0     1135 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/requirements.py
--rw-r--r--   0        0        0     7651 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/settings_service.py
--rw-r--r--   0        0        0      282 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/base.py
--rw-r--r--   0        0        0    19585 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/catalog.py
--rw-r--r--   0        0        0     2362 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/mapper.py
--rw-r--r--   0        0        0    23536 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/tap.py
--rw-r--r--   0        0        0     5573 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/singer/target.py
--rw-r--r--   0        0        0     5850 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/superset.py
--rw-r--r--   0        0        0      269 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin/utility.py
--rw-r--r--   0        0        0    16700 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_install_service.py
--rw-r--r--   0        0        0    17248 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_invoker.py
--rw-r--r--   0        0        0     6473 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_location_remove.py
--rw-r--r--   0        0        0     3931 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_lock_service.py
--rw-r--r--   0        0        0     2817 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_remove_service.py
--rw-r--r--   0        0        0     2180 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_repository.py
--rw-r--r--   0        0        0     3289 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/plugin_test_service.py
--rw-r--r--   0        0        0    20306 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project.py
--rw-r--r--   0        0        0     3999 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_add_service.py
--rw-r--r--   0        0        0    14180 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_files.py
--rw-r--r--   0        0        0     6581 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_init_service.py
--rw-r--r--   0        0        0    18330 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_plugins_service.py
--rw-r--r--   0        0        0     5118 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/project_settings_service.py
--rw-r--r--   0        0        0      262 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/dbt.py
--rw-r--r--   0        0        0    10141 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/runner/singer.py
--rw-r--r--   0        0        0     3769 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/schedule.py
--rw-r--r--   0        0        0    10918 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/schedule_service.py
--rw-r--r--   0        0        0     3384 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/select_service.py
--rw-r--r--   0        0        0      926 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/setting.py
--rw-r--r--   0        0        0    15081 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/setting_definition.py
--rw-r--r--   0        0        0    21245 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/settings_service.py
--rw-r--r--   0        0        0    46397 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/settings_store.py
--rw-r--r--   0        0        0     2573 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/sqlalchemy.py
--rw-r--r--   0        0        0     7282 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_service.py
--rw-r--r--   0        0        0     3728 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/__init__.py
--rw-r--r--   0        0        0     5482 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/azure.py
--rw-r--r--   0        0        0     2134 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/base.py
--rw-r--r--   0        0        0     3831 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/db.py
--rw-r--r--   0        0        0    17948 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/filesystem.py
--rw-r--r--   0        0        0     4170 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/google.py
--rw-r--r--   0        0        0     4860 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/state_store/s3.py
--rw-r--r--   0        0        0     4461 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/task_sets.py
--rw-r--r--   0        0        0     3993 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/task_sets_service.py
--rw-r--r--   0        0        0        0 2024-04-03 20:47:55.036203 meltano-3.4.0a1/src/meltano/core/tracking/.release_marker
--rw-r--r--   0        0        0     3614 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/README.md
--rw-r--r--   0        0        0      125 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/__init__.py
--rw-r--r--   0        0        0      470 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/cli.py
--rw-r--r--   0        0        0     6044 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/environment.py
--rw-r--r--   0        0        0     3790 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/exception.py
--rw-r--r--   0        0        0     4948 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/plugins.py
--rw-r--r--   0        0        0     4128 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/contexts/project.py
--rw-r--r--   0        0        0      918 2024-04-03 20:47:33.712166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1051 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1194 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
--rw-r--r--   0        0        0      720 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      748 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     6002 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     6501 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     6963 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
--rw-r--r--   0        0        0     7408 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
--rw-r--r--   0        0        0     4449 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     1403 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
--rw-r--r--   0        0        0     1462 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
--rw-r--r--   0        0        0     3920 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2109 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
--rw-r--r--   0        0        0     2812 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
--rw-r--r--   0        0        0     1202 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
--rw-r--r--   0        0        0      404 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/iglu.json
--rw-r--r--   0        0        0     9688 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/micro.conf
--rw-r--r--   0        0        0     1112 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/schemas.py
--rw-r--r--   0        0        0    18604 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/tracking/tracker.py
--rw-r--r--   0        0        0     3562 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/transform_add_service.py
--rw-r--r--   0        0        0     7708 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/upgrade_service.py
--rw-r--r--   0        0        0    25155 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/utils/__init__.py
--rw-r--r--   0        0        0     1451 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/utils/pidfile.py
--rw-r--r--   0        0        0     4105 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/validation_service.py
--rw-r--r--   0        0        0    15701 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/venv_service.py
--rw-r--r--   0        0        0     1521 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/core/yaml.py
--rw-r--r--   0        0        0      508 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/__init__.py
--rw-r--r--   0        0        0       12 2024-04-03 20:47:54.964203 meltano-3.4.0a1/src/meltano/migrations/db.lock
--rw-r--r--   0        0        0     1490 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/env.py
--rw-r--r--   0        0        0      495 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/script.py.mako
--rw-r--r--   0        0        0       67 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/utils/__init__.py
--rw-r--r--   0        0        0     1261 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/utils/dialect_typing.py
--rw-r--r--   0        0        0     1814 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
--rw-r--r--   0        0        0      972 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
--rw-r--r--   0        0        0      674 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
--rw-r--r--   0        0        0      802 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
--rw-r--r--   0        0        0      563 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
--rw-r--r--   0        0        0    11827 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
--rw-r--r--   0        0        0     2877 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/6ef30ab7b8e5_.py
--rw-r--r--   0        0        0     1095 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
--rw-r--r--   0        0        0      643 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
--rw-r--r--   0        0        0      786 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
--rw-r--r--   0        0        0     2026 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/b4c05e463b53_.py
--rw-r--r--   0        0        0      972 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
--rw-r--r--   0        0        0      699 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
--rw-r--r--   0        0        0      679 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
--rw-r--r--   0        0        0      486 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
--rw-r--r--   0        0        0    37186 2024-04-03 20:47:33.716166 meltano-3.4.0a1/src/meltano/schemas/meltano.schema.json
--rw-r--r--   0        0        0      438 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/asserts.py
--rw-r--r--   0        0        0     7479 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/conftest.py
--rw-r--r--   0        0        0     2174 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/cli.py
--rw-r--r--   0        0        0   125876 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/core.py
--rw-r--r--   0        0        0     2829 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/__init__.py
--rw-r--r--   0        0        0     2510 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/mssql.py
--rw-r--r--   0        0        0     1227 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/postgresql.py
--rw-r--r--   0        0        0     1222 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/postgresql_psycopg3.py
--rw-r--r--   0        0        0      328 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/db/sqlite.py
--rw-r--r--   0        0        0      752 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/__init__.py
--rw-r--r--   0        0        0      276 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/docker-compose.yml
--rw-r--r--   0        0        0     4132 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/docker/snowplow.py
--rw-r--r--   0        0        0     1535 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/fs.py
--rw-r--r--   0        0        0     3135 2024-04-03 20:47:33.716166 meltano-3.4.0a1/tests/fixtures/large_config_project/meltano.yml
--rw-r--r--   0        0        0    30013 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/large_config_project/schedule.yml
--rw-r--r--   0        0        0     1086 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/meltano.yml
--rw-r--r--   0        0        0      469 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/subconfig_2.yml
--rw-r--r--   0        0        0      394 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
--rw-r--r--   0        0        0      631 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/plugins/extractors/tap-custom/test.yml
--rw-r--r--   0        0        0     1136 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/fixtures/utils.py
--rw-r--r--   0        0        0    31067 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_add.py
--rw-r--r--   0        0        0    15154 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_cli.py
--rw-r--r--   0        0        0     5174 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_compile.py
--rw-r--r--   0        0        0     8595 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_config.py
--rw-r--r--   0        0        0    42025 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_elt.py
--rw-r--r--   0        0        0     1585 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_hub.py
--rw-r--r--   0        0        0     3577 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_initialize.py
--rw-r--r--   0        0        0    12665 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_install.py
--rw-r--r--   0        0        0     9285 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_invoke.py
--rw-r--r--   0        0        0     6777 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_job_cmd.py
--rw-r--r--   0        0        0     3771 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_lock.py
--rw-r--r--   0        0        0     1864 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_remove.py
--rw-r--r--   0        0        0    47456 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_run.py
--rw-r--r--   0        0        0     8502 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_schedule.py
--rw-r--r--   0        0        0     1140 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_select.py
--rw-r--r--   0        0        0    11532 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_state.py
--rw-r--r--   0        0        0     8268 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/cli/test_upgrade.py
--rw-r--r--   0        0        0     5381 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/behavior/test_canonical.py
--rw-r--r--   0        0        0     2155 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/behavior/test_hookable.py
--rw-r--r--   0        0        0    21766 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_extract_load.py
--rw-r--r--   0        0        0      241 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_parser.py
--rw-r--r--   0        0        0      933 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_plugin_command.py
--rw-r--r--   0        0        0     7736 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/block/test_singer.py
--rw-r--r--   0        0        0     2302 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/container/test_container_spec.py
--rw-r--r--   0        0        0     6783 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/hub/test_meltano_hub_service.py
--rw-r--r--   0        0        0     2076 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_finder.py
--rw-r--r--   0        0        0     6240 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_job.py
--rw-r--r--   0        0        0     2579 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/job/test_stale_job_failer.py
--rw-r--r--   0        0        0     3357 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_formatters.py
--rw-r--r--   0        0        0      806 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_logging_utils.py
--rw-r--r--   0        0        0     7398 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/logging/test_output_logger.py
--rw-r--r--   0        0        0    32051 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_catalog.py
--rw-r--r--   0        0        0      562 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_mapper.py
--rw-r--r--   0        0        0    37590 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_tap.py
--rw-r--r--   0        0        0     3690 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_target.py
--rw-r--r--   0        0        0     3921 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_airflow.py
--rw-r--r--   0        0        0     2396 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_command.py
--rw-r--r--   0        0        0    22146 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin.py
--rw-r--r--   0        0        0      174 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_config_service.py
--rw-r--r--   0        0        0    35208 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_settings.py
--rw-r--r--   0        0        0     5963 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/plugin/test_superset.py
--rw-r--r--   0        0        0     7999 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/runner/test_runner.py
--rw-r--r--   0        0        0     2807 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_db.py
--rw-r--r--   0        0        0    21574 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_filesystem.py
--rw-r--r--   0        0        0     6765 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/state_store/test_state_store.py
--rw-r--r--   0        0        0     1558 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_db_compat.py
--rw-r--r--   0        0        0     1813 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_db_connection.py
--rw-r--r--   0        0        0     5217 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_elt_context.py
--rw-r--r--   0        0        0     2610 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_environment_service.py
--rw-r--r--   0        0        0    13772 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_environment_variables.py
--rw-r--r--   0        0        0     2274 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_locked_definition_service.py
--rw-r--r--   0        0        0     2108 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_meltano_file.py
--rw-r--r--   0        0        0     3128 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_meltano_invoker.py
--rw-r--r--   0        0        0     4094 2024-04-03 20:47:33.720166 meltano-3.4.0a1/tests/meltano/core/test_plugin_install_service.py
--rw-r--r--   0        0        0     6101 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_invoker.py
--rw-r--r--   0        0        0     3127 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_lock_service.py
--rw-r--r--   0        0        0     5749 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_remove_service.py
--rw-r--r--   0        0        0     5776 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_plugin_test_service.py
--rw-r--r--   0        0        0     4319 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project.py
--rw-r--r--   0        0        0     8892 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_add_service.py
--rw-r--r--   0        0        0    16326 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_files.py
--rw-r--r--   0        0        0     3281 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_init_service.py
--rw-r--r--   0        0        0     8071 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_plugins_service.py
--rw-r--r--   0        0        0     7238 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_project_settings_service.py
--rw-r--r--   0        0        0     9759 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_schedule_service.py
--rw-r--r--   0        0        0     2766 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_setting_definition.py
--rw-r--r--   0        0        0    22226 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_settings_store.py
--rw-r--r--   0        0        0     3665 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_state_service.py
--rw-r--r--   0        0        0     2430 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_task_sets.py
--rw-r--r--   0        0        0     2645 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_task_sets_service.py
--rw-r--r--   0        0        0     7126 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_utils.py
--rw-r--r--   0        0        0     1813 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_validation_service.py
--rw-r--r--   0        0        0    10040 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/test_venv_service.py
--rw-r--r--   0        0        0     1980 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_environment_context.py
--rw-r--r--   0        0        0     5708 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_exception.py
--rw-r--r--   0        0        0     3061 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_plugins.py
--rw-r--r--   0        0        0     1271 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_project_context.py
--rw-r--r--   0        0        0      684 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_schemas.py
--rw-r--r--   0        0        0    19704 2024-04-03 20:47:33.724166 meltano-3.4.0a1/tests/meltano/core/tracking/test_tracker.py
--rw-r--r--   0        0        0     8964 1970-01-01 00:00:00.000000 meltano-3.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1048 2024-04-12 21:49:27.862604 meltano-3.4.0a2/LICENSE
+-rw-r--r--   0        0        0     5237 2024-04-12 21:49:27.862604 meltano-3.4.0a2/README.md
+-rw-r--r--   0        0        0    19419 2024-04-12 21:49:27.998604 meltano-3.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-12 21:49:27.998604 meltano-3.4.0a2/src/meltano/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/__init__.py
+-rw-r--r--   0        0        0       73 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/__main__.py
+-rw-r--r--   0        0        0     6770 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/add.py
+-rw-r--r--   0        0        0     6006 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/cli.py
+-rw-r--r--   0        0        0     3806 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/compile.py
+-rw-r--r--   0        0        0    14489 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/config.py
+-rw-r--r--   0        0        0      406 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/docs.py
+-rw-r--r--   0        0        0      507 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/dragon.py
+-rw-r--r--   0        0        0    17244 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/elt.py
+-rw-r--r--   0        0        0     2548 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/environment.py
+-rw-r--r--   0        0        0     1671 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/hub.py
+-rw-r--r--   0        0        0     2221 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/initialize.py
+-rw-r--r--   0        0        0     4100 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/install.py
+-rw-r--r--   0        0        0      181 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/__init__.py
+-rw-r--r--   0        0        0    16395 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/config.py
+-rw-r--r--   0        0        0      241 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/interactive/utils.py
+-rw-r--r--   0        0        0     6275 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/invoke.py
+-rw-r--r--   0        0        0    10060 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/job.py
+-rw-r--r--   0        0        0     3804 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/lock.py
+-rw-r--r--   0        0        0     2242 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/params.py
+-rw-r--r--   0        0        0     2789 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/remove.py
+-rw-r--r--   0        0        0     7299 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/run.py
+-rw-r--r--   0        0        0    12993 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/schedule.py
+-rw-r--r--   0        0        0      770 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/schema.py
+-rw-r--r--   0        0        0     4446 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/select.py
+-rw-r--r--   0        0        0    10590 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/state.py
+-rw-r--r--   0        0        0     4344 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/upgrade.py
+-rw-r--r--   0        0        0    23965 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/utils.py
+-rw-r--r--   0        0        0     4185 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/__init__.py
+-rw-r--r--   0        0        0    13060 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/canonical.py
+-rw-r--r--   0        0        0     3962 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/hookable.py
+-rw-r--r--   0        0        0      192 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/name_eq.py
+-rw-r--r--   0        0        0     1187 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/versioned.py
+-rw-r--r--   0        0        0      406 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/behavior/visitor.py
+-rw-r--r--   0        0        0      117 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/blockset.py
+-rw-r--r--   0        0        0    29706 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/extract_load.py
+-rw-r--r--   0        0        0     2705 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/future_utils.py
+-rw-r--r--   0        0        0     3946 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/ioblock.py
+-rw-r--r--   0        0        0    11236 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/parser.py
+-rw-r--r--   0        0        0     5745 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/plugin_command.py
+-rw-r--r--   0        0        0    12176 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/block/singer.py
+-rw-r--r--   0        0        0      128 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/initialize.yml
+-rw-r--r--   0        0        0     2773 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/bundle/settings.yml
+-rw-r--r--   0        0        0    10326 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/cli_messages.py
+-rw-r--r--   0        0        0     3094 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/config_service.py
+-rw-r--r--   0        0        0       81 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/__init__.py
+-rw-r--r--   0        0        0     2130 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/container_service.py
+-rw-r--r--   0        0        0     2997 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/container/container_spec.py
+-rw-r--r--   0        0        0     7391 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/db.py
+-rw-r--r--   0        0        0    14930 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/elt_context.py
+-rw-r--r--   0        0        0     6924 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/environment.py
+-rw-r--r--   0        0        0     2797 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/environment_service.py
+-rw-r--r--   0        0        0     3747 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/error.py
+-rw-r--r--   0        0        0      181 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/__init__.py
+-rw-r--r--   0        0        0    11085 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/client.py
+-rw-r--r--   0        0        0      896 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/hub/schema.py
+-rw-r--r--   0        0        0      103 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/__init__.py
+-rw-r--r--   0        0        0     5940 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/finder.py
+-rw-r--r--   0        0        0    11544 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/job.py
+-rw-r--r--   0        0        0     1036 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job/stale_job_failer.py
+-rw-r--r--   0        0        0     6015 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/job_state.py
+-rw-r--r--   0        0        0     2974 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/locked_definition_service.py
+-rw-r--r--   0        0        0      699 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/__init__.py
+-rw-r--r--   0        0        0     4530 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/formatters.py
+-rw-r--r--   0        0        0     5573 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/job_logging_service.py
+-rw-r--r--   0        0        0     7367 2024-04-12 21:49:28.002604 meltano-3.4.0a2/src/meltano/core/logging/output_logger.py
+-rw-r--r--   0        0        0     7084 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/logging/utils.py
+-rw-r--r--   0        0        0     3453 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/__init__.py
+-rw-r--r--   0        0        0      365 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/cache.py
+-rw-r--r--   0        0        0     4835 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/contexts.py
+-rw-r--r--   0        0        0     4867 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/jsonschema.py
+-rw-r--r--   0        0        0    18190 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/manifest/manifest.py
+-rw-r--r--   0        0        0     5137 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/meltano_file.py
+-rw-r--r--   0        0        0     2679 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/meltano_invoker.py
+-rw-r--r--   0        0        0     3665 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/migration_service.py
+-rw-r--r--   0        0        0      481 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/models.py
+-rw-r--r--   0        0        0      188 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/__init__.py
+-rw-r--r--   0        0        0     5707 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/airflow.py
+-rw-r--r--   0        0        0    27344 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/base.py
+-rw-r--r--   0        0        0     3638 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/command.py
+-rw-r--r--   0        0        0     1422 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/config_service.py
+-rw-r--r--   0        0        0      139 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/dbt/__init__.py
+-rw-r--r--   0        0        0     4072 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/dbt/base.py
+-rw-r--r--   0        0        0     2703 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/error.py
+-rw-r--r--   0        0        0     1849 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/factory.py
+-rw-r--r--   0        0        0     9890 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/file.py
+-rw-r--r--   0        0        0     2708 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/meltano_file.py
+-rw-r--r--   0        0        0    14822 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/project_plugin.py
+-rw-r--r--   0        0        0     1135 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/requirements.py
+-rw-r--r--   0        0        0     7651 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/settings_service.py
+-rw-r--r--   0        0        0      282 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/base.py
+-rw-r--r--   0        0        0    19585 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/catalog.py
+-rw-r--r--   0        0        0     2362 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/mapper.py
+-rw-r--r--   0        0        0    23896 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/tap.py
+-rw-r--r--   0        0        0     5573 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/singer/target.py
+-rw-r--r--   0        0        0     5850 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/superset.py
+-rw-r--r--   0        0        0      269 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin/utility.py
+-rw-r--r--   0        0        0    17407 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_install_service.py
+-rw-r--r--   0        0        0    17248 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_invoker.py
+-rw-r--r--   0        0        0     6473 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_location_remove.py
+-rw-r--r--   0        0        0     3931 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_lock_service.py
+-rw-r--r--   0        0        0     2817 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_remove_service.py
+-rw-r--r--   0        0        0     2180 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_repository.py
+-rw-r--r--   0        0        0     3289 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/plugin_test_service.py
+-rw-r--r--   0        0        0    20306 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project.py
+-rw-r--r--   0        0        0     3999 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_add_service.py
+-rw-r--r--   0        0        0    14180 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_files.py
+-rw-r--r--   0        0        0     6581 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_init_service.py
+-rw-r--r--   0        0        0    18330 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_plugins_service.py
+-rw-r--r--   0        0        0     5118 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/project_settings_service.py
+-rw-r--r--   0        0        0      262 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/__init__.py
+-rw-r--r--   0        0        0     2149 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/dbt.py
+-rw-r--r--   0        0        0    10141 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/runner/singer.py
+-rw-r--r--   0        0        0     3769 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/schedule.py
+-rw-r--r--   0        0        0    10918 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/schedule_service.py
+-rw-r--r--   0        0        0     3384 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/select_service.py
+-rw-r--r--   0        0        0      926 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/setting.py
+-rw-r--r--   0        0        0    15081 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/setting_definition.py
+-rw-r--r--   0        0        0    21245 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/settings_service.py
+-rw-r--r--   0        0        0    46397 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/settings_store.py
+-rw-r--r--   0        0        0     2573 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/sqlalchemy.py
+-rw-r--r--   0        0        0     7282 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_service.py
+-rw-r--r--   0        0        0     3728 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/__init__.py
+-rw-r--r--   0        0        0     5482 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/azure.py
+-rw-r--r--   0        0        0     2134 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/base.py
+-rw-r--r--   0        0        0     3831 2024-04-12 21:49:28.006604 meltano-3.4.0a2/src/meltano/core/state_store/db.py
+-rw-r--r--   0        0        0    17948 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/filesystem.py
+-rw-r--r--   0        0        0     4170 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/google.py
+-rw-r--r--   0        0        0     4860 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/state_store/s3.py
+-rw-r--r--   0        0        0     4461 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/task_sets.py
+-rw-r--r--   0        0        0     3993 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/task_sets_service.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:49:47.498551 meltano-3.4.0a2/src/meltano/core/tracking/.release_marker
+-rw-r--r--   0        0        0     3614 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/README.md
+-rw-r--r--   0        0        0      125 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/cli.py
+-rw-r--r--   0        0        0     6044 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/environment.py
+-rw-r--r--   0        0        0     3790 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/exception.py
+-rw-r--r--   0        0        0     4948 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/plugins.py
+-rw-r--r--   0        0        0     4128 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/contexts/project.py
+-rw-r--r--   0        0        0      918 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1051 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1194 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0      720 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      748 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     6002 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     6501 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     6963 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0
+-rw-r--r--   0        0        0     7408 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0
+-rw-r--r--   0        0        0     4449 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1403 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0     1462 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1
+-rw-r--r--   0        0        0     3920 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2109 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0
+-rw-r--r--   0        0        0     2812 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0
+-rw-r--r--   0        0        0     1202 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0
+-rw-r--r--   0        0        0      404 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/iglu.json
+-rw-r--r--   0        0        0     9688 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/micro.conf
+-rw-r--r--   0        0        0     1112 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/schemas.py
+-rw-r--r--   0        0        0    18604 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/tracking/tracker.py
+-rw-r--r--   0        0        0     3562 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/transform_add_service.py
+-rw-r--r--   0        0        0     7708 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/upgrade_service.py
+-rw-r--r--   0        0        0    25155 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/utils/__init__.py
+-rw-r--r--   0        0        0     1451 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/utils/pidfile.py
+-rw-r--r--   0        0        0     4105 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/validation_service.py
+-rw-r--r--   0        0        0    23806 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/venv_service.py
+-rw-r--r--   0        0        0     1521 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/core/yaml.py
+-rw-r--r--   0        0        0      508 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/__init__.py
+-rw-r--r--   0        0        0       12 2024-04-12 21:49:47.406551 meltano-3.4.0a2/src/meltano/migrations/db.lock
+-rw-r--r--   0        0        0     1490 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/env.py
+-rw-r--r--   0        0        0      495 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/script.py.mako
+-rw-r--r--   0        0        0       67 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     1261 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/utils/dialect_typing.py
+-rw-r--r--   0        0        0     1814 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py
+-rw-r--r--   0        0        0      972 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py
+-rw-r--r--   0        0        0      674 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py
+-rw-r--r--   0        0        0      802 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py
+-rw-r--r--   0        0        0      563 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py
+-rw-r--r--   0        0        0    11827 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py
+-rw-r--r--   0        0        0     2877 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/6ef30ab7b8e5_.py
+-rw-r--r--   0        0        0     1095 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py
+-rw-r--r--   0        0        0      643 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py
+-rw-r--r--   0        0        0      786 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py
+-rw-r--r--   0        0        0     2026 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/b4c05e463b53_.py
+-rw-r--r--   0        0        0      972 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py
+-rw-r--r--   0        0        0      699 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py
+-rw-r--r--   0        0        0      679 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py
+-rw-r--r--   0        0        0      486 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/migrations/versions/f4c225a9492f_create_dedicated_job_state_table.py
+-rw-r--r--   0        0        0    37569 2024-04-12 21:49:28.010604 meltano-3.4.0a2/src/meltano/schemas/meltano.schema.json
+-rw-r--r--   0        0        0      438 2024-04-12 21:49:28.010604 meltano-3.4.0a2/tests/asserts.py
+-rw-r--r--   0        0        0     7479 2024-04-12 21:49:28.010604 meltano-3.4.0a2/tests/conftest.py
+-rw-r--r--   0        0        0     2174 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/cli.py
+-rw-r--r--   0        0        0   125876 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/core.py
+-rw-r--r--   0        0        0     2829 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/mssql.py
+-rw-r--r--   0        0        0     1227 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/postgresql.py
+-rw-r--r--   0        0        0     1222 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/postgresql_psycopg3.py
+-rw-r--r--   0        0        0      328 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/db/sqlite.py
+-rw-r--r--   0        0        0      752 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/docker-compose.yml
+-rw-r--r--   0        0        0     4132 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/docker/snowplow.py
+-rw-r--r--   0        0        0     1535 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/fs.py
+-rw-r--r--   0        0        0     3135 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/large_config_project/meltano.yml
+-rw-r--r--   0        0        0    30013 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/large_config_project/schedule.yml
+-rw-r--r--   0        0        0     1086 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/meltano.yml
+-rw-r--r--   0        0        0      469 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/subconfig_2.yml
+-rw-r--r--   0        0        0      394 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/multifile_project/subfolder/subconfig_1.yml
+-rw-r--r--   0        0        0      631 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/plugins/extractors/tap-custom/test.yml
+-rw-r--r--   0        0        0     1136 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/fixtures/utils.py
+-rw-r--r--   0        0        0    31067 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_add.py
+-rw-r--r--   0        0        0    15154 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_cli.py
+-rw-r--r--   0        0        0     5174 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_compile.py
+-rw-r--r--   0        0        0     8595 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_config.py
+-rw-r--r--   0        0        0    42025 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_elt.py
+-rw-r--r--   0        0        0     1585 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_hub.py
+-rw-r--r--   0        0        0     3577 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_initialize.py
+-rw-r--r--   0        0        0    12665 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_install.py
+-rw-r--r--   0        0        0     9285 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_invoke.py
+-rw-r--r--   0        0        0     6777 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_job_cmd.py
+-rw-r--r--   0        0        0     3771 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_lock.py
+-rw-r--r--   0        0        0     1864 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_remove.py
+-rw-r--r--   0        0        0    47456 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_run.py
+-rw-r--r--   0        0        0     8502 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_schedule.py
+-rw-r--r--   0        0        0     1140 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_select.py
+-rw-r--r--   0        0        0    11532 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_state.py
+-rw-r--r--   0        0        0     8268 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/cli/test_upgrade.py
+-rw-r--r--   0        0        0     5381 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/behavior/test_canonical.py
+-rw-r--r--   0        0        0     2155 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/behavior/test_hookable.py
+-rw-r--r--   0        0        0    21766 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_extract_load.py
+-rw-r--r--   0        0        0      241 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_parser.py
+-rw-r--r--   0        0        0      933 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_plugin_command.py
+-rw-r--r--   0        0        0     7736 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/block/test_singer.py
+-rw-r--r--   0        0        0     2302 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/container/test_container_spec.py
+-rw-r--r--   0        0        0     6783 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/hub/test_meltano_hub_service.py
+-rw-r--r--   0        0        0     2076 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_finder.py
+-rw-r--r--   0        0        0     6240 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_job.py
+-rw-r--r--   0        0        0     2579 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/job/test_stale_job_failer.py
+-rw-r--r--   0        0        0     3357 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_formatters.py
+-rw-r--r--   0        0        0      806 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_logging_utils.py
+-rw-r--r--   0        0        0     7398 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/logging/test_output_logger.py
+-rw-r--r--   0        0        0    32051 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_catalog.py
+-rw-r--r--   0        0        0      562 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_mapper.py
+-rw-r--r--   0        0        0    37590 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_tap.py
+-rw-r--r--   0        0        0     3690 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_target.py
+-rw-r--r--   0        0        0     3921 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/test_airflow.py
+-rw-r--r--   0        0        0     2396 2024-04-12 21:49:28.014604 meltano-3.4.0a2/tests/meltano/core/plugin/test_command.py
+-rw-r--r--   0        0        0    22146 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin.py
+-rw-r--r--   0        0        0      174 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_config_service.py
+-rw-r--r--   0        0        0    35208 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_settings.py
+-rw-r--r--   0        0        0     5963 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/plugin/test_superset.py
+-rw-r--r--   0        0        0     7999 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/runner/test_runner.py
+-rw-r--r--   0        0        0     2807 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_db.py
+-rw-r--r--   0        0        0    21574 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_filesystem.py
+-rw-r--r--   0        0        0     6765 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/state_store/test_state_store.py
+-rw-r--r--   0        0        0     1558 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_db_compat.py
+-rw-r--r--   0        0        0     1813 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_db_connection.py
+-rw-r--r--   0        0        0     5217 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_elt_context.py
+-rw-r--r--   0        0        0     2610 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_environment_service.py
+-rw-r--r--   0        0        0    13772 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_environment_variables.py
+-rw-r--r--   0        0        0     2274 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_locked_definition_service.py
+-rw-r--r--   0        0        0     2108 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_meltano_file.py
+-rw-r--r--   0        0        0     3128 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_meltano_invoker.py
+-rw-r--r--   0        0        0     4094 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_install_service.py
+-rw-r--r--   0        0        0     6101 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_invoker.py
+-rw-r--r--   0        0        0     3127 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_lock_service.py
+-rw-r--r--   0        0        0     5749 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_remove_service.py
+-rw-r--r--   0        0        0     5776 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_plugin_test_service.py
+-rw-r--r--   0        0        0     4319 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project.py
+-rw-r--r--   0        0        0     8892 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_add_service.py
+-rw-r--r--   0        0        0    16326 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_files.py
+-rw-r--r--   0        0        0     3281 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_init_service.py
+-rw-r--r--   0        0        0     8071 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_plugins_service.py
+-rw-r--r--   0        0        0     7238 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_project_settings_service.py
+-rw-r--r--   0        0        0     9759 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_schedule_service.py
+-rw-r--r--   0        0        0     2766 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_setting_definition.py
+-rw-r--r--   0        0        0    22226 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_settings_store.py
+-rw-r--r--   0        0        0     3665 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_state_service.py
+-rw-r--r--   0        0        0     2430 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_task_sets.py
+-rw-r--r--   0        0        0     2645 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_task_sets_service.py
+-rw-r--r--   0        0        0     7126 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_utils.py
+-rw-r--r--   0        0        0     1813 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_validation_service.py
+-rw-r--r--   0        0        0    12409 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/test_venv_service.py
+-rw-r--r--   0        0        0     1980 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_environment_context.py
+-rw-r--r--   0        0        0     5708 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_exception.py
+-rw-r--r--   0        0        0     3061 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_plugins.py
+-rw-r--r--   0        0        0     1271 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_project_context.py
+-rw-r--r--   0        0        0      684 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_schemas.py
+-rw-r--r--   0        0        0    19704 2024-04-12 21:49:28.018604 meltano-3.4.0a2/tests/meltano/core/tracking/test_tracker.py
+-rw-r--r--   0        0        0     9032 1970-01-01 00:00:00.000000 meltano-3.4.0a2/PKG-INFO
```

### Comparing `meltano-3.4.0a1/LICENSE` & `meltano-3.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/README.md` & `meltano-3.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/pyproject.toml` & `meltano-3.4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltano"
-version = "3.4.0a1"
+version = "3.4.0a2"
 description = "Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love."
 authors = ["Meltano <hello@meltano.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/meltano/meltano"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
@@ -43,15 +43,15 @@
 aiodocker = "^0.21.0"
 alembic = "^1.13.1"
 atomicwrites = "^1.2.1"
 azure-common = {version = "^1.1.28", optional = true}
 azure-core = {version = "^1.30.1", optional = true}
 azure-identity = {version = "^1.15.0", optional = true}
 azure-storage-blob = {version = "^12.19.1", optional = true}
-boto3 = {version = "^1.34.74", optional = true}
+boto3 = {version = "^1.34.79", optional = true}
 check-jsonschema = "^0.28.1"
 click = "^8.1"
 click-default-group = "^1.2.4"
 click-didyoumean = "^0.3.1"
 croniter = "^2.0.3"
 fasteners = "^0.19"
 flatten-dict = "^0"
@@ -61,15 +61,15 @@
 jsonschema = "^4.21"
 packaging = "^24.0"
 platformdirs = "^4.2.0"
 psutil = "^5.9.8"
 psycopg = {version = "^3.1.18", extras = ["binary"], optional = true}
 psycopg2-binary = {version="^2.9.9", optional=true}
 pyjwt = "^2.6.0"
-pymssql = {version = "^2.2.11", optional = true}
+pymssql = {version = "^2.3.0", optional = true}
 python = ">=3.8,<3.13"
 python-dateutil = "^2.9.0"
 python-dotenv = "^1.0.1"
 python-slugify = "^8.0.4"
 python-ulid = "^1.1.0"
 pyyaml = "^6.0.1"
 questionary = "^2.0.1"
@@ -78,40 +78,42 @@
 "ruamel.yaml" = "^0.18.6"
 setuptools = {version = "^69.2.0", python = ">=3.12"}
 smart-open = "^7.0.4"
 snowplow-tracker = "^1.0.2"
 sqlalchemy = "^2.0.29"
 structlog = "^24.1.0"
 tabulate = "^0.9.0"
-typing-extensions = "^4.10.0"
+typing-extensions = "^4.11.0"
 tzlocal = "^5.2"
 # Compatibility issues with boto: https://github.com/boto/botocore/pull/3034
 urllib3 = "<2"
+uv = { version = ">=0.1.24,<0.2", optional = true }
 virtualenv = "^20.25.1"
 yaspin = "^2.3.0"
 
 [tool.poetry.extras]
 azure = ["azure-storage-blob", "azure-common", "azure-core", "azure-identity"]
 gcs = ["google-cloud-storage"]
 mssql = ["pymssql"]
 postgres = ["psycopg"]
 psycopg2 = ["psycopg2-binary"]
 s3 = ["boto3"]
+uv = ["uv"]
 
 [tool.poetry.group.dev.dependencies]
 backoff = "^2.1.2"
 black = "^24.3.0"
-boto3-stubs = {extras = ["essential"], version = "1.34.74"}
+boto3-stubs = {extras = ["essential"], version = "1.34.79"}
 bumpversion = "^0.6.0"
 colorama = "^0.4.4"
 coverage = {extras = ["toml"], version = ">=7.3.2,!=7.3.3"}
 freezegun = "^1.4.0"
 hypothesis = "^6.100.0"
 mock = "^5.0.2"
-moto = "^5.0.4"
+moto = "^5.0.5"
 mypy = "^1.9.0"
 pre-commit = "^3.5.0"
 pytest = "^8.1.1"
 pytest-asyncio = "^0.23.6"
 pytest-cov = "^5.0.0"
 pytest-docker = "^3.1"
 pytest-httpserver = "^1.0.10"
@@ -468,15 +470,15 @@
 skip_covered = true
 
 [tool.commitizen]
 name = "cz_version_bump"
 prerelease_offset = 1
 tag_format = "v$major.$minor.$patch$prerelease"
 changelog_merge_prerelease = true
-version = "3.4.0a1"
+version = "3.4.0a2"
 version_files = [
   "pyproject.toml:^version =",
   "src/meltano/__init__.py:^__version__ =",
   'docs/package.json:^  "version":',
 ]
 
 [tool.mypy]
```

### Comparing `meltano-3.4.0a1/src/meltano/cli/__init__.py` & `meltano-3.4.0a2/src/meltano/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/add.py` & `meltano-3.4.0a2/src/meltano/cli/add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/cli.py` & `meltano-3.4.0a2/src/meltano/cli/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/compile.py` & `meltano-3.4.0a2/src/meltano/cli/compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/config.py` & `meltano-3.4.0a2/src/meltano/cli/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/elt.py` & `meltano-3.4.0a2/src/meltano/cli/elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/environment.py` & `meltano-3.4.0a2/src/meltano/cli/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/hub.py` & `meltano-3.4.0a2/src/meltano/cli/hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/initialize.py` & `meltano-3.4.0a2/src/meltano/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/install.py` & `meltano-3.4.0a2/src/meltano/cli/install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/interactive/config.py` & `meltano-3.4.0a2/src/meltano/cli/interactive/config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/invoke.py` & `meltano-3.4.0a2/src/meltano/cli/invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/job.py` & `meltano-3.4.0a2/src/meltano/cli/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/lock.py` & `meltano-3.4.0a2/src/meltano/cli/lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/params.py` & `meltano-3.4.0a2/src/meltano/cli/params.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/remove.py` & `meltano-3.4.0a2/src/meltano/cli/remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/run.py` & `meltano-3.4.0a2/src/meltano/cli/run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/schedule.py` & `meltano-3.4.0a2/src/meltano/cli/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/schema.py` & `meltano-3.4.0a2/src/meltano/cli/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/select.py` & `meltano-3.4.0a2/src/meltano/cli/select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/state.py` & `meltano-3.4.0a2/src/meltano/cli/state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/upgrade.py` & `meltano-3.4.0a2/src/meltano/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/utils.py` & `meltano-3.4.0a2/src/meltano/cli/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/cli/validate.py` & `meltano-3.4.0a2/src/meltano/cli/validate.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/behavior/canonical.py` & `meltano-3.4.0a2/src/meltano/core/behavior/canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/behavior/hookable.py` & `meltano-3.4.0a2/src/meltano/core/behavior/hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/behavior/versioned.py` & `meltano-3.4.0a2/src/meltano/core/behavior/versioned.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/blockset.py` & `meltano-3.4.0a2/src/meltano/core/block/blockset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/extract_load.py` & `meltano-3.4.0a2/src/meltano/core/block/extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/future_utils.py` & `meltano-3.4.0a2/src/meltano/core/block/future_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/ioblock.py` & `meltano-3.4.0a2/src/meltano/core/block/ioblock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/parser.py` & `meltano-3.4.0a2/src/meltano/core/block/parser.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/plugin_command.py` & `meltano-3.4.0a2/src/meltano/core/block/plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/block/singer.py` & `meltano-3.4.0a2/src/meltano/core/block/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/bundle/settings.yml` & `meltano-3.4.0a2/src/meltano/core/bundle/settings.yml`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,24 @@
   value: logging.yaml
 
 # Snowplow Tracking
 - name: snowplow.collector_endpoints
   kind: array
   value: ["https://sp.meltano.com"]
 
+# venv
+- name: venv.backend
+  value: virtualenv
+  kind: options
+  options:
+  - label: virtualenv
+    value: virtualenv
+  - label: uv
+    value: uv
+
 # Feature Flags
 # Global "experimental" flag.
 - name: experimental
   kind: boolean
   value: False
 # Control whether references to undefined env vars causes hard fail.
 - name: ff.strict_env_var_mode
```

### Comparing `meltano-3.4.0a1/src/meltano/core/cli_messages.py` & `meltano-3.4.0a2/src/meltano/core/cli_messages.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/config_service.py` & `meltano-3.4.0a2/src/meltano/core/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/container/container_service.py` & `meltano-3.4.0a2/src/meltano/core/container/container_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/container/container_spec.py` & `meltano-3.4.0a2/src/meltano/core/container/container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/db.py` & `meltano-3.4.0a2/src/meltano/core/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/elt_context.py` & `meltano-3.4.0a2/src/meltano/core/elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/environment.py` & `meltano-3.4.0a2/src/meltano/core/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/environment_service.py` & `meltano-3.4.0a2/src/meltano/core/environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/error.py` & `meltano-3.4.0a2/src/meltano/core/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/hub/client.py` & `meltano-3.4.0a2/src/meltano/core/hub/client.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/hub/schema.py` & `meltano-3.4.0a2/src/meltano/core/hub/schema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/job/finder.py` & `meltano-3.4.0a2/src/meltano/core/job/finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/job/job.py` & `meltano-3.4.0a2/src/meltano/core/job/job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/job/stale_job_failer.py` & `meltano-3.4.0a2/src/meltano/core/job/stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/job_state.py` & `meltano-3.4.0a2/src/meltano/core/job_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/locked_definition_service.py` & `meltano-3.4.0a2/src/meltano/core/locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/logging/__init__.py` & `meltano-3.4.0a2/src/meltano/core/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/logging/formatters.py` & `meltano-3.4.0a2/src/meltano/core/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/logging/job_logging_service.py` & `meltano-3.4.0a2/src/meltano/core/logging/job_logging_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/logging/output_logger.py` & `meltano-3.4.0a2/src/meltano/core/logging/output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/logging/utils.py` & `meltano-3.4.0a2/src/meltano/core/logging/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/manifest/__init__.py` & `meltano-3.4.0a2/src/meltano/core/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/manifest/contexts.py` & `meltano-3.4.0a2/src/meltano/core/manifest/contexts.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/manifest/jsonschema.py` & `meltano-3.4.0a2/src/meltano/core/manifest/jsonschema.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/manifest/manifest.py` & `meltano-3.4.0a2/src/meltano/core/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/meltano_file.py` & `meltano-3.4.0a2/src/meltano/core/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/meltano_invoker.py` & `meltano-3.4.0a2/src/meltano/core/meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/migration_service.py` & `meltano-3.4.0a2/src/meltano/core/migration_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/airflow.py` & `meltano-3.4.0a2/src/meltano/core/plugin/airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/base.py` & `meltano-3.4.0a2/src/meltano/core/plugin/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/command.py` & `meltano-3.4.0a2/src/meltano/core/plugin/command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/config_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin/config_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/dbt/base.py` & `meltano-3.4.0a2/src/meltano/core/plugin/dbt/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/error.py` & `meltano-3.4.0a2/src/meltano/core/plugin/error.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/factory.py` & `meltano-3.4.0a2/src/meltano/core/plugin/factory.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/file.py` & `meltano-3.4.0a2/src/meltano/core/plugin/file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/meltano_file.py` & `meltano-3.4.0a2/src/meltano/core/plugin/meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/project_plugin.py` & `meltano-3.4.0a2/src/meltano/core/plugin/project_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/requirements.py` & `meltano-3.4.0a2/src/meltano/core/plugin/requirements.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/settings_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/singer/base.py` & `meltano-3.4.0a2/src/meltano/core/plugin/singer/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/singer/catalog.py` & `meltano-3.4.0a2/src/meltano/core/plugin/singer/catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/singer/mapper.py` & `meltano-3.4.0a2/src/meltano/core/plugin/singer/mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/singer/tap.py` & `meltano-3.4.0a2/src/meltano/core/plugin/singer/tap.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,26 +302,38 @@
         if custom_state_filename := plugin_invoker.plugin_config_extras["_state"]:
             custom_state_path = plugin_invoker.project.root.joinpath(
                 custom_state_filename,
             )
 
             try:
                 shutil.copy(custom_state_path, state_path)
-                logger.info(f"Found state in {custom_state_filename}")  # noqa: G004
             except FileNotFoundError as err:
                 raise PluginExecutionError(
                     f"Could not find state file {custom_state_path}",  # noqa: EM102
                 ) from err
 
+            logger.info(f"Found state in {custom_state_filename}")  # noqa: G004
             return
-        # the `state.json` is stored in the database
-        if state := StateService(
+
+        # the `state.json` is stored in a state backend
+        state_service = StateService(
             project=elt_context.project,
             session=elt_context.session,
-        ).get_state(elt_context.job.job_name):
+        )
+        try:
+            state = state_service.get_state(elt_context.job.job_name)
+        except Exception as err:  # pragma: no cover
+            logger.error(
+                err.args[0],
+                state_backend=state_service.state_store_manager.label,
+            )
+            msg = "Failed to retrieve state"
+            raise PluginExecutionError(msg) from err
+
+        if state:
             if state.get(SINGER_STATE_KEY):
                 with state_path.open("w") as state_file:
                     json.dump(state.get(SINGER_STATE_KEY), state_file, indent=2)
         else:
             logger.warning("No state was found, complete import.")
 
     @hook("before_invoke")
```

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/singer/target.py` & `meltano-3.4.0a2/src/meltano/core/plugin/singer/target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin/superset.py` & `meltano-3.4.0a2/src/meltano/core/plugin/superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_install_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin_install_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     PluginInstallError,
     PluginInstallWarning,
 )
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.settings_service import PluginSettingsService
 from meltano.core.settings_service import FeatureFlags
 from meltano.core.utils import EnvVarMissingBehavior, expand_env_vars, noop
-from meltano.core.venv_service import VenvService
+from meltano.core.venv_service import UvVenvService, VenvService
 
 if t.TYPE_CHECKING:
     from meltano.core.plugin.project_plugin import ProjectPlugin
     from meltano.core.project import Project
 
 logger = logging.getLogger(__name__)
 
@@ -517,21 +517,43 @@
     Args:
         project: Meltano Project.
         plugin: `ProjectPlugin` to install.
         clean: Flag to clean install.
         force: Whether to ignore the Python version required by plugins.
         env: Environment variables to use when expanding the pip install args.
         kwargs: Unused additional arguments for the installation of the plugin.
+
+    Raises:
+        ValueError: If the venv backend is not supported.
     """
     pip_install_args = get_pip_install_args(project, plugin, env=env)
+    backend = project.settings.get("venv.backend", "virtualenv")
+
+    if backend == "virtualenv":
+        service = VenvService(
+            project=project,
+            python=plugin.python,
+            namespace=plugin.type,
+            name=plugin.venv_name,
+        )
+    elif backend == "uv":  # pragma: no cover
+        logger.warning("The uv backend is experimental")
+        service = UvVenvService(
+            project=project,
+            python=plugin.python,
+            namespace=plugin.type,
+            name=plugin.venv_name,
+        )
+    else:  # pragma: no cover
+        msg = f"Unsupported venv backend: {backend}"
+        raise ValueError(msg)
 
-    await VenvService(
-        project=project,
-        python=plugin.python,
-        namespace=plugin.type,
-        name=plugin.venv_name,
-    ).install(
+    await service.install(
         pip_install_args=("--ignore-requires-python", *pip_install_args)
         if force
         else pip_install_args,
         clean=clean,
+        env={
+            **os.environ,
+            **project.dotenv_env,
+        },
     )
```

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_invoker.py` & `meltano-3.4.0a2/src/meltano/core/plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_location_remove.py` & `meltano-3.4.0a2/src/meltano/core/plugin_location_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_lock_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_remove_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_repository.py` & `meltano-3.4.0a2/src/meltano/core/plugin_repository.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/plugin_test_service.py` & `meltano-3.4.0a2/src/meltano/core/plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project.py` & `meltano-3.4.0a2/src/meltano/core/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project_add_service.py` & `meltano-3.4.0a2/src/meltano/core/project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project_files.py` & `meltano-3.4.0a2/src/meltano/core/project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project_init_service.py` & `meltano-3.4.0a2/src/meltano/core/project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project_plugins_service.py` & `meltano-3.4.0a2/src/meltano/core/project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/project_settings_service.py` & `meltano-3.4.0a2/src/meltano/core/project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/runner/dbt.py` & `meltano-3.4.0a2/src/meltano/core/runner/dbt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/runner/singer.py` & `meltano-3.4.0a2/src/meltano/core/runner/singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/schedule.py` & `meltano-3.4.0a2/src/meltano/core/schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/schedule_service.py` & `meltano-3.4.0a2/src/meltano/core/schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/select_service.py` & `meltano-3.4.0a2/src/meltano/core/select_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/setting.py` & `meltano-3.4.0a2/src/meltano/core/setting.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/setting_definition.py` & `meltano-3.4.0a2/src/meltano/core/setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/settings_service.py` & `meltano-3.4.0a2/src/meltano/core/settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/settings_store.py` & `meltano-3.4.0a2/src/meltano/core/settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/sqlalchemy.py` & `meltano-3.4.0a2/src/meltano/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_service.py` & `meltano-3.4.0a2/src/meltano/core/state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/__init__.py` & `meltano-3.4.0a2/src/meltano/core/state_store/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/azure.py` & `meltano-3.4.0a2/src/meltano/core/state_store/azure.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/base.py` & `meltano-3.4.0a2/src/meltano/core/state_store/base.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/db.py` & `meltano-3.4.0a2/src/meltano/core/state_store/db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/filesystem.py` & `meltano-3.4.0a2/src/meltano/core/state_store/filesystem.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/google.py` & `meltano-3.4.0a2/src/meltano/core/state_store/google.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/state_store/s3.py` & `meltano-3.4.0a2/src/meltano/core/state_store/s3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/task_sets.py` & `meltano-3.4.0a2/src/meltano/core/task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/task_sets_service.py` & `meltano-3.4.0a2/src/meltano/core/task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/README.md` & `meltano-3.4.0a2/src/meltano/core/tracking/README.md`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/contexts/cli.py` & `meltano-3.4.0a2/src/meltano/core/tracking/contexts/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/contexts/environment.py` & `meltano-3.4.0a2/src/meltano/core/tracking/contexts/environment.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/contexts/exception.py` & `meltano-3.4.0a2/src/meltano/core/tracking/contexts/exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/contexts/plugins.py` & `meltano-3.4.0a2/src/meltano/core/tracking/contexts/plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/contexts/project.py` & `meltano-3.4.0a2/src/meltano/core/tracking/contexts/project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/block_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/cli_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-2-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/environment_context/jsonschema/1-3-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exception_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/exit_event/jsonschema/1-0-1`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/plugins_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/project_context/jsonschema/1-1-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0` & `meltano-3.4.0a2/src/meltano/core/tracking/iglu-client-embedded/schemas/com.meltano/telemetry_state_change_event/jsonschema/1-0-0`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/micro.conf` & `meltano-3.4.0a2/src/meltano/core/tracking/micro.conf`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/schemas.py` & `meltano-3.4.0a2/src/meltano/core/tracking/schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/tracking/tracker.py` & `meltano-3.4.0a2/src/meltano/core/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/transform_add_service.py` & `meltano-3.4.0a2/src/meltano/core/transform_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/upgrade_service.py` & `meltano-3.4.0a2/src/meltano/core/upgrade_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/utils/__init__.py` & `meltano-3.4.0a2/src/meltano/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/utils/pidfile.py` & `meltano-3.4.0a2/src/meltano/core/utils/pidfile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/validation_service.py` & `meltano-3.4.0a2/src/meltano/core/validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/core/venv_service.py` & `meltano-3.4.0a2/src/meltano/core/venv_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 """Manage Python virtual environments."""
 
 from __future__ import annotations
 
 import asyncio
+import contextlib
 import hashlib
 import logging
 import os
 import platform
 import shlex
 import shutil
 import subprocess
 import sys
 import typing as t
+from asyncio.subprocess import Process
 from functools import cached_property
 from numbers import Number
 from pathlib import Path
 
 from meltano.core.error import AsyncSubprocessError, MeltanoError
 
 if t.TYPE_CHECKING:
-    from asyncio.subprocess import Process
     from collections.abc import Iterable
 
     from meltano.core.project import Project
 
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
+
+if sys.version_info < (3, 12):
+    from typing_extensions import override
+else:
+    from typing import override
+
+
 logger = logging.getLogger(__name__)
 
+StdErrExtractor: TypeAlias = t.Callable[[Process], t.Awaitable[t.Union[str, None]]]
+
 
 class VirtualEnv:
     """Info about a single virtual environment."""
 
     _SUPPORTED_PLATFORMS = {
         "Linux",
         "Darwin",
@@ -247,31 +261,34 @@
             "pip.log",
         ).resolve()
 
     async def install(
         self,
         pip_install_args: t.Sequence[str],
         clean: bool = False,
+        *,
+        env: dict[str, str | None] | None = None,
     ) -> None:
         """Configure a virtual environment, then run pip install with the given args.
 
         Args:
             pip_install_args: Arguments passed to `pip install`.
             clean: Whether to not attempt to use an existing virtual environment.
+            env: Environment variables to pass to the subprocess.
         """
         if not clean and self.requires_clean_install(pip_install_args):
             logger.debug(
                 f"Packages for '{self.namespace}/{self.name}' have changed so "  # noqa: G004
                 "performing a clean install.",
             )
             clean = True
 
         self.clean_run_files()
 
-        await self._pip_install(pip_install_args=pip_install_args, clean=clean)
+        await self._pip_install(pip_install_args=pip_install_args, clean=clean, env=env)
         self.write_fingerprint(pip_install_args)
 
     def requires_clean_install(self, pip_install_args: t.Sequence[str]) -> bool:
         """Determine whether a clean install is needed.
 
         Args:
             pip_install_args: The arguments being passed to `pip install`, used
@@ -307,60 +324,83 @@
                 self.namespace,
                 self.name,
             )
         except FileNotFoundError:
             # If the VirtualEnv has never been created before do nothing
             logger.debug("No old virtual environment to remove")
 
+    async def create_venv(
+        self,
+        *,
+        extract_stderr: StdErrExtractor,
+    ) -> Process:
+        """Create a new virtual environment.
+
+        Args:
+            extract_stderr: Async function that is provided the completed failed
+                process, and returns its error string or `None`.
+
+        Returns:
+            The Python process creating the virtual environment.
+        """
+        return await exec_async(
+            sys.executable,
+            "-m",
+            "virtualenv",
+            "--python",
+            self.venv.python_path,
+            str(self.venv.root),
+            extract_stderr=extract_stderr,
+        )
+
     async def create(self) -> Process:
         """Create a new virtual environment.
 
         Raises:
             AsyncSubprocessError: The virtual environment could not be created.
 
         Returns:
             The Python process creating the virtual environment.
         """
         logger.debug(f"Creating virtual environment for '{self.namespace}/{self.name}'")  # noqa: G004
 
         async def extract_stderr(proc: Process):
             return (await t.cast(asyncio.StreamReader, proc.stdout).read()).decode(
-                "unicode_escape",
+                "utf-8",
                 errors="replace",
             )
 
         try:
-            return await exec_async(
-                sys.executable,
-                "-m",
-                "virtualenv",
-                "--python",
-                self.venv.python_path,
-                str(self.venv.root),
-                extract_stderr=extract_stderr,
-            )
+            return await self.create_venv(extract_stderr=extract_stderr)
         except AsyncSubprocessError as err:
             raise AsyncSubprocessError(
                 f"Could not create the virtualenv for '{self.namespace}/{self.name}'",  # noqa: EM102
                 process=err.process,
                 stderr=await err.stderr,
             ) from err
 
-    async def upgrade_pip(self) -> Process:
+    async def upgrade_installer(
+        self,
+        *,
+        env: dict[str, str | None] | None = None,
+    ) -> Process | None:
         """Upgrade the `pip` package to the latest version in the virtual environment.
 
+        Args:
+            env: Environment variables to pass to the subprocess.
+
         Raises:
             AsyncSubprocessError: Failed to upgrade pip to the latest version.
 
         Returns:
             The process running `pip install --upgrade ...`.
         """
         logger.debug(f"Upgrading pip for '{self.namespace}/{self.name}'")  # noqa: G004
         try:
-            return await self._pip_install(("--upgrade", "pip"))
+            return await self._pip_install(("--upgrade", "pip"), env=env)
         except AsyncSubprocessError as err:
             raise AsyncSubprocessError(
                 "Failed to upgrade pip to the latest version.",  # noqa: EM101
                 err.process,
             ) from err
 
     def read_fingerprint(self) -> str | None:
@@ -402,35 +442,109 @@
         absolute_executable_windows = absolute_executable.with_suffix(".exe")
         return (
             absolute_executable_windows
             if absolute_executable_windows.exists()
             else absolute_executable
         )
 
+    async def install_pip_args(
+        self,
+        pip_install_args: t.Sequence[str],
+        *,
+        extract_stderr: StdErrExtractor = _extract_stderr,
+        env: dict[str, str | None] | None = None,
+    ) -> Process:
+        """Return the `pip install` arguments to use.
+
+        Args:
+            pip_install_args: The arguments to pass to `pip install`.
+            extract_stderr: Async function that is provided the completed failed
+                process, and returns its error string or `None`.
+            env: Environment variables to pass to the subprocess.
+
+        Returns:
+            The process running `pip install` with the provided args.
+        """
+        return await exec_async(
+            str(self.exec_path("python")),
+            "-m",
+            "pip",
+            "install",
+            "--log",
+            str(self.pip_log_path),
+            *pip_install_args,
+            extract_stderr=extract_stderr,
+            env=env,
+        )
+
+    async def uninstall_package(self, package: str) -> Process:
+        """Uninstall a single package.
+
+        Args:
+            package: The package name.
+
+        Returns:
+            The process running `pip uninstall` with the provided package.
+        """
+        return await exec_async(
+            str(self.exec_path("python")),
+            "-m",
+            "pip",
+            "uninstall",
+            "--yes",
+            package,
+            extract_stderr=_extract_stderr,
+        )
+
+    async def handle_installation_error(
+        self,
+        err: AsyncSubprocessError,
+    ) -> AsyncSubprocessError:
+        """Handle an error that occurred during installation.
+
+        Args:
+            err: The error that occurred during installation.
+
+        Returns:
+            The error that occurred during installation with additional context.
+        """
+        logger.info(
+            "Logged pip install output to %s",  # noqa: WPS323
+            self.pip_log_path,
+        )
+        return AsyncSubprocessError(
+            f"Failed to install plugin '{self.name}'.",
+            err.process,
+            stderr=await err.stderr,
+        )
+
     async def _pip_install(
         self,
         pip_install_args: t.Sequence[str],
         clean: bool = False,
+        *,
+        env: dict[str, str | None] | None = None,
     ) -> Process:
         """Install a package using `pip` in the proper virtual environment.
 
         Args:
             pip_install_args: The arguments to pass to `pip install`.
             clean: Whether the installation should be done in a clean venv.
+            env: Environment variables to pass to the subprocess.
 
         Raises:
             AsyncSubprocessError: The command failed.
 
         Returns:
             The process running `pip install` with the provided args.
         """
         if clean:
             self.clean()
             await self.create()
-            await self.upgrade_pip()
+            await self.upgrade_installer(env=env)
 
         pip_install_args_str = shlex.join(pip_install_args)
         log_msg_prefix = (
             f"Upgrading with args {pip_install_args_str!r} in existing"
             if "--upgrade" in pip_install_args
             else f"Installing with args {pip_install_args_str!r} into"
         )
@@ -438,30 +552,181 @@
             f"{log_msg_prefix} virtual environment for '{self.namespace}/{self.name}'",  # noqa: G004
         )
 
         async def extract_stderr(proc: Process) -> str | None:  # pragma: no cover
             if not proc.stdout:
                 return None
 
-            return (await proc.stdout.read()).decode("unicode_escape", errors="replace")
+            return (await proc.stdout.read()).decode("utf-8", errors="replace")
 
         try:
-            return await exec_async(
-                str(self.exec_path("python")),
-                "-m",
-                "pip",
-                "install",
-                "--log",
-                str(self.pip_log_path),
-                *pip_install_args,
+            return await self.install_pip_args(
+                pip_install_args,
                 extract_stderr=extract_stderr,
+                env=env,
             )
-        except AsyncSubprocessError as err:
-            logger.info(
-                "Logged pip install output to %s",  # noqa: WPS323
-                self.pip_log_path,
-            )
-            raise AsyncSubprocessError(
-                f"Failed to install plugin '{self.name}'.",  # noqa: EM102
-                err.process,
-                stderr=await err.stderr,
-            ) from err
+        except AsyncSubprocessError as err:  # noqa: WPS329
+            raise await self.handle_installation_error(err) from err
+
+
+class UvVenvService(VenvService):
+    """Manages virtual environments using `uv`."""
+
+    @staticmethod
+    def _find_uv() -> str:  # noqa: WPS605
+        """Find the `uv` executable.
+
+        Tries to import the `uv` package and use its `find_uv_bin` function to find the
+        `uv` executable. If that fails, falls back to using the `uv` executable on the
+        system PATH. If it can't be found on the PATH, returns `"uv"`.
+
+        Adapted from https://github.com/wntrblm/nox/blob/55c7eaf2eb03feb4a4b79e74966c542b75d61401/nox/virtualenv.py#L42-L54.
+
+        Copyright 2016 Alethea Katherine Flowers
+
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+
+           http://www.apache.org/licenses/LICENSE-2.0
+
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+
+        Returns:
+            A string representing the path to the `uv` executable.
+
+        Raises:
+            MeltanoError: The `uv` executable could not be found.
+        """
+        with contextlib.suppress(ImportError, FileNotFoundError):
+            from uv import find_uv_bin
+
+            return find_uv_bin()
+
+        # Fall back to PATH.
+        uv = shutil.which("uv")
+
+        if not uv:
+            error = "Could not find the 'uv' executable"
+            instruction = "Please install 'meltano[uv]' or install 'uv' globally."
+            raise MeltanoError(error, instruction)
+
+        return uv
+
+    def __init__(self, *args: t.Any, **kwargs: t.Any):
+        """Initialize the `UvVenvService`.
+
+        Args:
+            args: Positional arguments for the VenvService.
+            kwargs: Keyword arguments for the VenvService.
+        """
+        super().__init__(*args, **kwargs)
+        self.uv = self._find_uv()
+        logger.debug("Using uv executable at %s", self.uv)
+
+    @override
+    async def upgrade_installer(
+        self,
+        *,
+        env: dict[str, str | None] | None = None,
+    ) -> Process | None:
+        """No-op for `uv` virtual environments.
+
+        Args:
+            env: Environment variables to pass to the subprocess.
+        """
+
+    @override
+    async def install_pip_args(
+        self,
+        pip_install_args: t.Sequence[str],
+        *,
+        extract_stderr: StdErrExtractor = _extract_stderr,
+        env: dict[str, str | None] | None = None,
+    ) -> Process:
+        """Run `pip install` in the plugin's virtual environment.
+
+        Args:
+            pip_install_args: The arguments to pass to `pip install`.
+            extract_stderr: Async function that is provided the completed failed
+                process, and returns its error string or `None`.
+            env: Environment variables to pass to the subprocess.
+
+        Returns:
+            The process running `pip install` with the provided args.
+        """
+        return await exec_async(
+            self.uv,
+            "pip",
+            "install",
+            "--python",
+            str(self.exec_path("python")),
+            *pip_install_args,
+            extract_stderr=extract_stderr,
+            env=env,
+        )
+
+    @override
+    async def uninstall_package(self, package: str) -> Process:
+        """Uninstall a single package using `uv`.
+
+        Args:
+            package: The package name.
+
+        Returns:
+            The process running `pip uninstall` with the provided package.
+        """
+        return await exec_async(
+            self.uv,
+            "pip",
+            "uninstall",
+            "--python",
+            str(self.exec_path("python")),
+            package,
+        )
+
+    @override
+    async def handle_installation_error(
+        self,
+        err: AsyncSubprocessError,
+    ) -> AsyncSubprocessError:
+        """Handle an error that occurred during installation.
+
+        Args:
+            err: The subprocess error that occurred during installation.
+
+        Returns:
+            The error that occurred during installation with additional context.
+        """
+        return AsyncSubprocessError(
+            f"Failed to install plugin '{self.name}'.",
+            err.process,
+            stderr=await err.stderr,
+        )
+
+    @override
+    async def create_venv(
+        self,
+        *,
+        extract_stderr: StdErrExtractor,
+    ) -> Process:
+        """Create a new virtual environment using `uv`.
+
+        Args:
+            extract_stderr: Async function that is provided the completed failed
+                process, and returns its error string or `None`.
+
+        Returns:
+            The Python process creating the virtual environment.
+        """
+        return await exec_async(
+            self.uv,
+            "virtualenv",
+            "--python",
+            self.venv.python_path,
+            str(self.venv.root),
+            extract_stderr=extract_stderr,
+        )
```

### Comparing `meltano-3.4.0a1/src/meltano/core/yaml.py` & `meltano-3.4.0a2/src/meltano/core/yaml.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/env.py` & `meltano-3.4.0a2/src/meltano/migrations/env.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/utils/dialect_typing.py` & `meltano-3.4.0a2/src/meltano/migrations/utils/dialect_typing.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/13e8639c6d2b_add_state_edit_to_job_state_enum.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/23ea52e6d784_add_resource_type_to_embed_token.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/367228df6a43_add_trigger_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/53e97221d99f_add_run_id_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/5b43800443d1_rename_job_to_job_run_and_job_id_to_job_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/6828cc5b1a4f_create_dedicated_state_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/6ef30ab7b8e5_.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/6ef30ab7b8e5_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/87d9638f6ac6_add_subscription.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/990c0665f3ce_ensure_user_login_count_default_value.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/a3e2b0a4937d_add_login_audit_columns.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/b4c05e463b53_.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/b4c05e463b53_.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/ceb00d7ff3bd_create_the_embedtoken_table.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/d135f52a6f49_add_last_heartbeat_at_column_to_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py` & `meltano-3.4.0a2/src/meltano/migrations/versions/e4fbabc3fed6_add_last_activity_at_column.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/src/meltano/schemas/meltano.schema.json` & `meltano-3.4.0a2/src/meltano/schemas/meltano.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975%*

 * *Differences: {"'properties'": "{'venv': OrderedDict([('type', 'object'), ('description', 'Configuration for "*

 * *                 "plugin virtual environments.'), ('properties', OrderedDict([('backend', "*

 * *                 "OrderedDict([('type', 'string'), ('description', 'The virtual environment "*

 * *                 "backend to use.'), ('default', 'virtualenv'), ('enum', ['virtualenv', "*

 * *                 "'uv'])]))]))])}"}*

```diff
@@ -1185,14 +1185,29 @@
                     "default": "systemdb",
                     "description": "The URI pointing to the backend to use.",
                     "type": "string"
                 }
             },
             "type": "object"
         },
+        "venv": {
+            "description": "Configuration for plugin virtual environments.",
+            "properties": {
+                "backend": {
+                    "default": "virtualenv",
+                    "description": "The virtual environment backend to use.",
+                    "enum": [
+                        "virtualenv",
+                        "uv"
+                    ],
+                    "type": "string"
+                }
+            },
+            "type": "object"
+        },
         "version": {
             "const": 1
         }
     },
     "title": "JSON Schema for meltano.yml",
     "type": "object"
 }
```

### Comparing `meltano-3.4.0a1/tests/conftest.py` & `meltano-3.4.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/cli.py` & `meltano-3.4.0a2/tests/fixtures/cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/core.py` & `meltano-3.4.0a2/tests/fixtures/core.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/db/__init__.py` & `meltano-3.4.0a2/tests/fixtures/db/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/db/mssql.py` & `meltano-3.4.0a2/tests/fixtures/db/mssql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/db/postgresql.py` & `meltano-3.4.0a2/tests/fixtures/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/db/postgresql_psycopg3.py` & `meltano-3.4.0a2/tests/fixtures/db/postgresql_psycopg3.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/docker/__init__.py` & `meltano-3.4.0a2/tests/fixtures/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/docker/snowplow.py` & `meltano-3.4.0a2/tests/fixtures/docker/snowplow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/fs.py` & `meltano-3.4.0a2/tests/fixtures/fs.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/large_config_project/meltano.yml` & `meltano-3.4.0a2/tests/fixtures/large_config_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/large_config_project/schedule.yml` & `meltano-3.4.0a2/tests/fixtures/large_config_project/schedule.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/multifile_project/meltano.yml` & `meltano-3.4.0a2/tests/fixtures/multifile_project/meltano.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/plugins/extractors/tap-custom/test.yml` & `meltano-3.4.0a2/tests/fixtures/plugins/extractors/tap-custom/test.yml`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/fixtures/utils.py` & `meltano-3.4.0a2/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_add.py` & `meltano-3.4.0a2/tests/meltano/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_cli.py` & `meltano-3.4.0a2/tests/meltano/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_compile.py` & `meltano-3.4.0a2/tests/meltano/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_config.py` & `meltano-3.4.0a2/tests/meltano/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_elt.py` & `meltano-3.4.0a2/tests/meltano/cli/test_elt.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_hub.py` & `meltano-3.4.0a2/tests/meltano/cli/test_hub.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_initialize.py` & `meltano-3.4.0a2/tests/meltano/cli/test_initialize.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_install.py` & `meltano-3.4.0a2/tests/meltano/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_invoke.py` & `meltano-3.4.0a2/tests/meltano/cli/test_invoke.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_job_cmd.py` & `meltano-3.4.0a2/tests/meltano/cli/test_job_cmd.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_lock.py` & `meltano-3.4.0a2/tests/meltano/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_remove.py` & `meltano-3.4.0a2/tests/meltano/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_run.py` & `meltano-3.4.0a2/tests/meltano/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_schedule.py` & `meltano-3.4.0a2/tests/meltano/cli/test_schedule.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_select.py` & `meltano-3.4.0a2/tests/meltano/cli/test_select.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_state.py` & `meltano-3.4.0a2/tests/meltano/cli/test_state.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/cli/test_upgrade.py` & `meltano-3.4.0a2/tests/meltano/cli/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/behavior/test_canonical.py` & `meltano-3.4.0a2/tests/meltano/core/behavior/test_canonical.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/behavior/test_hookable.py` & `meltano-3.4.0a2/tests/meltano/core/behavior/test_hookable.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/block/test_extract_load.py` & `meltano-3.4.0a2/tests/meltano/core/block/test_extract_load.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/block/test_plugin_command.py` & `meltano-3.4.0a2/tests/meltano/core/block/test_plugin_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/block/test_singer.py` & `meltano-3.4.0a2/tests/meltano/core/block/test_singer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/container/test_container_spec.py` & `meltano-3.4.0a2/tests/meltano/core/container/test_container_spec.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/hub/test_meltano_hub_service.py` & `meltano-3.4.0a2/tests/meltano/core/hub/test_meltano_hub_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/job/test_finder.py` & `meltano-3.4.0a2/tests/meltano/core/job/test_finder.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/job/test_job.py` & `meltano-3.4.0a2/tests/meltano/core/job/test_job.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/job/test_stale_job_failer.py` & `meltano-3.4.0a2/tests/meltano/core/job/test_stale_job_failer.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/logging/test_formatters.py` & `meltano-3.4.0a2/tests/meltano/core/logging/test_formatters.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/logging/test_logging_utils.py` & `meltano-3.4.0a2/tests/meltano/core/logging/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/logging/test_output_logger.py` & `meltano-3.4.0a2/tests/meltano/core/logging/test_output_logger.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_catalog.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_catalog.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_mapper.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_mapper.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_tap.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_tap.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/singer/test_target.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/singer/test_target.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/test_airflow.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/test_airflow.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/test_command.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/test_command.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/test_plugin_settings.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/test_plugin_settings.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/plugin/test_superset.py` & `meltano-3.4.0a2/tests/meltano/core/plugin/test_superset.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/runner/test_runner.py` & `meltano-3.4.0a2/tests/meltano/core/runner/test_runner.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/state_store/test_db.py` & `meltano-3.4.0a2/tests/meltano/core/state_store/test_db.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/state_store/test_filesystem.py` & `meltano-3.4.0a2/tests/meltano/core/state_store/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/state_store/test_state_store.py` & `meltano-3.4.0a2/tests/meltano/core/state_store/test_state_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_db_compat.py` & `meltano-3.4.0a2/tests/meltano/core/test_db_compat.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_db_connection.py` & `meltano-3.4.0a2/tests/meltano/core/test_db_connection.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_elt_context.py` & `meltano-3.4.0a2/tests/meltano/core/test_elt_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_environment_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_environment_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_environment_variables.py` & `meltano-3.4.0a2/tests/meltano/core/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_locked_definition_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_locked_definition_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_meltano_file.py` & `meltano-3.4.0a2/tests/meltano/core/test_meltano_file.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_meltano_invoker.py` & `meltano-3.4.0a2/tests/meltano/core/test_meltano_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_plugin_install_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_plugin_install_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_plugin_invoker.py` & `meltano-3.4.0a2/tests/meltano/core/test_plugin_invoker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_plugin_lock_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_plugin_lock_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_plugin_remove_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_plugin_remove_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_plugin_test_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_plugin_test_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project.py` & `meltano-3.4.0a2/tests/meltano/core/test_project.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project_add_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_project_add_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project_files.py` & `meltano-3.4.0a2/tests/meltano/core/test_project_files.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project_init_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_project_init_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project_plugins_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_project_plugins_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_project_settings_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_project_settings_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_schedule_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_schedule_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_setting_definition.py` & `meltano-3.4.0a2/tests/meltano/core/test_setting_definition.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_settings_store.py` & `meltano-3.4.0a2/tests/meltano/core/test_settings_store.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_state_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_state_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_task_sets.py` & `meltano-3.4.0a2/tests/meltano/core/test_task_sets.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_task_sets_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_task_sets_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_utils.py` & `meltano-3.4.0a2/tests/meltano/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_validation_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_validation_service.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/test_venv_service.py` & `meltano-3.4.0a2/tests/meltano/core/test_venv_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import os
 import platform
 import re
 import subprocess
 import sys
 import typing as t
+from asyncio.subprocess import Process
 
 import mock
 import pytest
 
-from meltano.core.error import MeltanoError
+from meltano.core.error import AsyncSubprocessError, MeltanoError
 from meltano.core.plugin import PluginType
 from meltano.core.plugin.project_plugin import ProjectPlugin
 from meltano.core.plugin_install_service import install_pip_plugin
-from meltano.core.venv_service import VenvService, VirtualEnv
+from meltano.core.venv_service import UvVenvService, VenvService, VirtualEnv
 
 if t.TYPE_CHECKING:
     from meltano.core.project import Project
 
 
 def _check_venv_created_with_python(project: Project, python: str | None):
     with mock.patch(
@@ -122,27 +123,15 @@
             )
 
         # Make sure the venv exists already
         await subject.install(["example"], clean=True)
         venv_dir = subject.project.venvs_dir("namespace", "name")
 
         # remove the package, then check that after a regular install the package exists
-        run = subprocess.run(
-            [
-                venv_dir.joinpath("bin/python"),
-                "-m",
-                "pip",
-                "uninstall",
-                "--yes",
-                "example",
-            ],
-            check=True,
-            capture_output=True,
-        )
-
+        await subject.uninstall_package("example")
         await subject.install(["example"])
 
         # ensure that the package is installed
         run = subprocess.run(
             [venv_dir.joinpath("bin/python"), "-m", "pip", "list"],
             check=True,
             capture_output=True,
@@ -283,7 +272,74 @@
             VirtualEnv(root, python="test-python-executable")
 
         with pytest.raises(
             MeltanoError,
             match="Python executable 'test-python-executable' was not found",
         ):
             VirtualEnv(root, python="test-python-executable")
+
+
+class TestUvVenvService:
+    @pytest.fixture()
+    def subject(self, project):
+        return UvVenvService(project=project, namespace="namespace", name="name")
+
+    def test_find_uv_builtin(self, project: Project, monkeypatch: pytest.MonkeyPatch):
+        monkeypatch.setattr("uv.find_uv_bin", lambda: "/usr/bin/uv")
+        service = UvVenvService(project=project, namespace="namespace", name="name")
+        assert service.uv == "/usr/bin/uv"
+
+    def test_find_uv_global(self, project: Project, monkeypatch: pytest.MonkeyPatch):
+        def raise_import_error():
+            raise ImportError
+
+        monkeypatch.setattr("uv.find_uv_bin", raise_import_error)
+        monkeypatch.setattr("shutil.which", lambda _: "/usr/bin/uv")
+
+        service = UvVenvService(project=project, namespace="namespace", name="name")
+        assert service.uv == "/usr/bin/uv"
+
+    def test_find_uv_not_found(self, project: Project, monkeypatch: pytest.MonkeyPatch):
+        def raise_import_error():
+            raise ImportError
+
+        monkeypatch.setattr("uv.find_uv_bin", raise_import_error)
+        monkeypatch.setattr("shutil.which", lambda _: None)
+
+        with pytest.raises(MeltanoError, match="Could not find the 'uv' executable"):
+            UvVenvService(project=project, namespace="namespace", name="name")
+
+    @pytest.mark.asyncio()
+    @pytest.mark.usefixtures("project")
+    async def test_install(self, subject: UvVenvService):
+        # Make sure the venv exists already
+        await subject.install(["cowsay"], clean=True)
+
+        # remove the package, then check that after a regular install the package exists
+        await subject.uninstall_package("cowsay")
+        await subject.install(["cowsay"])
+
+        run = subprocess.run(
+            [
+                subject.uv,
+                "pip",
+                "list",
+                "--python",
+                str(subject.exec_path("python")),
+            ],
+            check=True,
+            capture_output=True,
+        )
+        assert "cowsay" in str(run.stdout)
+
+    async def test_handle_installation_error(self, subject: UvVenvService):
+        process = mock.Mock(spec=Process)
+        process.stderr = "Some error"
+
+        with mock.patch(
+            "meltano.core.venv_service.UvVenvService.install_pip_args",
+            side_effect=AsyncSubprocessError("Something went wrong", process),
+        ), pytest.raises(
+            AsyncSubprocessError,
+            match="Failed to install plugin 'name'",
+        ):
+            await subject.install(["cowsay"])
```

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_environment_context.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_environment_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_exception.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_exception.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_plugins.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_plugins.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_project_context.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_project_context.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_schemas.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_schemas.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/tests/meltano/core/tracking/test_tracker.py` & `meltano-3.4.0a2/tests/meltano/core/tracking/test_tracker.py`

 * *Files identical despite different names*

### Comparing `meltano-3.4.0a1/PKG-INFO` & `meltano-3.4.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltano
-Version: 3.4.0a1
+Version: 3.4.0a2
 Summary: Meltano is your CLI for ELT+: Open Source, Flexible, and Scalable. Move, transform, and test your data with confidence using a streamlined data engineering workflow you’ll love.
 Home-page: https://meltano.com
 License: MIT
 Keywords: Meltano,ELT,Data integration,singer-io,dbt
 Author: Meltano
 Author-email: hello@meltano.com
 Requires-Python: >=3.8,<3.13
@@ -20,22 +20,23 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Provides-Extra: azure
 Provides-Extra: gcs
 Provides-Extra: mssql
 Provides-Extra: postgres
 Provides-Extra: psycopg2
 Provides-Extra: s3
+Provides-Extra: uv
 Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: atomicwrites (>=1.2.1,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-core (>=1.30.1,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "azure"
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0) ; extra == "azure"
-Requires-Dist: boto3 (>=1.34.74,<2.0.0) ; extra == "s3"
+Requires-Dist: boto3 (>=1.34.79,<2.0.0) ; extra == "s3"
 Requires-Dist: check-jsonschema (>=0.28.1,<0.29.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: click-didyoumean (>=0.3.1,<0.4.0)
 Requires-Dist: croniter (>=2.0.3,<3.0.0)
 Requires-Dist: fasteners (>=0.19,<0.20)
 Requires-Dist: flatten-dict (>=0,<1)
@@ -45,15 +46,15 @@
 Requires-Dist: jsonschema (>=4.21,<5.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "psycopg2"
 Requires-Dist: psycopg[binary] (>=3.1.18,<4.0.0) ; extra == "postgres"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
-Requires-Dist: pymssql (>=2.2.11,<3.0.0) ; extra == "mssql"
+Requires-Dist: pymssql (>=2.3.0,<3.0.0) ; extra == "mssql"
 Requires-Dist: python-dateutil (>=2.9.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: questionary (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -61,17 +62,18 @@
 Requires-Dist: ruamel.yaml (>=0.18.6,<0.19.0)
 Requires-Dist: setuptools (>=69.2.0,<70.0.0) ; python_version >= "3.12"
 Requires-Dist: smart-open (>=7.0.4,<8.0.0)
 Requires-Dist: snowplow-tracker (>=1.0.2,<2.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Requires-Dist: tzlocal (>=5.2,<6.0)
 Requires-Dist: urllib3 (<2)
+Requires-Dist: uv (>=0.1.24,<0.2) ; extra == "uv"
 Requires-Dist: virtualenv (>=20.25.1,<21.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Changelog, https://github.com/meltano/meltano/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://docs.meltano.com
 Project-URL: Issue Tracker, https://github.com/meltano/meltano/issues
 Project-URL: Repository, https://github.com/meltano/meltano
 Project-URL: Slack, https://meltano.com/slack
```
