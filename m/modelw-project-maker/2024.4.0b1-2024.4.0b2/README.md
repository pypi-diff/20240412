# Comparing `tmp/modelw_project_maker-2024.4.0b1.tar.gz` & `tmp/modelw_project_maker-2024.4.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_project_maker-2024.4.0b1.tar", max compression
+gzip compressed data, was "modelw_project_maker-2024.4.0b2.tar", max compression
```

## Comparing `modelw_project_maker-2024.4.0b1.tar` & `modelw_project_maker-2024.4.0b2.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     5377 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/README.md
--rw-r--r--   0        0        0     1357 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__init__.py
--rw-r--r--   0        0        0     8748 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__main__.py
--rw-r--r--   0        0        0       45 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/errors.py
--rw-r--r--   0        0        0      143 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/__init__.py
--rw-r--r--   0        0        0     4470 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_api.py
--rw-r--r--   0        0        0     6518 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_base.py
--rw-r--r--   0        0        0      703 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_common.py
--rw-r--r--   0        0        0     3836 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_front.py
--rw-r--r--   0        0        0     3446 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/namer.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/py.typed
--rw-r--r--   0        0        0      178 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.editorconfig
--rw-r--r--   0        0        0       27 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.formatignore
--rw-r--r--   0        0        0     3042 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.gitignore
--rw-r--r--   0        0        0       77 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.prettierrc
--rw-r--r--   0        0        0     1488 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/README.md
--rw-r--r--   0        0        0     3034 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.dockerignore
--rw-r--r--   0        0        0      373 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.env-template
--rw-r--r--   0        0        0      181 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/Dockerfile
--rw-r--r--   0        0        0      236 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/Makefile
--rw-r--r--   0        0        0     1140 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
--rw-r--r--   0        0        0       93 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
--rw-r--r--   0        0        0     8633 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
--rw-r--r--   0        0        0     2818 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
--rw-r--r--   0        0        0     2031 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
--rw-r--r--   0        0        0      655 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
--rw-r--r--   0        0        0      233 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
--rwxr-xr-x   0        0        0      755 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
--rwxr-xr-x   0        0        0      240 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
--rwxr-xr-x   0        0        0      471 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
--rwxr-xr-x   0        0        0      844 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
--rwxr-xr-x   0        0        0      903 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
--rwxr-xr-x   0        0        0     1092 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
--rwxr-xr-x   0        0        0      658 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
--rwxr-xr-x   0        0        0      718 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
--rwxr-xr-x   0        0        0      485 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
--rwxr-xr-x   0        0        0     2749 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
--rwxr-xr-x   0        0        0     2067 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
--rw-r--r--   0        0        0     1883 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
--rw-r--r--   0        0        0      159 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
--rw-r--r--   0        0        0     3921 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
--rw-r--r--   0        0        0     3150 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
--rw-r--r--   0        0        0     1343 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
--rw-r--r--   0        0        0     2486 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
--rw-r--r--   0        0        0      194 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
--rw-r--r--   0        0        0      386 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
--rw-r--r--   0        0        0       70 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
--rw-r--r--   0        0        0      851 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
--rw-r--r--   0        0        0      273 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
--rw-r--r--   0        0        0      220 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
--rw-r--r--   0        0        0     2076 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
--rw-r--r--   0        0        0     1682 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
--rw-r--r--   0        0        0      443 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
--rw-r--r--   0        0        0       89 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/.gitignore
--rw-r--r--   0        0        0     7233 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/README.md
--rw-r--r--   0        0        0        0 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/__init__.py
--rw-r--r--   0        0        0      400 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/conftest.py
--rw-r--r--   0        0        0      451 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/features/README.md
--rw-r--r--   0        0        0     3001 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/features/smoke-test.feature
--rw-r--r--   0        0        0      224 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/README.md
--rw-r--r--   0        0        0      126 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/__init__.py
--rw-r--r--   0        0        0      748 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/data.py
--rw-r--r--   0        0        0     5289 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/front.py
--rw-r--r--   0        0        0     1033 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/reporting.py
--rw-r--r--   0        0        0     1885 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/utils.py
--rw-r--r--   0        0        0     5334 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/hooks.py
--rw-r--r--   0        0        0    16126 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/reporter.py
--rw-r--r--   0        0        0     2242 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/utils.py
--rw-r--r--   0        0        0      142 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/__init__.py
--rw-r--r--   0        0        0     3458 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_given.py
--rw-r--r--   0        0        0     4797 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_then.py
--rw-r--r--   0        0        0     3484 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_when.py
--rw-r--r--   0        0        0     3537 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/utils.py
--rw-r--r--   0        0        0      680 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_features.py
--rw-r--r--   0        0        0    11758 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_utils.py
--rwxr-xr-x   0        0        0      666 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/manage.py
--rwxr-xr-x   0        0        0      151 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/pmanage
--rw-r--r--   0        0        0     1473 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/pyproject.toml
--rw-r--r--   0        0        0     3034 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.dockerignore
--rw-r--r--   0        0        0      174 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.env-template
--rw-r--r--   0        0        0      332 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.eslintrc.js
--rw-r--r--   0        0        0        8 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.gitignore
--rw-r--r--   0        0        0       13 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.nvmrc
--rw-r--r--   0        0        0      185 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/Dockerfile
--rw-r--r--   0        0        0     1601 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/README.md
--rw-r--r--   0        0        0      112 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/blocks/title-1.vue
--rw-r--r--   0        0        0    11513 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue
--rw-r--r--   0        0        0     2941 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/error.vue
--rw-r--r--   0        0        0     6320 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/middleware/wagtail.ts
--rw-r--r--   0        0        0      738 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js
--rw-r--r--   0        0        0      869 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/package.json
--rw-r--r--   0        0        0      655 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue
--rw-r--r--   0        0        0       80 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
--rw-r--r--   0        0        0      483 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/plugins/dom.client.ts
--rw-r--r--   0        0        0      505 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/plugins/dom.server.ts
--rw-r--r--   0        0        0      439 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/stores/layout.js
--rw-r--r--   0        0        0       98 2024-04-10 07:30:32.706843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/tsconfig.json
--rw-r--r--   0        0        0     7602 2024-04-10 07:30:32.702843 modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template.py
--rw-r--r--   0        0        0     6645 1970-01-01 00:00:00.000000 modelw_project_maker-2024.4.0b1/PKG-INFO
+-rw-r--r--   0        0        0     5377 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/README.md
+-rw-r--r--   0        0        0     1357 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/__init__.py
+-rw-r--r--   0        0        0     8748 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/errors.py
+-rw-r--r--   0        0        0      143 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/__init__.py
+-rw-r--r--   0        0        0     4470 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_api.py
+-rw-r--r--   0        0        0     6518 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_base.py
+-rw-r--r--   0        0        0      703 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_common.py
+-rw-r--r--   0        0        0     3836 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_front.py
+-rw-r--r--   0        0        0     3446 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/namer.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/py.typed
+-rw-r--r--   0        0        0      178 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/.editorconfig
+-rw-r--r--   0        0        0       27 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/.formatignore
+-rw-r--r--   0        0        0     3042 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/.gitignore
+-rw-r--r--   0        0        0       77 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/.prettierrc
+-rw-r--r--   0        0        0     1488 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/README.md
+-rw-r--r--   0        0        0     3034 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/.dockerignore
+-rw-r--r--   0        0        0      373 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/.env-template
+-rw-r--r--   0        0        0      181 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/Dockerfile
+-rw-r--r--   0        0        0      236 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/Makefile
+-rw-r--r--   0        0        0     1140 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/__init__.py
+-rw-r--r--   0        0        0       93 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/__init__.py
+-rw-r--r--   0        0        0     8633 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2818 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py
+-rw-r--r--   0        0        0      655 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html
+-rw-r--r--   0        0        0      233 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/cms/home_page.html
+-rwxr-xr-x   0        0        0      755 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg
+-rwxr-xr-x   0        0        0      240 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/edit.svg
+-rwxr-xr-x   0        0        0      471 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-inverse.svg
+-rwxr-xr-x   0        0        0      844 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg
+-rwxr-xr-x   0        0        0      903 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg
+-rwxr-xr-x   0        0        0     1092 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg
+-rwxr-xr-x   0        0        0      658 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg
+-rwxr-xr-x   0        0        0      718 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg
+-rwxr-xr-x   0        0        0      485 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick.svg
+-rwxr-xr-x   0        0        0     2749 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg
+-rwxr-xr-x   0        0        0     2067 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg
+-rw-r--r--   0        0        0     1883 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html
+-rw-r--r--   0        0        0      159 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/__init__.py
+-rw-r--r--   0        0        0     3150 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py
+-rw-r--r--   0        0        0     1343 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py
+-rw-r--r--   0        0        0     2486 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py
+-rw-r--r--   0        0        0      194 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/__init__.py
+-rw-r--r--   0        0        0      386 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/consumers.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/realtime/models.py
+-rw-r--r--   0        0        0       70 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/__init__.py
+-rw-r--r--   0        0        0      851 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py
+-rw-r--r--   0        0        0      273 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/celery.py
+-rw-r--r--   0        0        0      220 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/routing.py
+-rw-r--r--   0        0        0     2076 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py
+-rw-r--r--   0        0        0     1682 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py
+-rw-r--r--   0        0        0      443 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/wsgi.py
+-rw-r--r--   0        0        0       89 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/.gitignore
+-rw-r--r--   0        0        0     7274 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/conftest.py
+-rw-r--r--   0        0        0      451 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/features/README.md
+-rw-r--r--   0        0        0     3001 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/features/smoke-test.feature
+-rw-r--r--   0        0        0      224 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/README.md
+-rw-r--r--   0        0        0      126 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/data.py
+-rw-r--r--   0        0        0     5289 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/front.py
+-rw-r--r--   0        0        0     1033 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/reporting.py
+-rw-r--r--   0        0        0     1885 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/utils.py
+-rw-r--r--   0        0        0     5334 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/hooks.py
+-rw-r--r--   0        0        0    16126 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/report/reporter.py
+-rw-r--r--   0        0        0     2242 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/report/utils.py
+-rw-r--r--   0        0        0      142 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/__init__.py
+-rw-r--r--   0        0        0     3458 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_given.py
+-rw-r--r--   0        0        0     4797 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_then.py
+-rw-r--r--   0        0        0     3484 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_when.py
+-rw-r--r--   0        0        0     3537 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/utils.py
+-rw-r--r--   0        0        0      680 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/test_features.py
+-rw-r--r--   0        0        0    11758 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/test_utils.py
+-rwxr-xr-x   0        0        0      666 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/manage.py
+-rwxr-xr-x   0        0        0      151 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/pmanage
+-rw-r--r--   0        0        0     1473 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/pyproject.toml
+-rw-r--r--   0        0        0     3034 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.dockerignore
+-rw-r--r--   0        0        0      174 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.env-template
+-rw-r--r--   0        0        0      332 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.eslintrc.js
+-rw-r--r--   0        0        0        8 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.gitignore
+-rw-r--r--   0        0        0       13 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.nvmrc
+-rw-r--r--   0        0        0      185 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/Dockerfile
+-rw-r--r--   0        0        0     1601 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/README.md
+-rw-r--r--   0        0        0      112 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/components/blocks/title-1.vue
+-rw-r--r--   0        0        0    11513 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/components/server-templated-component.vue
+-rw-r--r--   0        0        0     2941 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/error.vue
+-rw-r--r--   0        0        0     6320 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/middleware/wagtail.ts
+-rw-r--r--   0        0        0      738 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/nuxt.config.js
+-rw-r--r--   0        0        0      884 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/package.json
+-rw-r--r--   0        0        0      655 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/pages/[...wagtail].vue
+-rw-r--r--   0        0        0       80 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/pages/no-wagtail-index.vue
+-rw-r--r--   0        0        0      483 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/plugins/dom.client.ts
+-rw-r--r--   0        0        0      505 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/plugins/dom.server.ts
+-rw-r--r--   0        0        0      439 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/stores/layout.js
+-rw-r--r--   0        0        0       98 2024-04-12 11:01:14.762648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/tsconfig.json
+-rw-r--r--   0        0        0     7602 2024-04-12 11:01:14.758648 modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template.py
+-rw-r--r--   0        0        0     6645 1970-01-01 00:00:00.000000 modelw_project_maker-2024.4.0b2/PKG-INFO
```

### Comparing `modelw_project_maker-2024.4.0b1/README.md` & `modelw_project_maker-2024.4.0b2/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/pyproject.toml` & `modelw_project_maker-2024.4.0b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-project-maker"
-version = "2024.4.0b1"
+version = "2024.4.0b2"
 packages = [
     {  include = "model_w/project_maker", from = "src" }
 ]
 
 description = "A tool to create Model-W-compliant projects"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
```

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/__main__.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/__main__.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_api.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_api.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_base.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_base.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_common.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_common.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/maker/_front.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/maker/_front.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/namer.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/namer.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/.gitignore` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/.gitignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/README.md` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/.dockerignore` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/README.md` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/migrations/0002_homepage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/cross.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder-open-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/plus.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/tick-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail-inverse.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/icons/wagtail.svg`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/cms/templates/wagtail/userbar/templates/base.html`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/models.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/serializers.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/apps/people/views.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/asgi.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/settings.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/___project_name__snake___/django/urls.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/README.md` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     definition.
 
 ## Installation
 
 After installing the project, you will need to install the Playwright browsers
 with: `playwright install` (Remember to have your virtual environment activated)
 
-## How to use in this BDD folder in a pre-existing ModelW project?
+## How to use this BDD folder in a pre-existing ModelW project?
 
 -   Copy this entire [bdd/](./) folder into /api of your ModelW project.
 -   Copy the configs in [pyproject.toml](../pyproject.toml) for:
     -   `tool.poetry.group.test.dependencies`
-    -   `tool.pytest.ini_options`
+    -   `tool.pytest.ini_options` (update settings location for your project)
 -   `poetry lock --no-update` (to sync the new dependencies)
 -   `poetry install` (to install the new dependencies)
 -   `playwright install` (in your Poetry env)
 
 ## Quick start
 
 The recipe for creating BDD tests is:
```

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/features/smoke-test.feature` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/features/smoke-test.feature`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/data.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/data.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/front.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/front.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/reporting.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/reporting.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/fixtures/utils.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/hooks.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/hooks.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/reporter.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/report/reporter.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/report/utils.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/report/utils.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_given.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_given.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_then.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_then.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/common_when.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/common_when.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/step_definitions/utils.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/step_definitions/utils.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_features.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/test_features.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/bdd/test_utils.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/bdd/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/manage.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/manage.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/api/pyproject.toml` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/.dockerignore` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/.dockerignore`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/README.md` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/README.md`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/components/server-templated-component.vue` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/components/server-templated-component.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/error.vue` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/error.vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/middleware/wagtail.ts` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/middleware/wagtail.ts`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/nuxt.config.js` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/nuxt.config.js`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/package.json` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9966666666666667%*

 * *Differences: {"'dependencies'": "{'@model-w/preset-nuxt3': '>=2024.4.0-beta.2 && <2024.5.0'}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "dependencies": {
         "@model-w/axios": "1.x",
-        "@model-w/preset-nuxt3": "2024.4.0-beta.2",
+        "@model-w/preset-nuxt3": ">=2024.4.0-beta.2 && <2024.5.0",
         "@model-w/proxy": "2.x",
         "@model-w/sentry": "1.x",
         "@pinia/nuxt": "^0.5.1",
         "@vuelidate/core": "2.0.x",
         "@vuelidate/validators": "2.0.x",
         "defu": "^6.1.4",
         "http-proxy-middleware": "^2.0.x",
```

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template/front/pages/[...wagtail].vue` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template/front/pages/[...wagtail].vue`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/src/model_w/project_maker/template.py` & `modelw_project_maker-2024.4.0b2/src/model_w/project_maker/template.py`

 * *Files identical despite different names*

### Comparing `modelw_project_maker-2024.4.0b1/PKG-INFO` & `modelw_project_maker-2024.4.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-project-maker
-Version: 2024.4.0b1
+Version: 2024.4.0b2
 Summary: A tool to create Model-W-compliant projects
 Home-page: https://github.com/ModelW/project-maker
 License: WTFPL
 Keywords: model-w,django,nuxt,boilerplate,template
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.11,<4.0
```

