# Comparing `tmp/dbgpt-0.5.4.tar.gz` & `tmp/dbgpt-0.5.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.4.tar", last modified: Fri Apr 12 06:38:07 2024, max compression
+gzip compressed data, was "dbgpt-0.5.4rc0.tar", last modified: Thu Apr 11 05:05:19 2024, max compression
```

## Comparing `dbgpt-0.5.4.tar` & `dbgpt-0.5.4rc0.tar`

### file list

```diff
@@ -1,461 +1,461 @@
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:07.031286 dbgpt-0.5.4/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.4/LICENSE
--rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.4/MANIFEST.in
--rw-r--r--   0 staneyffer   (501) staff       (20)    30379 2024-04-12 06:38:07.030610 dbgpt-0.5.4/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.4/README.md
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.724772 dbgpt-0.5.4/dbgpt/
--rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.731660 dbgpt-0.5.4/dbgpt/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13806 2024-04-12 06:30:46.000000 dbgpt-0.5.4/dbgpt/_private/config.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1625 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/_private/llm_metadata.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      983 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/_private/pydantic.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.4/dbgpt/_version.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.732385 dbgpt-0.5.4/dbgpt/agent/
--rw-r--r--   0 staneyffer   (501) staff       (20)      944 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.739139 dbgpt-0.5.4/dbgpt/agent/actions/
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5106 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/blank_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/chart_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/code_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4312 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/dashboard_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/indicator_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/actions/plugin_action.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.746368 dbgpt-0.5.4/dbgpt/agent/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3463 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/agent_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    35778 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/agent/core/base_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5616 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/base_team.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.748335 dbgpt-0.5.4/dbgpt/agent/core/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3496 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/llm/llm.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/llm/llm_client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.749691 dbgpt-0.5.4/dbgpt/agent/core/llm/strategy/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/llm/strategy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/llm/strategy/priority.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3632 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/role.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      455 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/core/user_proxy_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.755724 dbgpt-0.5.4/dbgpt/agent/expand/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/Indicator_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/agent/expand/code_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/dashboard_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5410 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/data_scientist_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2710 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/plugin_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22052 2024-04-12 06:30:46.000000 dbgpt-0.5.4/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1680 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/expand/summary_assistant_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.758148 dbgpt-0.5.4/dbgpt/agent/memory/
--rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/memory/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/memory/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/memory/default_gpts_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/memory/gpts_memory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.761447 dbgpt-0.5.4/dbgpt/agent/plan/
--rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.764570 dbgpt-0.5.4/dbgpt/agent/plan/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/awel/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10858 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/awel/agent_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6004 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/awel/agent_operator_resource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8312 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/awel/team_awel_layout.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/plan_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7577 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/planner_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plan/team_auto_plan.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.768041 dbgpt-0.5.4/dbgpt/agent/plugin/
--rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.771197 dbgpt-0.5.4/dbgpt/agent/plugin/commands/
--rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.771927 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/
--rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.775536 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/
--rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/command.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22478 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/command_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/commands/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/generator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/plugin/plugins_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.780799 dbgpt-0.5.4/dbgpt/agent/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3698 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/resource/resource_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/agent/resource/resource_db_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/resource/resource_knowledge_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/resource/resource_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/resource/resource_plugin_api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.782510 dbgpt-0.5.4/dbgpt/agent/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/agent/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/agent/util/cmp.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.783743 dbgpt-0.5.4/dbgpt/cli/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/cli/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/cli/cli_scripts.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.790784 dbgpt-0.5.4/dbgpt/client/
--rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.4/dbgpt/client/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/client/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.4/dbgpt/client/app.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14121 2024-04-12 06:30:46.000000 dbgpt-0.5.4/dbgpt/client/client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3718 2024-03-28 01:32:30.000000 dbgpt-0.5.4/dbgpt/client/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3562 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/client/flow.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6906 2024-03-22 07:58:46.000000 dbgpt-0.5.4/dbgpt/client/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9418 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/client/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10595 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/component.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.792705 dbgpt-0.5.4/dbgpt/configs/
--rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/configs/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/configs/model_config.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.793918 dbgpt-0.5.4/dbgpt/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.797020 dbgpt-0.5.4/dbgpt/core/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/_private/example_base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/_private/prompt_registry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.797949 dbgpt-0.5.4/dbgpt/core/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)     6044 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/awel/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.801747 dbgpt-0.5.4/dbgpt/core/awel/dag/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/dag/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.4/dbgpt/core/awel/dag/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3515 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/core/awel/dag/dag_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/dag/loader.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.806156 dbgpt-0.5.4/dbgpt/core/awel/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    33486 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/core/awel/flow/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/core/awel/flow/compat.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/flow/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    28676 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/core/awel/flow/flow_factory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.809641 dbgpt-0.5.4/dbgpt/core/awel/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/core/awel/operators/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/operators/common_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/operators/stream_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.810981 dbgpt-0.5.4/dbgpt/core/awel/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/resource/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.813022 dbgpt-0.5.4/dbgpt/core/awel/runner/
--rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/runner/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/awel/runner/job_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/awel/runner/local_runner.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.815235 dbgpt-0.5.4/dbgpt/core/awel/task/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/task/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/task/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/awel/task/task_impl.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.819782 dbgpt-0.5.4/dbgpt/core/awel/trigger/
--rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37793 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/trigger/trigger_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.822442 dbgpt-0.5.4/dbgpt/core/awel/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/util/_typing_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/util/http_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/awel/util/parameter_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.831421 dbgpt-0.5.4/dbgpt/core/interface/
--rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/embeddings.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.4/dbgpt/core/interface/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3793 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31087 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/core/interface/llm.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    42772 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/message.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.837255 dbgpt-0.5.4/dbgpt/core/interface/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/message_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    16374 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/prompt_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/operators/retriever.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/core/interface/output_parser.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    26524 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/prompt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1725 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/interface/serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15124 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/interface/storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.838081 dbgpt-0.5.4/dbgpt/core/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/core/operators/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.840224 dbgpt-0.5.4/dbgpt/core/operators/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/operators/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/operators/flow/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/core/operators/flow/dict_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.841624 dbgpt-0.5.4/dbgpt/core/schema/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/core/schema/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3868 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/core/schema/api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.845206 dbgpt-0.5.4/dbgpt/datasource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/conn_spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/db_conn_info.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.847564 dbgpt-0.5.4/dbgpt/datasource/manages/
--rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/manages/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.4/dbgpt/datasource/manages/connect_config_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/manages/connector_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.848331 dbgpt-0.5.4/dbgpt/datasource/nosql/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/nosql/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.849823 dbgpt-0.5.4/dbgpt/datasource/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.4/dbgpt/datasource/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/operators/datasource_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.857302 dbgpt-0.5.4/dbgpt/datasource/rdbms/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_doris.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_hive.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_mssql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_mysql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.858036 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.858688 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.860394 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.4/dbgpt/datasource/redis.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.863602 dbgpt-0.5.4/dbgpt/model/
--rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.871893 dbgpt-0.5.4/dbgpt/model/adapter/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/embeddings_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/fschat_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/model/adapter/hf_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/model_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/model/adapter/old_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/model/adapter/proxy_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/adapter/vllm_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/cli.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.873319 dbgpt-0.5.4/dbgpt/model/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/model/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/parameter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.874755 dbgpt-0.5.4/dbgpt/model/proxy/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/model/proxy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.885176 dbgpt-0.5.4/dbgpt/model/proxy/llms/
--rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/baichuan.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/bard.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/chatgpt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/claude.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/gemini.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/moonshot.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/proxy_model.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/tongyi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/wenxin.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/yi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/proxy/llms/zhipu.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.887840 dbgpt-0.5.4/dbgpt/model/utils/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/utils/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/model/utils/chatgpt_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/utils/llm_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/model/utils/token_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.889490 dbgpt-0.5.4/dbgpt/rag/
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.893347 dbgpt-0.5.4/dbgpt/rag/assembler/
--rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/assembler/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/assembler/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/assembler/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/assembler/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/assembler/summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/chunk_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.896351 dbgpt-0.5.4/dbgpt/rag/embedding/
--rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/embedding/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/embedding/_wrapped.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/embedding/embedding_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    24178 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/embedding/embeddings.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.898016 dbgpt-0.5.4/dbgpt/rag/evaluation/
--rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/evaluation/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/evaluation/retriever.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.900375 dbgpt-0.5.4/dbgpt/rag/extractor/
--rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/extractor/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/extractor/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/extractor/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.900998 dbgpt-0.5.4/dbgpt/rag/graph/
--rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/graph/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.908278 dbgpt-0.5.4/dbgpt/rag/knowledge/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/csv.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/docx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/html.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/json.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/markdown.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/pdf.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/pptx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/string.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/txt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/knowledge/url.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.914465 dbgpt-0.5.4/dbgpt/rag/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/operators/assembler.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/operators/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.4/dbgpt/rag/operators/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/operators/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/operators/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/operators/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/operators/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/operators/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/operators/schema_linking.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/operators/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.918116 dbgpt-0.5.4/dbgpt/rag/retriever/
--rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/retriever/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/retriever/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/retriever/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/retriever/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/retriever/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/rag/retriever/rewrite.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.920153 dbgpt-0.5.4/dbgpt/rag/schemalinker/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/schemalinker/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/schemalinker/base_linker.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/schemalinker/schema_linking.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.922179 dbgpt-0.5.4/dbgpt/rag/summary/
--rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/summary/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/summary/db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/summary/db_summary_client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3964 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/summary/rdbms_db_summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.924642 dbgpt-0.5.4/dbgpt/rag/text_splitter/
--rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/text_splitter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/rag/text_splitter/text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/rag/text_splitter/token_splitter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.926569 dbgpt-0.5.4/dbgpt/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.931000 dbgpt-0.5.4/dbgpt/storage/cache/
--rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/embedding_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/llm_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/operators.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.931873 dbgpt-0.5.4/dbgpt/storage/cache/protocol/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/protocol/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.932945 dbgpt-0.5.4/dbgpt/storage/cache/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/storage/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/storage/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.934177 dbgpt-0.5.4/dbgpt/storage/cache/storage/disk/
--rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/storage/disk/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.936138 dbgpt-0.5.4/dbgpt/storage/chat_history/
--rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/chat_history/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/chat_history/chat_history_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/chat_history/storage_adapter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.940318 dbgpt-0.5.4/dbgpt/storage/metadata/
--rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/metadata/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9255 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/metadata/_base_dao.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/metadata/db_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/metadata/db_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/metadata/db_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/schema.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.945272 dbgpt-0.5.4/dbgpt/storage/vector_store/
--rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7796 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8232 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/chroma_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/connector.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/filters.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    21307 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/milvus_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3462 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/pgvector_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6749 2024-04-10 06:34:08.000000 dbgpt-0.5.4/dbgpt/storage/vector_store/weaviate_store.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.967408 dbgpt-0.5.4/dbgpt/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/_db_migration_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/annotations.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/api_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.968069 dbgpt-0.5.4/dbgpt/util/benchmarks/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/benchmarks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.969094 dbgpt-0.5.4/dbgpt/util/benchmarks/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/benchmarks/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9300 2024-04-12 06:30:46.000000 dbgpt-0.5.4/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/chat_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/code_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.4/dbgpt/util/command_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/config_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.970395 dbgpt-0.5.4/dbgpt/util/console/
--rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/util/console/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/util/console/console.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/custom_data_structure.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.4/dbgpt/util/date_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.973840 dbgpt-0.5.4/dbgpt/util/dbgpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9344 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11619 2024-03-27 07:42:00.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/repo.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5905 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/dbgpts/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/error_types.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/executor_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1313 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/fastapi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/formatting.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/function_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/global_helper.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/util/i18n_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/util/json_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/memory_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/model_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/module_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/net_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.974641 dbgpt-0.5.4/dbgpt/util/network/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/util/network/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9777 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/util/network/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/openai_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      545 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/pagination_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/parameter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/path_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/pd_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8661 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/prompt_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.975525 dbgpt-0.5.4/dbgpt/util/serialization/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/serialization/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-03-25 14:27:11.000000 dbgpt-0.5.4/dbgpt/util/serialization/json_serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/similarity_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/singleton.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.979978 dbgpt-0.5.4/dbgpt/util/speech/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/brian.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/eleven_labs.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/gtts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/macos_tts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/speech/say.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/splitter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/util/string_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.4/dbgpt/util/system_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.984705 dbgpt-0.5.4/dbgpt/util/tracer/
--rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/tracer/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/util/tracer/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/util/tracer/span_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/tracer/tracer_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/util/tracer/tracer_impl.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/tracer/tracer_middleware.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.4/dbgpt/util/utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.986786 dbgpt-0.5.4/dbgpt/vis/
--rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.4/dbgpt/vis/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.993062 dbgpt-0.5.4/dbgpt/vis/tags/
--rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_agent_message.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_agent_plans.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_chart.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_code.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_dashboard.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_gpts_execution.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_gpts_result.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.4/dbgpt/vis/tags/vis_plugin.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-12 06:38:06.728416 dbgpt-0.5.4/dbgpt.egg-info/
--rw-r--r--   0 staneyffer   (501) staff       (20)    30379 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    12638 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/SOURCES.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/dependency_links.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/entry_points.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)     4943 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/requires.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-12 06:38:06.000000 dbgpt-0.5.4/dbgpt.egg-info/top_level.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-12 06:38:07.031422 dbgpt-0.5.4/setup.cfg
--rw-r--r--   0 staneyffer   (501) staff       (20)    23342 2024-04-11 14:37:18.000000 dbgpt-0.5.4/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.368039 dbgpt-0.5.4rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.4rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.4rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:19.367289 dbgpt-0.5.4rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.973762 dbgpt-0.5.4rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.981845 dbgpt-0.5.4rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13796 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1625 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      983 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.4rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.982750 dbgpt-0.5.4rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      944 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.989166 dbgpt-0.5.4rc0/dbgpt/agent/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5106 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/actions/plugin_action.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.996611 dbgpt-0.5.4rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3463 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    35778 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5616 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.998902 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3496 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.000032 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/priority.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3632 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      455 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.005797 dbgpt-0.5.4rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-11 02:57:34.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5410 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/data_scientist_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2710 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/plugin_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22133 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1680 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/expand/summary_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.008669 dbgpt-0.5.4rc0/dbgpt/agent/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/memory/gpts_memory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.012326 dbgpt-0.5.4rc0/dbgpt/agent/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.016378 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10858 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6004 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8312 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7577 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.019545 dbgpt-0.5.4rc0/dbgpt/agent/plugin/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.022966 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.023575 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.026320 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22478 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/plugin/plugins_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.030330 dbgpt-0.5.4rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3698 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 01:48:23.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_db_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_knowledge_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_plugin_api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.032017 dbgpt-0.5.4rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 04:29:39.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.033422 dbgpt-0.5.4rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.041821 dbgpt-0.5.4rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14121 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3718 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3562 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6906 2024-03-22 07:58:46.000000 dbgpt-0.5.4rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9418 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10595 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.043705 dbgpt-0.5.4rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.044635 dbgpt-0.5.4rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.047812 dbgpt-0.5.4rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.048644 dbgpt-0.5.4rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6044 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.053927 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3515 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.059666 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33486 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    28676 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.064144 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.065894 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.068366 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.071359 dbgpt-0.5.4rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.077642 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37793 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.081292 dbgpt-0.5.4rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2237 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.093577 dbgpt-0.5.4rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3793 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31087 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    42772 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.101651 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16374 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26524 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1725 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15124 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.102606 dbgpt-0.5.4rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.105315 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.107003 dbgpt-0.5.4rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3868 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.111492 dbgpt-0.5.4rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114151 dbgpt-0.5.4rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.114912 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.116360 dbgpt-0.5.4rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.126686 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.127572 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.128426 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.130689 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.4rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.135298 dbgpt-0.5.4rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.150106 dbgpt-0.5.4rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.152289 dbgpt-0.5.4rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.154070 dbgpt-0.5.4rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.165126 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.167691 dbgpt-0.5.4rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.169670 dbgpt-0.5.4rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.174299 dbgpt-0.5.4rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.178536 dbgpt-0.5.4rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24178 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.180597 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.184058 dbgpt-0.5.4rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.187268 dbgpt-0.5.4rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.203704 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.217047 dbgpt-0.5.4rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.222651 dbgpt-0.5.4rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.224784 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.227962 dbgpt-0.5.4rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3964 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.231422 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.233812 dbgpt-0.5.4rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.238853 dbgpt-0.5.4rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.240028 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.241804 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.243560 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.245833 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.250741 dbgpt-0.5.4rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9255 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.257290 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7796 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8232 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    21307 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3462 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6749 2024-04-10 06:34:08.000000 dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298070 dbgpt-0.5.4rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.298880 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.300181 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9300 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.301400 dbgpt-0.5.4rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.4rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.304988 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9344 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11619 2024-03-27 07:42:00.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5905 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1313 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.305930 dbgpt-0.5.4rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9777 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      545 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8661 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.306804 dbgpt-0.5.4rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-03-25 14:27:11.000000 dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.310685 dbgpt-0.5.4rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.4rc0/dbgpt/util/system_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.315968 dbgpt-0.5.4rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-10 19:49:14.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.4rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.317582 dbgpt-0.5.4rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 04:24:29.000000 dbgpt-0.5.4rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:19.323394 dbgpt-0.5.4rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-11 05:05:18.977858 dbgpt-0.5.4rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    30382 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12638 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4943 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-11 05:05:18.000000 dbgpt-0.5.4rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-11 05:05:19.368143 dbgpt-0.5.4rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23342 2024-04-11 01:47:19.000000 dbgpt-0.5.4rc0/setup.py
```

### Comparing `dbgpt-0.5.4/LICENSE` & `dbgpt-0.5.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/PKG-INFO` & `dbgpt-0.5.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.4
+Version: 0.5.4rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -315,94 +315,94 @@
 Requires-Dist: pymysql; extra == "default"
 Requires-Dist: torch==2.2.1; extra == "default"
 Requires-Dist: torchvision==0.17.1; extra == "default"
 Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
 Provides-Extra: all
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: duckdb; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: thrift; extra == "all"
 Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: dashscope; extra == "all"
 Requires-Dist: jinja2; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf==3.20.3; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: importlib-resources==5.12.0; extra == "all"
 Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: termcolor; extra == "all"
 Requires-Dist: spacy==3.5.3; extra == "all"
-Requires-Dist: pympler; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: fastapi==0.98.0; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: seaborn; extra == "all"
 Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: vllm; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: auto-gpt-plugin-template; extra == "all"
 Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: chardet; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
```

### Comparing `dbgpt-0.5.4/README.md` & `dbgpt-0.5.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/_private/config.py` & `dbgpt-0.5.4rc0/dbgpt/_private/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """Initialize the Config class"""
 
         self.NEW_SERVER_MODE = False
         self.SERVER_LIGHT_MODE = False
 
         # Gradio language version: en, zh
         self.LANGUAGE = os.getenv("LANGUAGE", "en")
-        self.DBGPT_WEBSERVER_PORT = int(os.getenv("DBGPT_WEBSERVER_PORT", 5670))
+        self.WEB_SERVER_PORT = int(os.getenv("WEB_SERVER_PORT", 5000))
 
         self.debug_mode = False
         self.skip_reprompt = False
         self.temperature = float(os.getenv("TEMPERATURE", 0.7))
 
         # self.NUM_GPUS = int(os.getenv("NUM_GPUS", 1))
```

### Comparing `dbgpt-0.5.4/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.4rc0/dbgpt/_private/llm_metadata.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/_private/pydantic.py` & `dbgpt-0.5.4rc0/dbgpt/_private/pydantic.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/blank_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/blank_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/chart_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/chart_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/code_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/code_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/dashboard_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/dashboard_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/indicator_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/indicator_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/actions/plugin_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/actions/plugin_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/agent_manage.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/agent_manage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/base_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/base_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/base_team.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/base_team.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/llm/llm.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/llm/llm_client.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/llm/strategy/priority.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/llm/strategy/priority.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/core/role.py` & `dbgpt-0.5.4rc0/dbgpt/agent/core/role.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/Indicator_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/Indicator_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/code_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/code_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/dashboard_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/dashboard_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/data_scientist_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/data_scientist_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/plugin_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/plugin_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/retrieve_summary_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,18 +250,22 @@
             is_success = check_pass
             # 5.Optimize wrong answers myself
             if not check_pass:
                 reply_message.content = reason
             reply_message.success = is_success
         return reply_message
 
-    async def correctness_check(
-        self, message: AgentMessage
+    async def verify(
+        self,
+        message: AgentMessage,
+        sender: Agent,
+        reviewer: Optional[Agent] = None,
+        **kwargs,
     ) -> Tuple[bool, Optional[str]]:
-        """Verify the correctness of the results."""
+        """Verify the correctness of the message."""
         action_report = message.action_report
         task_result = ""
         if action_report:
             task_result = action_report.get("content", "")
 
         check_result, model = await self.thinking(
             messages=[
```

### Comparing `dbgpt-0.5.4/dbgpt/agent/expand/summary_assistant_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/expand/summary_assistant_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/memory/base.py` & `dbgpt-0.5.4rc0/dbgpt/agent/memory/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/memory/default_gpts_memory.py` & `dbgpt-0.5.4rc0/dbgpt/agent/memory/default_gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/memory/gpts_memory.py` & `dbgpt-0.5.4rc0/dbgpt/agent/memory/gpts_memory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/awel/agent_operator.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/awel/agent_operator_resource.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/agent_operator_resource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/awel/team_awel_layout.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/awel/team_awel_layout.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/plan_action.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/plan_action.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/planner_agent.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/planner_agent.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plan/team_auto_plan.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plan/team_auto_plan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/command.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/command_manage.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/command_manage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/commands/exceptions.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/generator.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/generator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/loader.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/plugin/plugins_util.py` & `dbgpt-0.5.4rc0/dbgpt/agent/plugin/plugins_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/resource_api.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/resource_db_api.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_db_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Database resource client API."""
 import logging
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Iterator, List, Optional, Union
+from typing import Iterator, List, Optional, Union, TYPE_CHECKING
 
 from .resource_api import AgentResource, ResourceClient, ResourceType
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceDbClient(ResourceClient):
```

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/resource_knowledge_api.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_knowledge_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/resource_loader.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/resource/resource_plugin_api.py` & `dbgpt-0.5.4rc0/dbgpt/agent/resource/resource_plugin_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/agent/util/cmp.py` & `dbgpt-0.5.4rc0/dbgpt/agent/util/cmp.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.4rc0/dbgpt/cli/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/_cli.py` & `dbgpt-0.5.4rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/app.py` & `dbgpt-0.5.4rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/client.py` & `dbgpt-0.5.4rc0/dbgpt/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         version: str = "v2",
         timeout: Optional[httpx._types.TimeoutTypes] = 120,
     ):
         """Create the client.
 
         Args:
             api_base: Optional[str], a full URL for the DB-GPT API.
-                Defaults to the `http://localhost:5670/api/v2`.
+                Defaults to the `http://localhost:5000/api/v2`.
             api_key: Optional[str], The dbgpt api key to use for authentication.
                 Defaults to None.
             timeout: Optional[httpx._types.TimeoutTypes]: The timeout to use.
                 Defaults to None.
             In most cases, pass in a float number to specify the timeout in seconds.
         Returns:
             None
@@ -73,22 +73,22 @@
 
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5670/api/v2"
+            DBGPT_API_BASE = "http://localhost:5000/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             client.chat(model="chatgpt_proxyllm", messages="Hello?")
         """
         if not api_base:
             api_base = os.getenv(
-                "DBGPT_API_BASE", f"http://localhost:5670/{CLIENT_API_PATH}/{version}"
+                "DBGPT_API_BASE", f"http://localhost:5000/{CLIENT_API_PATH}/{version}"
             )
         if not api_key:
             api_key = os.getenv("DBGPT_API_KEY")
         if api_base and is_valid_url(api_base):
             self._api_url = api_base
         else:
             raise ValueError(f"api url {api_base} does not exist or is not accessible.")
@@ -142,15 +142,15 @@
             ChatCompletionResponse: The chat completion response.
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5670/api/v2"
+            DBGPT_API_BASE = "http://localhost:5000/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             res = await client.chat(model="chatgpt_proxyllm", messages="Hello?")
         """
         request = ChatCompletionRequestBody(
             model=model,
             messages=messages,
@@ -218,15 +218,15 @@
 
         Examples:
         --------
         .. code-block:: python
 
             from dbgpt.client import Client
 
-            DBGPT_API_BASE = "http://localhost:5670/api/v2"
+            DBGPT_API_BASE = "http://localhost:5000/api/v2"
             DBGPT_API_KEY = "dbgpt"
             client = Client(api_base=DBGPT_API_BASE, api_key=DBGPT_API_KEY)
             res = await client.chat_stream(model="chatgpt_proxyllm", messages="Hello?")
         """
         request = ChatCompletionRequestBody(
             model=model,
             messages=messages,
```

### Comparing `dbgpt-0.5.4/dbgpt/client/datasource.py` & `dbgpt-0.5.4rc0/dbgpt/client/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/flow.py` & `dbgpt-0.5.4rc0/dbgpt/client/flow.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/client/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/client/schema.py` & `dbgpt-0.5.4rc0/dbgpt/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/component.py` & `dbgpt-0.5.4rc0/dbgpt/component.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/configs/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/configs/model_config.py` & `dbgpt-0.5.4rc0/dbgpt/configs/model_config.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.4rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.4rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/dag/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/flow/compat.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/compat.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/task/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/trigger/ext_http_trigger.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/ext_http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.4rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/cache.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/embeddings.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/llm.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/message.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/message.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/output_parser.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/prompt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/interface/storage.py` & `dbgpt-0.5.4rc0/dbgpt/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.4rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/core/schema/api.py` & `dbgpt-0.5.4rc0/dbgpt/core/schema/api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/base.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/manages/connect_config_db.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/manages/connect_config_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_duckdb.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.4rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/template.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/cli.py` & `dbgpt-0.5.4rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.4rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/parameter.py` & `dbgpt-0.5.4rc0/dbgpt/model/parameter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/base.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/moonshot.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.4rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.4rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.4rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/embedding/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.4rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/evaluation/retriever.py` & `dbgpt-0.5.4rc0/dbgpt/rag/evaluation/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/csv.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/html.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/markdown.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/string.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/string.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/txt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/knowledge/url.py` & `dbgpt-0.5.4rc0/dbgpt/rag/knowledge/url.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/retriever/base.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/retriever/rerank.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.4rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.4rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/summary/rdbms_db_summary.py` & `dbgpt-0.5.4rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.4rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.4rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.4rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.4rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/schema.py` & `dbgpt-0.5.4rc0/dbgpt/storage/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/connector.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/connector.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/filters.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.4rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/annotations.py` & `dbgpt-0.5.4rc0/dbgpt/util/annotations.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/api_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.4rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 model_name = "vicuna-7b-v1.5"
 model_path = LLM_MODEL_CONFIG[model_name]
 # or vllm
 model_type = "huggingface"
 
-controller_addr = "http://127.0.0.1:5670"
+controller_addr = "http://127.0.0.1:5000"
 
 result_csv_file = None
 
 parallel_nums = [1, 2, 4, 16, 32]
 # parallel_nums = [1, 2, 4]
```

### Comparing `dbgpt-0.5.4/dbgpt/util/chat_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/code_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/code_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/command_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/command_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     from dbgpt.util.parameter_utils import EnvArgumentParser
 
     env_to_app = {}
     env_to_app.update(os.environ)
     app_env = EnvArgumentParser._kwargs_to_env_key_value(kwargs)
     env_to_app.update(app_env)
-    cmd = f"uvicorn {app} --host 0.0.0.0 --port 5670"
+    cmd = f"uvicorn {app} --host 0.0.0.0 --port 5000"
     if "windows" in platform.system().lower():
         raise Exception("Not support on windows")
     else:  # macOS, Linux, and other Unix-like systems
         process = subprocess.Popen(cmd, shell=True, env=env_to_app)
     print(f"Started {app} with gunicorn in background with pid: {process.pid}")
 
 
@@ -133,16 +133,16 @@
                 if connections is not None and len(ports) == 0:
                     for connection in connections:
                         if connection.status == psutil.CONN_LISTEN:
                             ports.append(connection.laddr.port)
         except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
             pass
 
-    # Sort ports with preference for 8000 and 5670
-    ports.sort(key=lambda x: (x != 8000, x != 5670, x))
+    # Sort ports with preference for 8000 and 5000
+    ports.sort(key=lambda x: (x != 8000, x != 5000, x))
     return ports
 
 
 @lru_cache()
 def _detect_controller_address() -> str:
     controller_addr = os.getenv("CONTROLLER_ADDRESS")
     if controller_addr:
```

### Comparing `dbgpt-0.5.4/dbgpt/util/config_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/console/console.py` & `dbgpt-0.5.4rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.4rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/repo.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/dbgpts/template.py` & `dbgpt-0.5.4rc0/dbgpt/util/dbgpts/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/error_types.py` & `dbgpt-0.5.4rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/executor_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/fastapi.py` & `dbgpt-0.5.4rc0/dbgpt/util/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/formatting.py` & `dbgpt-0.5.4rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/function_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/function_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/global_helper.py` & `dbgpt-0.5.4rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/json_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/model_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/module_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/net_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/network/_cli.py` & `dbgpt-0.5.4rc0/dbgpt/util/network/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/openai_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/pagination_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/pd_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/prompt_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.4rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/similarity_util.py` & `dbgpt-0.5.4rc0/dbgpt/util/similarity_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/singleton.py` & `dbgpt-0.5.4rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/speech/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/speech/brian.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/speech/say.py` & `dbgpt-0.5.4rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/string_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/system_utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/base.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/span_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.4rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/util/utils.py` & `dbgpt-0.5.4rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/vis/__init__.py` & `dbgpt-0.5.4rc0/dbgpt/vis/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """GPT-Vis Module."""
 
-from .base import Vis  # noqa: F401
 from .client import vis_client  # noqa: F401
+from .base import Vis  # noqa: F401
 from .tags.vis_agent_message import VisAgentMessages  # noqa: F401
 from .tags.vis_agent_plans import VisAgentPlans  # noqa: F401
 from .tags.vis_chart import VisChart  # noqa: F401
 from .tags.vis_code import VisCode  # noqa: F401
 from .tags.vis_dashboard import VisDashboard  # noqa: F401
 from .tags.vis_plugin import VisPlugin  # noqa: F401
```

### Comparing `dbgpt-0.5.4/dbgpt/vis/base.py` & `dbgpt-0.5.4rc0/dbgpt/vis/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/vis/client.py` & `dbgpt-0.5.4rc0/dbgpt/vis/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/vis/tags/vis_chart.py` & `dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_chart.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt/vis/tags/vis_dashboard.py` & `dbgpt-0.5.4rc0/dbgpt/vis/tags/vis_dashboard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.4rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.4
+Version: 0.5.4rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -315,94 +315,94 @@
 Requires-Dist: pymysql; extra == "default"
 Requires-Dist: torch==2.2.1; extra == "default"
 Requires-Dist: torchvision==0.17.1; extra == "default"
 Requires-Dist: torchaudio==2.2.1; extra == "default"
 Requires-Dist: cpm_kernels; extra == "default"
 Requires-Dist: rocksdict; extra == "default"
 Provides-Extra: all
-Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: duckdb; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: gTTS==2.3.1; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: fastapi==0.98.0; extra == "all"
-Requires-Dist: bs4; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: thrift; extra == "all"
 Requires-Dist: python-multipart; extra == "all"
+Requires-Dist: clickhouse-connect; extra == "all"
+Requires-Dist: pymysql; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: torchaudio==2.2.1; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: importlib-resources==5.12.0; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: dashscope; extra == "all"
 Requires-Dist: jinja2; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: rich; extra == "all"
-Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: protobuf==3.20.3; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: rocksdict; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: pyspark; extra == "all"
 Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: importlib-resources==5.12.0; extra == "all"
 Requires-Dist: aiohttp==3.8.4; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: langchain>=0.0.286; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: openai; extra == "all"
 Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: cachetools; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: fschat; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
-Requires-Dist: python-docx; extra == "all"
-Requires-Dist: termcolor; extra == "all"
 Requires-Dist: spacy==3.5.3; extra == "all"
-Requires-Dist: pympler; extra == "all"
+Requires-Dist: python-docx; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: pymysql; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: fastapi==0.98.0; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: seaborn; extra == "all"
 Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: vllm; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: shortuuid; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
 Requires-Dist: msgpack; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: pypdf; extra == "all"
-Requires-Dist: chromadb==0.4.10; extra == "all"
+Requires-Dist: auto-gpt-plugin-template; extra == "all"
 Requires-Dist: pydantic<2,>=1; extra == "all"
-Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: chardet; extra == "all"
+Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: openpyxl==3.1.2; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: cachetools; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: typeguard; extra == "all"
+Requires-Dist: gTTS==2.3.1; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
```

### Comparing `dbgpt-0.5.4/dbgpt.egg-info/SOURCES.txt` & `dbgpt-0.5.4rc0/dbgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.4/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.4rc0/dbgpt.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -22,94 +22,94 @@
 colorama==0.4.6
 tomlkit
 rich
 termcolor
 pandas==2.0.3
 
 [all]
-rocksdict
-duckdb
-typeguard
-click
-gTTS==2.3.1
-torch==2.2.1
-aiofiles
-pyspark
-sqlparse==0.4.4
-psutil==5.9.4
-coloredlogs
-openpyxl==3.1.2
-mysqlclient==2.1.0
-fastapi==0.98.0
-bs4
-chardet==5.1.0
-openai
-psycopg2
-llama-cpp-python
-thrift
 python-multipart
+clickhouse-connect
+pymysql
+GitPython
+markdown
+psycopg2
+pymssql
+chromadb==0.4.10
+torchaudio==2.2.1
+alembic==1.12.0
+schedule
+importlib-resources==5.12.0
+duckdb-engine
+prettytable
+dashscope
 jinja2
-graphviz
-xlrd==2.0.1
-seaborn
-rich
-langchain>=0.0.286
+uvicorn
+duckdb
+SQLAlchemy<2.0.29,>=2.0.25
+python-dotenv==1.0.0
+gpt4all
+chardet
+python-pptx
+llama-cpp-python
+sentencepiece
 protobuf==3.20.3
+colorama==0.4.6
+mysqlclient==2.1.0
+coloredlogs
+fschat
+pypdf
+torchvision==0.17.1
+rocksdict
+sqlparse==0.4.4
+xlrd==2.0.1
+tomlkit
+pympler
+sentence-transformers
+click
+pandas==2.0.3
+pyspark
 tiktoken
-auto-gpt-plugin-template
-importlib-resources==5.12.0
 aiohttp==3.8.4
+zhipuai
+torch==2.2.1
+transformers>=4.34.0
+pymilvus
+langchain>=0.0.286
+thrift
+bs4
+openai
 thrift_sasl
-cpm_kernels
-torchvision==0.17.1
-tokenizers>=0.14
-uvicorn
-cachetools
-httpx
-dashscope
-fschat
-tomlkit
-python-docx
-termcolor
 spacy==3.5.3
-pympler
+python-docx
+aiofiles
+tokenizers>=0.14
+graphviz
 weaviate-client
-pydoris<2.0.0,>=1.0.2
-pymssql
-pymilvus
-pymysql
-python-dotenv==1.0.0
+accelerate>=0.20.3
+psutil==5.9.4
+httpx
+fastapi==0.98.0
+chardet==5.1.0
+pyhive
+seaborn
 bitsandbytes
-schedule
 vllm
-zhipuai
-prettytable
-markdown
-sentence-transformers
-shortuuid
-sentencepiece
-SQLAlchemy<2.0.29,>=2.0.25
-duckdb-engine
-GitPython
-colorama==0.4.6
-accelerate>=0.20.3
-pandas==2.0.3
-transformers>=4.34.0
 msgpack
-gpt4all
-alembic==1.12.0
-jsonschema
-python-pptx
-clickhouse-connect
-pypdf
-chromadb==0.4.10
+auto-gpt-plugin-template
 pydantic<2,>=1
-torchaudio==2.2.1
-pyhive
-chardet
+pydoris<2.0.0,>=1.0.2
+rich
+openpyxl==3.1.2
+jsonschema
+cachetools
+termcolor
+shortuuid
+typeguard
+gTTS==2.3.1
+cpm_kernels
 
 [bitsandbytes]
 bitsandbytes
 
 [cache]
 rocksdict
```

### Comparing `dbgpt-0.5.4/setup.py` & `dbgpt-0.5.4rc0/setup.py`

 * *Files identical despite different names*

