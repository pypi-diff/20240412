# Comparing `tmp/empaia_app_test_suite-3.5.0.tar.gz` & `tmp/empaia_app_test_suite-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empaia_app_test_suite-3.5.0.tar", max compression
+gzip compressed data, was "empaia_app_test_suite-3.6.0.tar", max compression
```

## Comparing `empaia_app_test_suite-3.5.0.tar` & `empaia_app_test_suite-3.6.0.tar`

### file list

```diff
@@ -1,160 +1,182 @@
--rw-r--r--   0        0        0     1288 2022-06-20 13:46:27.206227 empaia_app_test_suite-3.5.0/LICENSE
--rw-r--r--   0        0        0     6610 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/README.md
--rw-r--r--   0        0        0       87 2022-06-20 13:46:27.206227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/__init__.py
--rw-r--r--   0        0        0     2624 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli.py
--rw-r--r--   0        0        0        0 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/__init__.py
--rw-r--r--   0        0        0     2944 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/apps_cli.py
--rw-r--r--   0        0        0     1305 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/cases_cli.py
--rw-r--r--   0        0        0     5978 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/jobs_cli.py
--rw-r--r--   0        0        0     4684 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/main_cli.py
--rw-r--r--   0        0        0     3902 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/services_cli.py
--rw-r--r--   0        0        0     2491 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/slides_cli.py
--rw-r--r--   0        0        0        0 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/__init__.py
--rw-r--r--   0        0        0     5244 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/apps_commands.py
--rw-r--r--   0        0        0      921 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/cases_commands.py
--rw-r--r--   0        0        0        0 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/__init__.py
--rw-r--r--   0        0        0     4216 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/app_helper.py
--rw-r--r--   0        0        0     4329 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/data_helper.py
--rw-r--r--   0        0        0     2784 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/job_helper.py
--rw-r--r--   0        0        0    10654 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/job_validation_helper.py
--rw-r--r--   0        0        0     4218 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/wsi_helper.py
--rw-r--r--   0        0        0    13307 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/jobs_commands.py
--rw-r--r--   0        0        0     8804 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/services_commands.py
--rw-r--r--   0        0        0     2993 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/slides_commands.py
--rw-r--r--   0        0        0     5179 2023-12-15 15:08:15.953308 empaia_app_test_suite-3.5.0/empaia_app_test_suite/constants.py
--rw-r--r--   0        0        0     3984 2023-12-11 08:14:53.087858 empaia_app_test_suite-3.5.0/empaia_app_test_suite/custom_models.py
--rw-r--r--   0        0        0       56 2022-06-20 13:46:27.896227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.git
--rw-r--r--   0        0        0       32 2022-06-20 13:46:32.866227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitignore
--rw-r--r--   0        0        0      845 2022-06-20 13:46:32.866227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-06-20 13:46:32.866227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1447 2022-11-16 07:47:09.788307 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab-ci.yml
--rw-r--r--   0        0        0     2876 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2022-06-20 13:46:32.866227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/LICENSE
--rw-r--r--   0        0        0      302 2022-11-10 18:02:43.824370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/README.md
--rw-r--r--   0        0        0        0 2023-07-21 06:44:58.550682 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/__init__.py
--rw-r--r--   0        0        0      949 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/commons.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/marketplace/__init__.py
--rw-r--r--   0        0        0    18692 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/marketplace/app.py
--rw-r--r--   0        0        0    65744 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/poetry.lock
--rw-r--r--   0        0        0      803 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/pyproject.toml
--rw-r--r--   0        0        0       36 2022-06-20 13:46:32.866227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/setup.cfg
--rw-r--r--   0        0        0       69 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/singletons.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/__init__.py
--rw-r--r--   0        0        0     3983 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/tests/__init__.py
--rw-r--r--   0        0        0     8415 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/__init__.py
--rw-r--r--   0        0        0    12942 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/annotations.py
--rw-r--r--   0        0        0     3965 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/classes.py
--rw-r--r--   0        0        0    11890 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/collections.py
--rw-r--r--   0        0        0     2403 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/jobs.py
--rw-r--r--   0        0        0     6361 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/primitives.py
--rw-r--r--   0        0        0      429 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/server_settings.py
--rw-r--r--   0        0        0     6573 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/clinical.py
--rw-r--r--   0        0        0     3549 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/commons.py
--rw-r--r--   0        0        0     4109 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/examination.py
--rw-r--r--   0        0        0      990 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/id_mapper.py
--rw-r--r--   0        0        0     8317 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/job.py
--rw-r--r--   0        0        0     2180 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/slide.py
--rw-r--r--   0        0        0     2850 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/storage.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/tests/__init__.py
--rw-r--r--   0        0        0      448 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/__init__.py
--rw-r--r--   0        0        0    15111 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/annotations.py
--rw-r--r--   0        0        0     4202 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/classes.py
--rw-r--r--   0        0        0    21704 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/collections.py
--rw-r--r--   0        0        0      359 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/commons.py
--rw-r--r--   0        0        0      403 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/jobs.py
--rw-r--r--   0        0        0    18622 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/pixelmaps.py
--rw-r--r--   0        0        0     7321 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/primitives.py
--rw-r--r--   0        0        0      429 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/server_settings.py
--rw-r--r--   0        0        0     6573 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/clinical.py
--rw-r--r--   0        0        0     3966 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/commons.py
--rw-r--r--   0        0        0     9235 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/examination.py
--rw-r--r--   0        0        0      990 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/id_mapper.py
--rw-r--r--   0        0        0    12754 2023-12-15 15:07:57.372425 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/job.py
--rw-r--r--   0        0        0     2353 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/slide.py
--rw-r--r--   0        0        0     2850 2023-10-30 06:38:10.907943 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/storage.py
--rw-r--r--   0        0        0        0 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/__init__.py
--rw-r--r--   0        0        0      373 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_examination.py
--rw-r--r--   0        0        0      500 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
--rw-r--r--   0        0        0     2829 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py
--rw-r--r--   0        0        0     1816 2022-11-10 18:02:43.834370 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py
--rw-r--r--   0        0        0     2445 2022-11-26 17:47:46.729699 empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
--rw-r--r--   0        0        0       67 2022-06-24 09:48:43.526106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.git
--rw-r--r--   0        0        0       31 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitignore
--rw-r--r--   0        0        0      845 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0      791 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
--rw-r--r--   0        0        0      224 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitmodules
--rw-r--r--   0        0        0     1301 2023-12-15 15:08:00.372447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2023-10-30 06:38:18.637941 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/LICENSE
--rw-r--r--   0        0        0     6254 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/README.md
--rw-r--r--   0        0        0        0 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     3578 2023-12-15 15:08:00.372447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml
--rw-r--r--   0        0        0   111314 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/poetry.lock
--rw-r--r--   0        0        0        0 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     1232 2022-11-10 18:03:03.984365 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
--rw-r--r--   0        0        0      111 2022-06-24 09:49:09.757240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
--rw-r--r--   0        0        0        8 2022-06-24 09:49:09.767240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
--rw-r--r--   0        0        0      845 2022-08-25 20:48:38.152860 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      697 2022-08-25 20:48:38.152860 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1064 2023-10-30 06:38:01.597945 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/LICENSE
--rw-r--r--   0        0        0     1505 2022-06-24 09:49:09.767240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
--rw-r--r--   0        0        0    12338 2022-06-24 09:49:09.767240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
--rw-r--r--   0        0        0    17247 2022-06-24 09:49:09.767240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
--rw-r--r--   0        0        0    23793 2023-12-15 06:56:41.475261 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
--rw-r--r--   0        0        0      283 2022-11-10 18:03:11.674363 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
--rw-r--r--   0        0        0      170 2022-06-24 09:49:09.767240 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
--rw-r--r--   0        0        0    13873 2023-10-30 06:38:01.597945 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
--rw-r--r--   0        0        0     5744 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
--rw-r--r--   0        0        0      457 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
--rw-r--r--   0        0        0     4091 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
--rw-r--r--   0        0        0        0 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
--rw-r--r--   0        0        0     2674 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
--rw-r--r--   0        0        0        0 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
--rw-r--r--   0        0        0     5958 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
--rw-r--r--   0        0        0    17983 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
--rw-r--r--   0        0        0     2149 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
--rw-r--r--   0        0        0      880 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/pyproject.toml
--rw-r--r--   0        0        0      260 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/sample.env
--rw-r--r--   0        0        0       36 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/setup.cfg
--rw-r--r--   0        0        0        0 2022-06-24 09:48:43.536106 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
--rw-r--r--   0        0        0     9129 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
--rw-r--r--   0        0        0    23309 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
--rw-r--r--   0        0        0    10278 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
--rw-r--r--   0        0        0    38860 2023-12-15 15:08:00.382447 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
--rw-r--r--   0        0        0    10465 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
--rw-r--r--   0        0        0        0 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
--rw-r--r--   0        0        0    43777 2023-10-30 06:38:18.637941 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
--rw-r--r--   0        0        0     2186 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
--rw-r--r--   0        0        0    34033 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
--rw-r--r--   0        0        0     2345 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
--rw-r--r--   0        0        0    42456 2023-10-30 06:38:18.637941 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
--rw-r--r--   0        0        0     3024 2023-07-21 06:45:11.261616 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
--rw-r--r--   0        0        0      864 2022-06-27 11:28:42.551431 empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
--rw-r--r--   0        0        0     2999 2023-12-15 15:08:15.953308 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/docker-compose.yml
--rw-r--r--   0        0        0       48 2022-06-20 13:46:27.216227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/nginx/Dockerfile
--rw-r--r--   0        0        0     1263 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/nginx/nginx.conf
--rw-r--r--   0        0        0     1256 2023-07-21 06:45:05.060762 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile
--rw-r--r--   0        0        0        0 2022-06-20 13:46:32.886227 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__init__.py
--rw-r--r--   0        0        0     8492 2023-07-21 06:45:05.060762 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py
--rw-r--r--   0        0        0    10005 2023-07-21 06:45:05.060762 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py
--rw-r--r--   0        0        0     1750 2023-07-21 06:45:05.060762 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/timed_cache.py
--rw-r--r--   0        0        0      361 2023-10-30 06:38:25.757939 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml
--rw-r--r--   0        0        0     1164 2023-07-21 06:39:28.469332 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile
--rw-r--r--   0        0        0       81 2023-07-21 06:39:28.469332 empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/entrypoint.sh
--rw-r--r--   0        0        0    19739 2023-12-15 15:08:15.953308 empaia_app_test_suite-3.5.0/empaia_app_test_suite/settings.py
--rw-r--r--   0        0        0        0 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_aaa.py
--rw-r--r--   0        0        0     2681 2023-12-15 15:08:15.953308 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_commons.py
--rw-r--r--   0        0        0     8701 2023-12-11 08:14:53.087858 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_mds.py
--rw-r--r--   0        0        0     2183 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_mps.py
--rw-r--r--   0        0        0     5652 2023-10-30 06:36:52.827963 empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_print.py
--rw-r--r--   0        0        0     3035 2023-12-15 15:08:15.953308 empaia_app_test_suite-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     8337 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1288 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/LICENSE
+-rw-r--r--   0        0        0     6468 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/README.md
+-rw-r--r--   0        0        0       87 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/__init__.py
+-rw-r--r--   0        0        0     2624 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/__init__.py
+-rw-r--r--   0        0        0     2944 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/apps_cli.py
+-rw-r--r--   0        0        0     1305 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/cases_cli.py
+-rw-r--r--   0        0        0     5978 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/jobs_cli.py
+-rw-r--r--   0        0        0     4560 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/main_cli.py
+-rw-r--r--   0        0        0     3766 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/services_cli.py
+-rw-r--r--   0        0        0     2491 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/slides_cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/__init__.py
+-rw-r--r--   0        0        0     5244 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/apps_commands.py
+-rw-r--r--   0        0        0      921 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/cases_commands.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/__init__.py
+-rw-r--r--   0        0        0     4216 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/app_helper.py
+-rw-r--r--   0        0        0     4329 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/data_helper.py
+-rw-r--r--   0        0        0     2784 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/job_helper.py
+-rw-r--r--   0        0        0    10654 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/job_validation_helper.py
+-rw-r--r--   0        0        0     4223 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/wsi_helper.py
+-rw-r--r--   0        0        0    13307 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/jobs_commands.py
+-rw-r--r--   0        0        0     9990 2024-04-12 06:35:08.194527 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/services_commands.py
+-rw-r--r--   0        0        0     2990 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/slides_commands.py
+-rw-r--r--   0        0        0     5154 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/constants.py
+-rw-r--r--   0        0        0     3936 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/custom_models.py
+-rw-r--r--   0        0        0       56 2023-06-22 12:40:49.959750 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.git
+-rw-r--r--   0        0        0       32 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitignore
+-rw-r--r--   0        0        0      845 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1447 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3164 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/LICENSE
+-rw-r--r--   0        0        0      302 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/__init__.py
+-rw-r--r--   0        0        0      965 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/commons.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/marketplace/__init__.py
+-rw-r--r--   0        0        0    18692 2023-10-24 08:36:22.461963 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/marketplace/app.py
+-rw-r--r--   0        0        0    65744 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/poetry.lock
+-rw-r--r--   0        0        0      803 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/setup.cfg
+-rw-r--r--   0        0        0       69 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/singletons.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/__init__.py
+-rw-r--r--   0        0        0     3983 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/access_token_tools.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/tests/__init__.py
+-rw-r--r--   0        0        0     8415 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/__init__.py
+-rw-r--r--   0        0        0    12942 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/annotations.py
+-rw-r--r--   0        0        0     3965 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/classes.py
+-rw-r--r--   0        0        0    11890 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/collections.py
+-rw-r--r--   0        0        0     2403 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/jobs.py
+-rw-r--r--   0        0        0     6361 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/primitives.py
+-rw-r--r--   0        0        0      429 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/server_settings.py
+-rw-r--r--   0        0        0     6835 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/clinical.py
+-rw-r--r--   0        0        0     3549 2024-03-22 07:41:19.304381 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/commons.py
+-rw-r--r--   0        0        0     4109 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/examination.py
+-rw-r--r--   0        0        0      990 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/id_mapper.py
+-rw-r--r--   0        0        0     8317 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/job.py
+-rw-r--r--   0        0        0     2180 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/slide.py
+-rw-r--r--   0        0        0     1154 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/storage.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/tests/__init__.py
+-rw-r--r--   0        0        0      448 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/__init__.py
+-rw-r--r--   0        0        0    15111 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/annotations.py
+-rw-r--r--   0        0        0     4202 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/classes.py
+-rw-r--r--   0        0        0    21704 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/collections.py
+-rw-r--r--   0        0        0      359 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/commons.py
+-rw-r--r--   0        0        0      403 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/jobs.py
+-rw-r--r--   0        0        0    18622 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/pixelmaps.py
+-rw-r--r--   0        0        0     7321 2023-12-14 09:42:07.958409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/primitives.py
+-rw-r--r--   0        0        0      429 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/server_settings.py
+-rw-r--r--   0        0        0     7623 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/clinical.py
+-rw-r--r--   0        0        0     3966 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/commons.py
+-rw-r--r--   0        0        0     9235 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/examination.py
+-rw-r--r--   0        0        0      990 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/id_mapper.py
+-rw-r--r--   0        0        0    12754 2023-12-14 09:42:07.968409 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/job.py
+-rw-r--r--   0        0        0     2353 2023-10-19 12:59:08.082835 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/slide.py
+-rw-r--r--   0        0        0     1154 2024-03-15 06:55:56.170309 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/storage.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/__init__.py
+-rw-r--r--   0        0        0      373 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_examination.py
+-rw-r--r--   0        0        0      500 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0     2829 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py
+-rw-r--r--   0        0        0     1816 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py
+-rw-r--r--   0        0        0     2445 2023-06-22 12:40:54.369752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
+-rw-r--r--   0        0        0       67 2023-06-22 12:40:50.889751 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.git
+-rw-r--r--   0        0        0       31 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitignore
+-rw-r--r--   0        0        0      845 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0      791 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
+-rw-r--r--   0        0        0      224 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitmodules
+-rw-r--r--   0        0        0     1301 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-10-19 12:59:17.394289 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/LICENSE
+-rw-r--r--   0        0        0     6254 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     3578 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml
+-rw-r--r--   0        0        0   111314 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/poetry.lock
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
+-rw-r--r--   0        0        0      111 2023-06-22 12:40:55.299753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
+-rw-r--r--   0        0        0        8 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
+-rw-r--r--   0        0        0      845 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      697 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1064 2023-10-24 08:36:09.870495 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/LICENSE
+-rw-r--r--   0        0        0     1505 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
+-rw-r--r--   0        0        0    12338 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
+-rw-r--r--   0        0        0    17247 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
+-rw-r--r--   0        0        0    23793 2023-12-14 09:42:23.801837 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
+-rw-r--r--   0        0        0      283 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
+-rw-r--r--   0        0        0      170 2023-06-22 12:40:56.369753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
+-rw-r--r--   0        0        0    13873 2023-10-24 08:36:09.870495 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
+-rw-r--r--   0        0        0     5744 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
+-rw-r--r--   0        0        0      457 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
+-rw-r--r--   0        0        0     4091 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
+-rw-r--r--   0        0        0     2674 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
+-rw-r--r--   0        0        0     5958 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
+-rw-r--r--   0        0        0    17983 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
+-rw-r--r--   0        0        0     2149 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
+-rw-r--r--   0        0        0      880 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/sample.env
+-rw-r--r--   0        0        0       36 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
+-rw-r--r--   0        0        0     9129 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
+-rw-r--r--   0        0        0    23309 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
+-rw-r--r--   0        0        0    10278 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
+-rw-r--r--   0        0        0    38860 2023-12-14 09:42:16.471788 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
+-rw-r--r--   0        0        0    10465 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-22 12:40:56.359753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/.git
+-rw-r--r--   0        0        0       31 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/.gitignore
+-rw-r--r--   0        0        0      845 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0      295 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/.gitlab-ci.yml
+-rw-r--r--   0        0        0      462 2023-10-19 12:59:49.109069 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/LICENSE
+-rw-r--r--   0        0        0     1245 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/README.md
+-rw-r--r--   0        0        0    16218 2023-10-19 12:59:49.119069 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/__init__.py
+-rw-r--r--   0        0        0    43897 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/poetry.lock
+-rw-r--r--   0        0        0      689 2023-10-19 12:59:49.119069 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/pyproject.toml
+-rwxr-xr-x   0        0        0       36 2023-06-22 12:40:56.379753 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/empaia_sender_auth/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
+-rw-r--r--   0        0        0    43777 2023-10-19 12:59:17.394289 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
+-rw-r--r--   0        0        0     2186 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
+-rw-r--r--   0        0        0    34033 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
+-rw-r--r--   0        0        0     2345 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
+-rw-r--r--   0        0        0    42456 2023-10-19 12:59:17.394289 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
+-rw-r--r--   0        0        0     3024 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
+-rw-r--r--   0        0        0      864 2023-06-22 12:40:54.379752 empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1397 2024-04-10 06:48:52.572954 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/Dockerfile
+-rw-r--r--   0        0        0        0 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/cds_plugin_isyntax/__init__.py
+-rw-r--r--   0        0        0      208 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/cds_plugin_isyntax/__main__.py
+-rw-r--r--   0        0        0    16612 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/cds_plugin_isyntax/slide.py
+-rw-r--r--   0        0        0     1715 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/cds_plugin_isyntax/slide_utils.py
+-rw-r--r--   0        0        0      377 2024-04-10 06:48:52.572954 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/pyproject.toml
+-rw-r--r--   0        0        0     1164 2024-03-20 10:49:45.302396 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/mirax/Dockerfile
+-rw-r--r--   0        0        0       81 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/mirax/entrypoint.sh
+-rw-r--r--   0        0        0        0 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/__init__.py
+-rw-r--r--   0        0        0     4460 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/backend_server.py
+-rw-r--r--   0        0        0     1114 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/base_slide_instance.py
+-rw-r--r--   0        0        0      424 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/log_utils.py
+-rw-r--r--   0        0        0      987 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/response_handler.py
+-rw-r--r--   0        0        0    10873 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/slide_utils.py
+-rw-r--r--   0        0        0     6169 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/slide_worker.py
+-rw-r--r--   0        0        0     1380 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/worker_cache.py
+-rw-r--r--   0        0        0      244 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/poetry.lock
+-rw-r--r--   0        0        0      277 2024-03-20 07:30:37.976791 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/pyproject.toml
+-rw-r--r--   0        0        0     3672 2024-04-12 06:34:24.483495 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/docker-compose.yml
+-rw-r--r--   0        0        0       48 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/nginx/Dockerfile
+-rw-r--r--   0        0        0     1263 2024-03-15 15:30:40.191766 empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/nginx/nginx.conf
+-rw-r--r--   0        0        0    21052 2024-04-12 06:35:24.456165 empaia_app_test_suite-3.6.0/empaia_app_test_suite/settings.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-06-22 12:40:49.019749 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_aaa.py
+-rw-r--r--   0        0        0     2681 2024-01-03 07:47:10.073807 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_commons.py
+-rw-r--r--   0        0        0     7603 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_mds.py
+-rw-r--r--   0        0        0     2183 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_mps.py
+-rw-r--r--   0        0        0     5652 2023-10-24 08:51:23.534687 empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_print.py
+-rw-r--r--   0        0        0     3256 2024-04-12 06:10:21.079806 empaia_app_test_suite-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.6.0/PKG-INFO
```

### Comparing `empaia_app_test_suite-3.5.0/LICENSE` & `empaia_app_test_suite-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/README.md` & `empaia_app_test_suite-3.6.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # EMPAIA App Test Suite (EATS)
 
 ## Requirements
 
-* The EMPAIA App Test Suite requires Python 3.8.
+* The EMPAIA App Test Suite requires Python 3.10.
 * Supported Operating Systems are Linux, Windows and MacOS
   * for **Windows** the EATS requires the usage of WSL 2 (Windows Subsystem for Linux) with Docker for Windows
 
 ## Installation
 
 There are different possibilities to install the EMPAIA App Test Suite depending on your intended use:
 
@@ -69,37 +69,28 @@
 
 Run the EATS CLI app with
 
 ```bash
 eats
 ```
 
-To force pull and build services and submodules:
+To force pull and build services:
 
 ```bash
-eats services up ./wsi-mount-points.json --build --pull
+eats services up <wsi-mount-points-path> --build --pull
 ```
 
 ## Usage
 
 **For detailed instructions take a look at the [App Developer Documentation](https://developer.empaia.org/app_developer_docs/#/)**
 
-Define absolute paths to directories containing WSIs in a `./wsi-mount-points.json` file as follows:
-
-```json
-{
-    "/absolute/local/path/to/wsis/dir1": "/data/",
-    "/absolute/local/path/to/wsis/dir2": "/data2/"
-}
-```
-
 Start all backend services in Docker containers using the `eats services up` command. WSI directories are mounted into the WSI Service container. Only WSIs contained in one of the specified directories can be used as a job input.
 
 ```bash
-eats services up ./wsi-mount-points.json
+eats services up <wsi-mount-points-path>
 ```
 
 You can perform health checks of running backend services.
 
 ```bash
 eats services health
 ```
@@ -130,49 +121,49 @@
 ```bash
 eats jobs run ./job.env
 ```
 
 The job ID can be retrieved from the `job.env` file to be used in other commands.
 
 ```bash
-export $(xargs <job.env)
+export $(xargs < job.env)
 echo $EMPAIA_JOB_ID
 ```
 
 Regularly check the jobs status until it is `COMPLETED`.
 
 ```bash
-eats jobs status ${EMPAIA_JOB_ID}
+eats jobs status $EMPAIA_JOB_ID
 ```
 
 The job ID is used as the container name. It can be used to retrieved docker logs.
 
 ```bash
-docker logs ${EMPAIA_JOB_ID}
+docker logs $EMPAIA_JOB_ID
 ```
 
 Open `localhost:8888/wbc3` in a Browser to review job results using the Workbench Client 3.0.
 
 In addition, the job results can be exported to JSON files in a `job-outputs` directory.
 
 ```bash
-eats jobs export ${EMPAIA_JOB_ID} ./job-outputs
+eats jobs export $EMPAIA_JOB_ID ./job-outputs
 ```
 
 If a job is taking too long or is stuck, the job can be aborted.
 
 ```bash
-eats jobs abort ${EMPAIA_JOB_ID}
+eats jobs abort $EMPAIA_JOB_ID
 ```
 
-To inspect backend service logs the `docker logs` command can used directly. The names of all service containers can be retrieved using the `eats services list` command.
+To inspect backend service logs the `docker logs` command can be used directly. The names of all service containers can be retrieved using the `eats services list` command.
 
 ```bash
 eats services list  # print list of service names
-docker logs ${SERVICE_NAME}
+docker logs <SERVICE_NAME>
 ```
 
 It is possible to register and run multiple jobs without restart backend services. The services can be stopped, if they are not needed anymore. All created data is available when the services are started again.
 
 ```bash
 eats services down
 ```
@@ -202,38 +193,37 @@
 black empaia_app_test_suite tests check_version.py
 pycodestyle empaia_app_test_suite tests check_version.py
 pylint empaia_app_test_suite tests check_version.py
 ```
 
 ### Tests
 
-Create `./wsi-mount-points.json`:
+Create a directory in which the WSI [CMU-1.svs](http://openslide.cs.cmu.edu/download/openslide-testdata/Aperio/CMU-1.svs) is located in a subdirectory "Aperio":
 
-```JSON
-{
-  "/path/to/testdata/Aperio/": "/data",
-  "/path/to/testdata/Fluorescence OME-Tif/": "/data2"
-}
+```
+WSI_BASE_PATH
+└── Aperio
+    └── CMU-1.svs
 ```
 
 ```bash
 # run cli command tests
-pytest tests/commands --maxfail=1 -s -v
+pytest tests/commands --maxfail=1 -s -v --mount-point <WSI_BASE_PATH>
 
-eats services up ./wsi-mount-points.json --build --pull
+eats services up <WSI_BASE_PATH> --build --pull
 
 # run sample apps tests
 pytest tests/sample_apps_tests --maxfail=1 -s -v
 ```
 
 If a test from `tests/sample_apps` fails, use `docker logs <servicename>` for debugging.
 
 ### Test GPU support
 
 ```bash
-eats services up ./wsi-mount-points.json --build --pull --gpu-driver nvidia
+eats services up <WSI_BASE_PATH> --build --pull --gpu-driver nvidia
 
-# run cli command test
+# run gpu sample apps test
 pytest tests/gpu_support_test
 ```
 
 If docker is locally installed with support for CUDA and a supported GPU is available on the host system the test must succeed. If the test fails please check if docker is correctly installed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/apps_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/apps_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/cases_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/cases_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/jobs_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/jobs_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/main_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/main_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             None, "--version", callback=version_callback, is_eager=True, help=const.VERSION_HELP
         ),
     ):
         return
 
     @app.command("exec")
     def _(
-        wsi_mount_points_file: Path = typer.Argument(..., help=const.WSI_MOUNT_POINTS_FILE_HELP),
+        wsi_mount_point: Path = typer.Argument(..., help=const.WSI_MOUNT_POINT_HELP),
         ead_file: Path = typer.Argument(..., help=const.EAD_FILE_HELP),
         docker_image: str = typer.Argument(..., help=const.DOCKER_IMAGE_HELP),
         input_dir: Path = typer.Argument(..., help=const.INPUT_DIR_HELP),
         output_dir: Path = typer.Argument(..., help=const.OUTPUT_DIR_HELP),
         job_mode: Optional[str] = typer.Argument("standalone", help=const.JOB_MODE),
         build: bool = typer.Option(False, "--build", help=const.BUILD_HELP),
         pull: bool = typer.Option(False, "--pull", help=const.PULL_HELP),
@@ -48,26 +48,23 @@
         frontend_token_exp: int = typer.Option(60, "--frontend-token-exp", help=const.FRONTEND_TOKEN_EXP),
         scope_token_exp: int = typer.Option(300, "--scope-token-exp", help=const.SCOPE_TOKEN_EXP),
         app_ui_frame_ancestors: str = typer.Option(None, "--app-ui-frame-ancestors", help=const.FRAME_ANCENSTORS_HELP),
         app_ui_connect_src: str = typer.Option(None, "--app-ui-connect-src", help=const.CONNECT_SOURCE_HELP),
         app_ui_disable_csp: bool = typer.Option(False, "--app-ui-disable-csp", help=const.DISABLE_CSP_HELP),
         alt_user: bool = typer.Option(False, "--alt-user", help=const.ALT_USER_HELP),
     ):
-        with open(wsi_mount_points_file, encoding="utf-8") as f:
-            wsi_mount_points = json.load(f)
-
         with open(ead_file, "r", encoding="utf-8") as f:
             ead = json.load(f)
 
         client = docker.from_env()
 
         services_down(client=client, volume_prefix=volume_prefix)
         services_up(
             client=client,
-            wsi_mount_points=wsi_mount_points,
+            wsi_mount_point=wsi_mount_point,
             docker_config=docker_config,
             build=build,
             pull=pull,
             nginx_port=nginx_port,
             wbs_url=wbs_url,
             isyntax_sdk=isyntax_sdk,
             mirax_plugin=mirax_plugin,
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/services_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/services_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from pathlib import Path
 
 import docker
 import typer
 
 import empaia_app_test_suite.constants as const
 from empaia_app_test_suite.commands.services_commands import (
@@ -14,15 +13,15 @@
     services_wait,
 )
 
 
 def init_services_cli(services_app):
     @services_app.command("up")
     def _(
-        wsi_mount_points_file: Path = typer.Argument(..., help=const.WSI_MOUNT_POINTS_FILE_HELP),
+        wsi_mount_point: Path = typer.Argument(..., help=const.WSI_MOUNT_POINT_HELP),
         build: bool = typer.Option(False, "--build", help=const.BUILD_HELP),
         pull: bool = typer.Option(False, "--pull", help=const.PULL_HELP),
         docker_config: Path = typer.Option(None, "--docker-config", help=const.DOCKER_CONFIG_FILE_HELP),
         nginx_port: int = typer.Option(8888, "--nginx-port", help=const.NGINX_PORT_HELP),
         wbs_url: str = typer.Option(None, "--wbs-url", help=const.WBS_URL_HELP),
         isyntax_sdk: str = typer.Option(None, "--isyntax-sdk", help=const.ISYNTAX_SDK_HELP),
         mirax_plugin: str = typer.Option(None, "--mirax-plugin", help=const.MIRAX_PLUGIN_HELP),
@@ -30,22 +29,19 @@
         gpu_driver: str = typer.Option(None, "--gpu-driver", help=const.GPU_DRIVER_HELP),
         frontend_token_exp: int = typer.Option(86400, "--frontend-token-exp", help=const.FRONTEND_TOKEN_EXP),
         scope_token_exp: int = typer.Option(300, "--scope-token-exp", help=const.SCOPE_TOKEN_EXP),
         app_ui_frame_ancestors: str = typer.Option(None, "--app-ui-frame-ancestors", help=const.FRAME_ANCENSTORS_HELP),
         app_ui_connect_src: str = typer.Option(None, "--app-ui-connect-src", help=const.CONNECT_SOURCE_HELP),
         app_ui_disable_csp: bool = typer.Option(False, "--app-ui-disable-csp", help=const.DISABLE_CSP_HELP),
     ):
-        with open(wsi_mount_points_file, encoding="utf-8") as f:
-            wsi_mount_points = json.load(f)
-
         client = docker.from_env()
         services_down(client=client, volume_prefix=volume_prefix)
         services_up(
             client=client,
-            wsi_mount_points=wsi_mount_points,
+            wsi_mount_point=wsi_mount_point,
             docker_config=docker_config,
             build=build,
             pull=pull,
             nginx_port=nginx_port,
             wbs_url=wbs_url,
             isyntax_sdk=isyntax_sdk,
             mirax_plugin=mirax_plugin,
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/cli_definitions/slides_cli.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/cli_definitions/slides_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/apps_commands.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/apps_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/cases_commands.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/cases_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/app_helper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/app_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/data_helper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/data_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/job_helper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/job_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/job_validation_helper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/job_validation_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/helper/wsi_helper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/helper/wsi_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,26 +66,25 @@
                     error_msg = (
                         f"Slide with id [{wsi_info.id}] already exists but with a different value for {p}: [{wsi[p]}]."
                     )
                     raise Exception(error_msg)
             existing_wsis.append(wsi_info)
         else:
             new_wsis.append(wsi_info)
-        # check values equal in SMS
+        # check values equal in CDS
         r = requests.get(f"{mds_url}/private/v3/slides/{wsi_info.id}/storage")
-        if r.status_code != 404:  # Not "Not found" (= already exists)
-            existing_slide_sms = r.json()
-            for address in existing_slide_sms["storage_addresses"]:
-                if address["main_address"]:
-                    if address["address"] != wsi_info.path:
-                        error_msg = (
-                            f"Slide with id [{wsi_info.id}] already exists "
-                            f"but with a different path: {address['address']}"
-                        )
-                        raise Exception(error_msg)
+        if r.status_code not in [400, 404]:  # Not "Not found" (= already exists)
+            existing_slide_cds = r.json()
+            wsi_info_path_without_root = wsi_info.path.replace("/data/", "")
+            if existing_slide_cds["main_storage_address"]["path"] != wsi_info_path_without_root:
+                error_msg = (
+                    f"Slide with id [{wsi_info.id}] already exists "
+                    f"but with a different path: {existing_slide_cds['main_storage_address']['path']}"
+                )
+                raise Exception(error_msg)
     return new_wsis, existing_wsis
 
 
 def validate_wsis_current_job_inputs(wsis_to_register: List[WsiInput]):
     no_duplicate_wsis = []
     duplicate_wsis = []
     wsis = {}
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/jobs_commands.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/jobs_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/services_commands.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/services_commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from pathlib import Path
 from time import sleep
 
 import docker
 import requests
 
 from empaia_app_test_suite import settings
 from empaia_app_test_suite.constants import SERVICE_API_MAPPING
@@ -80,15 +79,15 @@
         if service["name"] in SERVICE_API_MAPPING and "service" in service["name"]:
             exposed_services.append(service["name"])
     return exposed_services
 
 
 def services_list(client):
     services = settings.get_services()
-    for plugin in ["isyntax-backend", "mirax-backend"]:
+    for plugin in ["cds-plugin-isyntax", "cds-plugin-mirax"]:
         try:
             client.containers.get(plugin)
             services.append({"name": plugin})
         except docker.errors.NotFound:
             pass
     databases = settings.get_databases()
     return [service["name"] for service in services] + [db["name"] for db in databases]
@@ -119,15 +118,15 @@
             with PrintStep(f"Removing volume: {v}", catch_exc=True):
                 vol = client.volumes.get(v)
                 vol.remove(force=True)
 
 
 def services_up(
     client,
-    wsi_mount_points,
+    wsi_mount_point,
     build,
     pull,
     docker_config=None,
     nginx_port=None,
     wbs_url=None,
     isyntax_sdk=None,
     mirax_plugin=None,
@@ -146,21 +145,19 @@
                 error_reasons.append("'--app-ui-connect-src'")
             if app_ui_frame_ancestors:
                 error_reasons.append("'--app-ui-frame-ancestors'")
             raise Exception(
                 (f"The parameter '--app-ui-disable-csp' and {' / '.join(error_reasons)} cannot be used together")
             )
 
-    with PrintStep("Check WSI mount points"):
-        for key, val in wsi_mount_points.items():
-            key_path = Path(key)
-            val_path = val
-
-            assert key_path.is_absolute()
-            assert val_path.startswith("/")
+    with PrintStep("Check WSI mount point"):
+        if wsi_mount_point.suffix == ".json":
+            raise Exception(("Mount points as .json files are no longer supported (changed in EATS version 3.6.0)!"))
+        if not wsi_mount_point.is_absolute():
+            raise Exception((f"Mount point '{str(wsi_mount_point)}' not valid. Must be absolute!"))
 
     services = settings.get_services(
         nginx_port=nginx_port,
         wbs_url=wbs_url,
         isyntax_sdk=isyntax_sdk,
         mirax_plugin=mirax_plugin,
         gpu_driver=gpu_driver,
@@ -197,17 +194,25 @@
                 except docker.errors.ImageNotFound:
                     build_for_service = True
 
             if build_for_service:
                 with PrintStep(f"Building image: {image}"):
                     buildargs = None
                     dockerfile_path = service.get("dockerfile_path")
-                    client.images.build(
-                        path=service["path"], tag=image, buildargs=buildargs, dockerfile=dockerfile_path
-                    )
+                    try:
+                        client.images.build(
+                            path=service["path"], tag=image, buildargs=buildargs, dockerfile=dockerfile_path
+                        )
+                    except docker.errors.BuildError as e:
+                        print("Hey something went wrong with image build!")
+                        for line in e.build_log:
+                            if "stream" in line:
+                                print(line["stream"].strip())
+                        raise
+
     for db in databases:
         name = db["name"]
 
         volumes = {_volume_name(db["volume"]["name"], volume_prefix): {"bind": db["volume"]["mount"], "mode": "rw"}}
 
         with PrintStep(f"Starting: {name}"):
             client.containers.run(
@@ -227,31 +232,51 @@
         with PrintStep(f"Starting: {name}"):
             volumes = {}
 
             if "volume" in service:
                 volume = service["volume"]
                 volumes[_volume_name(volume["name"], volume_prefix)] = {"bind": volume["mount"], "mode": "rw"}
 
-            if str(name) in ["wsi-service", "isyntax-backend", "mirax-backend"]:
-                for key, val in wsi_mount_points.items():
-                    volumes[key] = {"bind": val, "mode": "ro"}
+            if str(name) in [
+                "clinical-data-service",
+                "cds-plugin-openslide",
+                "cds-plugin-tiffslide",
+                "cds-plugin-tifffile",
+                "cds-plugin-pil",
+                "cds-plugin-wsidicom",
+                "cds-plugin-isyntax",
+                "cds-plugin-mirax",
+            ]:
+                volumes[wsi_mount_point] = {"bind": "/data", "mode": "ro"}
 
             if name == "job-execution-service":
                 if docker_config is not None:
                     # just check valid json:
                     with open(docker_config, encoding="utf-8") as f:
                         _docker_conf = json.load(f)
                     volumes[docker_config] = {"bind": "/root/.docker/config.json", "mode": "ro"}
 
             network = settings.EATS_NET
 
-            client.containers.run(
-                service["image"],
-                name=service["name"],
-                detach=True,
-                network=network,
-                environment=service["environment"],
-                command=service["command"],
-                ports=service.get("ports"),
-                volumes=volumes,
-                extra_hosts=service.get("extra_hosts"),
-            )
+            if "command" in service:
+                client.containers.run(
+                    service["image"],
+                    name=service["name"],
+                    detach=True,
+                    network=network,
+                    environment=service["environment"],
+                    command=service["command"],
+                    ports=service.get("ports"),
+                    volumes=volumes,
+                    extra_hosts=service.get("extra_hosts"),
+                )
+            else:
+                client.containers.run(
+                    service["image"],
+                    name=service["name"],
+                    detach=True,
+                    network=network,
+                    environment=service["environment"],
+                    ports=service.get("ports"),
+                    volumes=volumes,
+                    extra_hosts=service.get("extra_hosts"),
+                )
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/commands/slides_commands.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/commands/slides_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         slide_id = slide["id"]
         if slide["deleted"]:
             slide["path"] = ""
         else:
             r = requests.get(f"{mds_url}/private/v3/slides/{slide_id}/storage")
             r.raise_for_status()
             storage = r.json()
-            slide["path"] = storage["storage_addresses"][0]["address"]
+            slide["path"] = storage["main_storage_address"]["path"]
     return slides
 
 
 def delete_slide(client, slide_id):
     mds_url = get_service_url(client=client, service_name="medical-data-service")
 
     # delete storage
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/constants.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 }
 
 
 # CLI help texts
 
 # Services
 VERSION_HELP = "Shows eats version"
-WSI_MOUNT_POINTS_FILE_HELP = (
-    "Path to JSON file containing mount point mappings of local WSI storage dirs (keys) "
-    "to be mounted in WSI Service container dirs (values)."
+WSI_MOUNT_POINT_HELP = (
+    "Path to local WSI storage directory. "
+    "Specified directory will be mounted in relevant docker containers under '/data'."
 )
 BUILD_HELP = "Force to build new nginx custom image (needed if nginx port has changed)"
 PULL_HELP = "Force to pull service images"
 GPU_HELP = "Enable GPU utilization for containerized app."
 GPU_DRIVER_HELP = "GPU driver to use for App images, e.g. 'nvidia' (default: no GPU)"
 TRIALS_SERVICES_HELP = "Number of times to try connecting to all services"
 WBS_PORT_HELP = "Listen port of workbench-service container"
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/custom_models.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/custom_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 class WsiInput(BaseModel):
     type: Literal["wsi"]
     id: Optional[str] = None
     path: str
     tissue: str = None
     stain: str = None
     block: str = None
-    secondary_files: Optional[List[str]] = None
 
     model_config = ConfigDict(extra="forbid")
 
 
 class OptionalForTestSuitePrimitive(BaseModel):
     name: Optional[str] = None
     creator_type: Optional[str] = None
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/.gitlab-ci.yml` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/CHANGELOG.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# 0.5.2
+
+* added `CaseQuery` model to v3
+* updated pydantic settings definition
+
+# 0.5.1
+
+* fix order of datatypes in app ui storage union
+
+# 0.5.0 (and also 0.4.11)
+
+* rework `SlideStorage` models
+
+# 0.4.10
+
+* added optional property `main_storage_address` to `PostClinicalSlide` model
+
 # 0.4.9
 
 * added pixelmap models
 
 # 0.4.8
 
 * removed tag value `HE` from model examples
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/LICENSE` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/commons.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     message: Optional[str] = Field(
         default=None, examples=["Database offline"], description="Message describing the status further if needed"
     )
 
 
 class ModelSettings(BaseSettings):
     disable_post_validation: bool = False
-    model_config = SettingsConfigDict(env_file=".env", env_prefix="models_")
+    model_config = SettingsConfigDict(env_file=".env", env_prefix="models_", extra="ignore")
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/marketplace/app.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/marketplace/app.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/poetry.lock` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/pyproject.toml` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "models"
-version = "0.4.9"
+version = "0.5.2"
 description = ""
 authors = ["Christoph Jansen <Christoph.Jansen@charite.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "<2.5.0"
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/access_token_tools.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/annotations.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/classes.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/collections.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/jobs.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/jobs.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/annotation/primitives.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/clinical.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/clinical.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         examples=[False],
         description="Flag indicating whether the underlying slide files and mappings have been deleted",
     )
 
     __hash__ = object.__hash__
 
 
-class PostClinicalSlide(PutClinicalSlide):
+class PostClinicalSlideCore(PutClinicalSlide):
     """Information needed for creating a new Slide, excluding derived DB attributes"""
 
     id: Optional[UUID4] = Field(
         default=None,
         examples=["b10648a7-340d-43fc-a2d9-4d91cc86f33f"],
         description="Unique ID of the slide",
     )
@@ -63,15 +63,23 @@
     case_id: UUID4 = Field(
         ...,
         examples=["b10648a7-340d-43fc-a2d9-4d91cc86f33f"],
         description="The ID of the case this slide belongs to",
     )
 
 
-class ClinicalSlide(PostClinicalSlide):
+class PostClinicalSlide(PostClinicalSlideCore):
+    main_path: Optional[str] = Field(
+        default=None,
+        examples=["path/to/file_or_directory"],
+        description="Main path to WSI that can be accessed by the Clinical Data Service",
+    )
+
+
+class ClinicalSlide(PostClinicalSlideCore):
     """Class representing an individual Slide. A Slide belongs to a specific Case, identified
     by its ID, and shows a specimen of a certain Tissue with some Stain applied to it.
     In this first version, all this information is contained directly within the Slide class,
     but might also be separated into individual Stain, Block, Specimen etc. classes later on.
     """
 
     created_at: Timestamp = Field(
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/commons.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/examination.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/examination.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/id_mapper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/job.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v1/slide.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v1/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/annotations.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/classes.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/collections.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/pixelmaps.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/pixelmaps.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/annotation/primitives.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/clinical.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/clinical.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         examples=[False],
         description="Flag indicating whether the underlying slide files and mappings have been deleted",
     )
 
     __hash__ = object.__hash__
 
 
-class PostClinicalSlide(PutClinicalSlide):
+class PostClinicalSlideCore(PutClinicalSlide):
     """Information needed for creating a new Slide, excluding derived DB attributes"""
 
     id: Optional[UUID4] = Field(
         default=None,
         examples=["b10648a7-340d-43fc-a2d9-4d91cc86f33f"],
         description="Unique ID of the slide",
     )
@@ -63,15 +63,23 @@
     case_id: UUID4 = Field(
         ...,
         examples=["b10648a7-340d-43fc-a2d9-4d91cc86f33f"],
         description="The ID of the case this slide belongs to",
     )
 
 
-class ClinicalSlide(PostClinicalSlide):
+class PostClinicalSlide(PostClinicalSlideCore):
+    main_path: Optional[str] = Field(
+        default=None,
+        examples=["path/to/file_or_directory"],
+        description="Main path to WSI that can be accessed by the Clinical Data Service",
+    )
+
+
+class ClinicalSlide(PostClinicalSlideCore):
     """Class representing an individual Slide. A Slide belongs to a specific Case, identified
     by its ID, and shows a specimen of a certain Tissue with some Stain applied to it.
     In this first version, all this information is contained directly within the Slide class,
     but might also be separated into individual Stain, Block, Specimen etc. classes later on.
     """
 
     created_at: Timestamp = Field(
@@ -167,14 +175,41 @@
                 )
             ]
         ],
         description="The actual cases",
     )
 
 
+class CaseQuery(RestrictedBaseModel):
+    """Query for one or more cases."""
+
+    cases: Optional[conlist(UUID4, min_length=1)] = Field(
+        default=None,
+        examples=[
+            [
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+            ]
+        ],
+        description="List of case Ids",
+    )
+    slides: Optional[conlist(UUID4, min_length=1)] = Field(
+        default=None,
+        examples=[
+            [
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+                "b10648a7-340d-43fc-a2d9-4d91cc86f33f",
+            ]
+        ],
+        description="List of slide Ids",
+    )
+
+
 class ClinicalSlideList(RestrictedBaseModel):
     """Wrapper for a collections of Slides, possibly filtered, including total count before paging"""
 
     item_count: ItemCount = Field(
         examples=[1],
         description="Total number of slides matching the query",
     )
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/commons.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/examination.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/examination.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,14 @@
         description="List of triggered app jobs",
     )
 
 
 StrAppUiStorage = constr(max_length=10000, strict=True)
 
 
-AppUiStorageContent = Dict[StrAppUiStorage, Union[StrAppUiStorage, StrictInt, StrictFloat, StrictBool]]
+AppUiStorageContent = Dict[StrAppUiStorage, Union[StrAppUiStorage, StrictBool, StrictInt, StrictFloat]]
 
 
 class AppUiStorage(RestrictedBaseModel):
     content: AppUiStorageContent = Field(
         examples=[{"key1": "val1", "key2": 42}], description="Dictionary of key-value-pairs"
     )
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/id_mapper.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/job.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/slide.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/LICENSE` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/README.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/poetry.lock` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/LICENSE` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/pyproject.toml` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/nginx/nginx.conf` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/mirax/Dockerfile`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/settings.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pydantic import BaseModel
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from empaia_app_test_suite import __version__
 from empaia_app_test_suite.constants import STATIC_ALT_USER_ID, STATIC_ORGANIZATION_ID, STATIC_USER_ID
 
 EATS_NET = "eats"
+CDS_BASE_PLUGINS = "cds-plugin-tiffslide|cds-plugin-wsidicom|cds-plugin-pil;1|cds-plugin-tifffile|cds-plugin-openslide"
 
 
 def get_docker_compose_dict():
     path_to_this_file = pathlib.Path(__file__).parent.absolute()
     path_to_docker_compose_file = os.path.join(path_to_this_file, "services", "docker-compose.yml")
     with open(path_to_docker_compose_file, encoding="utf-8") as stream:
         return yaml.safe_load(stream)
@@ -85,64 +86,73 @@
     scope_token_exp = scope_token_exp or 86400
 
     jes_gpu_worker = ";" if gpu_driver else ""
     jes_cpu_worker = ";x1" if not gpu_driver else ""
 
     wbs_url = wbs_url.rstrip("/") if wbs_url else f"http://localhost:{nginx_port}/wbs-api"
 
+    cds_plugins = CDS_BASE_PLUGINS
+    if isyntax_sdk:
+        cds_plugins = "cds-plugin-isyntax|" + cds_plugins
+    if mirax_plugin:
+        cds_plugins = "cds-plugin-mirax|" + cds_plugins
+
     if app_ui_frame_ancestors is None:
         app_ui_frame_ancestors = ""
 
     if app_ui_connect_src is None:
         app_ui_connect_src = ""
 
     path_to_this_file = pathlib.Path(__file__).parent.absolute()
     path_to_services = os.path.join(path_to_this_file, "services")
     default_version = f"eats-{__version__}"
 
     docker_compose_dict = get_docker_compose_dict()
 
     services = []
-    enable_isyntax_plugin = -1
-    enable_mirax_plugin = -1
 
     # check for isyntax sdk
     isyntax_sdk_path = os.path.join(
         path_to_services,
-        "wsi-service-plugin-isyntax/isyntax_backend",
+        "clinical_data_service/wsi_format_plugins/isyntax",
         "philips-pathologysdk-2.0-ubuntu18_04_py36_research.zip",
     )
     if isyntax_sdk:
-        enable_isyntax_plugin = 1
         shutil.copy(isyntax_sdk, isyntax_sdk_path)
         services.append(
             {
-                "name": "isyntax-backend",
-                "environment": {},
+                "name": "cds-plugin-isyntax",
+                "dockerfile_path": str(
+                    pathlib.Path(path_to_services, "clinical_data_service/wsi_format_plugins/isyntax/Dockerfile")
+                ),
+                "environment": {"PLUGIN_ISYNTAX_DATA_DIR": "/data"},
                 "ports": {},
                 "command": [],
-                "path": str(pathlib.Path(path_to_services, "wsi-service-plugin-isyntax/isyntax_backend")),
+                "path": str(pathlib.Path(path_to_services, "clinical_data_service/wsi_format_plugins")),
             }
         )
 
+    # check for mirax
     mirax_plugin_path = os.path.join(
         path_to_services,
-        "wsi-service-plugin-mirax/mirax_backend",
+        "clinical_data_service/wsi_format_plugins/mirax",
         "mirax_backend.zip",
     )
     if mirax_plugin:
-        enable_mirax_plugin = 1
         shutil.copy(mirax_plugin, mirax_plugin_path)
         services.append(
             {
-                "name": "mirax-backend",
-                "environment": {},
+                "name": "cds-plugin-mirax",
+                "dockerfile_path": str(
+                    pathlib.Path(path_to_services, "clinical_data_service/wsi_format_plugins/mirax/Dockerfile")
+                ),
+                "environment": {"CPM_DATA_DIR": "/data"},
                 "ports": {},
                 "command": [],
-                "path": str(pathlib.Path(path_to_services, "wsi-service-plugin-mirax/mirax_backend")),
+                "path": str(pathlib.Path(path_to_services, "clinical_data_service/wsi_format_plugins/mirax")),
             }
         )
 
     services.extend(
         [
             {
                 "name": "app-service",
@@ -222,97 +232,116 @@
                     "ES_API_V1_INTEGRATION": "examination_service.api.v1.integrations.disable_auth:DisableAuth",
                     "NO_PROXY": "eats-postgres-db",
                 },
                 "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
                 "ports": {},
             },
             {
+                "name": "cds-plugin-openslide",
+                "image": docker_compose_dict["services"]["cds-plugin-openslide"]["image"],
+                "environment": {"PLUGIN_OPENSLIDE_DATA_DIR": "/data"},
+            },
+            {
+                "name": "cds-plugin-tiffslide",
+                "image": docker_compose_dict["services"]["cds-plugin-tiffslide"]["image"],
+                "environment": {"PLUGIN_TIFFSLIDE_DATA_DIR": "/data"},
+            },
+            {
+                "name": "cds-plugin-tifffile",
+                "image": docker_compose_dict["services"]["cds-plugin-tifffile"]["image"],
+                "environment": {"PLUGIN_TIFFFILE_DATA_DIR": "/data"},
+            },
+            {
+                "name": "cds-plugin-pil",
+                "image": docker_compose_dict["services"]["cds-plugin-pil"]["image"],
+                "environment": {"PLUGIN_PIL_DATA_DIR": "/data"},
+            },
+            {
+                "name": "cds-plugin-wsidicom",
+                "image": docker_compose_dict["services"]["cds-plugin-wsidicom"]["image"],
+                "environment": {"PLUGIN_WSIDICOM_DATA_DIR": "/data"},
+            },
+            {
                 "name": "clinical-data-service",
                 "image": docker_compose_dict["services"]["clinical-data-service"]["image"],
                 "environment": {
                     "CDS_DB_HOST": "eats-postgres-db",
                     "CDS_DB_PORT": 5432,
                     "CDS_DB": "eats",
                     "CDS_DB_USERNAME": "empaia",
                     "CDS_DB_PASSWORD": "empaia",
+                    "CDS_DATA_DIR": "/data",
+                    "CDS_MAX_RETURNED_REGION_SIZE": 25000000,
+                    "CDS_PLUGIN_ADDRESSES": cds_plugins,
+                    "CDS_MIGRATION_STORAGE_ADDRESS_LEGACY_DATA_DIR": "/data",
                     "CDS_ALLOW_EXTERNAL_IDS": "True",
                     "NO_PROXY": "eats-postgres-db",
                 },
                 "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
                 "ports": {},
             },
             {
-                "name": "storage-mapper-service",
-                "image": docker_compose_dict["services"]["storage-mapper-service"]["image"],
-                "environment": {
-                    "SM_DB_USERNAME": "empaia",
-                    "SM_DB_PASSWORD": "empaia",
-                    "SM_DB": "eats",
-                    "SM_DB_HOST": "eats-postgres-db",
-                    "SM_DB_PORT": 5432,
-                    "NO_PROXY": "eats-postgres-db",
-                },
-                "command": [],
-                "ports": {},
-            },
-            {
-                "name": "wsi-service",
-                "image": docker_compose_dict["services"]["wsi-service"]["image"],
-                "environment": {
-                    "WS_DATA_DIR": "/data",
-                    "WS_MAPPER_ADDRESS": "http://storage-mapper-service:8000/v1/slides/{slide_id}",
-                    "WS_PLUGIN_PRIORITY_ISYNTAX": enable_isyntax_plugin,
-                    "WS_PLUGIN_PRIORITY_MIRAX": enable_mirax_plugin,
-                    "NO_PROXY": "storage-mapper-service",
-                },
-                "command": [],
-                "ports": {},
-            },
-            {
                 "name": "medical-data-service",
                 "image": docker_compose_dict["services"]["medical-data-service"]["image"],
                 "environment": {
                     "MDS_API_INTEGRATION": "medical_data_service.api.integrations.disable_auth:DisableAuth",
-                    "MDS_WS_URL": "http://wsi-service:8080",
-                    "MDS_SMS_URL": "http://storage-mapper-service:8000",
                     "MDS_JS_URL": "http://job-service:8000",
                     "MDS_AS_URL": "http://annotation-service:8000",
                     "MDS_CDS_URL": "http://clinical-data-service:8000",
                     "MDS_ES_URL": "http://examination-service:8000",
                     "MDS_ROOT_PATH": "/mds-api",
-                    "NO_PROXY": "wsi-service,storage-mapper-service,job-service,annotation-service,"
-                    + "clinical-data-service,examination-service",
+                    "MDS_ENABLE_STORAGE_ROUTES": True,
+                    "NO_PROXY": "job-service,annotation-service,clinical-data-service,examination-service",
                 },
-                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "--workers=2", "medical_data_service.app:app"],
+                "command": [
+                    "uvicorn",
+                    "--host=0.0.0.0",
+                    "--port=8000",
+                    "--workers=2",
+                    "--root-path=/mds-api",
+                    "medical_data_service.app:app",
+                ],
                 "ports": {},
             },
             {
                 "name": "marketplace-service-mock",
                 "image": docker_compose_dict["services"]["marketplace-service-mock"]["image"],
                 "environment": {
                     "MPSM_API_INTEGRATION": "marketplace_service_mock.api.integrations.disable_auth:DisableAuth",
                     "MPSM_ROOT_PATH": "/mps-api",
                     "MPSM_DISABLE_API_V0": "True",
                     "MPSM_ENABLE_API_V1": "True",
                 },
-                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "marketplace_service_mock.app:app"],
+                "command": [
+                    "uvicorn",
+                    "--host=0.0.0.0",
+                    "--port=8000",
+                    "--root-path=/mps-api",
+                    "marketplace_service_mock.app:app",
+                ],
                 "ports": {},
                 "volume": {
                     "name": "marketplace-service-mock-vol",
                     "mount": "/data",
                 },
             },
             {
                 "name": "aaa-service-mock",
                 "image": docker_compose_dict["services"]["aaa-service-mock"]["image"],
                 "environment": {
                     "AAAM_API_INTEGRATION": "aaa_service_mock.api.integrations.disable_auth:DisableAuth",
                     "AAAM_ROOT_PATH": "/aaa-api",
                 },
-                "command": ["uvicorn", "--host=0.0.0.0", "--port=8000", "aaa_service_mock.app:app"],
+                "command": [
+                    "uvicorn",
+                    "--host=0.0.0.0",
+                    "--port=8000",
+                    "--root-path=/aaa-api",
+                    "aaa_service_mock.app:app",
+                ],
                 "ports": {},
                 "volume": {
                     "name": "aaa-service-mock-vol",
                     "mount": "/data",
                 },
             },
             {
@@ -380,26 +409,31 @@
                     "WBS_CORS_ALLOW_ORIGINS": '["*"]',
                     "WBS_API_V1_INTEGRATION": "workbench_service.api.v1.integrations.disable_auth:DisableAuth",
                     "WBS_API_V2_INTEGRATION": "workbench_service.api.v2.integrations.disable_auth:DisableAuth",
                     "WBS_API_V3_INTEGRATION": "workbench_service.api.v3.integrations.disable_auth:DisableAuth",
                     "WBS_ORGANIZATION_ID": STATIC_ORGANIZATION_ID,
                     "WBS_CLIENT_ID": "wbs",
                     "WBS_FRONTEND_TOKEN_EXP": frontend_token_exp,
-                    "WBS_ROOT_PATH": "/wbs-api",
+                    # "WBS_ROOT_PATH": "/wbs-api",
                     "WBS_APP_UI_FRAME_ANCESTORS": app_ui_frame_ancestors,
                     "WBS_APP_UI_CONNECT_SRC": app_ui_connect_src,
                     "NO_PROXY": (
                         "aaa-service-mock,medical-data-service,app-service,job-execution-service,"
                         "marketplace-service-mock,workbench-client-v3-generic-ui"
                     ),
                     "WBS_GENERIC_APP_UI_V3_URL": "http://workbench-client-v3-generic-ui",
                     "WBS_FRONTEND_CSP_URL": f"http://localhost:{nginx_port}",
                     "WBS_DISABLE_CSP_SETTINGS": app_ui_disable_csp,
                 },
-                "command": ["run.sh", "--host=0.0.0.0", "--port=8000"],
+                "command": [
+                    "run.sh",
+                    "--host=0.0.0.0",
+                    "--port=8000",
+                    "--root-path=/wbs-api",
+                ],
                 "ports": {},
                 "extra_hosts": {"host.docker.internal": "host-gateway"},
             },
             {
                 "name": "workbench-client-v3",
                 "image": docker_compose_dict["services"]["workbench-client-v3"]["image"],
                 "environment": {
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_commons.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_mds.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_mds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List
-from uuid import uuid4
 
 import requests
 
 from empaia_app_test_suite.constants import JOB_MODES, STATIC_ALT_USER_ID, STATIC_CASE_ID, STATIC_USER_ID
 from empaia_app_test_suite.custom_models import WsiInput
 
 
@@ -43,57 +42,30 @@
     # add job to examination
     r = requests.put(f"{mds_url}/v3/examinations/{ex_id}/jobs/{job_id}/add")
     r.raise_for_status()
 
 
 def register_wsis(wsis_to_register: List[WsiInput], mds_url: str):
     url_cds = f"{mds_url}/private/v3/slides"
-    url_storage = f"{mds_url}/private/v3/slides/storage"
     for wsi_info in wsis_to_register:
         # CDS
         post_data_cds = {
             "tissue": wsi_info.tissue,
             "stain": wsi_info.stain,
             "block": wsi_info.block,
             "id": wsi_info.id,
             "case_id": STATIC_CASE_ID,
+            "main_path": wsi_info.path,
         }
         r = requests.post(url_cds, json=post_data_cds, params={"external_ids": True})
         r.raise_for_status()
-        if r.status_code in [200, 201]:
-            # SMS
-            post_data_storage = _build_post_data_storage(wsi_info=wsi_info)
-            r = requests.post(url_storage, json=post_data_storage)
-            r.raise_for_status()
     wsi_ids = [wsi.id for wsi in wsis_to_register]
     return wsi_ids
 
 
-def _build_post_data_storage(wsi_info: WsiInput):
-    storage_addresses = []
-    storage_addresses.append(_build_storage_address(slide_id=wsi_info.id, address=wsi_info.path, main_address=True))
-
-    if wsi_info.secondary_files and len(wsi_info.secondary_files) > 0:
-        for secondary_file in wsi_info.secondary_files:
-            storage_addresses.append(
-                _build_storage_address(slide_id=wsi_info.id, address=secondary_file, main_address=False)
-            )
-
-    return {"slide_id": wsi_info.id, "storage_type": "fs", "storage_addresses": storage_addresses}
-
-
-def _build_storage_address(slide_id: str, address: str, main_address: bool):
-    return {
-        "storage_address_id": str(uuid4()),
-        "slide_id": slide_id,
-        "address": str(address),
-        "main_address": main_address,
-    }
-
-
 def create_job(app_id: str, mds_url: str, job_mode: str, creator_id: str, creator_type: str = "SCOPE"):
     job = {
         "app_id": app_id,
         "creator_id": creator_id,
         "creator_type": creator_type,
         "mode": JOB_MODES[job_mode],
         "containerized": True,
```

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_mps.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_mps.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/empaia_app_test_suite/utils/utils_print.py` & `empaia_app_test_suite-3.6.0/empaia_app_test_suite/utils/utils_print.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.5.0/pyproject.toml` & `empaia_app_test_suite-3.6.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "empaia-app-test-suite"
-version = "3.5.0"
+version = "3.6.0"
 description = "The EMPAIA App Test Suite (EATS)"
 license = "MIT"
 
 # Authors / Maintainers
-authors = ["EMPAIA <dev-support@empaia.org>"]
-maintainers = ["EMPAIA <dev-support@empaia.org>"]
+authors = ["EMPAIA <support@empaia.org>"]
+maintainers = ["EMPAIA <support@empaia.org>"]
 
 # URLs
 homepage = "https://developer.empaia.org/app_developer_docs/#/"
 repository = "https://gitlab.com/empaia/integration/empaia-app-test-suite"
 documentation = "https://developer.empaia.org/app_developer_docs/#/"
 readme = "README.md"
 
@@ -25,47 +25,49 @@
     "Operating System :: POSIX",
     "Topic :: Software Development",
     "Topic :: Software Development :: Testing",
 ]
 
 exclude = ["empaia_app_test_suite/services/", "**/__pycache__/"]
 include = [
-    "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile",
-    "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml",
-    "empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/*",
-    "empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile",
-    "empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/entrypoint.sh",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/*",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/utils/cds_plugin_utils/*",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/Dockerfile",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/pyproject.toml",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/isyntax/cds_plugin_isyntax/*",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/mirax/Dockerfile",
+    "empaia_app_test_suite/services/clinical_data_service/wsi_format_plugins/mirax/entrypoint.sh",
     "empaia_app_test_suite/services/nginx/Dockerfile",
     "empaia_app_test_suite/services/nginx/nginx.conf",
     "empaia_app_test_suite/services/docker-compose.yml",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://gitlab.com/empaia/integration/empaia-app-test-suite/-/issues"
 
 [tool.poetry.scripts]
 empaia-app-test-suite = 'empaia_app_test_suite.cli:app'
 eats = 'empaia_app_test_suite.cli:app'
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 jsonschema = "^4.4.0"
 toml = "^0.10.2"
-docker = "^6.0.0"
+docker = "^7.0.0"
 prettytable = "^3.2.0"
 PyYAML = "^6.0"
 requests = "2.31.0"
 typer = { extras = ["all"], version = "^0.9.0" }
-pydantic = "<2.5.0"
+pydantic = "^2.5.0"
 pydantic-settings = "^2.0.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+black = "^24.0.0"
 pillow = "^10.0.0"
-pytest = "^7.3.1"
+pytest = "^8.0.0"
 pycodestyle = "^2.10.0"
 pylint = "^3.0.0"
 
 [tool.pytest.ini_options]
 norecursedirs = ["empaia_app_test_suite/services"]
 
 [tool.black]
```

### Comparing `empaia_app_test_suite-3.5.0/PKG-INFO` & `empaia_app_test_suite-3.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 Metadata-Version: 2.1
 Name: empaia-app-test-suite
-Version: 3.5.0
+Version: 3.6.0
 Summary: The EMPAIA App Test Suite (EATS)
 Home-page: https://developer.empaia.org/app_developer_docs/#/
 License: MIT
 Author: EMPAIA
-Author-email: dev-support@empaia.org
+Author-email: support@empaia.org
 Maintainer: EMPAIA
-Maintainer-email: dev-support@empaia.org
-Requires-Python: >=3.8,<4.0
+Maintainer-email: support@empaia.org
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: docker (>=6.0.0,<7.0.0)
+Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: prettytable (>=3.2.0,<4.0.0)
-Requires-Dist: pydantic (<2.5.0)
+Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://gitlab.com/empaia/integration/empaia-app-test-suite/-/issues
 Project-URL: Documentation, https://developer.empaia.org/app_developer_docs/#/
 Project-URL: Repository, https://gitlab.com/empaia/integration/empaia-app-test-suite
 Description-Content-Type: text/markdown
 
 # EMPAIA App Test Suite (EATS)
 
 ## Requirements
 
-* The EMPAIA App Test Suite requires Python 3.8.
+* The EMPAIA App Test Suite requires Python 3.10.
 * Supported Operating Systems are Linux, Windows and MacOS
   * for **Windows** the EATS requires the usage of WSL 2 (Windows Subsystem for Linux) with Docker for Windows
 
 ## Installation
 
 There are different possibilities to install the EMPAIA App Test Suite depending on your intended use:
 
@@ -109,37 +108,28 @@
 
 Run the EATS CLI app with
 
 ```bash
 eats
 ```
 
-To force pull and build services and submodules:
+To force pull and build services:
 
 ```bash
-eats services up ./wsi-mount-points.json --build --pull
+eats services up <wsi-mount-points-path> --build --pull
 ```
 
 ## Usage
 
 **For detailed instructions take a look at the [App Developer Documentation](https://developer.empaia.org/app_developer_docs/#/)**
 
-Define absolute paths to directories containing WSIs in a `./wsi-mount-points.json` file as follows:
-
-```json
-{
-    "/absolute/local/path/to/wsis/dir1": "/data/",
-    "/absolute/local/path/to/wsis/dir2": "/data2/"
-}
-```
-
 Start all backend services in Docker containers using the `eats services up` command. WSI directories are mounted into the WSI Service container. Only WSIs contained in one of the specified directories can be used as a job input.
 
 ```bash
-eats services up ./wsi-mount-points.json
+eats services up <wsi-mount-points-path>
 ```
 
 You can perform health checks of running backend services.
 
 ```bash
 eats services health
 ```
@@ -170,49 +160,49 @@
 ```bash
 eats jobs run ./job.env
 ```
 
 The job ID can be retrieved from the `job.env` file to be used in other commands.
 
 ```bash
-export $(xargs <job.env)
+export $(xargs < job.env)
 echo $EMPAIA_JOB_ID
 ```
 
 Regularly check the jobs status until it is `COMPLETED`.
 
 ```bash
-eats jobs status ${EMPAIA_JOB_ID}
+eats jobs status $EMPAIA_JOB_ID
 ```
 
 The job ID is used as the container name. It can be used to retrieved docker logs.
 
 ```bash
-docker logs ${EMPAIA_JOB_ID}
+docker logs $EMPAIA_JOB_ID
 ```
 
 Open `localhost:8888/wbc3` in a Browser to review job results using the Workbench Client 3.0.
 
 In addition, the job results can be exported to JSON files in a `job-outputs` directory.
 
 ```bash
-eats jobs export ${EMPAIA_JOB_ID} ./job-outputs
+eats jobs export $EMPAIA_JOB_ID ./job-outputs
 ```
 
 If a job is taking too long or is stuck, the job can be aborted.
 
 ```bash
-eats jobs abort ${EMPAIA_JOB_ID}
+eats jobs abort $EMPAIA_JOB_ID
 ```
 
-To inspect backend service logs the `docker logs` command can used directly. The names of all service containers can be retrieved using the `eats services list` command.
+To inspect backend service logs the `docker logs` command can be used directly. The names of all service containers can be retrieved using the `eats services list` command.
 
 ```bash
 eats services list  # print list of service names
-docker logs ${SERVICE_NAME}
+docker logs <SERVICE_NAME>
 ```
 
 It is possible to register and run multiple jobs without restart backend services. The services can be stopped, if they are not needed anymore. All created data is available when the services are started again.
 
 ```bash
 eats services down
 ```
@@ -242,39 +232,38 @@
 black empaia_app_test_suite tests check_version.py
 pycodestyle empaia_app_test_suite tests check_version.py
 pylint empaia_app_test_suite tests check_version.py
 ```
 
 ### Tests
 
-Create `./wsi-mount-points.json`:
+Create a directory in which the WSI [CMU-1.svs](http://openslide.cs.cmu.edu/download/openslide-testdata/Aperio/CMU-1.svs) is located in a subdirectory "Aperio":
 
-```JSON
-{
-  "/path/to/testdata/Aperio/": "/data",
-  "/path/to/testdata/Fluorescence OME-Tif/": "/data2"
-}
+```
+WSI_BASE_PATH
+└── Aperio
+    └── CMU-1.svs
 ```
 
 ```bash
 # run cli command tests
-pytest tests/commands --maxfail=1 -s -v
+pytest tests/commands --maxfail=1 -s -v --mount-point <WSI_BASE_PATH>
 
-eats services up ./wsi-mount-points.json --build --pull
+eats services up <WSI_BASE_PATH> --build --pull
 
 # run sample apps tests
 pytest tests/sample_apps_tests --maxfail=1 -s -v
 ```
 
 If a test from `tests/sample_apps` fails, use `docker logs <servicename>` for debugging.
 
 ### Test GPU support
 
 ```bash
-eats services up ./wsi-mount-points.json --build --pull --gpu-driver nvidia
+eats services up <WSI_BASE_PATH> --build --pull --gpu-driver nvidia
 
-# run cli command test
+# run gpu sample apps test
 pytest tests/gpu_support_test
 ```
 
 If docker is locally installed with support for CUDA and a supported GPU is available on the host system the test must succeed. If the test fails please check if docker is correctly installed.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

