# Comparing `tmp/fastapi_jsonapi-2.6.0.tar.gz` & `tmp/fastapi_jsonapi-2.7.0.tar.gz`

## Comparing `fastapi_jsonapi-2.6.0.tar` & `fastapi_jsonapi-2.7.0.tar`

### file list

```diff
@@ -1,118 +1,118 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_limited_methods.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_minimal.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/custom_filter_example.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/asgi.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/config.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/main.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/api/__init__.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/api/views_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/extensions/__init__.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/helpers/__init__.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/child.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/computer.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/enums.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/parent.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/parent_child_association.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/post.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/post_comment.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/user.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/user_bio.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/child.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/computer.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/parent.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/post.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/user.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/asgi.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/main.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/urls.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/api/__init__.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/api/user.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/__init__.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/enums.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/pydantic/user.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/tortoise/user.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/VERSION
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/__init__.py
--rw-r--r--   0        0        0    25785 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/api.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_typing.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/jsonapi_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/py.typed
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/querystring.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema_base.py
--rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema_builder.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/signature.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/splitter.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/validation_utils.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/atomic.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/atomic_handler.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py
--rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/__init__.py
--rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/base.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/orm.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/shared.py
--rw-r--r--   0        0        0    35502 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sqla_orm.py
--rw-r--r--   0        0        0    17077 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/tortoise_orm.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/fields/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/fields/enum.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/fields/mixins.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/__init__.py
--rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
--rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sorting/__init__.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/base.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/handlers.py
--rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/json_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/misc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/misc/sqla/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/misc/sqla/generics/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/misc/sqla/generics/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/__init__.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/dependency_helper.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/exceptions.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/sqla.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/__init__.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/detail_view.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/list_view.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/utils.py
--rw-r--r--   0        0        0    17855 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/view_base.py
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/LICENSE
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/README.md
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/pyproject.toml
--rw-r--r--   0        0        0     7823 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/__init__.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_limited_methods.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_minimal.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/custom_filter_example.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/asgi.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/config.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/main.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/__init__.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/views_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/helpers/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/child.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/computer.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/enums.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent_child_association.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post_comment.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user_bio.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/child.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/computer.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/asgi.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/main.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/urls.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/__init__.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/user.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/faker.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/__init__.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/enums.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/user.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/__init__.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/user.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/VERSION
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/__init__.py
+-rw-r--r--   0        0        0    25785 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/api.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_typing.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/jsonapi_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/py.typed
+-rw-r--r--   0        0        0    10504 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/querystring.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_base.py
+-rw-r--r--   0        0        0    22054 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_builder.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/signature.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/splitter.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/validation_utils.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic_handler.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py
+-rw-r--r--   0        0        0     6612 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/__init__.py
+-rw-r--r--   0        0        0    18596 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/base.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/orm.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/shared.py
+-rw-r--r--   0        0        0    37874 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sqla_orm.py
+-rw-r--r--   0        0        0    17077 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/tortoise_orm.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/enum.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/mixins.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/__init__.py
+-rw-r--r--   0        0        0    17542 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/__init__.py
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/base.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/handlers.py
+-rw-r--r--   0        0        0     5331 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/json_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/generics/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/misc/sqla/generics/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/__init__.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/dependency_helper.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/exceptions.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/sqla.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/detail_view.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/list_view.py
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/utils.py
+-rw-r--r--   0        0        0    17950 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/view_base.py
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/LICENSE
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/README.md
+-rw-r--r--   0        0        0     5160 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7869 2020-02-02 00:00:00.000000 fastapi_jsonapi-2.7.0/PKG-INFO
```

### Comparing `fastapi_jsonapi-2.6.0/examples/api_limited_methods.py` & `fastapi_jsonapi-2.7.0/examples/api_limited_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_minimal.py` & `fastapi_jsonapi-2.7.0/examples/api_minimal.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/custom_filter_example.py` & `fastapi_jsonapi-2.7.0/examples/custom_filter_example.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/main.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/urls.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/api/views_base.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/api/views_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/extensions/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/__init__.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/child.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/computer.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/computer.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/parent.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/parent_child_association.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/post.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/post_comment.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/user_bio.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/__init__.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/child.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/computer.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/computer.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/parent.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/parent_child_association.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/post.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/post_comment.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/models/schemas/user_bio.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/base_model_mixin.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py` & `fastapi_jsonapi-2.7.0/examples/api_for_sqlalchemy/utils/sqlalchemy/fields/enum.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/main.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/urls.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/urls.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/api/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/api/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/factories/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/factories/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/meta_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/helpers/updaters/update_user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/pydantic/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/pydantic/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/examples/api_for_tortoise_orm/models/tortoise/user.py` & `fastapi_jsonapi-2.7.0/examples/api_for_tortoise_orm/models/tortoise/user.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/__init__.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/api.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/api.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/querystring.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/querystring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """Helper to deal with querystring parameters according to jsonapi specification."""
+from collections import defaultdict
 from functools import cached_property
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Optional,
     Type,
-    Union,
 )
 from urllib.parse import unquote
 
 import simplejson as json
 from fastapi import (
     FastAPI,
     Request,
 )
 from pydantic import (
     BaseModel,
     Field,
 )
 from starlette.datastructures import QueryParams
 
+from fastapi_jsonapi.api import RoutersJSONAPI
 from fastapi_jsonapi.exceptions import (
     BadRequest,
     InvalidField,
     InvalidFilters,
     InvalidInclude,
     InvalidSort,
+    InvalidType,
 )
 from fastapi_jsonapi.schema import (
     get_model_field,
     get_relationships,
-    get_schema_from_type,
 )
 from fastapi_jsonapi.splitter import SPLIT_REL
 
 if TYPE_CHECKING:
     from fastapi_jsonapi.data_typing import TypeSchema
 
 
@@ -85,41 +86,53 @@
         self.qs: QueryParams = request.query_params
         self.config: Dict[str, Any] = getattr(self.app, "config", {})
         self.ALLOW_DISABLE_PAGINATION: bool = self.config.get("ALLOW_DISABLE_PAGINATION", True)
         self.MAX_PAGE_SIZE: int = self.config.get("MAX_PAGE_SIZE", 10000)
         self.MAX_INCLUDE_DEPTH: int = self.config.get("MAX_INCLUDE_DEPTH", 3)
         self.headers: HeadersQueryStringManager = HeadersQueryStringManager(**dict(self.request.headers))
 
-    def _get_key_values(self, name: str) -> Dict[str, Union[List[str], str]]:
+    def _extract_item_key(self, key: str) -> str:
+        try:
+            key_start = key.index("[") + 1
+            key_end = key.index("]")
+            return key[key_start:key_end]
+        except Exception:
+            msg = "Parse error"
+            raise BadRequest(msg, parameter=key)
+
+    def _get_unique_key_values(self, name: str) -> Dict[str, str]:
         """
         Return a dict containing key / values items for a given key, used for items like filters, page, etc.
 
         :param name: name of the querystring parameter
         :return: a dict of key / values items
         :raises BadRequest: if an error occurred while parsing the querystring.
         """
-        results: Dict[str, Union[List[str], str]] = {}
+        results = {}
 
         for raw_key, value in self.qs.multi_items():
             key = unquote(raw_key)
-            try:
-                if not key.startswith(name):
-                    continue
+            if not key.startswith(name):
+                continue
 
-                key_start = key.index("[") + 1
-                key_end = key.index("]")
-                item_key = key[key_start:key_end]
-
-                if "," in value:
-                    results.update({item_key: value.split(",")})
-                else:
-                    results.update({item_key: value})
-            except Exception:
-                msg = "Parse error"
-                raise BadRequest(msg, parameter=key)
+            item_key = self._extract_item_key(key)
+            results[item_key] = value
+
+        return results
+
+    def _get_multiple_key_values(self, name: str) -> Dict[str, List]:
+        results = defaultdict(list)
+
+        for raw_key, value in self.qs.multi_items():
+            key = unquote(raw_key)
+            if not key.startswith(name):
+                continue
+
+            item_key = self._extract_item_key(key)
+            results[item_key].extend(value.split(","))
 
         return results
 
     @classmethod
     def _simple_filters(cls, dict_: Dict[str, Any]) -> List[Dict[str, Any]]:
         """Filter creation."""
         return [{"name": key, "op": "eq", "val": value} for (key, value) in dict_.items()]
@@ -130,15 +143,15 @@
         Return original querystring but containing only managed keys.
 
         :return: dict of managed querystring parameter
         """
         return {
             key: value
             for (key, value) in self.qs.multi_items()
-            if key.startswith(self.managed_keys) or self._get_key_values("filter[")
+            if key.startswith(self.managed_keys) or self._get_unique_key_values("filter[")
         }
 
     @property
     def filters(self) -> List[dict]:
         """
         Return filters from query string.
 
@@ -155,16 +168,16 @@
                 raise InvalidFilters(msg)
 
             if not isinstance(loaded_filters, list):
                 msg = f"Incorrect filters format, expected list of conditions but got {type(loaded_filters).__name__}"
                 raise InvalidFilters(msg)
 
             results.extend(loaded_filters)
-        if self._get_key_values("filter["):
-            results.extend(self._simple_filters(self._get_key_values("filter[")))
+        if filter_key_values := self._get_unique_key_values("filter["):
+            results.extend(self._simple_filters(filter_key_values))
         return results
 
     @cached_property
     def pagination(self) -> PaginationQueryStringManager:
         """
         Return all page parameters as a dict.
 
@@ -182,29 +195,27 @@
             query_string = {'page[number]': '25', 'page[size]': '10'}
             parsed_query.pagination
             {'number': '25', 'size': '10'}
 
         :raises BadRequest: if the client is not allowed to disable pagination.
         """
         # check values type
-        pagination_data: Dict[str, Union[List[str], str]] = self._get_key_values("page")
+        pagination_data: Dict[str, str] = self._get_unique_key_values("page")
         pagination = PaginationQueryStringManager(**pagination_data)
         if pagination_data.get("size") is None:
             pagination.size = None
         if pagination.size:
             if self.ALLOW_DISABLE_PAGINATION is False and pagination.size == 0:
                 msg = "You are not allowed to disable pagination"
                 raise BadRequest(msg, parameter="page[size]")
             if self.MAX_PAGE_SIZE and pagination.size > self.MAX_PAGE_SIZE:
                 pagination.size = self.MAX_PAGE_SIZE
 
         return pagination
 
-    # TODO: finally use this! upgrade Sqlachemy Data Layer
-    #  and add to all views (get list/detail, create, patch)
     @property
     def fields(self) -> Dict[str, List[str]]:
         """
         Return fields wanted by client.
 
         :return: a dict of sparse fieldsets information
 
@@ -212,34 +223,40 @@
 
             {
                 "user": ['name', 'email'],
             }
 
         :raises InvalidField: if result field not in schema.
         """
-        if self.request.method != "GET":
-            msg = "attribute 'fields' allowed only for GET-method"
-            raise InvalidField(msg)
-        fields = self._get_key_values("fields")
-        for key, value in fields.items():
-            if not isinstance(value, list):
-                value = [value]  # noqa: PLW2901
-                fields[key] = value
+        fields = self._get_multiple_key_values("fields")
+        for resource_type, field_names in fields.items():
             # TODO: we have registry for models (BaseModel)
             # TODO: create `type to schemas` registry
-            schema: Type[BaseModel] = get_schema_from_type(key, self.app)
-            for field in value:
-                if field not in schema.__fields__:
+
+            if resource_type not in RoutersJSONAPI.all_jsonapi_routers:
+                msg = f"Application has no resource with type {resource_type!r}"
+                raise InvalidType(msg)
+
+            schema: Type[BaseModel] = self._get_schema(resource_type)
+
+            for field_name in field_names:
+                if field_name == "":
+                    continue
+
+                if field_name not in schema.__fields__:
                     msg = "{schema} has no attribute {field}".format(
                         schema=schema.__name__,
-                        field=field,
+                        field=field_name,
                     )
                     raise InvalidField(msg)
 
-        return fields
+        return {resource_type: set(field_names) for resource_type, field_names in fields.items()}
+
+    def _get_schema(self, resource_type: str) -> Type[BaseModel]:
+        return RoutersJSONAPI.all_jsonapi_routers[resource_type]._schema
 
     def get_sorts(self, schema: Type["TypeSchema"]) -> List[Dict[str, str]]:
         """
         Return fields to sort by including sort name for SQLAlchemy and row sort parameter for other ORMs.
 
         :return: a list of sorting information
```

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema_base.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/schema_builder.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/schema_builder.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/signature.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/signature.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/validation_utils.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/validation_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/atomic.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/atomic_handler.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/atomic_handler.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/prepared_atomic_operation.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/atomic/schemas.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/atomic/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/base.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/shared.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/shared.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sqla_orm.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sqla_orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module is a CRUD interface between resource managers and the sqlalchemy ORM"""
 import logging
-from typing import TYPE_CHECKING, Any, Iterable, List, Optional, Tuple, Type
+from typing import TYPE_CHECKING, Any, Iterable, List, Literal, Optional, Tuple, Type, Union
 
 from sqlalchemy import delete, func, select
-from sqlalchemy.exc import DBAPIError, IntegrityError, NoResultFound
+from sqlalchemy.exc import DBAPIError, IntegrityError, MissingGreenlet, NoResultFound
 from sqlalchemy.ext.asyncio import AsyncSession, AsyncSessionTransaction
 from sqlalchemy.inspection import inspect
 from sqlalchemy.orm import joinedload, selectinload
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.orm.collections import InstrumentedList
 from sqlalchemy.sql import column, distinct
 
@@ -40,14 +40,17 @@
 
 if TYPE_CHECKING:
     from pydantic import BaseModel as PydanticBaseModel
     from sqlalchemy.sql import Select
 
 log = logging.getLogger(__name__)
 
+ModelTypeOneOrMany = Union[TypeModel, list[TypeModel]]
+ActionTrigger = Literal["create", "update"]
+
 
 class SqlalchemyDataLayer(BaseDataLayer):
     """Sqlalchemy data layer"""
 
     def __init__(
         self,
         schema: Type[TypeSchema],
@@ -130,20 +133,96 @@
 
         py_type = col.type.python_type
         if not isinstance(value, py_type):
             value = py_type(value)
 
         return value
 
-    async def apply_relationships(self, obj: TypeModel, data_create: BaseJSONAPIItemInSchema) -> None:
+    async def link_relationship_object(
+        self,
+        obj: TypeModel,
+        relation_name: str,
+        related_data: Optional[ModelTypeOneOrMany],
+        action_trigger: ActionTrigger,
+    ):
         """
-        TODO: move generic code to another method
+        Links target object with relationship object or objects
+
+        :param obj:
+        :param relation_name:
+        :param related_data:
+        :param action_trigger: indicates which one operation triggered relationships applying
+        """
+        # todo: relation name may be different?
+        setattr(obj, relation_name, related_data)
+
+    async def check_object_has_relationship_or_raise(self, obj: TypeModel, relation_name: str):
+        """
+        Checks that there is relationship with relation_name in obj
+
+        :param obj:
+        :param relation_name:
+        """
+        try:
+            hasattr(obj, relation_name)
+        except MissingGreenlet:
+            raise InternalServerError(
+                detail=(
+                    f"Error of loading the {relation_name!r} relationship. "
+                    f"Please add this relationship to include query parameter explicitly."
+                ),
+                parameter="include",
+            )
+
+    async def get_related_data_to_link(
+        self,
+        related_model: TypeModel,
+        relationship_info: RelationshipInfo,
+        relationship_in: Union[
+            BaseJSONAPIRelationshipDataToOneSchema,
+            BaseJSONAPIRelationshipDataToManySchema,
+        ],
+    ) -> Optional[ModelTypeOneOrMany]:
+        """
+        Retrieves object or objects to link from database
+
+        :param related_model:
+        :param relationship_info:
+        :param relationship_in:
+        """
+        if not relationship_in.data:
+            return [] if relationship_info.many else None
+
+        if relationship_info.many:
+            assert isinstance(relationship_in, BaseJSONAPIRelationshipDataToManySchema)
+            return await self.get_related_objects_list(
+                related_model=related_model,
+                related_id_field=relationship_info.id_field_name,
+                ids=[r.id for r in relationship_in.data],
+            )
+
+        assert isinstance(relationship_in, BaseJSONAPIRelationshipDataToOneSchema)
+        return await self.get_related_object(
+            related_model=related_model,
+            related_id_field=relationship_info.id_field_name,
+            id_value=relationship_in.data.id,
+        )
+
+    async def apply_relationships(
+        self,
+        obj: TypeModel,
+        data_create: BaseJSONAPIItemInSchema,
+        action_trigger: ActionTrigger,
+    ) -> None:
+        """
+        Handles relationships passed in request
 
         :param obj:
         :param data_create:
+        :param action_trigger: indicates which one operation triggered relationships applying
         :return:
         """
         relationships: "PydanticBaseModel" = data_create.relationships
         if relationships is None:
             return
 
         schema_fields = self.schema.__fields__ or {}
@@ -163,34 +242,23 @@
                     "relationship info for %s in schema %s extra not found",
                     relation_name,
                     self.schema.__name__,
                 )
                 continue
 
             relationship_info: RelationshipInfo = field.field_info.extra["relationship"]
-
-            # ...
             related_model = get_related_model_cls(type(obj), relation_name)
+            related_data = await self.get_related_data_to_link(
+                related_model=related_model,
+                relationship_info=relationship_info,
+                relationship_in=relationship_in,
+            )
 
-            if relationship_info.many:
-                assert isinstance(relationship_in, BaseJSONAPIRelationshipDataToManySchema)
-                related_data = await self.get_related_objects_list(
-                    related_model=related_model,
-                    related_id_field=relationship_info.id_field_name,
-                    ids=[r.id for r in relationship_in.data],
-                )
-            else:
-                assert isinstance(relationship_in, BaseJSONAPIRelationshipDataToOneSchema)
-                related_data = await self.get_related_object(
-                    related_model=related_model,
-                    related_id_field=relationship_info.id_field_name,
-                    id_value=relationship_in.data.id,
-                )
-            # todo: relation name may be different?
-            setattr(obj, relation_name, related_data)
+            await self.check_object_has_relationship_or_raise(obj, relation_name)
+            await self.link_relationship_object(obj, relation_name, related_data, action_trigger)
 
     async def create_object(self, data_create: BaseJSONAPIItemInSchema, view_kwargs: dict) -> TypeModel:
         """
         Create an object through sqlalchemy.
 
         :param data_create: the data validated by pydantic.
         :param view_kwargs: kwargs from the resource view.
@@ -199,15 +267,15 @@
         log.debug("Create object with data %s", data_create)
         # todo: pydantic v2 model_dump()
         model_kwargs = data_create.attributes.dict()
         model_kwargs = self._apply_client_generated_id(data_create, model_kwargs=model_kwargs)
         await self.before_create_object(model_kwargs=model_kwargs, view_kwargs=view_kwargs)
 
         obj = self.model(**model_kwargs)
-        await self.apply_relationships(obj, data_create)
+        await self.apply_relationships(obj, data_create, action_trigger="create")
 
         self.session.add(obj)
         try:
             await self.save()
         except IntegrityError:
             log.exception("Could not create object with data create %s", data_create)
             msg = "Object creation error"
@@ -325,15 +393,15 @@
         :param obj: an object from sqlalchemy.
         :param data_update: the data validated by pydantic.
         :param view_kwargs: kwargs from the resource view.
         :return: True if object have changed else False.
         """
         new_data = data_update.attributes.dict(exclude_unset=True)
 
-        await self.apply_relationships(obj, data_update)
+        await self.apply_relationships(obj, data_update, action_trigger="update")
 
         await self.before_update_object(obj, model_kwargs=new_data, view_kwargs=view_kwargs)
 
         missing = object()
 
         has_updated = False
         for field_name, new_value in new_data.items():
@@ -382,16 +450,18 @@
         """
         Delete an object through sqlalchemy.
 
         :param obj: an item from sqlalchemy.
         :param view_kwargs: kwargs from the resource view.
         """
         await self.before_delete_object(obj, view_kwargs)
+        stmt = delete(self.model).where(self.model.id == obj.id)
+
         try:
-            await self.session.delete(obj)
+            await self.session.execute(stmt)
             await self.save()
         except DBAPIError as e:
             await self.session.rollback()
 
             err_message = f"Got an error {e.__class__.__name__} deleting object {view_kwargs}"
             log.error(err_message, exc_info=e)
```

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/tortoise_orm.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/fields/mixins.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_operation.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/filtering/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/data_layers/sorting/tortoise_orm.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/__init__.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/base.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/exceptions/json_api.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/exceptions/json_api.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/dependency_helper.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/dependency_helper.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/utils/sqla.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/utils/sqla.py`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/detail_view.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/detail_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 )
 
 from fastapi_jsonapi import BadRequest
 from fastapi_jsonapi.schema import (
     BaseJSONAPIItemInSchema,
     JSONAPIResultDetailSchema,
 )
+from fastapi_jsonapi.views.utils import handle_jsonapi_fields
 from fastapi_jsonapi.views.view_base import ViewBase
 
 if TYPE_CHECKING:
     from fastapi_jsonapi.data_layers.base import BaseDataLayer
 
 logger = logging.getLogger(__name__)
 
@@ -30,30 +31,32 @@
     ) -> "BaseDataLayer":
         return await self.get_data_layer_for_detail(extra_view_deps)
 
     async def handle_get_resource_detail(
         self,
         object_id: Union[int, str],
         **extra_view_deps,
-    ):
+    ) -> Union[JSONAPIResultDetailSchema, Dict]:
         dl: "BaseDataLayer" = await self.get_data_layer(extra_view_deps)
 
         view_kwargs = {dl.url_id_field: object_id}
         db_object = await dl.get_object(view_kwargs=view_kwargs, qs=self.query_params)
 
-        return self._build_detail_response(db_object)
+        response = self._build_detail_response(db_object)
+        return handle_jsonapi_fields(response, self.query_params, self.jsonapi)
 
     async def handle_update_resource(
         self,
         obj_id: str,
         data_update: BaseJSONAPIItemInSchema,
         **extra_view_deps,
-    ) -> JSONAPIResultDetailSchema:
+    ) -> Union[JSONAPIResultDetailSchema, Dict]:
         dl: "BaseDataLayer" = await self.get_data_layer(extra_view_deps)
-        return await self.process_update_object(dl=dl, obj_id=obj_id, data_update=data_update)
+        response = await self.process_update_object(dl=dl, obj_id=obj_id, data_update=data_update)
+        return handle_jsonapi_fields(response, self.query_params, self.jsonapi)
 
     async def process_update_object(
         self,
         dl: "BaseDataLayer",
         obj_id: str,
         data_update: BaseJSONAPIItemInSchema,
     ):
```

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/list_view.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/list_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, Union
 
 from fastapi_jsonapi.schema import (
     BaseJSONAPIItemInSchema,
     JSONAPIResultDetailSchema,
     JSONAPIResultListSchema,
 )
+from fastapi_jsonapi.views.utils import handle_jsonapi_fields
 from fastapi_jsonapi.views.view_base import ViewBase
 
 if TYPE_CHECKING:
     from fastapi_jsonapi.data_layers.base import BaseDataLayer
 
 logger = logging.getLogger(__name__)
 
@@ -30,29 +31,31 @@
 
     async def get_data_layer(
         self,
         extra_view_deps: Dict[str, Any],
     ) -> "BaseDataLayer":
         return await self.get_data_layer_for_list(extra_view_deps)
 
-    async def handle_get_resource_list(self, **extra_view_deps) -> JSONAPIResultListSchema:
+    async def handle_get_resource_list(self, **extra_view_deps) -> Union[JSONAPIResultListSchema, Dict]:
         dl: "BaseDataLayer" = await self.get_data_layer(extra_view_deps)
         query_params = self.query_params
         count, items_from_db = await dl.get_collection(qs=query_params)
         total_pages = self._calculate_total_pages(count)
 
-        return self._build_list_response(items_from_db, count, total_pages)
+        response = self._build_list_response(items_from_db, count, total_pages)
+        return handle_jsonapi_fields(response, query_params, self.jsonapi)
 
     async def handle_post_resource_list(
         self,
         data_create: BaseJSONAPIItemInSchema,
         **extra_view_deps,
-    ) -> JSONAPIResultDetailSchema:
+    ) -> Union[JSONAPIResultDetailSchema, Dict]:
         dl: "BaseDataLayer" = await self.get_data_layer(extra_view_deps)
-        return await self.process_create_object(dl=dl, data_create=data_create)
+        response = await self.process_create_object(dl=dl, data_create=data_create)
+        return handle_jsonapi_fields(response, self.query_params, self.jsonapi)
 
     async def process_create_object(self, dl: "BaseDataLayer", data_create: BaseJSONAPIItemInSchema):
         created_object = await dl.create_object(data_create=data_create, view_kwargs={})
 
         created_object_id = dl.get_object_id(created_object)
 
         view_kwargs = {dl.url_id_field: created_object_id}
@@ -64,8 +67,9 @@
         dl: "BaseDataLayer" = await self.get_data_layer(extra_view_deps)
         query_params = self.query_params
         count, items_from_db = await dl.get_collection(qs=query_params)
         total_pages = self._calculate_total_pages(count)
 
         await dl.delete_objects(items_from_db, {})
 
-        return self._build_list_response(items_from_db, count, total_pages)
+        response = self._build_list_response(items_from_db, count, total_pages)
+        return handle_jsonapi_fields(response, self.query_params, self.jsonapi)
```

### Comparing `fastapi_jsonapi-2.6.0/fastapi_jsonapi/views/view_base.py` & `fastapi_jsonapi-2.7.0/fastapi_jsonapi/views/view_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from fastapi_jsonapi.data_typing import (
     TypeModel,
     TypeSchema,
 )
 from fastapi_jsonapi.schema import (
     JSONAPIObjectSchema,
     JSONAPIResultListMetaSchema,
+    JSONAPIResultListSchema,
     get_related_schema,
 )
 from fastapi_jsonapi.schema_base import BaseModel, RelationshipInfo
 from fastapi_jsonapi.schema_builder import JSONAPIObjectSchemas
 from fastapi_jsonapi.splitter import SPLIT_REL
 from fastapi_jsonapi.views.utils import (
     HTTPMethod,
@@ -181,15 +182,20 @@
             name=f"Result{self.__class__.__name__}",
             object_jsonapi_schema=object_schemas.object_jsonapi_schema,
             includes_schemas=object_schemas.included_schemas_list,
         )
 
         return detail_jsonapi_schema(data=result_object, **extras)
 
-    def _build_list_response(self, items_from_db: List[TypeModel], count: int, total_pages: int):
+    def _build_list_response(
+        self,
+        items_from_db: List[TypeModel],
+        count: int,
+        total_pages: int,
+    ) -> JSONAPIResultListSchema:
         result_objects, object_schemas, extras = self._build_response(items_from_db, self.jsonapi.schema_list)
 
         # we need to build a new schema here
         # because we'd like to exclude some fields (relationships, includes, etc)
         list_jsonapi_schema = self.jsonapi.schema_builder.build_schema_for_list_result(
             name=f"Result{self.__class__.__name__}",
             object_jsonapi_schema=object_schemas.object_jsonapi_schema,
```

### Comparing `fastapi_jsonapi-2.6.0/.gitignore` & `fastapi_jsonapi-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/LICENSE` & `fastapi_jsonapi-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/README.md` & `fastapi_jsonapi-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_jsonapi-2.6.0/pyproject.toml` & `fastapi_jsonapi-2.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dynamic = ["version"]
 description = "FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)"
 readme = "README.md"
 license = "MIT"
 authors = [
     { name = "Aleksey Nekrasov", email = "a.nekrasov@mts.ai" },
     { name = "Suren Khorenyan", email = "s.khorenyan@mts.ai" },
+    { name = "German Bernadskiy", email = "german11235813@gmail.com" },
 ]
 keywords = [
     "fastapi",
     "jsonapi",
     "json:api",
 ]
 classifiers = [
@@ -68,24 +69,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = [
     "fastapi_jsonapi"
 ]
 
 [tool.poetry]
-name = "fastapi-jsonapi"
-version = "2.6.0"
-description = "FastAPI extension to create REST web api according to JSON:API specification"
-authors = [
-    "Aleksei Nekrasov <nekrasov.aleks@mail.ru>",
-    "Suren Khorenyan <surenkhorenyan@gmail.com>",
-    "German Bernadskiy <german11235813@gmail.com>",
-]
-license = "MIT"
-readme = "README.md"
+package-mode = false
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = ">=0.79.0"
 pydantic = ">=1.9.1"
 simplejson = ">=3.17.6"
 uvicorn = ">=0.18.2"
```

### Comparing `fastapi_jsonapi-2.6.0/PKG-INFO` & `fastapi_jsonapi-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: FastAPI-JSONAPI
-Version: 2.6.0
+Version: 2.7.0
 Summary: FastAPI extension to create REST web api according to JSON:API 1.0 specification with FastAPI, Pydantic and data provider of your choice (SQLAlchemy, Tortoise ORM)
 Project-URL: Documentation, https://fastapi-jsonapi.readthedocs.io/
 Project-URL: Source, https://github.com/mts-ai/FastAPI-JSONAPI
-Author-email: Aleksey Nekrasov <a.nekrasov@mts.ai>, Suren Khorenyan <s.khorenyan@mts.ai>
+Author-email: Aleksey Nekrasov <a.nekrasov@mts.ai>, Suren Khorenyan <s.khorenyan@mts.ai>, German Bernadskiy <german11235813@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: fastapi,json:api,jsonapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

