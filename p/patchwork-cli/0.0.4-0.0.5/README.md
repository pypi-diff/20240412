# Comparing `tmp/patchwork_cli-0.0.4.tar.gz` & `tmp/patchwork_cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.4.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.5.tar", max compression
```

## Comparing `patchwork_cli-0.0.4.tar` & `patchwork_cli-0.0.5.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0    34523 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0     5239 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/__main__.py
--rw-r--r--   0        0        0     2849 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    12408 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/client/scm.py
--rw-r--r--   0        0        0      816 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/common/utils.py
--rw-r--r--   0        0        0     1546 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/managed_files.py
--rw-r--r--   0        0        0     2775 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     4783 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/README.md
--rw-r--r--   0        0        0     2182 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      809 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5434 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0     5418 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/README.md
--rw-r--r--   0        0        0      704 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2495 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2210 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0     3832 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/README.md
--rw-r--r--   0        0        0      612 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3551 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0     3631 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      608 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/README.md
--rw-r--r--   0        0        0      276 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/step.py
--rw-r--r--   0        0        0     5970 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0     2437 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/CallOpenAI.py
--rw-r--r--   0        0        0      503 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CallOpenAI/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0     1358 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0     8811 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-04-09 08:55:30.591286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0     8880 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0     1648 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0    12392 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0     3344 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0     3182 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0     1652 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/README.md
--rw-r--r--   0        0        0      903 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1387 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4744 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0     2026 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/TestScanDepscan.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      677 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1055 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0     1481 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     2101 2024-04-09 08:55:30.595286 patchwork_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6918 1970-01-01 00:00:00.000000 patchwork_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5534 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/__main__.py
+-rw-r--r--   0        0        0     3036 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    12704 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0      816 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1546 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/managed_files.py
+-rw-r--r--   0        0        0     2775 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     4783 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      809 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5434 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5418 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      704 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2210 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3832 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      612 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3551 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3631 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0      276 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/step.py
+-rw-r--r--   0        0        0     5970 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0     2437 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0     3853 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/CallOpenAI.py
+-rw-r--r--   0        0        0      503 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0     8519 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0     8880 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0     1648 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0    12392 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0     3366 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0     3182 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0     1652 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/README.md
+-rw-r--r--   0        0        0      903 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1764 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4744 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0     2026 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/TestScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1055 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2101 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 patchwork_cli-0.0.5/PKG-INFO
```

### Comparing `patchwork_cli-0.0.4/LICENSE` & `patchwork_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/README.md` & `patchwork_cli-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
 You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
 
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+
+```bash
+patchwork AutoFix --config /path/to/patchwork-configs/patchflows
+```
+
 ## PatchWork in CI
 
 You can also run PatchWork in a CI environment with ease:
 
 ### Jenkins CI
 
 ```groovy
```

### Comparing `patchwork_cli-0.0.4/patchwork/app.py` & `patchwork_cli-0.0.5/patchwork/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import importlib
 import json
+import traceback
 from pathlib import Path
 
 import click
 import yaml
 
 from patchwork.logger import init_cli_logger, logger
 
@@ -69,17 +70,21 @@
 
         if equal_sign == "":
             # treat --key as a flag
             inputs[key] = True
         else:
             # treat --key=value as a key-value pair
             inputs[key] = value
-
-    patchflow_instance = patchflow_class(inputs)
-    patchflow_instance.run()
+    try:
+        patchflow_instance = patchflow_class(inputs)
+        patchflow_instance.run()
+    except Exception as e:
+        logger.debug(traceback.format_exc())
+        logger.error(f"Error running patchflow {patchflow}: {e}")
+        exit(1)
 
     data_format_mapping = {
         "yaml": yaml.dump,
         "json": json.dumps,
     }
 
     if output is not None:
```

### Comparing `patchwork_cli-0.0.4/patchwork/common/client/scm.py` & `patchwork_cli-0.0.5/patchwork/common/client/scm.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,16 +133,21 @@
         return self._mr.web_url
 
     def set_pr_description(self, body: str) -> None:
         self._mr.description = PullRequestProtocol._apply_pr_template(self, body)
         self._mr.save()
 
     def create_comment(
-        self, path: str, body: str, start_line: int | None = None, end_line: int | None = None
+        self, body: str, path: str | None = None, start_line: int | None = None, end_line: int | None = None
     ) -> str | None:
+        final_body = f"{_COMMENT_MARKER} \n{PullRequestProtocol._apply_pr_template(self, body)}"
+        if path is None:
+            note = self._mr.notes.create({"body": final_body})
+            return f"#note_{note.get_id()}"
+
         while True:
             try:
                 commit = self._mr.commits().next()
             except StopIteration:
                 continue
 
             break
@@ -157,15 +162,14 @@
             if diff.head_commit_sha == commit.get_id():
                 break
 
         base_commit = diff.base_commit_sha
         head_commit = diff.head_commit_sha
 
         try:
-            final_body = f"{_COMMENT_MARKER} \n{PullRequestProtocol._apply_pr_template(self, body)}"
             discussion = self._mr.discussions.create(
                 {
                     "body": final_body,
                     "position": {
                         "base_sha": base_commit,
                         "start_sha": base_commit,
                         "head_sha": head_commit,
@@ -183,22 +187,27 @@
 
         for note in discussion.attributes["notes"]:
             return f"#note_{note['id']}"
 
         return None
 
     def reset_comments(self) -> None:
-        for discussion in self._mr.discussions.list():
+        for discussion in self._mr.discussions.list(iterator=True):
             for note in discussion.attributes["notes"]:
-                if note["type"] == "DiffNote" and note["body"].startswith(_COMMENT_MARKER):
+                if note["body"].startswith(_COMMENT_MARKER):
                     discussion.notes.delete(note["id"])
 
     def file_diffs(self) -> dict[str, str]:
-        files = self._mr.diffs.list()
-        return {file.attributes["new_path"]: file.attributes["diff"] for file in files}
+        diffs = self._mr.diffs.list()
+        latest_diff = max(diffs, key=lambda diff: diff.created_at, default=None)
+        if latest_diff is None:
+            return {}
+
+        files = self._mr.diffs.get(latest_diff.id).diffs
+        return {file["new_path"]: file["diff"] for file in files}
 
 
 class GithubPullRequest(PullRequestProtocol):
     def __init__(self, pr: PullRequest):
         self._pr = pr
 
     def url(self) -> str:
@@ -332,15 +341,15 @@
 
         try:
             pr_id = url_parts[-1]
         except ValueError:
             logger.error(f"Invalid PR URL: {url}")
             return None
 
-        slug = "/".join(url_parts[-4:-2])
+        slug = "/".join(url_parts[-5:-3])
 
         return self.find_pr_by_id(slug, int(pr_id))
 
     def find_pr_by_id(self, slug: str, pr_id: int) -> PullRequestProtocol | None:
         project = self.gitlab.projects.get(slug)
         try:
             mr = project.mergerequests.get(pr_id)
```

### Comparing `patchwork_cli-0.0.4/patchwork/common/utils.py` & `patchwork_cli-0.0.5/patchwork/common/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/logger.py` & `patchwork_cli-0.0.5/patchwork/logger.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/README.md` & `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/README.md` & `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/README.md` & `patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/PRReview.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/README.md` & `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/patchflows/README.md` & `patchwork_cli-0.0.5/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.5/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.5/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.5/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.5/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,84 @@
     uri = artifact_location.get("uri")
     if uri is not None:
         return parse_sarif_location(base_path, uri)
 
     return None
 
 
+def transform_sarif_results(
+    sarif_data: dict, base_path: Path, context_length: int, vulnerability_limit: int
+) -> dict[tuple[str, int, int, int], list[str]]:
+    # Process each result in SARIF data
+    grouped_messages = defaultdict(list)
+    vulnerability_count = 0
+    for run_idx, run in enumerate(sarif_data.get("runs", [])):
+        artifact_locations = [
+            parse_sarif_location(base_path, artifact["location"]["uri"]) for artifact in run.get("artifacts", [])
+        ]
+
+        for result_idx, result in enumerate(run.get("results", [])):
+            for location_idx, location in enumerate(result.get("locations", [])):
+                physical_location = location.get("physicalLocation", {})
+
+                artifact_location = physical_location.get("artifactLocation", {})
+                uri = resolve_artifact_location(base_path, artifact_location, artifact_locations)
+                if uri is None:
+                    logger.warn(
+                        f'Unable to find file for ".runs[{run_idx}].results[{result_idx}].locations[{location_idx}]"'
+                    )
+                    continue
+
+                region = physical_location.get("region", {})
+                start_line = region.get("startLine", 1)
+                end_line = region.get("endLine", start_line)
+                start_line = start_line - 1
+
+                # Generate file path assuming code is in the current working directory
+                file_path = str(uri.relative_to(base_path))
+
+                # Extract lines from the code file
+                logger.info(f"Extracting context for {file_path} at {start_line}:{end_line}")
+                try:
+                    with open_with_chardet(file_path, "r") as file:
+                        src = file.read()
+
+                    source_lines = src.splitlines(keepends=True)
+                    context_start, context_end = get_source_code_context(
+                        file_path, source_lines, start_line, end_line, context_length
+                    )
+
+                    source_code_context = None
+                    if context_start is not None and context_end is not None:
+                        source_code_context = "".join(source_lines[context_start:context_end])
+
+                except FileNotFoundError:
+                    context_start = None
+                    context_end = None
+                    source_code_context = None
+                    logger.info(f"File not found in the current working directory: {file_path}")
+
+                if source_code_context is None:
+                    logger.info(f"No context found for {file_path} at {start_line}:{end_line}")
+                    continue
+
+                start = context_start if context_start is not None else start_line
+                end = context_end if context_end is not None else end_line
+
+                grouped_messages[(uri, start, end, source_code_context)].append(
+                    result.get("message", {}).get("text", "")
+                )
+
+                vulnerability_count = vulnerability_count + 1
+                if 0 < vulnerability_limit <= vulnerability_count:
+                    return grouped_messages
+
+    return grouped_messages
+
+
 class ExtractCode(Step):
     required_keys = {"sarif_file_path"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
@@ -108,95 +178,25 @@
             raise ValueError(f'SARIF file path does not exist or is not a file: "{self.sarif_file_path}"')
 
         # Check and set number of lines to extract
         self.context_length = inputs.get("context_size", 1000)
         self.vulnerability_limit = inputs.get("vulnerability_limit", 10)
 
         # Prepare for data extraction
-        self.extracted_data = []
         self.extracted_code_contexts = []
 
     def run(self) -> dict:
         # Load SARIF data
         with open_with_chardet(self.sarif_file_path, "r") as file:
             sarif_data = json.load(file)
 
         vulnerability_count = 0
         base_path = Path.cwd()
-        # Process each result in SARIF data
-        grouped_messages = defaultdict(list)
-        for run_idx, run in enumerate(sarif_data.get("runs", [])):
-            artifact_locations = [
-                parse_sarif_location(base_path, artifact["location"]["uri"]) for artifact in run.get("artifacts", [])
-            ]
-
-            for result_idx, result in enumerate(run.get("results", [])):
-                for location_idx, location in enumerate(result.get("locations", [])):
-                    physical_location = location.get("physicalLocation", {})
-
-                    artifact_location = physical_location.get("artifactLocation", {})
-                    uri = resolve_artifact_location(base_path, artifact_location, artifact_locations)
-                    if uri is None:
-                        logger.warn(
-                            f'Unable to find file for ".runs[{run_idx}].results[{result_idx}].locations[{location_idx}]"'
-                        )
-                        continue
-
-                    region = physical_location.get("region", {})
-                    start_line = region.get("startLine", 1)
-                    end_line = region.get("endLine", start_line)
-                    start_line = start_line - 1
-
-                    # Generate file path assuming code is in the current working directory
-                    file_path = str(uri.relative_to(base_path))
-
-                    # Extract lines from the code file
-                    logger.info(f"Extracting context for {file_path} at {start_line}:{end_line}")
-                    try:
-                        with open_with_chardet(file_path, "r") as file:
-                            src = file.read()
-
-                        source_lines = src.splitlines(keepends=True)
-                        context_start, context_end = get_source_code_context(
-                            file_path, source_lines, start_line, end_line, self.context_length
-                        )
-
-                        source_code_context = None
-                        if context_start is not None and context_end is not None:
-                            source_code_context = "".join(source_lines[context_start:context_end])
-
-                    except FileNotFoundError:
-                        context_start = None
-                        context_end = None
-                        source_code_context = None
-                        logger.info(f"File not found in the current working directory: {file_path}")
-
-                    if source_code_context is None:
-                        logger.info(f"No context found for {file_path} at {start_line}:{end_line}")
-                        continue
-
-                    start = context_start if context_start is not None else start_line
-                    end = context_end if context_end is not None else end_line
-                    self.extracted_data.append(
-                        {
-                            "affectedCode": source_code_context,
-                            "startLine": start,
-                            "endLine": end,
-                            "uri": file_path,
-                            "messageText": result.get("message", {}).get("text", ""),
-                        }
-                    )
-
-                    grouped_messages[(uri, start, end, source_code_context)].append(
-                        result.get("message", {}).get("text", "")
-                    )
 
-                    vulnerability_count = vulnerability_count + 1
-                    if 0 < self.vulnerability_limit <= vulnerability_count:
-                        break
+        grouped_messages = transform_sarif_results(sarif_data, base_path, self.context_length, self.vulnerability_limit)
 
         self.extracted_code_contexts = [
             {
                 "uri": str(file_path),
                 "startLine": start,
                 "endLine": end,
                 "affectedCode": context,
```

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.5/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,17 @@
         self.code_snippets_path = inputs[CODE_SNIPPETS_KEY]
         self.extracted_responses = inputs[UPDATED_SNIPPETS_KEY]
 
     def run(self) -> dict:
         code_snippets = load_json_file(self.code_snippets_path)
 
         modified_code_files = []
-        sorted_list = sorted(zip(code_snippets, self.extracted_responses), key=lambda x: x[0]["startLine"], reverse=True)
+        sorted_list = sorted(
+            zip(code_snippets, self.extracted_responses), key=lambda x: x[0]["startLine"], reverse=True
+        )
         for code_snippet, extracted_response in sorted_list:
             uri = code_snippet["uri"]
             start_line = code_snippet["startLine"]
             end_line = code_snippet["endLine"]
             new_code = extracted_response.get("patch")
             if new_code is None:
                 continue
```

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.5/patchwork/steps/PreparePR/PreparePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.5/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/README.md` & `patchwork_cli-0.0.5/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ScanDepscan/TestScanDepscan.py` & `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/TestScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/patchwork/steps/__init__.py` & `patchwork_cli-0.0.5/patchwork/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.4/pyproject.toml` & `patchwork_cli-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["patched.code"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
```

### Comparing `patchwork_cli-0.0.4/PKG-INFO` & `patchwork_cli-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 License: AGPL
 Author: patched.code
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -112,14 +112,20 @@
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
 You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
 
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+
+```bash
+patchwork AutoFix --config /path/to/patchwork-configs/patchflows
+```
+
 ## PatchWork in CI
 
 You can also run PatchWork in a CI environment with ease:
 
 ### Jenkins CI
 
 ```groovy
```

