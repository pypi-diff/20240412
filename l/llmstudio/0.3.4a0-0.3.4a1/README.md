# Comparing `tmp/llmstudio-0.3.4a0.tar.gz` & `tmp/llmstudio-0.3.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmstudio-0.3.4a0.tar", max compression
+gzip compressed data, was "llmstudio-0.3.4a1.tar", max compression
```

## Comparing `llmstudio-0.3.4a0.tar` & `llmstudio-0.3.4a1.tar`

### file list

```diff
@@ -1,180 +1,137 @@
--rw-r--r--   0        0        0    16725 2023-10-25 19:12:01.905719 llmstudio-0.3.4a0/LICENSE
--rw-r--r--   0        0        0     4185 2024-03-12 16:29:10.044197 llmstudio-0.3.4a0/README.md
--rw-r--r--   0        0        0       30 2024-03-12 16:29:03.304965 llmstudio-0.3.4a0/llmstudio/__init__.py
--rw-r--r--   0        0        0     2509 2024-03-26 15:51:14.043712 llmstudio-0.3.4a0/llmstudio/cli.py
--rw-r--r--   0        0        0       56 2023-10-25 19:12:01.912932 llmstudio-0.3.4a0/llmstudio/client.py
--rw-r--r--   0        0        0     1573 2024-04-09 10:18:39.968791 llmstudio-0.3.4a0/llmstudio/config.py
--rw-r--r--   0        0        0     6177 2024-03-26 15:00:35.441651 llmstudio-0.3.4a0/llmstudio/engine/__init__.py
--rw-r--r--   0        0        0     5623 2024-03-12 16:29:03.306116 llmstudio-0.3.4a0/llmstudio/engine/config.yaml
--rw-r--r--   0        0        0      314 2024-03-12 16:29:03.306426 llmstudio-0.3.4a0/llmstudio/engine/providers/__init__.py
--rw-r--r--   0        0        0     3434 2024-03-12 16:29:03.306712 llmstudio-0.3.4a0/llmstudio/engine/providers/anthropic.py
--rw-r--r--   0        0        0     2569 2024-03-12 16:29:03.306982 llmstudio-0.3.4a0/llmstudio/engine/providers/azure.py
--rw-r--r--   0        0        0     3227 2024-03-12 16:29:03.307231 llmstudio-0.3.4a0/llmstudio/engine/providers/ollama.py
--rw-r--r--   0        0        0     2194 2024-03-12 16:29:03.307463 llmstudio-0.3.4a0/llmstudio/engine/providers/openai.py
--rw-r--r--   0        0        0    13776 2024-03-27 10:53:38.433785 llmstudio-0.3.4a0/llmstudio/engine/providers/provider.py
--rw-r--r--   0        0        0     3844 2024-03-27 11:26:19.885989 llmstudio-0.3.4a0/llmstudio/llm/__init__.py
--rw-r--r--   0        0        0     2114 2024-03-12 16:29:03.308235 llmstudio-0.3.4a0/llmstudio/llm/langchain.py
--rw-r--r--   0        0        0        0 2024-03-12 16:29:03.308290 llmstudio-0.3.4a0/llmstudio/tests/__init__.py
--rw-r--r--   0        0        0     1165 2024-03-12 16:29:03.308665 llmstudio-0.3.4a0/llmstudio/tests/conftest.py
--rw-r--r--   0        0        0     3007 2024-03-12 16:29:10.045037 llmstudio-0.3.4a0/llmstudio/tests/engine/test_engine.py
--rw-r--r--   0        0        0     3926 2024-03-12 16:29:03.309224 llmstudio-0.3.4a0/llmstudio/tests/engine/test_providers.py
--rw-r--r--   0        0        0     1800 2024-04-09 10:18:39.969173 llmstudio-0.3.4a0/llmstudio/tracking/__init__.py
--rw-r--r--   0        0        0      575 2024-04-09 10:18:39.969455 llmstudio-0.3.4a0/llmstudio/tracking/database.py
--rw-r--r--   0        0        0        0 2024-04-09 10:18:39.969555 llmstudio-0.3.4a0/llmstudio/tracking/logs/__init__.py
--rw-r--r--   0        0        0      797 2024-04-09 10:18:39.969770 llmstudio-0.3.4a0/llmstudio/tracking/logs/crud.py
--rw-r--r--   0        0        0     1513 2024-04-09 10:18:39.969920 llmstudio-0.3.4a0/llmstudio/tracking/logs/endpoints.py
--rw-r--r--   0        0        0      578 2024-04-09 10:18:39.970063 llmstudio-0.3.4a0/llmstudio/tracking/logs/models.py
--rw-r--r--   0        0        0      834 2024-04-09 10:18:39.970159 llmstudio-0.3.4a0/llmstudio/tracking/logs/schemas.py
--rw-r--r--   0        0        0        0 2024-04-09 10:18:39.970227 llmstudio-0.3.4a0/llmstudio/tracking/session/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-09 10:18:39.970379 llmstudio-0.3.4a0/llmstudio/tracking/session/crud.py
--rw-r--r--   0        0        0     1438 2024-04-09 10:18:39.970521 llmstudio-0.3.4a0/llmstudio/tracking/session/endpoints.py
--rw-r--r--   0        0        0      542 2024-04-09 10:18:39.970664 llmstudio-0.3.4a0/llmstudio/tracking/session/models.py
--rw-r--r--   0        0        0      409 2024-04-09 10:18:39.970809 llmstudio-0.3.4a0/llmstudio/tracking/session/schemas.py
--rw-r--r--   0        0        0     1460 2024-04-09 10:18:39.971001 llmstudio-0.3.4a0/llmstudio/tracking/tracker.py
--rw-r--r--   0        0        0       40 2023-12-11 19:01:37.798213 llmstudio-0.3.4a0/llmstudio/ui/.eslintrc.json
--rw-r--r--   0        0        0       36 2023-12-11 18:27:20.719105 llmstudio-0.3.4a0/llmstudio/ui/.git/COMMIT_EDITMSG
--rw-r--r--   0        0        0        0 2024-03-26 15:56:20.641454 llmstudio-0.3.4a0/llmstudio/ui/.git/FETCH_HEAD
--rw-r--r--   0        0        0       21 2023-12-11 18:27:20.719645 llmstudio-0.3.4a0/llmstudio/ui/.git/HEAD
--rw-r--r--   0        0        0      137 2023-12-11 18:27:20.719924 llmstudio-0.3.4a0/llmstudio/ui/.git/config
--rw-r--r--   0        0        0       73 2023-12-11 18:27:20.720282 llmstudio-0.3.4a0/llmstudio/ui/.git/description
--rwxr-xr-x   0        0        0      478 2023-12-11 18:27:20.721058 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0        0        0      896 2023-12-11 18:27:20.721542 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/commit-msg.sample
--rwxr-xr-x   0        0        0     4726 2023-12-11 18:27:20.721915 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0        0        0      189 2023-12-11 18:27:20.722141 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/post-update.sample
--rwxr-xr-x   0        0        0      424 2023-12-11 18:27:20.722509 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0        0        0     1643 2023-12-11 18:27:20.722942 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-commit.sample
--rwxr-xr-x   0        0        0      416 2023-12-11 18:27:20.723163 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0        0        0     1374 2023-12-11 18:27:20.723362 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-push.sample
--rwxr-xr-x   0        0        0     4898 2023-12-11 18:27:20.723702 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0        0        0      544 2023-12-11 18:27:20.724007 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/pre-receive.sample
--rwxr-xr-x   0        0        0     1492 2023-12-11 18:27:20.724328 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0        0        0     2783 2023-12-11 18:27:20.724522 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0        0        0     3650 2023-12-11 18:27:20.724788 llmstudio-0.3.4a0/llmstudio/ui/.git/hooks/update.sample
--rw-r--r--   0        0        0     1369 2023-12-11 18:27:20.725252 llmstudio-0.3.4a0/llmstudio/ui/.git/index
--rw-r--r--   0        0        0      240 2023-12-11 18:27:20.725965 llmstudio-0.3.4a0/llmstudio/ui/.git/info/exclude
--rw-r--r--   0        0        0      197 2023-12-11 18:27:20.726581 llmstudio-0.3.4a0/llmstudio/ui/.git/logs/HEAD
--rw-r--r--   0        0        0      197 2023-12-11 18:27:20.727271 llmstudio-0.3.4a0/llmstudio/ui/.git/logs/refs/heads/main
--rw-r--r--   0        0        0       83 2023-12-11 18:27:20.728272 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/18/2cd5e1b7b0f624758c8b796521d0e5584cecbe
--rw-r--r--   0        0        0      272 2023-12-11 18:27:20.728726 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/1a/f3b8f01934a8fdd694eb5747b8115f01419199
--rw-r--r--   0        0        0      155 2023-12-11 18:27:20.729189 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/2d/8cf29032c670297ab01a772fb619ec20121ca2
--rw-r--r--   0        0        0    50047 2023-12-11 18:27:20.730156 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/30/2ab9ffef38e2190bedb21ccbf7aed3eba35433
--rw-r--r--   0        0        0       84 2023-12-11 18:27:20.730628 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/33/ad091d26d8a9dc95ebdf616e217d985ec215b8
--rw-r--r--   0        0        0      297 2023-12-11 18:27:20.731050 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/40/e027fbefc15026f37d0e7d8b37e9d8f6e532b1
--rw-r--r--   0        0        0      738 2023-12-11 18:27:20.731455 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/51/74b28c565c285e3e312ec5178be64fbeca8398
--rw-r--r--   0        0        0     9641 2023-12-11 18:27:20.732160 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/71/8d6fea4835ec2d246af9800eddb7ffb276240c
--rw-r--r--   0        0        0       89 2023-12-11 18:27:20.732574 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/76/7719fc4fba59345ae29e29159c9aff270f5819
--rw-r--r--   0        0        0      390 2023-12-11 18:27:20.732982 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/92/dbd2331fc36396cd5d9862709f8e9708193ac1
--rw-r--r--   0        0        0      260 2023-12-11 18:27:20.734152 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/9b/9867255623524c7d90ebc18c040799a6b2c6b1
--rw-r--r--   0        0        0     1568 2023-12-11 18:27:20.735060 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/b9/73266263f2fb83a6c385966c1c3656a60503be
--rw-r--r--   0        0        0      153 2023-12-11 18:27:20.735487 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/be/f290dd43c11955bd7224e7c1e8db7ece45807a
--rw-r--r--   0        0        0       54 2023-12-11 18:27:20.735902 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/bf/fb357a7122523ec94045523758c4b825b448ef
--rw-r--r--   0        0        0      729 2023-12-11 18:27:20.736477 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/c4/033664f80d3cb9cb687fb5facbc82aedb302f6
--rw-r--r--   0        0        0      375 2023-12-11 18:27:20.737066 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/d2/f84222734f27b623d1c80dda3561b04d1284af
--rw-r--r--   0        0        0       46 2023-12-11 18:27:20.737742 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/e3/97ba02717230d1328c71f52f12655120e8760c
--rw-r--r--   0        0        0      315 2023-12-11 18:27:20.738140 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/e5/9724b283f9cb9a63ce04a2405128164607a14a
--rw-r--r--   0        0        0      258 2023-12-11 18:27:20.738559 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/fd/3dbb571a12a1c3baf000db049e141c888d05a8
--rw-r--r--   0        0        0      257 2023-12-11 18:27:20.738768 llmstudio-0.3.4a0/llmstudio/ui/.git/objects/fd/81e885836d815b8019694a910a93d86a43cb66
--rw-r--r--   0        0        0       41 2023-12-11 18:27:20.739608 llmstudio-0.3.4a0/llmstudio/ui/.git/refs/heads/main
--rw-r--r--   0        0        0      391 2023-12-11 19:01:37.798312 llmstudio-0.3.4a0/llmstudio/ui/.gitignore
--rw-r--r--   0        0        0      157 2023-12-11 19:01:37.798390 llmstudio-0.3.4a0/llmstudio/ui/.prettierrc.json
--rw-r--r--   0        0        0      601 2024-03-26 14:37:08.858230 llmstudio-0.3.4a0/llmstudio/ui/__init__.py
--rw-r--r--   0        0        0      327 2023-12-11 19:01:37.799270 llmstudio-0.3.4a0/llmstudio/ui/components.json
--rw-r--r--   0        0        0       98 2023-12-11 19:01:37.799337 llmstudio-0.3.4a0/llmstudio/ui/global.d.ts
--rw-r--r--   0        0        0       94 2023-12-11 19:01:37.799413 llmstudio-0.3.4a0/llmstudio/ui/next.config.js
--rw-r--r--   0        0        0   154026 2024-01-16 12:06:19.562727 llmstudio-0.3.4a0/llmstudio/ui/package-lock.json
--rw-r--r--   0        0        0     2697 2024-03-26 11:19:39.036108 llmstudio-0.3.4a0/llmstudio/ui/package.json
--rw-r--r--   0        0        0       82 2023-12-11 19:01:37.801005 llmstudio-0.3.4a0/llmstudio/ui/postcss.config.js
--rw-r--r--   0        0        0    34679 2023-12-11 19:01:37.801113 llmstudio-0.3.4a0/llmstudio/ui/public/logo.json
--rw-r--r--   0        0        0     1026 2023-12-11 18:27:34.699408 llmstudio-0.3.4a0/llmstudio/ui/public/svg/ai.svg
--rw-r--r--   0        0        0      212 2023-12-11 18:27:34.699893 llmstudio-0.3.4a0/llmstudio/ui/public/svg/arrow.svg
--rw-r--r--   0        0        0      617 2023-12-11 19:01:37.801212 llmstudio-0.3.4a0/llmstudio/ui/public/svg/compare.svg
--rw-r--r--   0        0        0      872 2023-12-11 18:27:34.700682 llmstudio-0.3.4a0/llmstudio/ui/public/svg/home.svg
--rw-r--r--   0        0        0      482 2023-12-11 18:27:34.700961 llmstudio-0.3.4a0/llmstudio/ui/public/svg/load.svg
--rw-r--r--   0        0        0     2894 2023-12-11 18:27:34.701440 llmstudio-0.3.4a0/llmstudio/ui/public/svg/magic.svg
--rw-r--r--   0        0        0      535 2023-12-11 18:27:34.701731 llmstudio-0.3.4a0/llmstudio/ui/public/svg/play.svg
--rw-r--r--   0        0        0     4669 2023-12-11 18:27:34.702336 llmstudio-0.3.4a0/llmstudio/ui/public/svg/playground.svg
--rw-r--r--   0        0        0      526 2023-12-11 18:27:34.702778 llmstudio-0.3.4a0/llmstudio/ui/public/svg/plus.svg
--rw-r--r--   0        0        0     1243 2023-12-11 18:27:34.703255 llmstudio-0.3.4a0/llmstudio/ui/public/svg/settings.svg
--rw-r--r--   0        0        0     1803 2023-12-11 18:27:34.703621 llmstudio-0.3.4a0/llmstudio/ui/public/svg/sparkles.svg
--rw-r--r--   0        0        0      118 2023-12-11 19:01:37.801396 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/compare/page.tsx
--rw-r--r--   0        0        0      992 2024-03-12 16:29:10.045979 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx
--rw-r--r--   0        0        0     3719 2024-03-12 16:29:10.046151 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/dashboard/page.tsx
--rw-r--r--   0        0        0     2200 2023-12-11 19:01:37.802701 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx
--rw-r--r--   0        0        0     3847 2024-03-25 17:27:35.433056 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx
--rw-r--r--   0        0        0     4986 2023-12-11 19:01:37.802864 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx
--rw-r--r--   0        0        0     3301 2023-12-11 19:01:37.802936 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx
--rw-r--r--   0        0        0     1635 2023-12-14 17:50:14.618144 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx
--rw-r--r--   0        0        0     1333 2023-12-11 19:01:37.803075 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx
--rw-r--r--   0        0        0     1942 2023-12-11 19:01:37.803142 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx
--rw-r--r--   0        0        0     1671 2023-12-11 19:01:37.803210 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx
--rw-r--r--   0        0        0     7206 2024-03-25 17:29:39.773208 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx
--rw-r--r--   0        0        0     1982 2024-03-12 16:29:03.312683 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx
--rw-r--r--   0        0        0     1539 2023-12-11 19:01:37.803446 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx
--rw-r--r--   0        0        0      639 2023-12-11 19:01:37.803513 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx
--rw-r--r--   0        0        0     2561 2023-12-11 19:01:37.803588 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx
--rw-r--r--   0        0        0     1131 2023-12-11 19:01:37.803651 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx
--rw-r--r--   0        0        0     2777 2023-12-11 19:01:37.803720 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx
--rw-r--r--   0        0        0      266 2023-12-11 19:01:37.803820 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/index.tsx
--rw-r--r--   0        0        0     1239 2024-03-12 16:29:03.312940 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx
--rw-r--r--   0        0        0     1013 2024-03-12 16:29:03.313153 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx
--rw-r--r--   0        0        0      654 2024-03-12 16:29:03.313408 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx
--rw-r--r--   0        0        0      957 2024-03-12 16:29:03.313702 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx
--rw-r--r--   0        0        0     1092 2024-03-12 16:29:03.313962 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx
--rw-r--r--   0        0        0      707 2023-12-11 19:01:37.804335 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/page.tsx
--rw-r--r--   0        0        0     1917 2024-03-12 16:29:03.314221 llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/store.tsx
--rw-r--r--   0        0        0    15406 2023-12-11 19:01:37.804706 llmstudio-0.3.4a0/llmstudio/ui/src/app/favicon.ico
--rw-r--r--   0        0        0     1567 2024-01-16 11:50:05.598045 llmstudio-0.3.4a0/llmstudio/ui/src/app/globals.css
--rw-r--r--   0        0        0      858 2024-01-16 11:38:37.175729 llmstudio-0.3.4a0/llmstudio/ui/src/app/layout.tsx
--rw-r--r--   0        0        0      223 2024-03-12 16:29:03.314620 llmstudio-0.3.4a0/llmstudio/ui/src/app/page.tsx
--rw-r--r--   0        0        0     1721 2023-12-11 19:01:37.805081 llmstudio-0.3.4a0/llmstudio/ui/src/components/CodeBlock/index.tsx
--rw-r--r--   0        0        0     2840 2023-12-11 19:01:37.805198 llmstudio-0.3.4a0/llmstudio/ui/src/components/CopyButton/index.tsx
--rw-r--r--   0        0        0     1507 2024-03-12 16:29:10.046432 llmstudio-0.3.4a0/llmstudio/ui/src/components/Header/index.tsx
--rw-r--r--   0        0        0     6315 2023-12-11 19:01:37.805428 llmstudio-0.3.4a0/llmstudio/ui/src/components/Markdown/index.tsx
--rw-r--r--   0        0        0      871 2023-12-11 19:01:37.805531 llmstudio-0.3.4a0/llmstudio/ui/src/components/Theme/index.tsx
--rw-r--r--   0        0        0      323 2023-12-11 19:01:37.805640 llmstudio-0.3.4a0/llmstudio/ui/src/components/Toaster/index.tsx
--rw-r--r--   0        0        0      332 2024-01-16 11:17:40.396156 llmstudio-0.3.4a0/llmstudio/ui/src/components/theme-provider.tsx
--rw-r--r--   0        0        0     1991 2023-12-11 19:01:37.805827 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/accordion.tsx
--rw-r--r--   0        0        0     4455 2023-12-11 19:01:37.805917 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/alert-dialog.tsx
--rw-r--r--   0        0        0     1584 2023-12-11 19:01:37.805988 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/alert.tsx
--rw-r--r--   0        0        0      154 2023-12-11 19:01:37.806052 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/aspect-ratio.tsx
--rw-r--r--   0        0        0     1419 2023-12-11 19:01:37.806133 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/avatar.tsx
--rw-r--r--   0        0        0     1128 2023-12-11 19:01:37.806199 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/badge.tsx
--rw-r--r--   0        0        0     1835 2023-12-11 19:01:37.806267 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/button.tsx
--rw-r--r--   0        0        0     2623 2023-12-11 19:01:37.806344 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/calendar.tsx
--rw-r--r--   0        0        0     1877 2023-12-11 19:01:37.806433 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/card.tsx
--rw-r--r--   0        0        0     1070 2023-12-11 19:01:37.806496 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/checkbox.tsx
--rw-r--r--   0        0        0      329 2023-12-11 19:01:37.806575 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/collapsible.tsx
--rw-r--r--   0        0        0     4867 2023-12-11 19:01:37.806676 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/command.tsx
--rw-r--r--   0        0        0     7260 2023-12-11 19:01:37.806781 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/context-menu.tsx
--rw-r--r--   0        0        0     3870 2023-12-11 19:01:37.806860 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/dialog.tsx
--rw-r--r--   0        0        0     7309 2023-12-11 19:01:37.806976 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/dropdown-menu.tsx
--rw-r--r--   0        0        0     4085 2023-12-11 19:01:37.807058 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/form.tsx
--rw-r--r--   0        0        0     1198 2023-12-11 19:01:37.807134 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/hover-card.tsx
--rw-r--r--   0        0        0      824 2023-12-11 19:01:37.807197 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/input.tsx
--rw-r--r--   0        0        0      724 2023-12-11 19:01:37.807264 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/label.tsx
--rw-r--r--   0        0        0     7988 2023-12-11 19:01:37.807379 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/menubar.tsx
--rw-r--r--   0        0        0     5046 2023-12-11 19:01:37.807484 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/navigation-menu.tsx
--rw-r--r--   0        0        0     1244 2023-12-11 19:01:37.807577 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/popover.tsx
--rw-r--r--   0        0        0      791 2023-12-11 19:01:37.807658 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/progress.tsx
--rw-r--r--   0        0        0     1481 2023-12-11 19:01:37.807744 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/radio-group.tsx
--rw-r--r--   0        0        0     1656 2023-12-11 19:01:37.807816 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/scroll-area.tsx
--rw-r--r--   0        0        0     5629 2023-12-11 19:01:37.807893 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/select.tsx
--rw-r--r--   0        0        0      770 2023-12-11 19:01:37.807958 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/separator.tsx
--rw-r--r--   0        0        0     4302 2023-12-11 19:01:37.808061 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/sheet.tsx
--rw-r--r--   0        0        0      261 2023-12-11 19:01:37.808142 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/skeleton.tsx
--rw-r--r--   0        0        0     1091 2023-12-11 19:01:37.808218 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/slider.tsx
--rw-r--r--   0        0        0     1153 2023-12-11 19:01:37.808300 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/switch.tsx
--rw-r--r--   0        0        0     2765 2023-12-11 19:01:37.808380 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/table.tsx
--rw-r--r--   0        0        0     1897 2023-12-11 19:01:37.808453 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/tabs.tsx
--rw-r--r--   0        0        0      772 2023-12-11 19:01:37.808528 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/textarea.tsx
--rw-r--r--   0        0        0     4845 2023-12-11 19:01:37.808636 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toast.tsx
--rw-r--r--   0        0        0      794 2023-12-11 19:01:37.808712 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toaster.tsx
--rw-r--r--   0        0        0     1748 2023-12-11 19:01:37.808802 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toggle-group.tsx
--rw-r--r--   0        0        0     1449 2023-12-11 19:01:37.808881 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toggle.tsx
--rw-r--r--   0        0        0     1159 2023-12-11 19:01:37.808957 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/tooltip.tsx
--rw-r--r--   0        0        0     3934 2023-12-11 19:01:37.809043 llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/use-toast.ts
--rw-r--r--   0        0        0     1802 2023-12-11 19:01:37.809170 llmstudio-0.3.4a0/llmstudio/ui/src/lib/utils.ts
--rw-r--r--   0        0        0     6560 2024-03-12 16:29:10.046746 llmstudio-0.3.4a0/llmstudio/ui/tailwind.config.js
--rw-r--r--   0        0        0      694 2023-12-11 19:01:37.809465 llmstudio-0.3.4a0/llmstudio/ui/tsconfig.json
--rw-r--r--   0        0        0     1075 2024-04-09 10:34:14.915237 llmstudio-0.3.4a0/pyproject.toml
--rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 llmstudio-0.3.4a0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/LICENSE
+-rw-r--r--   0        0        0     4185 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/README.md
+-rw-r--r--   0        0        0       30 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/cli.py
+-rw-r--r--   0        0        0       56 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/client.py
+-rw-r--r--   0        0        0     1573 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/config.py
+-rw-r--r--   0        0        0     6177 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/__init__.py
+-rw-r--r--   0        0        0     5623 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/config.yaml
+-rw-r--r--   0        0        0      314 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/__init__.py
+-rw-r--r--   0        0        0     3434 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/anthropic.py
+-rw-r--r--   0        0        0     2569 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/azure.py
+-rw-r--r--   0        0        0     3227 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/ollama.py
+-rw-r--r--   0        0        0     2194 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/openai.py
+-rw-r--r--   0        0        0    13776 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/engine/providers/provider.py
+-rw-r--r--   0        0        0     3844 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/llm/__init__.py
+-rw-r--r--   0        0        0     2114 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/llm/langchain.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/__init__.py
+-rw-r--r--   0        0        0     1165 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/conftest.py
+-rw-r--r--   0        0        0     3007 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/engine/test_engine.py
+-rw-r--r--   0        0        0     3926 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tests/engine/test_providers.py
+-rw-r--r--   0        0        0     1800 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tracking/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-12 13:53:28.367324 llmstudio-0.3.4a1/llmstudio/tracking/database.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/crud.py
+-rw-r--r--   0        0        0     1513 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/endpoints.py
+-rw-r--r--   0        0        0      578 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/models.py
+-rw-r--r--   0        0        0      834 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/logs/schemas.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/__init__.py
+-rw-r--r--   0        0        0     1339 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/crud.py
+-rw-r--r--   0        0        0     1438 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/endpoints.py
+-rw-r--r--   0        0        0      554 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/models.py
+-rw-r--r--   0        0        0      409 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/session/schemas.py
+-rw-r--r--   0        0        0     1459 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/tracking/tracker.py
+-rw-r--r--   0        0        0       40 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.eslintrc.json
+-rw-r--r--   0        0        0      391 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.gitignore
+-rw-r--r--   0        0        0      157 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/.prettierrc.json
+-rw-r--r--   0        0        0      601 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/components.json
+-rw-r--r--   0        0        0       98 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/global.d.ts
+-rw-r--r--   0        0        0       94 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/next.config.js
+-rw-r--r--   0        0        0   154026 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/package-lock.json
+-rw-r--r--   0        0        0     2697 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/package.json
+-rw-r--r--   0        0        0       82 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/postcss.config.js
+-rw-r--r--   0        0        0    34679 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/logo.json
+-rw-r--r--   0        0        0     1026 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/ai.svg
+-rw-r--r--   0        0        0      212 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/arrow.svg
+-rw-r--r--   0        0        0      617 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/compare.svg
+-rw-r--r--   0        0        0      872 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/home.svg
+-rw-r--r--   0        0        0      482 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/load.svg
+-rw-r--r--   0        0        0     2894 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/magic.svg
+-rw-r--r--   0        0        0      535 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/play.svg
+-rw-r--r--   0        0        0     4669 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/playground.svg
+-rw-r--r--   0        0        0      526 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/plus.svg
+-rw-r--r--   0        0        0     1243 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/settings.svg
+-rw-r--r--   0        0        0     1803 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/public/svg/sparkles.svg
+-rw-r--r--   0        0        0      118 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/compare/page.tsx
+-rw-r--r--   0        0        0      992 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx
+-rw-r--r--   0        0        0     3719 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/page.tsx
+-rw-r--r--   0        0        0     2200 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx
+-rw-r--r--   0        0        0     3847 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx
+-rw-r--r--   0        0        0     4986 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx
+-rw-r--r--   0        0        0     3301 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx
+-rw-r--r--   0        0        0     1635 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx
+-rw-r--r--   0        0        0     1333 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx
+-rw-r--r--   0        0        0     1942 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx
+-rw-r--r--   0        0        0     1671 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx
+-rw-r--r--   0        0        0     7206 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx
+-rw-r--r--   0        0        0     1982 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx
+-rw-r--r--   0        0        0     1539 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx
+-rw-r--r--   0        0        0      639 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx
+-rw-r--r--   0        0        0     2561 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx
+-rw-r--r--   0        0        0     1131 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx
+-rw-r--r--   0        0        0     2777 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx
+-rw-r--r--   0        0        0      266 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/index.tsx
+-rw-r--r--   0        0        0     1239 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx
+-rw-r--r--   0        0        0     1013 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx
+-rw-r--r--   0        0        0      654 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx
+-rw-r--r--   0        0        0      957 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx
+-rw-r--r--   0        0        0     1092 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx
+-rw-r--r--   0        0        0      707 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/page.tsx
+-rw-r--r--   0        0        0     1917 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/store.tsx
+-rw-r--r--   0        0        0    15406 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/favicon.ico
+-rw-r--r--   0        0        0     1567 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/globals.css
+-rw-r--r--   0        0        0      858 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/layout.tsx
+-rw-r--r--   0        0        0      223 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/app/page.tsx
+-rw-r--r--   0        0        0     1721 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/CodeBlock/index.tsx
+-rw-r--r--   0        0        0     2840 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/CopyButton/index.tsx
+-rw-r--r--   0        0        0     1507 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Header/index.tsx
+-rw-r--r--   0        0        0     6315 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Markdown/index.tsx
+-rw-r--r--   0        0        0      871 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Theme/index.tsx
+-rw-r--r--   0        0        0      323 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/Toaster/index.tsx
+-rw-r--r--   0        0        0      332 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/theme-provider.tsx
+-rw-r--r--   0        0        0     1991 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/accordion.tsx
+-rw-r--r--   0        0        0     4455 2024-04-12 13:53:28.371324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert-dialog.tsx
+-rw-r--r--   0        0        0     1584 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert.tsx
+-rw-r--r--   0        0        0      154 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/aspect-ratio.tsx
+-rw-r--r--   0        0        0     1419 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/avatar.tsx
+-rw-r--r--   0        0        0     1128 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/badge.tsx
+-rw-r--r--   0        0        0     1835 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/button.tsx
+-rw-r--r--   0        0        0     2623 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/calendar.tsx
+-rw-r--r--   0        0        0     1877 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/card.tsx
+-rw-r--r--   0        0        0     1070 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/checkbox.tsx
+-rw-r--r--   0        0        0      329 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/collapsible.tsx
+-rw-r--r--   0        0        0     4867 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/command.tsx
+-rw-r--r--   0        0        0     7260 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/context-menu.tsx
+-rw-r--r--   0        0        0     3870 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dialog.tsx
+-rw-r--r--   0        0        0     7309 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dropdown-menu.tsx
+-rw-r--r--   0        0        0     4085 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/form.tsx
+-rw-r--r--   0        0        0     1198 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/hover-card.tsx
+-rw-r--r--   0        0        0      824 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/input.tsx
+-rw-r--r--   0        0        0      724 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/label.tsx
+-rw-r--r--   0        0        0     7988 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/menubar.tsx
+-rw-r--r--   0        0        0     5046 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/navigation-menu.tsx
+-rw-r--r--   0        0        0     1244 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/popover.tsx
+-rw-r--r--   0        0        0      791 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/progress.tsx
+-rw-r--r--   0        0        0     1481 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/radio-group.tsx
+-rw-r--r--   0        0        0     1656 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/scroll-area.tsx
+-rw-r--r--   0        0        0     5629 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/select.tsx
+-rw-r--r--   0        0        0      770 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/separator.tsx
+-rw-r--r--   0        0        0     4302 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/sheet.tsx
+-rw-r--r--   0        0        0      261 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/skeleton.tsx
+-rw-r--r--   0        0        0     1091 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/slider.tsx
+-rw-r--r--   0        0        0     1153 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/switch.tsx
+-rw-r--r--   0        0        0     2765 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/table.tsx
+-rw-r--r--   0        0        0     1897 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tabs.tsx
+-rw-r--r--   0        0        0      772 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/textarea.tsx
+-rw-r--r--   0        0        0     4845 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toast.tsx
+-rw-r--r--   0        0        0      794 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toaster.tsx
+-rw-r--r--   0        0        0     1748 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle-group.tsx
+-rw-r--r--   0        0        0     1449 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle.tsx
+-rw-r--r--   0        0        0     1159 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tooltip.tsx
+-rw-r--r--   0        0        0     3934 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/use-toast.ts
+-rw-r--r--   0        0        0     1802 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/src/lib/utils.ts
+-rw-r--r--   0        0        0     6560 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/tailwind.config.js
+-rw-r--r--   0        0        0      694 2024-04-12 13:53:28.375324 llmstudio-0.3.4a1/llmstudio/ui/tsconfig.json
+-rw-r--r--   0        0        0     1075 2024-04-12 13:53:41.399306 llmstudio-0.3.4a1/pyproject.toml
+-rw-r--r--   0        0        0     5550 1970-01-01 00:00:00.000000 llmstudio-0.3.4a1/PKG-INFO
```

### Comparing `llmstudio-0.3.4a0/LICENSE` & `llmstudio-0.3.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/README.md` & `llmstudio-0.3.4a1/README.md`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/cli.py` & `llmstudio-0.3.4a1/llmstudio/cli.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/config.py` & `llmstudio-0.3.4a1/llmstudio/config.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/__init__.py` & `llmstudio-0.3.4a1/llmstudio/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/config.yaml` & `llmstudio-0.3.4a1/llmstudio/engine/config.yaml`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/providers/anthropic.py` & `llmstudio-0.3.4a1/llmstudio/engine/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/providers/azure.py` & `llmstudio-0.3.4a1/llmstudio/engine/providers/azure.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/providers/ollama.py` & `llmstudio-0.3.4a1/llmstudio/engine/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/providers/openai.py` & `llmstudio-0.3.4a1/llmstudio/engine/providers/openai.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/engine/providers/provider.py` & `llmstudio-0.3.4a1/llmstudio/engine/providers/provider.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/llm/__init__.py` & `llmstudio-0.3.4a1/llmstudio/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/llm/langchain.py` & `llmstudio-0.3.4a1/llmstudio/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tests/conftest.py` & `llmstudio-0.3.4a1/llmstudio/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tests/engine/test_engine.py` & `llmstudio-0.3.4a1/llmstudio/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tests/engine/test_providers.py` & `llmstudio-0.3.4a1/llmstudio/tests/engine/test_providers.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/__init__.py` & `llmstudio-0.3.4a1/llmstudio/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/database.py` & `llmstudio-0.3.4a1/llmstudio/tracking/database.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/logs/crud.py` & `llmstudio-0.3.4a1/llmstudio/tracking/logs/crud.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/logs/endpoints.py` & `llmstudio-0.3.4a1/llmstudio/tracking/logs/endpoints.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/logs/models.py` & `llmstudio-0.3.4a1/llmstudio/tracking/logs/models.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/logs/schemas.py` & `llmstudio-0.3.4a1/llmstudio/tracking/logs/schemas.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/session/crud.py` & `llmstudio-0.3.4a1/llmstudio/tracking/session/crud.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 def get_session_by_session_id(
     db: Session, session_id: str, skip: int = 0, limit: int = 100
 ):
     return (
         db.query(models.SessionDefault)
         .filter(models.SessionDefault.session_id == session_id)
+        .order_by(models.SessionDefault.created_at.asc())
         .offset(skip)
         .limit(limit)
         .all()
     )
 
 
 def get_session_by_message_id(db: Session, message_id: int):
```

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/session/endpoints.py` & `llmstudio-0.3.4a1/llmstudio/tracking/session/endpoints.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/session/models.py` & `llmstudio-0.3.4a1/llmstudio/tracking/session/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from sqlalchemy.sql import func
 
 from llmstudio.tracking.database import Base
 
 
 class SessionDefault(Base):
     __tablename__ = "sessions"
-    message_id = Column(Integer, primary_key=True)
+    message_id = Column(Integer, primary_key=True, index=True)
     session_id = Column(String, index=True)
     chat_history = Column(JSON)
     extras = Column(JSON)
     updated_at = Column(
         DateTime(timezone=True), onupdate=func.now(), server_default=func.now()
     )
     created_at = Column(DateTime(timezone=True), server_default=func.now())
```

### Comparing `llmstudio-0.3.4a0/llmstudio/tracking/tracker.py` & `llmstudio-0.3.4a1/llmstudio/tracking/tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             headers={"accept": "application/json", "Content-Type": "application/json"},
             data=json.dumps(data),
             timeout=100,
         )
         return req
 
     def get_session(self, session_id: str):
-        req = self._session.post(
+        req = self._session.get(
             f"http://{TRACKING_HOST}:{TRACKING_PORT}/api/tracking/session/{session_id}",
             headers={"accept": "application/json", "Content-Type": "application/json"},
             timeout=100,
         )
         return req
 
     def add_extras(self, message_id: int):
```

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/__init__.py` & `llmstudio-0.3.4a1/llmstudio/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/package-lock.json` & `llmstudio-0.3.4a1/llmstudio/ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/package.json` & `llmstudio-0.3.4a1/llmstudio/ui/package.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/logo.json` & `llmstudio-0.3.4a1/llmstudio/ui/public/logo.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/ai.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/ai.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/compare.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/compare.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/home.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/home.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/magic.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/magic.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/play.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/play.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/playground.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/playground.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/plus.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/plus.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/settings.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/settings.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/public/svg/sparkles.svg` & `llmstudio-0.3.4a1/llmstudio/ui/public/svg/sparkles.svg`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/hooks/useDashboardFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/dashboard/page.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/dashboard/page.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ColumnHeader.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/DataTable.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/FacetedFilter.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Pagination.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/RowActions.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/Toolbar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/UserNav.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/ViewOptions.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/DataTable/columns.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Input.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/LogSheet.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelItem.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/ModelSelector.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Output.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/components/Parameters.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useChat.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useExport.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useLogsFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useModelFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/hooks/useParameterFetch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/page.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/page.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/(llm)/playground/store.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/(llm)/playground/store.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/favicon.ico` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/globals.css` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/globals.css`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/app/layout.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/app/layout.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/CodeBlock/index.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/CodeBlock/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/CopyButton/index.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/CopyButton/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/Header/index.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/Header/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/Markdown/index.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/Markdown/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/Theme/index.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/Theme/index.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/accordion.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/accordion.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/alert-dialog.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert-dialog.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/alert.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/alert.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/avatar.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/avatar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/badge.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/badge.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/button.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/button.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/calendar.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/calendar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/card.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/card.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/checkbox.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/checkbox.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/command.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/command.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/context-menu.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/context-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/dialog.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dialog.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/dropdown-menu.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/dropdown-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/form.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/form.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/hover-card.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/hover-card.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/input.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/input.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/label.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/label.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/menubar.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/menubar.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/navigation-menu.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/navigation-menu.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/popover.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/popover.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/progress.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/progress.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/radio-group.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/radio-group.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/scroll-area.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/scroll-area.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/select.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/select.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/separator.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/separator.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/sheet.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/sheet.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/slider.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/slider.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/switch.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/switch.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/table.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/table.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/tabs.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tabs.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/textarea.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/textarea.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toast.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toast.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toaster.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toaster.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toggle-group.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle-group.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/toggle.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/toggle.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/tooltip.tsx` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/tooltip.tsx`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/components/ui/use-toast.ts` & `llmstudio-0.3.4a1/llmstudio/ui/src/components/ui/use-toast.ts`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/src/lib/utils.ts` & `llmstudio-0.3.4a1/llmstudio/ui/src/lib/utils.ts`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/tailwind.config.js` & `llmstudio-0.3.4a1/llmstudio/ui/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/llmstudio/ui/tsconfig.json` & `llmstudio-0.3.4a1/llmstudio/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `llmstudio-0.3.4a0/pyproject.toml` & `llmstudio-0.3.4a1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llmstudio"
-version = "0.3.4a0"
+version = "0.3.4a1"
 description = "Prompt Perfection at Your Fingertips"
 authors = ["Cláudio Lemos <claudio@tensorops.ai>"]
 license = "MIT"
 homepage = "https://llmstudio.ai/"
 repository = "https://github.com/tensoropsai/llmstudio"
 documentation = "https://docs.llmstudio.ai"
 readme = "README.md"
```

### Comparing `llmstudio-0.3.4a0/PKG-INFO` & `llmstudio-0.3.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmstudio
-Version: 0.3.4a0
+Version: 0.3.4a1
 Summary: Prompt Perfection at Your Fingertips
 Home-page: https://llmstudio.ai/
 License: MIT
 Keywords: ml,ai,llm,llmops,openai,langchain,chatgpt,llmstudio,tensorops
 Author: Cláudio Lemos
 Author-email: claudio@tensorops.ai
 Requires-Python: >=3.9,<4.0
```

