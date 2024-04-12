# Comparing `tmp/gpt_engineer-0.2.8.tar.gz` & `tmp/gpt_engineer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_engineer-0.2.8.tar", max compression
+gzip compressed data, was "gpt_engineer-0.2.9.tar", max compression
```

## Comparing `gpt_engineer-0.2.8.tar` & `gpt_engineer-0.2.9.tar`

### file list

```diff
@@ -1,54 +1,65 @@
--rw-r--r--   0        0        0     1068 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/LICENSE
--rw-r--r--   0        0        0     4320 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/README.md
--rw-r--r--   0        0        0      160 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/__init__.py
--rw-r--r--   0        0        0        0 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/__init__.py
--rw-r--r--   0        0        0      500 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/__init__.py
--rw-r--r--   0        0        0     5891 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/cli_agent.py
--rw-r--r--   0        0        0     5539 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/collect.py
--rw-r--r--   0        0        0    13342 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/file_selector.py
--rw-r--r--   0        0        0     6614 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/learning.py
--rw-r--r--   0        0        0     6586 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/applications/cli/main.py
--rw-r--r--   0        0        0     1527 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/__main__.py
--rw-r--r--   0        0        0        0 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/__init__.py
--rw-r--r--   0        0        0     2961 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py
--rw-r--r--   0        0        0     1631 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md
--rw-r--r--   0        0        0     4331 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md
--rw-r--r--   0        0        0      645 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md
--rw-r--r--   0        0        0     2813 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt
--rw-r--r--   0        0        0     2744 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt
--rw-r--r--   0        0        0     6503 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/load.py
--rw-r--r--   0        0        0     3260 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gptme/load.py
--rw-r--r--   0        0        0      420 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/load.py
--rw-r--r--   0        0        0     2697 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/run.py
--rw-r--r--   0        0        0     1340 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/benchmark/types.py
--rw-r--r--   0        0        0        0 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/core/__init__.py
--rw-r--r--   0        0        0     7285 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/core/ai.py
--rw-r--r--   0        0        0      829 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/core/base_agent.py
--rw-r--r--   0        0        0     1360 2024-02-11 09:57:42.699935 gpt_engineer-0.2.8/gpt_engineer/core/base_execution_env.py
--rw-r--r--   0        0        0      118 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/base_memory.py
--rw-r--r--   0        0        0     6338 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/chat_to_files.py
--rw-r--r--   0        0        0        0 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/__init__.py
--rw-r--r--   0        0        0       30 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/constants.py
--rw-r--r--   0        0        0     2734 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/disk_execution_env.py
--rw-r--r--   0        0        0     8060 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/disk_memory.py
--rw-r--r--   0        0        0     1177 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/file_store.py
--rw-r--r--   0        0        0      492 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/paths.py
--rw-r--r--   0        0        0     2828 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/simple_agent.py
--rw-r--r--   0        0        0     5986 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/default/steps.py
--rw-r--r--   0        0        0     2221 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/files_dict.py
--rw-r--r--   0        0        0      427 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/preprompts_holder.py
--rw-r--r--   0        0        0     5588 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/token_usage.py
--rw-r--r--   0        0        0      754 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/core/version_manager.py
--rw-r--r--   0        0        0      228 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/clarify
--rw-r--r--   0        0        0      467 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/entrypoint
--rw-r--r--   0        0        0      496 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/file_format
--rw-r--r--   0        0        0      498 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/file_format_fix
--rw-r--r--   0        0        0      998 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/generate
--rw-r--r--   0        0        0     2314 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/improve
--rw-r--r--   0        0        0      548 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/philosophy
--rw-r--r--   0        0        0      165 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/preprompts/roadmap
--rw-r--r--   0        0        0        0 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/tools/__init__.py
--rw-r--r--   0        0        0     7496 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/tools/custom_steps.py
--rw-r--r--   0        0        0     1699 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/gpt_engineer/tools/supported_languages.py
--rw-r--r--   0        0        0     2496 2024-02-11 09:57:42.703935 gpt_engineer-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5623 1970-01-01 00:00:00.000000 gpt_engineer-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5024 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/README.md
+-rw-r--r--   0        0        0      160 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/__init__.py
+-rw-r--r--   0        0        0     8888 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/cli_agent.py
+-rw-r--r--   0        0        0     5749 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/collect.py
+-rw-r--r--   0        0        0    17912 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/file_selector.py
+-rw-r--r--   0        0        0     9812 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/learning.py
+-rw-r--r--   0        0        0    16232 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/applications/cli/main.py
+-rw-r--r--   0        0        0     3200 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/__main__.py
+-rw-r--r--   0        0        0     3822 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/load.py
+-rw-r--r--   0        0        0      555 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/problem.py
+-rw-r--r--   0        0        0       98 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/apps/problems.py
+-rw-r--r--   0        0        0      381 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/__init__.py
+-rw-r--r--   0        0        0     6202 2024-04-12 09:05:38.888566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/eval_tools.py
+-rw-r--r--   0        0        0     1631 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md
+-rw-r--r--   0        0        0     4331 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md
+-rw-r--r--   0        0        0      645 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md
+-rw-r--r--   0        0        0     2813 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt
+-rw-r--r--   0        0        0     2744 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt
+-rw-r--r--   0        0        0     7958 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/load.py
+-rw-r--r--   0        0        0     4086 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gptme/load.py
+-rw-r--r--   0        0        0     1320 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/load.py
+-rw-r--r--   0        0        0     3587 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/load.py
+-rw-r--r--   0        0        0      531 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/problem.py
+-rw-r--r--   0        0        0       93 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/mbpp/problems.py
+-rw-r--r--   0        0        0     4244 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/run.py
+-rw-r--r--   0        0        0     2417 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/benchmark/types.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/__init__.py
+-rw-r--r--   0        0        0    14416 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/ai.py
+-rw-r--r--   0        0        0     1015 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_agent.py
+-rw-r--r--   0        0        0     1191 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_execution_env.py
+-rw-r--r--   0        0        0      485 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/base_memory.py
+-rw-r--r--   0        0        0     8902 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/chat_to_files.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/constants.py
+-rw-r--r--   0        0        0     3618 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/disk_execution_env.py
+-rw-r--r--   0        0        0     9680 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/disk_memory.py
+-rw-r--r--   0        0        0     1802 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/file_store.py
+-rw-r--r--   0        0        0     2370 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/paths.py
+-rw-r--r--   0        0        0     3582 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/simple_agent.py
+-rw-r--r--   0        0        0    11984 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/default/steps.py
+-rw-r--r--   0        0        0    19158 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/diff.py
+-rw-r--r--   0        0        0     3877 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/files_dict.py
+-rw-r--r--   0        0        0     2389 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/git.py
+-rw-r--r--   0        0        0      869 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/preprompts_holder.py
+-rw-r--r--   0        0        0     4993 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/project_config.py
+-rw-r--r--   0        0        0      901 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/prompt.py
+-rw-r--r--   0        0        0     9483 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/token_usage.py
+-rw-r--r--   0        0        0      917 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/core/version_manager.py
+-rw-r--r--   0        0        0      228 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/clarify
+-rw-r--r--   0        0        0      432 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/entrypoint
+-rw-r--r--   0        0        0      496 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format
+-rw-r--r--   0        0        0     1555 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format_diff
+-rw-r--r--   0        0        0      498 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/file_format_fix
+-rw-r--r--   0        0        0      998 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/generate
+-rw-r--r--   0        0        0     1146 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/improve
+-rw-r--r--   0        0        0      548 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/philosophy
+-rw-r--r--   0        0        0      165 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/preprompts/roadmap
+-rw-r--r--   0        0        0        0 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/__init__.py
+-rw-r--r--   0        0        0     7691 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/custom_steps.py
+-rw-r--r--   0        0        0     1884 2024-04-12 09:05:38.892566 gpt_engineer-0.2.9/gpt_engineer/tools/supported_languages.py
+-rw-r--r--   0        0        0     2661 2024-04-12 09:05:38.896566 gpt_engineer-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6592 1970-01-01 00:00:00.000000 gpt_engineer-0.2.9/PKG-INFO
```

### Comparing `gpt_engineer-0.2.8/LICENSE` & `gpt_engineer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/README.md` & `gpt_engineer-0.2.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -49,32 +49,43 @@
 - Run `gpte <project_dir>` with a relative path to your folder
   - For example: `gpte projects/my-new-project` from the gpt-engineer directory root with your new folder in `projects/`
 
 ### Improve Existing Code
 - Locate a folder with code which you want to improve anywhere on your computer
 - Create a file called `prompt` (no extension) inside your new folder and fill it with instructions for how you want to improve the code
 - Run `gpte <project_dir> -i` with a relative path to your folder
-  - For example: `gpte projects/my-old-project` from the gpt-engineer directory root with your folder in `projects/`
+  - For example: `gpte projects/my-old-project -i` from the gpt-engineer directory root with your folder in `projects/`
 
 By running gpt-engineer you agree to our [terms](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/TERMS_OF_USE.md).
 
 
 ## Relation to gptengineer.app
 [gptengineer.app](https://gptengineer.app/) is a commercial project for automatic generation of web-apps.
 It features a UI for non-technical users, connected to a git controlled codebase.
 The gptengineer.app team is actively supporting the open source community.
 
 
 ## Features
 
+### Pre Prompts
 You can specify the "identity" of the AI agent by overriding the `preprompts` folder, with your own version of the `preprompts`, using the `--use-custom-preprompts` argument.
 
 Editing the `preprompts` is how you make the agent remember things between projects.
 
-You can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
+### Vision
+
+By default, GPT Engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifiying an image directory with the --image_directory flag and setting a vision capable model in the second cli argument.
+
+E.g. `gpte projects/example-vision gpt-4-vision-preview --prompt_file prompt/text --image_directory prompt/images -i`
+
+### Open source, local and alternative models
+
+By defaul GPT Engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
+
+With a little extra set up you can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
 
 ## Mission
 
 The gpt-engineer community mission is to **maintain tools that coding agent builders can use and facilitate collaboration in the open source community**.
 
 If you are interested in contributing to this, we are interested in having you.
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/applications/cli/collect.py` & `gpt_engineer-0.2.9/gpt_engineer/applications/cli/collect.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,101 @@
 """
+Module `collect` - Data Handling and RudderStack Integration
+
 This module provides functionalities to handle and send learning data to RudderStack
 for the purpose of analysis and to improve the gpt-engineer system. The data is sent
 only when the user gives consent to share.
 
-The module provides the following main functions:
-
-- `send_learning`: Directly send a learning data to RudderStack.
-- `collect_learnings`: Extract, possibly adjust, and send the learning data based on
-  provided input parameters.
-- `steps_file_hash`: Computes the SHA-256 hash of the steps file, which might be used
-  for identifying the exact version or changes in the steps.
+Functions:
+    send_learning(learning): Sends learning data to RudderStack.
+    collect_learnings(prompt, model, temperature, config, memory, review): Processes and sends learning data.
+    collect_and_send_human_review(prompt, model, temperature, config, memory): Collects human feedback and sends it.
 
 Dependencies:
-- hashlib: For generating SHA-256 hash.
-- typing: For type annotations.
-- gpt_engineer.core: Core functionalities of gpt-engineer.
-- gpt_engineer.cli.learning: Handles the extraction of learning data.
+    hashlib: For generating SHA-256 hash.
+    typing: For type annotations.
+    gpt_engineer.core: Core functionalities of gpt-engineer.
+    gpt_engineer.cli.learning: Handles the extraction of learning data.
 
-Note:
+Notes:
     Data sent to RudderStack is not shared with third parties and is used solely to
     improve gpt-engineer and allow it to handle a broader range of use cases.
     Consent logic is in gpt_engineer/learning.py.
-
 """
 
 from typing import Tuple
 
 from gpt_engineer.applications.cli.learning import (
     Learning,
     Review,
     extract_learning,
     human_review_input,
 )
 from gpt_engineer.core.default.disk_memory import DiskMemory
+from gpt_engineer.core.prompt import Prompt
 
 
 def send_learning(learning: Learning):
     """
     Send the learning data to RudderStack for analysis.
 
-    Note:
-    This function is only called if consent is given to share data.
-    Data is not shared to a third party. It is used with the sole purpose of
-    improving gpt-engineer, and letting it handle more use cases.
-    Consent logic is in gpt_engineer/learning.py
-
     Parameters
     ----------
     learning : Learning
-        The learning data to send.
+        An instance of the Learning class containing the data to be sent.
+
+    Notes
+    -----
+    This function is only called if consent is given to share data.
+    Data is not shared to a third party. It is used with the sole purpose of
+    improving gpt-engineer, and letting it handle more use cases.
+    Consent logic is in gpt_engineer/learning.py.
     """
     import rudderstack.analytics as rudder_analytics
 
     rudder_analytics.write_key = "2Re4kqwL61GDp7S8ewe6K5dbogG"
     rudder_analytics.dataPlaneUrl = "https://gptengineerezm.dataplane.rudderstack.com"
 
     rudder_analytics.track(
         user_id=learning.session,
         event="learning",
         properties=learning.to_dict(),  # type: ignore
     )
 
 
 def collect_learnings(
-    prompt: str,
+    prompt: Prompt,
     model: str,
     temperature: float,
     config: any,
     memory: DiskMemory,
     review: Review,
 ):
     """
     Collect the learning data and send it to RudderStack for analysis.
 
     Parameters
     ----------
+    prompt : str
+        The initial prompt or question that was provided to the model.
     model : str
-        The name of the model used.
+        The name of the model used for generating the response.
     temperature : float
-        The temperature used.
-    steps : List[Step]
-        The list of steps.
-    dbs : DBs
-        The database containing the workspace.
+        The temperature setting used in the model's response generation.
+    config : any
+        Configuration parameters used for the learning session.
+    memory : DiskMemory
+        An instance of DiskMemory for storing and retrieving data.
+    review : Review
+        An instance of Review containing human feedback on the model's response.
+
+    Notes
+    -----
+    This function attempts to send the learning data to RudderStack. If the data size exceeds
+    the maximum allowed size, it trims the data and retries sending it.
     """
     learnings = extract_learning(prompt, model, temperature, config, memory, review)
     try:
         send_learning(learnings)
     except RuntimeError:
         # try to remove some parts of learning that might be too big
         # rudderstack max event size is 32kb
@@ -126,40 +135,43 @@
 #     """
 #     with open(steps.__file__, "r") as f:
 #         content = f.read()
 #         return hashlib.sha256(content.encode("utf-8")).hexdigest()
 
 
 def collect_and_send_human_review(
-    prompt: str,
+    prompt: Prompt,
     model: str,
     temperature: float,
     config: Tuple[str, ...],
     memory: DiskMemory,
 ):
     """
-    Collects human feedback on the code and stores it in memory.
-
-    This function prompts the user for a review of the generated or improved code using the `human_review_input`
-    function. If a valid review is provided, it's serialized to JSON format and stored within the database's
-    memory under the "review" key.
-
-    Parameters:
-    - ai (AI): An instance of the AI model. Although not directly used within the function, it is kept as
-      a parameter for consistency with other functions.
-    - dbs (DBs): An instance containing the database configurations, user prompts, project metadata,
-      and memory storage. This function specifically interacts with the memory storage to save the human review.
-
-    Returns:
-    - list: Returns an empty list, indicating that there's no subsequent interaction with the LLM
-      or no further messages to be processed.
+    Collects human feedback on the code and sends it for analysis.
 
-    Notes:
-    - It's assumed that the `human_review_input` function handles all the interactions with the user to
-      gather feedback and returns either the feedback or None if no feedback was provided.
-    - Ensure that the database's memory has enough space or is set up correctly to store the serialized review data.
+    Parameters
+    ----------
+    prompt : str
+        The initial prompt or question that was provided to the model.
+    model : str
+        The name of the model used for generating the response.
+    temperature : float
+        The temperature setting used in the model's response generation.
+    config : Tuple[str, ...]
+        Configuration parameters used for the learning session.
+    memory : DiskMemory
+        An instance of DiskMemory for storing and retrieving data.
+
+    Returns
+    -------
+    None
+
+    Notes
+    -----
+    This function prompts the user for a review of the generated or improved code using the
+    `human_review_input` function. If a valid review is provided, it's serialized to JSON format
+    and stored within the database's memory under the "review" key.
     """
 
-    """Collects and stores human review of the code"""
     review = human_review_input()
     if review:
         collect_learnings(prompt, model, temperature, config, memory, review)
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/applications/cli/learning.py` & `gpt_engineer-0.2.9/gpt_engineer/applications/cli/learning.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,34 @@
 """
-This module provides tools and data structures for supporting a feedback loop in the GPT Engineer application.
+The `learning` module is designed to facilitate the collection and storage of user feedback on the outputs generated by the GPT Engineer tool. It provides mechanisms for obtaining user consent, capturing user reviews, and storing this information for future analysis and enhancement of the tool's performance.
 
-The primary intent of this module is to gather feedback from the user on the output of the gpt-engineer tool,
-with their consent, and to store this feedback for further analysis and improvement of the tool.
-
-Classes:
-----------
-Review:
-    Represents user's review of the generated code.
-Learning:
-    Represents the metadata and feedback collected for a session in which gpt-engineer was used.
-
-Functions:
-----------
-human_review_input() -> Review:
-    Interactively gathers feedback from the user regarding the performance of generated code.
-
-check_consent() -> bool:
-    Checks if the user has previously given consent to store their data and if not, asks for it.
-
-collect_consent() -> bool:
-    Verifies if the user has given consent to store their data or prompts for it.
-
-ask_if_can_store() -> bool:
-    Asks the user if it's permissible to store their data for gpt-engineer improvement.
-
-logs_to_string(steps: List[Step], logs: DB) -> str:
-    Converts logs of steps into a readable string format.
-
-extract_learning(model: str, temperature: float, steps: List[Step], dbs: DBs, steps_file_hash) -> Learning:
-    Extracts feedback and session details to create a Learning instance.
-
-get_session() -> str:
-    Retrieves a unique identifier for the current user session.
-
-Constants:
-----------
-TERM_CHOICES:
-    Terminal color choices for user interactive prompts.
+Classes
+-------
+Review : dataclass
+    Represents a user's review of the generated code, including whether it ran, was perfect, was useful, and any additional comments.
+Learning : dataclass
+    Encapsulates the metadata and feedback collected during a session of using the GPT Engineer tool, including the prompt, model, temperature, configuration, logs, session identifier, user review, and timestamp.
+
+Functions
+---------
+human_review_input() -> Optional[Review]
+    Interactively gathers feedback from the user regarding the performance of generated code and returns a Review instance.
+check_collection_consent() -> bool
+    Checks if the user has previously given consent to store their data and, if not, asks for it.
+ask_collection_consent() -> bool
+    Prompts the user for consent to store their data for the purpose of improving GPT Engineer.
+extract_learning(prompt: Prompt, model: str, temperature: float, config: Tuple[str, ...], memory: DiskMemory, review: Review) -> Learning
+    Extracts feedback and session details to create a Learning instance based on the provided parameters.
+get_session() -> str
+    Retrieves a unique identifier for the current user session, creating one if it does not exist.
+
+Constants
+---------
+TERM_CHOICES : tuple
+    Terminal color choices for user interactive prompts, formatted with termcolor for readability.
 """
 
 import json
 import random
 import tempfile
 
 from dataclasses import dataclass, field
@@ -49,30 +36,73 @@
 from pathlib import Path
 from typing import Optional, Tuple
 
 from dataclasses_json import dataclass_json
 from termcolor import colored
 
 from gpt_engineer.core.default.disk_memory import DiskMemory
+from gpt_engineer.core.prompt import Prompt
 
 
 @dataclass_json
 @dataclass
 class Review:
+    """
+    A dataclass that represents a user's review of the generated code.
+
+    Attributes
+    ----------
+    ran : Optional[bool]
+        Indicates whether the generated code ran without errors.
+    perfect : Optional[bool]
+        Indicates whether the generated code met all the user's requirements.
+    works : Optional[bool]
+        Indicates whether the generated code was useful, even if not perfect.
+    comments : str
+        Any additional comments provided by the user.
+    raw : str
+        A raw string representation of the user's responses.
+    """
+
     ran: Optional[bool]
     perfect: Optional[bool]
     works: Optional[bool]
     comments: str
     raw: str
 
 
 @dataclass_json
 @dataclass
 class Learning:
-    prompt: str
+    """
+    A dataclass that encapsulates the learning data collected during a GPT Engineer session.
+
+    Attributes
+    ----------
+    prompt : str
+        The initial prompt provided to the GPT Engineer.
+    model : str
+        The name of the model used during the session.
+    temperature : float
+        The temperature setting used for the model's responses.
+    config : str
+        A JSON string representing the configuration settings for the session.
+    logs : str
+        A JSON string representing the logs of the session.
+    session : str
+        A unique identifier for the user session.
+    review : Optional[Review]
+        The user's review of the generated code.
+    timestamp : str
+        The UTC timestamp when the learning data was created.
+    version : str
+        The version of the learning data schema.
+    """
+
+    prompt: Prompt
     model: str
     temperature: float
     config: str
     logs: str
     session: str
     review: Optional[Review]
     timestamp: str = field(default_factory=lambda: datetime.utcnow().isoformat())
@@ -87,80 +117,101 @@
     + colored("u", "yellow")
     + "(ncertain): "
 )
 
 
 def human_review_input() -> Optional[Review]:
     """
-    Ask the user to review the generated code and return their review.
+    Interactively prompts the user to review the generated code and returns their feedback encapsulated in a Review object.
+
+    This function will first check if the user has given consent to collect their feedback. If consent is given, it will ask the user a series of questions about the generated code's performance and capture their responses.
 
     Returns
     -------
-    Review
-        The user's review of the generated code.
+    Optional[Review]
+        A Review object containing the user's feedback, or None if consent is not given.
     """
     print()
     if not check_collection_consent():
         return None
     print()
     print(
         colored("To help gpt-engineer learn, please answer 3 questions:", "light_green")
     )
     print()
 
     ran = input("Did the generated code run at all? " + TERM_CHOICES)
-    while ran not in ("y", "n", "u"):
-        ran = input("Invalid input. Please enter y, n, or u: ")
-
-    perfect = ""
-    useful = ""
+    ran = ask_for_valid_input(ran)
 
     if ran == "y":
         perfect = input(
             "Did the generated code do everything you wanted? " + TERM_CHOICES
         )
-        while perfect not in ("y", "n", "u"):
-            perfect = input("Invalid input. Please enter y, n, or u: ")
+        perfect = ask_for_valid_input(perfect)
 
         if perfect != "y":
             useful = input("Did the generated code do anything useful? " + TERM_CHOICES)
-            while useful not in ("y", "n", "u"):
-                useful = input("Invalid input. Please enter y, n, or u: ")
+            useful = ask_for_valid_input(useful)
+        else:
+            useful = ""
+    else:
+        perfect = ""
+        useful = ""
 
-    comments = ""
     if perfect != "y":
         comments = input(
             "If you have time, please explain what was not working "
             + colored("(ok to leave blank)\n", "light_green")
         )
+    else:
+        comments = ""
 
     return Review(
         raw=", ".join([ran, perfect, useful]),
         ran={"y": True, "n": False, "u": None, "": None}[ran],
         works={"y": True, "n": False, "u": None, "": None}[useful],
         perfect={"y": True, "n": False, "u": None, "": None}[perfect],
         comments=comments,
     )
 
 
+def ask_for_valid_input(ran):
+    while ran not in ("y", "n", "u"):
+        ran = input("Invalid input. Please enter y, n, or u: ")
+    return ran
+
+
 def check_collection_consent() -> bool:
     """
-    Check if the user has given consent to store their data.
-    If not, ask for their consent.
+    Checks if the user has previously given consent to store their data for feedback collection.
+
+    This function looks for a file that stores the user's consent status. If the file exists and contains 'true', consent is assumed. If the file does not exist or does not contain 'true', the function will prompt the user for consent.
+
+    Returns
+    -------
+    bool
+        True if the user has given consent, False otherwise.
     """
     path = Path(".gpte_consent")
     if path.exists() and path.read_text() == "true":
         return True
     else:
         return ask_collection_consent()
 
 
 def ask_collection_consent() -> bool:
     """
-    Ask the user for consent to store their data.
+    Asks the user for their consent to store their data for the purpose of improving the GPT Engineer tool.
+
+    The user's response is recorded in a file for future reference. If the user consents, the function will write 'true' to the file. If the user does not consent, no data will be collected, and the function will not modify the file.
+
+    Returns
+    -------
+    bool
+        True if the user consents, False otherwise.
     """
     answer = input(
         "Is it ok if we store your prompts to help improve GPT Engineer? (y/n)"
     )
     while answer.lower() not in ("y", "n"):
         answer = input("Invalid input. Please enter y or n: ")
 
@@ -180,62 +231,65 @@
                 "light_green",
             )
         )
         return False
 
 
 def extract_learning(
-    prompt: str,
+    prompt: Prompt,
     model: str,
     temperature: float,
     config: Tuple[str, ...],
     memory: DiskMemory,
     review: Review,
 ) -> Learning:
     """
-    Extract the learning data from the steps and databases.
+    Constructs a Learning object containing the session's metadata and user feedback.
 
     Parameters
     ----------
+    prompt : str
+        The initial prompt provided to the GPT Engineer.
     model : str
-        The name of the model used.
+        The name of the model used during the session.
     temperature : float
-        The temperature used.
-    steps : List[Step]
-        The list of steps.
-    dbs : DBs
-        The databases containing the input, logs, memory, and workspace.
-    steps_file_hash : str
-        The hash of the steps file.
+        The temperature setting used for the model's responses.
+    config : Tuple[str, ...]
+        A tuple representing the configuration settings for the session.
+    memory : DiskMemory
+        An object representing the disk memory used during the session.
+    review : Review
+        The user's review of the generated code.
 
     Returns
     -------
     Learning
-        The extracted learning data.
+        An instance of Learning containing all the session details and user feedback.
     """
-    learning = Learning(
+    return Learning(
         prompt=prompt,
         model=model,
         temperature=temperature,
         config=json.dumps(config),
         session=get_session(),
         logs=memory.to_json(),
         review=review,
     )
-    return learning
 
 
 def get_session() -> str:
     """
-    Returns a unique user id for the current user project (session).
+    Retrieves or generates a unique identifier for the current user session.
+
+    This function attempts to read a unique user ID from a temporary file. If the file does not exist, it generates a new random ID, writes it to the file, and returns it. This ID is used to uniquely identify the user's session.
 
     Returns
     -------
     str
-        The unique user id.
+        A unique identifier for the user session.
     """
     path = Path(tempfile.gettempdir()) / "gpt_engineer_user_id.txt"
 
     try:
         if path.exists():
             user_id = path.read_text()
         else:
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/__main__.py` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,56 @@
+"""
+Main entry point for the benchmarking tool.
+
+This module provides a command-line interface for running benchmarks using Typer.
+It allows users to specify the path to an agent, the benchmark(s) to run, and other
+options such as verbosity.
+
+Functions
+---------
+get_agent : function
+    Dynamically imports and returns the default configuration agent from the given path.
+
+main : function
+    The main function that runs the specified benchmarks with the given agent.
+    Outputs the results to the console.
+
+Attributes
+----------
+__name__ : str
+    The standard boilerplate for invoking the main function when the script is executed.
+"""
 import importlib
 
 from typing import Annotated, Optional
 
 import typer
 
 from langchain.cache import SQLiteCache
 from langchain.globals import set_llm_cache
 
+from gpt_engineer.applications.cli.main import load_env_if_needed
 from gpt_engineer.benchmark.benchmarks.load import get_benchmark
 from gpt_engineer.benchmark.run import print_results, run
 
 
 def get_agent(path):
+    """
+    Dynamically imports and returns the default configuration agent from the given path.
+
+    Parameters
+    ----------
+    path : str
+        The file path to the module containing the default configuration agent.
+
+    Returns
+    -------
+    BaseAgent
+        An instance of the imported default configuration agent.
+    """
     # Dynamically import the python module at path
     agent_module = importlib.import_module(path.replace("/", ".").replace(".py", ""))
     return agent_module.default_config_agent()
 
 
 def main(
     path_to_agent: Annotated[
@@ -30,15 +65,34 @@
     task_name: Annotated[
         Optional[str], typer.Argument(help="optional task name in benchmark")
     ] = None,
     verbose: Annotated[
         bool, typer.Option(help="print results for each task", show_default=False)
     ] = False,
 ):
+    """
+    The main function that runs the specified benchmarks with the given agent and outputs the results to the console.
+
+    Parameters
+    ----------
+    path_to_agent : str
+        The file path to the Python module that contains a function called 'default_config_agent'.
+    benchmarks : str
+        A comma-separated string of benchmark names to run.
+    task_name : Optional[str], default=None
+        An optional task name to run within the benchmark.
+    verbose : bool, default=False
+        A flag to indicate whether to print results for each task.
+
+    Returns
+    -------
+    None
+    """
     set_llm_cache(SQLiteCache(database_path=".langchain.db"))
+    load_env_if_needed()
 
     benchmarks = benchmarks.split(",")
     for benchmark_name in benchmarks:
         benchmark = get_benchmark(benchmark_name)
         agent = get_agent(path_to_agent)
 
         results = run(agent, benchmark, task_name, verbose=verbose)
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/EVAL_NEW_CODE_RESULTS.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/IMPROVE_CODE_RESULTS.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/evals/README.md`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/snake_game_files.txt`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/known_code_blobs/web_todo_files.txt`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/benchmark/benchmarks/gpteng/load.py` & `gpt_engineer-0.2.9/gpt_engineer/benchmark/benchmarks/gpteng/load.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+"""
+Module for loading GPT-Eng evaluation tasks.
+
+This module provides functionality to load tasks for evaluating GPT-based models
+on engineering tasks. It converts predefined evaluation cases into Task objects
+that can be used to benchmark the performance of AI models.
+
+Functions
+---------
+expect_to_assertion : function
+    Converts an expected result dictionary to an assertion function.
+
+eval_to_task : function
+    Converts an evaluation case dictionary to a Task object.
+
+load_gpteng : function
+    Loads the GPT-Eng benchmark, which consists of a series of tasks for evaluation.
+"""
+
 from pathlib import Path
 
 from gpt_engineer.benchmark.benchmarks.gpteng.eval_tools import (
     check_evaluation_component,
 )
 from gpt_engineer.benchmark.types import Assertable, Benchmark, Task
 from gpt_engineer.core.chat_to_files import chat_to_files_dict
@@ -127,21 +146,48 @@
 #         ]
 #     }
 # ]
 #
 
 
 def expect_to_assertion(expected_result):
+    """
+    Converts an expected result dictionary to an assertion function.
+
+    Parameters
+    ----------
+    expected_result : dict
+        The dictionary containing the expected result configuration.
+
+    Returns
+    -------
+    function
+        An assertion function that takes an Assertable object and returns a boolean.
+    """
+
     def assertion(assertable: Assertable):
         return check_evaluation_component(expected_result, assertable.files)
 
     return assertion
 
 
 def eval_to_task(case):
+    """
+    Converts an evaluation case dictionary to a Task object.
+
+    Parameters
+    ----------
+    case : dict
+        The dictionary containing the evaluation case configuration.
+
+    Returns
+    -------
+    Task
+        A Task object constructed from the evaluation case dictionary.
+    """
     if "improve_code_prompt" in case:
         prompt = case["improve_code_prompt"]
     else:
         prompt = case["code_prompt"]
 
     return Task(
         name=case["name"],
@@ -152,10 +198,18 @@
             f"{e['type']}_{i}": expect_to_assertion(e)
             for i, e in enumerate(case["expected_results"])
         },
     )
 
 
 def load_gpteng():
+    """
+    Loads the GPT-Eng benchmark, which consists of a series of tasks for evaluation.
+
+    Returns
+    -------
+    Benchmark
+        A Benchmark object containing a list of Task objects for the GPT-Eng evaluation.
+    """
     return Benchmark(
         name="gpte_eval", tasks=[eval_to_task(case) for case in evaluations]
     )
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/core/base_execution_env.py` & `gpt_engineer-0.2.9/gpt_engineer/core/base_execution_env.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,18 @@
 from typing import Optional, Tuple
 
 from gpt_engineer.core.files_dict import FilesDict
 
 
 class BaseExecutionEnv(ABC):
     """
-    Abstract base class for an execution environment.
+    Abstract base class for an execution environment capable of running code.
 
-    This class defines the interface for execution environments that can run code.
-    Implementations of this class are expected to provide a method to execute code
-    and potentially handle the execution process.
-
-    Methods
-    -------
-    execute_program(code: Code) -> Popen:
-        Execute the given code and return the process handle.
+    This class defines the interface for execution environments that can execute commands,
+    handle processes, and manage file uploads and downloads.
     """
 
     @abstractmethod
     def run(self, command: str, timeout: Optional[int] = None) -> Tuple[str, str, int]:
         """
         Runs a command in the execution environment.
         """
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/core/default/disk_execution_env.py` & `gpt_engineer-0.2.9/gpt_engineer/core/default/disk_execution_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,87 @@
+"""
+Module for managing the execution environment on the local disk.
+
+This module provides a class that handles the execution of code stored on the local
+file system. It includes methods for uploading files to the execution environment,
+running commands, and capturing the output.
+
+Classes
+-------
+DiskExecutionEnv
+    An execution environment that runs code on the local file system and captures
+    the output of the execution.
+
+Imports
+-------
+- subprocess: For running shell commands.
+- time: For timing the execution of commands.
+- Path: For handling file system paths.
+- Optional, Tuple, Union: For type annotations.
+- BaseExecutionEnv: For inheriting the base execution environment interface.
+- FileStore: For managing file storage.
+- FilesDict: For handling collections of files.
+"""
+
 import subprocess
 import time
 
 from pathlib import Path
 from typing import Optional, Tuple, Union
 
 from gpt_engineer.core.base_execution_env import BaseExecutionEnv
 from gpt_engineer.core.default.file_store import FileStore
 from gpt_engineer.core.files_dict import FilesDict
 
 
 class DiskExecutionEnv(BaseExecutionEnv):
     """
-    An execution environment that runs code on the local file system.
+    An execution environment that runs code on the local file system and captures
+    the output of the execution.
 
     This class is responsible for executing code that is stored on disk. It ensures that
     the necessary entrypoint file exists and then runs the code using a subprocess. If the
     execution is interrupted by the user, it handles the interruption gracefully.
 
-    Attributes:
-        path (str): The file system path where the code is located and will be executed.
+    Attributes
+    ----------
+    store : FileStore
+        An instance of FileStore that manages the storage of files in the execution
+        environment.
     """
 
     def __init__(self, path: Union[str, Path, None] = None):
-        self.store = FileStore(path)
+        self.files = FileStore(path)
 
     def upload(self, files: FilesDict) -> "DiskExecutionEnv":
-        self.store.upload(files)
+        self.files.push(files)
         return self
 
     def download(self) -> FilesDict:
-        return self.store.download()
+        return self.files.pull()
 
     def popen(self, command: str) -> subprocess.Popen:
         p = subprocess.Popen(
             command,
             shell=True,
-            cwd=self.store.working_dir,
+            cwd=self.files.working_dir,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         return p
 
     def run(self, command: str, timeout: Optional[int] = None) -> Tuple[str, str, int]:
         start = time.time()
         print("\n--- Start of run ---")
         # while running, also print the stdout and stderr
         p = subprocess.Popen(
             command,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
-            cwd=self.store.working_dir,
+            cwd=self.files.working_dir,
             text=True,
             shell=True,
         )
         print("$", command)
         stdout_full, stderr_full = "", ""
 
         try:
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/core/default/disk_memory.py` & `gpt_engineer-0.2.9/gpt_engineer/core/default/disk_memory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """
-Module for simple file-based key-value database management.
+Disk Memory Module
+==================
 
 This module provides a simple file-based key-value database system, where keys are
-represented as filenames and values are the contents of these files. The primary class,
-DB, is responsible for the CRUD operations on the database. Additionally, the module
-provides a dataclass `DBs` that encapsulates multiple `DB` instances to represent different
-databases like memory, logs, preprompts, etc.
-
-Functions:
-    archive(dbs: DBs) -> None:
-        Archives the memory and workspace databases, moving their contents to
-        the archive database with a timestamp.
-
-Classes:
-    DB:
-        A simple key-value store implemented as a file-based system.
-
-    DBs:
-        A dataclass containing multiple DB instances representing different databases.
-
-Imports:
-    - datetime: For timestamp generation when archiving.
-    - shutil: For moving directories during archiving.
-    - dataclasses: For the DBs dataclass definition.
-    - pathlib: For path manipulations.
-    - typing: For type annotations.
+represented as filenames and values are the contents of these files. The `DiskMemory` class
+is responsible for the CRUD operations on the database.
+
+Attributes
+----------
+None
+
+Functions
+---------
+None
+
+Classes
+-------
+DiskMemory
+    A file-based key-value store where keys correspond to filenames and values to file contents.
 """
 
+import base64
 import json
 import shutil
 
+from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Iterator, Optional, Union
 
 from gpt_engineer.core.base_memory import BaseMemory
 from gpt_engineer.tools.supported_languages import SUPPORTED_LANGUAGES
 
 
@@ -42,189 +37,196 @@
     """
     A file-based key-value store where keys correspond to filenames and values to file contents.
 
     This class provides an interface to a file-based database, leveraging file operations to
     facilitate CRUD-like interactions. It allows for quick checks on the existence of keys,
     retrieval of values based on keys, and setting new key-value pairs.
 
-    Attributes:
-        path (Path): The directory path where the database files are stored.
-    """
-
-    """
-    A file-based key-value store where keys correspond to filenames and values to file contents.
-
-    This class provides an interface to a file-based database, leveraging file operations to
-    facilitate CRUD-like interactions. It allows for quick checks on the existence of keys,
-    retrieval of values based on keys, and setting new key-value pairs.
-
     Attributes
     ----------
     path : Path
         The directory path where the database files are stored.
-
-    Methods
-    -------
-    __contains__(key: str) -> bool:
-        Check if a file (key) exists in the database.
-
-    __getitem__(key: str) -> str:
-        Retrieve the content of a file (value) based on its name (key).
-
-    get(key: str, default: Optional[Any] = None) -> Any:
-        Fetch content of a file or return a default value if it doesn't exist.
-
-    __setitem__(key: Union[str, Path], val: str):
-        Set or update the content of a file in the database.
-
-    Note:
-    -----
-    Care should be taken when choosing keys (filenames) to avoid potential
-    security issues, such as directory traversal. The class implements some checks
-    for this but it's essential to validate inputs from untrusted sources.
     """
 
-    """A simple key-value store, where keys are filenames and values are file contents."""
-
     def __init__(self, path: Union[str, Path]):
         """
-        Initialize the DB class.
+        Initialize the DiskMemory class with a specified path.
 
         Parameters
         ----------
-        path : Union[str, Path]
-            The path to the directory where the database files are stored.
+        path : str or Path
+            The path to the directory where the database files will be stored.
+
         """
         self.path: Path = Path(path).absolute()
 
         self.path.mkdir(parents=True, exist_ok=True)
 
     def __contains__(self, key: str) -> bool:
         """
-        Check if a file with the specified name exists in the database.
+        Determine whether the database contains a file with the specified key.
 
         Parameters
         ----------
         key : str
-            The name of the file to check.
+            The key (filename) to check for existence in the database.
 
         Returns
         -------
         bool
-            True if the file exists, False otherwise.
+            Returns True if the file exists, False otherwise.
+
         """
         return (self.path / key).is_file()
 
     def __getitem__(self, key: str) -> str:
         """
-        Get the content of a file in the database.
+        Retrieve the content of a file in the database corresponding to the given key.
+        If the file is an image with a .png or .jpeg extension, it returns the content
+        in Base64-encoded string format.
 
         Parameters
         ----------
         key : str
-            The name of the file to get the content of.
+            The key (filename) whose content is to be retrieved.
 
         Returns
         -------
         str
-            The content of the file.
+            The content of the file associated with the key, or Base64-encoded string if it's a .png or .jpeg file.
 
         Raises
         ------
         KeyError
-            If the file does not exist in the database.
+            If the file corresponding to the key does not exist in the database.
         """
         full_path = self.path / key
 
         if not full_path.is_file():
             raise KeyError(f"File '{key}' could not be found in '{self.path}'")
-        with full_path.open("r", encoding="utf-8") as f:
-            return f.read()
+
+        if full_path.suffix in [".png", ".jpeg", ".jpg"]:
+            with full_path.open("rb") as image_file:
+                encoded_string = base64.b64encode(image_file.read()).decode("utf-8")
+                mime_type = "image/png" if full_path.suffix == ".png" else "image/jpeg"
+                return f"data:{mime_type};base64,{encoded_string}"
+        else:
+            with full_path.open("r", encoding="utf-8") as f:
+                return f.read()
 
     def get(self, key: str, default: Optional[Any] = None) -> Any:
         """
-        Get the content of a file in the database, or a default value if the file does not exist.
+        Retrieve the content of a file in the database, or return a default value if not found.
 
         Parameters
         ----------
         key : str
-            The name of the file to get the content of.
-        default : any, optional
-            The default value to return if the file does not exist, by default None.
+            The key (filename) whose content is to be retrieved.
+        default : Any, optional
+            The default value to return if the file does not exist. Default is None.
 
         Returns
         -------
-        any
-            The content of the file, or the default value if the file does not exist.
+        Any
+            The content of the file if it exists, a new DiskMemory instance if the key corresponds to a directory.
         """
+
+        item_path = self.path / key
         try:
-            return self[key]
-        except KeyError:
+            if item_path.is_file():
+                return self[key]
+            elif item_path.is_dir():
+                return DiskMemory(item_path)
+            else:
+                return default
+        except:
             return default
 
     def __setitem__(self, key: Union[str, Path], val: str) -> None:
         """
-        Set the content of a file in the database.
+        Set or update the content of a file in the database corresponding to the given key.
 
         Parameters
         ----------
-        key : Union[str, Path]
-            The name of the file to set the content of.
+        key : str or Path
+            The key (filename) where the content is to be set.
         val : str
-            The content to set.
+            The content to be written to the file.
 
         Raises
         ------
+        ValueError
+            If the key attempts to access a parent path.
         TypeError
-            If val is not string.
+            If the value is not a string.
+
         """
         if str(key).startswith("../"):
             raise ValueError(f"File name {key} attempted to access parent path.")
 
         if not isinstance(val, str):
             raise TypeError("val must be str")
 
         full_path = self.path / key
         full_path.parent.mkdir(parents=True, exist_ok=True)
 
         full_path.write_text(val, encoding="utf-8")
 
     def __delitem__(self, key: Union[str, Path]) -> None:
         """
-        Delete a file or directory in the database.
+        Delete a file or directory from the database corresponding to the given key.
 
         Parameters
         ----------
-        key : Union[str, Path]
-            The name of the file or directory to delete.
+        key : str or Path
+            The key (filename or directory name) to be deleted.
 
         Raises
         ------
         KeyError
-            If the file or directory does not exist in the database.
+            If the file or directory corresponding to the key does not exist in the database.
+
         """
         item_path = self.path / key
         if not item_path.exists():
             raise KeyError(f"Item '{key}' could not be found in '{self.path}'")
 
         if item_path.is_file():
             item_path.unlink()
         elif item_path.is_dir():
             shutil.rmtree(item_path)
 
     def __iter__(self) -> Iterator[str]:
+        """
+        Iterate over the keys (filenames) in the database.
+
+        Yields
+        ------
+        Iterator[str]
+            An iterator over the sorted list of keys (filenames) in the database.
+
+        """
         return iter(
             sorted(
                 str(item.relative_to(self.path))
                 for item in sorted(self.path.rglob("*"))
                 if item.is_file()
             )
         )
 
-    def __len__(self):
+    def __len__(self) -> int:
+        """
+        Get the number of files in the database.
+
+        Returns
+        -------
+        int
+            The number of files in the database.
+
+        """
         return len(list(self.__iter__()))
 
     def _supported_files(self) -> str:
         valid_extensions = {
             ext for lang in SUPPORTED_LANGUAGES for ext in lang["extensions"]
         }
         file_paths = [
@@ -236,19 +238,89 @@
 
     def _all_files(self) -> str:
         file_paths = [str(item) for item in self if Path(item).is_file()]
         return "\n".join(file_paths)
 
     def to_path_list_string(self, supported_code_files_only: bool = False) -> str:
         """
-        Returns directory as a list of file paths. Useful for passing to the LLM where it needs to understand the wider context of files available for reference.
+        Generate a string representation of the file paths in the database.
+
+        Parameters
+        ----------
+        supported_code_files_only : bool, optional
+            If True, filter the list to include only supported code file extensions.
+            Default is False.
+
+        Returns
+        -------
+        str
+            A newline-separated string of file paths.
+
         """
         if supported_code_files_only:
             return self._supported_files()
         else:
             return self._all_files()
 
     def to_dict(self) -> Dict[Union[str, Path], str]:
+        """
+        Convert the database contents to a dictionary.
+
+        Returns
+        -------
+        Dict[Union[str, Path], str]
+            A dictionary with keys as filenames and values as file contents.
+
+        """
         return {file_path: self[file_path] for file_path in self}
 
     def to_json(self) -> str:
+        """
+        Serialize the database contents to a JSON string.
+
+        Returns
+        -------
+        str
+            A JSON string representation of the database contents.
+
+        """
         return json.dumps(self.to_dict())
+
+    def log(self, key: Union[str, Path], val: str) -> None:
+        """
+        Append to a file or create and write to it if it doesn't exist.
+
+        Parameters
+        ----------
+        key : str or Path
+            The key (filename) where the content is to be appended.
+        val : str
+            The content to be appended to the file.
+
+        """
+
+        if str(key).startswith("../"):
+            raise ValueError(f"File name {key} attempted to access parent path.")
+
+        if not isinstance(val, str):
+            raise TypeError("val must be str")
+
+        full_path = self.path / "logs" / key
+        full_path.parent.mkdir(parents=True, exist_ok=True)
+
+        # Touch if it doesnt exist
+        if not full_path.exists():
+            full_path.touch()
+
+        with open(full_path, "a", encoding="utf-8") as file:
+            file.write(f"\n{datetime.now().isoformat()}\n")
+            file.write(val + "\n")
+
+    def archive_logs(self):
+        """
+        Moves all logs to archive directory based on current timestamp
+        """
+        if "logs" in self:
+            archive_dir = (
+                self.path / f"logs_{datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}"
+            )
+            shutil.move(self.path / "logs", archive_dir)
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/core/default/simple_agent.py` & `gpt_engineer-0.2.9/gpt_engineer/core/default/simple_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,51 @@
+"""
+Module for defining a simple agent that uses AI to manage code generation and improvement.
+
+This module provides a class that represents an agent capable of initializing and improving
+a codebase using AI. It handles interactions with the AI model, memory, and execution
+environment to generate and refine code based on user prompts.
+
+"""
+
 import tempfile
 
 from typing import Optional
 
 from gpt_engineer.core.ai import AI
 from gpt_engineer.core.base_agent import BaseAgent
 from gpt_engineer.core.base_execution_env import BaseExecutionEnv
 from gpt_engineer.core.base_memory import BaseMemory
 from gpt_engineer.core.default.disk_execution_env import DiskExecutionEnv
 from gpt_engineer.core.default.disk_memory import DiskMemory
 from gpt_engineer.core.default.paths import PREPROMPTS_PATH, memory_path
-from gpt_engineer.core.default.steps import gen_code, gen_entrypoint, improve
+from gpt_engineer.core.default.steps import gen_code, gen_entrypoint, improve_fn
 from gpt_engineer.core.files_dict import FilesDict
 from gpt_engineer.core.preprompts_holder import PrepromptsHolder
+from gpt_engineer.core.prompt import Prompt
 
 
 class SimpleAgent(BaseAgent):
     """
     An agent that uses AI to generate and improve code based on a given prompt.
 
     This agent is capable of initializing a codebase from a prompt and improving an existing
     codebase based on user input. It uses an AI model to generate and refine code, and it
     interacts with a repository and an execution environment to manage and execute the code.
 
-    Attributes:
-        memory (BaseRepository): The repository where the code and related data are stored.
-        execution_env (BaseExecutionEnv): The environment in which the code is executed.
-        ai (AI): The AI model used for generating and improving code.
+    Attributes
+    ----------
+    memory : BaseMemory
+        The memory interface where the code and related data are stored.
+    execution_env : BaseExecutionEnv
+        The execution environment in which the code is executed.
+    ai : AI
+        The AI model used for generating and improving code.
+    preprompts_holder : PrepromptsHolder
+        The holder for preprompt messages that guide the AI model.
     """
 
     def __init__(
         self,
         memory: BaseMemory,
         execution_env: BaseExecutionEnv,
         ai: AI = None,
@@ -47,30 +63,38 @@
         return cls(
             memory=DiskMemory(memory_path(path)),
             execution_env=DiskExecutionEnv(),
             ai=ai,
             preprompts_holder=preprompts_holder or PrepromptsHolder(PREPROMPTS_PATH),
         )
 
-    def init(self, prompt: str) -> FilesDict:
+    def init(self, prompt: Prompt) -> FilesDict:
         files_dict = gen_code(self.ai, prompt, self.memory, self.preprompts_holder)
         entrypoint = gen_entrypoint(
-            self.ai, files_dict, self.memory, self.preprompts_holder
+            self.ai, prompt, files_dict, self.memory, self.preprompts_holder
         )
         combined_dict = {**files_dict, **entrypoint}
         files_dict = FilesDict(combined_dict)
         return files_dict
 
     def improve(
         self,
         files_dict: FilesDict,
-        prompt: str,
+        prompt: Prompt,
         execution_command: Optional[str] = None,
     ) -> FilesDict:
-        files_dict = improve(
+        files_dict = improve_fn(
             self.ai, prompt, files_dict, self.memory, self.preprompts_holder
         )
         return files_dict
 
 
 def default_config_agent():
+    """
+    Creates an instance of SimpleAgent with default configuration.
+
+    Returns
+    -------
+    SimpleAgent
+        An instance of SimpleAgent with a temporary directory as its base path.
+    """
     return SimpleAgent.with_default_config(tempfile.mkdtemp())
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/preprompts/generate` & `gpt_engineer-0.2.9/gpt_engineer/preprompts/generate`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/preprompts/philosophy` & `gpt_engineer-0.2.9/gpt_engineer/preprompts/philosophy`

 * *Files identical despite different names*

### Comparing `gpt_engineer-0.2.8/gpt_engineer/tools/custom_steps.py` & `gpt_engineer-0.2.9/gpt_engineer/tools/custom_steps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,82 @@
 from platform import platform
 from sys import version_info
 from typing import List, Union
 
 from langchain.schema import AIMessage, HumanMessage, SystemMessage
-from termcolor import colored
 
 from gpt_engineer.core.ai import AI
 from gpt_engineer.core.base_execution_env import BaseExecutionEnv
 from gpt_engineer.core.base_memory import BaseMemory
 from gpt_engineer.core.chat_to_files import chat_to_files_dict
 from gpt_engineer.core.default.paths import CODE_GEN_LOG_FILE, ENTRYPOINT_FILE
-from gpt_engineer.core.default.steps import curr_fn, setup_sys_prompt
+from gpt_engineer.core.default.steps import curr_fn, improve_fn, setup_sys_prompt
 from gpt_engineer.core.files_dict import FilesDict
 from gpt_engineer.core.preprompts_holder import PrepromptsHolder
+from gpt_engineer.core.prompt import Prompt
 
 # Type hint for chat messages
 Message = Union[AIMessage, HumanMessage, SystemMessage]
-MAX_SELF_HEAL_ATTEMPTS = 2
+MAX_SELF_HEAL_ATTEMPTS = 10
 
 
-def get_platform_info():
-    """Returns the Platform: OS, and the Python version.
-    This is used for self healing.  There are some possible areas of conflict here if
-    you use a different version of Python in your virtualenv.  A better solution would
-    be to have this info printed from the virtualenv.
+def get_platform_info() -> str:
     """
+    Returns a string containing the OS and Python version information.
+
+    This function is used for self-healing by providing information about the current
+    operating system and Python version. It assumes that the Python version in the
+    virtual environment is the one being used.
+
+    Returns:
+        str: A string containing the OS and Python version information.
+    """
+
     v = version_info
     a = f"Python Version: {v.major}.{v.minor}.{v.micro}"
     b = f"\nOS: {platform()}\n"
     return a + b
 
 
 def self_heal(
     ai: AI,
     execution_env: BaseExecutionEnv,
     files_dict: FilesDict,
+    prompt: Prompt = None,
     preprompts_holder: PrepromptsHolder = None,
+    memory: BaseMemory = None,
 ) -> FilesDict:
-    """Attempts to execute the code from the entrypoint and if it fails,
-    sends the error output back to the AI with instructions to fix.
+    """
+    Attempts to execute the code from the entrypoint and if it fails, sends the error output back to the AI with instructions to fix.
+
+    Parameters
+    ----------
+    ai : AI
+        An instance of the AI model.
+    execution_env : BaseExecutionEnv
+        The execution environment where the code is run.
+    files_dict : FilesDict
+        A dictionary of file names to their contents.
+    preprompts_holder : PrepromptsHolder, optional
+        A holder for preprompt messages.
+
+    Returns
+    -------
+    FilesDict
+        The updated files dictionary after self-healing attempts.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the required entrypoint file does not exist in the code.
+    AssertionError
+        If the preprompts_holder is None.
+
+    Notes
+    -----
     This code will make `MAX_SELF_HEAL_ATTEMPTS` to try and fix the code
     before giving up.
     This makes the assuption that the previous step was `gen_entrypoint`,
     this code could work with `simple_gen`, or `gen_clarified_code` as well.
     """
 
     # step 1. execute the entrypoint
@@ -51,85 +85,69 @@
         raise FileNotFoundError(
             "The required entrypoint "
             + ENTRYPOINT_FILE
             + " does not exist in the code."
         )
 
     attempts = 0
-    messages = []
     if preprompts_holder is None:
         raise AssertionError("Prepromptsholder required for self-heal")
-    preprompts = preprompts_holder.get_preprompts()
     while attempts < MAX_SELF_HEAL_ATTEMPTS:
-        command = files_dict[ENTRYPOINT_FILE]
-        print(
-            colored(
-                "Do you want to execute this code? (Y/n)",
-                "red",
-            )
-        )
-        print()
-        print(command)
-        print()
-        if input("").lower() not in ["", "y", "yes"]:
-            print("Ok, not executing the code.")
-            return files_dict
-        print("Executing the code...")
-        stdout_full, stderr_full, returncode = execution_env.upload(files_dict).run(
-            f"bash {ENTRYPOINT_FILE}"
-        )
-        # get the result and output
-        # step 2. if the return code not 0, package and send to the AI
-        if returncode != 0:
-            print("run.sh failed.  Let's fix it.")
-
-            # pack results in an AI prompt
-
-            # Using the log from the previous step has all the code and
-            # the gen_entrypoint prompt inside.
-            if attempts < 1:
-                messages: List[Message] = [SystemMessage(content=files_dict.to_chat())]
-                messages.append(SystemMessage(content=get_platform_info()))
+        attempts += 1
+        timed_out = False
 
-            messages.append(SystemMessage(content=stdout_full + "\n " + stderr_full))
+        # Start the process
+        execution_env.upload(files_dict)
+        p = execution_env.popen(files_dict[ENTRYPOINT_FILE])
+
+        # Wait for the process to complete and get output
+        stdout_full, stderr_full = p.communicate()
+
+        if (p.returncode != 0 and p.returncode != 2) and not timed_out:
+            print("run.sh failed.  The log is:")
+            print(stdout_full.decode("utf-8"))
+            print(stderr_full.decode("utf-8"))
 
-            messages = ai.next(
-                messages, preprompts["file_format_fix"], step_name=curr_fn()
+            new_prompt = Prompt(
+                f"A program with this specification was requested:\n{prompt}\n, but running it produced the following output:\n{stdout_full}\n and the following errors:\n{stderr_full}. Please change it so that it fulfills the requirements."
             )
-        else:  # the process did not fail, we are done here.
-            return files_dict
-
-        files_dict = {**files_dict, **chat_to_files_dict(messages[-1].content.strip())}
-        attempts += 1
-
+            files_dict = improve_fn(
+                ai, new_prompt, files_dict, memory, preprompts_holder
+            )
+        else:
+            break
     return files_dict
 
 
 def clarified_gen(
-    ai: AI, prompt: str, memory: BaseMemory, preprompts_holder: PrepromptsHolder
+    ai: AI, prompt: Prompt, memory: BaseMemory, preprompts_holder: PrepromptsHolder
 ) -> FilesDict:
     """
-    Generates code based on clarifications obtained from the user.
+    Generates code based on clarifications obtained from the user and saves it to a specified workspace.
 
-    This function processes the messages logged during the user's clarification session
-    and uses them, along with the system's prompts, to guide the AI in generating code.
-    The generated code is saved to a specified workspace.
-
-    Parameters:
-    - ai (AI): An instance of the AI model, responsible for processing and generating the code.
-    - dbs (DBs): An instance containing the database configurations, which includes system
-      and input prompts.
-
-    Returns:
-    - List[dict]: A list of message dictionaries capturing the AI's interactions and generated
-      outputs during the code generation process.
+    Parameters
+    ----------
+    ai : AI
+        An instance of the AI model, responsible for processing and generating the code.
+    prompt : str
+        The user's clarification prompt.
+    memory : BaseMemory
+        The memory instance where the generated code log is saved.
+    preprompts_holder : PrepromptsHolder
+        A holder for preprompt messages.
+
+    Returns
+    -------
+    FilesDict
+        A dictionary of file names to their contents generated by the AI.
     """
+
     preprompts = preprompts_holder.get_preprompts()
     messages: List[Message] = [SystemMessage(content=preprompts["clarify"])]
-    user_input = prompt
+    user_input = prompt.text  # clarify does not work with vision right now
     while True:
         messages = ai.next(messages, user_input, step_name=curr_fn())
         msg = messages[-1].content.strip()
 
         if "nothing to clarify" in msg.lower():
             break
 
@@ -167,41 +185,48 @@
     messages = ai.next(
         messages,
         preprompts["generate"].replace("FILE_FORMAT", preprompts["file_format"]),
         step_name=curr_fn(),
     )
     print()
     chat = messages[-1].content.strip()
-    memory[CODE_GEN_LOG_FILE] = chat
+    memory.log(CODE_GEN_LOG_FILE, "\n\n".join(x.pretty_repr() for x in messages))
     files_dict = chat_to_files_dict(chat)
     return files_dict
 
 
 def lite_gen(
-    ai: AI, prompt: str, memory: BaseMemory, preprompts_holder: PrepromptsHolder
+    ai: AI, prompt: Prompt, memory: BaseMemory, preprompts_holder: PrepromptsHolder
 ) -> FilesDict:
     """
-    Executes the AI model using the main prompt and saves the generated results.
+    Executes the AI model using the main prompt and saves the generated results to the specified workspace.
 
-    This function invokes the AI model by feeding it the main prompt. After the
-    AI processes and generates the output, the function saves this output to the
-    specified workspace. The AI's output is also tracked using the current function's
-    name to provide context.
-
-    Parameters:
-    - ai (AI): An instance of the AI model.
-    - dbs (DBs): An instance containing the database configurations, including input prompts
-      and file formatting preferences.
+    Parameters
+    ----------
+    ai : AI
+        An instance of the AI model.
+    prompt : str
+        The main prompt to feed to the AI model.
+    memory : BaseMemory
+        The memory instance where the generated code log is saved.
+    preprompts_holder : PrepromptsHolder
+        A holder for preprompt messages.
+
+    Returns
+    -------
+    FilesDict
+        A dictionary of file names to their contents generated by the AI.
 
-    Returns:
-    - List[Message]: A list of message objects encapsulating the AI's output.
-
-    Note:
+    Notes
+    -----
     The function assumes the `ai.start` method and the `to_files` utility to be correctly
     set up and functional. Ensure these prerequisites before invoking `lite_gen`.
     """
+
     preprompts = preprompts_holder.get_preprompts()
-    messages = ai.start(prompt, preprompts["file_format"], step_name=curr_fn())
+    messages = ai.start(
+        prompt.to_langchain_content(), preprompts["file_format"], step_name=curr_fn()
+    )
     chat = messages[-1].content.strip()
-    memory[CODE_GEN_LOG_FILE] = chat
+    memory.log(CODE_GEN_LOG_FILE, "\n\n".join(x.pretty_repr() for x in messages))
     files_dict = chat_to_files_dict(chat)
     return files_dict
```

### Comparing `gpt_engineer-0.2.8/gpt_engineer/tools/supported_languages.py` & `gpt_engineer-0.2.9/gpt_engineer/tools/supported_languages.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+This module defines the supported programming languages for document chunking.
+
+Variables:
+    SUPPORTED_LANGUAGES (list): A list of dictionaries defining supported languages.
+"""
+
 SUPPORTED_LANGUAGES = [
     {"name": "Python", "extensions": [".py"], "tree_sitter_name": "python"},
     {
         "name": "JavaScript",
         "extensions": [".js", ".mjs"],
         "tree_sitter_name": "javascript",
     },
```

### Comparing `gpt_engineer-0.2.8/pyproject.toml` & `gpt_engineer-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-engineer"
-version = "0.2.8"
+version = "0.2.9"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 authors = ["Anton Osika <anton.osika@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/gpt-engineer-org/gpt-engineer"
 repository = "https://github.com/gpt-engineer-org/gpt-engineer"
 documentation = "https://gpt-engineer.readthedocs.io/en/latest/"
@@ -26,25 +26,31 @@
 dataclasses-json = "0.5.7"
 tiktoken = ">=0.0.4"
 tabulate = "0.9.0"
 python-dotenv = ">=0.21.0"
 langchain = "^0.1"
 langchain_openai = "*"
 toml = ">=0.10.2"
+tomlkit = "^0.12.4"
+pyperclip = "^1.8.2"
+langchain-anthropic = "^0.1.1"
+regex = "^2023.12.25"
+pillow = "^10.2.0"
+datasets = "^2.17.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.1"
 pytest-cov = "^4.1.0"
 black = "23.3.0"
 mypy = "1.3.0"
 ruff = ">=0.0.272"
 pre-commit = "3.3.3"
 tox = ">=3.0.0"
 
-# docs
+[tool.poetry.group.docs.dependencies]
 autodoc_pydantic = ">=1.8.0"
 myst_parser = ">=0.18.1"
 nbsphinx = ">=0.8.9"
 sphinx = ">=5.0.0"
 sphinx-autobuild = ">=2021.3.14"
 sphinx_book_theme = ">=0.3.3"
 sphinx_rtd_theme = ">=1.0.0"
```

### Comparing `gpt_engineer-0.2.8/PKG-INFO` & `gpt_engineer-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.2.8
+Version: 0.2.9
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Home-page: https://github.com/gpt-engineer-org/gpt-engineer
 License: MIT
 Author: Anton Osika
 Author-email: anton.osika@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -13,23 +13,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: doc
 Provides-Extra: test
 Requires-Dist: dataclasses-json (==0.5.7)
+Requires-Dist: datasets (>=2.17.1,<3.0.0)
 Requires-Dist: langchain (>=0.1,<0.2)
+Requires-Dist: langchain-anthropic (>=0.1.1,<0.2.0)
 Requires-Dist: langchain_openai
 Requires-Dist: openai (>=1.0,<2.0)
+Requires-Dist: pillow (>=10.2.0,<11.0.0)
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.0)
+Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Requires-Dist: rudder-sdk-python (>=2.0.2)
 Requires-Dist: tabulate (==0.9.0)
 Requires-Dist: termcolor (==2.3.0)
 Requires-Dist: tiktoken (>=0.0.4)
 Requires-Dist: toml (>=0.10.2)
+Requires-Dist: tomlkit (>=0.12.4,<0.13.0)
 Requires-Dist: typer (>=0.3.2)
 Project-URL: Documentation, https://gpt-engineer.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gpt-engineer-org/gpt-engineer
 Description-Content-Type: text/markdown
 
 # GPT-Engineer
 
@@ -82,32 +88,43 @@
 - Run `gpte <project_dir>` with a relative path to your folder
   - For example: `gpte projects/my-new-project` from the gpt-engineer directory root with your new folder in `projects/`
 
 ### Improve Existing Code
 - Locate a folder with code which you want to improve anywhere on your computer
 - Create a file called `prompt` (no extension) inside your new folder and fill it with instructions for how you want to improve the code
 - Run `gpte <project_dir> -i` with a relative path to your folder
-  - For example: `gpte projects/my-old-project` from the gpt-engineer directory root with your folder in `projects/`
+  - For example: `gpte projects/my-old-project -i` from the gpt-engineer directory root with your folder in `projects/`
 
 By running gpt-engineer you agree to our [terms](https://github.com/gpt-engineer-org/gpt-engineer/blob/main/TERMS_OF_USE.md).
 
 
 ## Relation to gptengineer.app
 [gptengineer.app](https://gptengineer.app/) is a commercial project for automatic generation of web-apps.
 It features a UI for non-technical users, connected to a git controlled codebase.
 The gptengineer.app team is actively supporting the open source community.
 
 
 ## Features
 
+### Pre Prompts
 You can specify the "identity" of the AI agent by overriding the `preprompts` folder, with your own version of the `preprompts`, using the `--use-custom-preprompts` argument.
 
 Editing the `preprompts` is how you make the agent remember things between projects.
 
-You can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
+### Vision
+
+By default, GPT Engineer expects text input via a `prompt` file. It can also accept imagine inputs for vision capable models. This can be useful for adding UX or architecture diagrams as additional context for GPT Engineer. You can do this by specifiying an image directory with the --image_directory flag and setting a vision capable model in the second cli argument.
+
+E.g. `gpte projects/example-vision gpt-4-vision-preview --prompt_file prompt/text --image_directory prompt/images -i`
+
+### Open source, local and alternative models
+
+By defaul GPT Engineer supports OpenAI Models via the OpenAI API or Azure Open AI API, and Anthropic models.
+
+With a little extra set up you can also run with open source models, like WizardCoder. See the [documentation](https://gpt-engineer.readthedocs.io/en/latest/open_models.html) for example instructions.
 
 ## Mission
 
 The gpt-engineer community mission is to **maintain tools that coding agent builders can use and facilitate collaboration in the open source community**.
 
 If you are interested in contributing to this, we are interested in having you.
```

