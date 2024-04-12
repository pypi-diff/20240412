# Comparing `tmp/fastapi_cruddy_framework-1.4.6.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.6.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.7.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.6.tar` & `fastapi_cruddy_framework-1.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.6/LICENSE
--rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.6/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    41190 2024-04-03 20:42:10.151471 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-04-10 21:01:56.572172 fastapi_cruddy_framework-1.4.6/pyproject.toml
--rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.7/LICENSE
+-rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.7/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    44639 2024-04-12 16:37:02.252154 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-04-12 16:37:41.085216 fastapi_cruddy_framework-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.7/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.6/LICENSE` & `fastapi_cruddy_framework-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/README.md` & `fastapi_cruddy_framework-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -628,15 +628,15 @@
 
 
 # -------------------------------------------------------------------------------------------
 # UTILITY FUNCTIONS FOR CONTROLLER CONFIGURATION
 # -------------------------------------------------------------------------------------------
 
 
-def assemblePolicies(*args: (Sequence)):
+def assemble_policies(*args: (Sequence)):
     merged = []
     for policy_set in args:
         for individual_policy in policy_set:
             merged.append(Depends(individual_policy))
     return merged
 
 
@@ -662,21 +662,22 @@
     # 2. Primary resource policies
     # 3. Related resource policies
     @controller.get(
         f'/{"{id}"}/{relationship_prop}',
         description=f"Get the '{foreign_model_name}' a '{resource_model_name}' belongs to",
         response_model=config.foreign_resource.schemas["single"],
         response_model_exclude_none=True,
-        dependencies=assemblePolicies(
+        dependencies=assemble_policies(
             policies_universal,
             policies_get_one,
             config.foreign_resource.policies["get_one"],
         ),
     )
     async def get_many_to_one(
+        request: Request,
         id: id_type = Path(..., alias="id"),
         columns: list[str] = Query(None, alias="columns"),
         where: Json = Query(None, alias="where"),
     ):
         origin_record: CruddyModel | None = await repository.get_by_id(id=id)
 
         # Consider raising 404 here and in get by ID
@@ -684,64 +685,96 @@
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND, detail=f"Record {id} not found"
             )
 
         # Build a query to use foreign resource to find related objects
 
         tgt_id = origin_record.model_dump()[near_col_name]
-        must_be = {far_col_name: {"*eq": tgt_id}}
-        where = must_be if where is None else {"*and": [must_be, where]}
 
-        _lifecycle_before = None
-        foreign_lifecycle_before = config.foreign_resource.repository.lifecycle[
+        _repo_lifecycle_before = None
+        foreign_repo_lifecycle_before = config.foreign_resource.repository.lifecycle[
             "before_get_one"
         ]
-        foreign_lifecycle_after = config.foreign_resource.repository.lifecycle[
+        foreign_repo_lifecycle_after = config.foreign_resource.repository.lifecycle[
             "after_get_one"
         ]
-        if foreign_lifecycle_before != None:
+        context_data = {
+            DATA_KEY: {
+                "id": tgt_id,
+                "where": where,
+            },
+            META_KEY: None,
+        }
+        # Execute the foreign controller lifecycle!
+        if config.foreign_resource.controller_lifecycles["before_get_one"]:
+            # If there is a user space lifecycle hook, run it (allows context mutations)
+            await config.foreign_resource.controller_lifecycles["before_get_one"](
+                request, context_data
+            )
+
+        must_be = {far_col_name: {"*eq": context_data[DATA_KEY]["id"]}}
+
+        if foreign_repo_lifecycle_before:
 
-            async def _shimmed_lifecycle_before():
-                await foreign_lifecycle_before(tgt_id)
+            async def _shimmed_repo_lifecycle_before(query_conf: dict):
+                shim_where = query_conf["where"]
+                await foreign_repo_lifecycle_before(
+                    context_data[DATA_KEY]["id"], shim_where
+                )
+                shim_where = (
+                    must_be if shim_where is None else {"*and": [must_be, shim_where]}
+                )
+                query_conf["where"] = shim_where
                 return
 
-            _lifecycle_before = _shimmed_lifecycle_before
+            _repo_lifecycle_before = _shimmed_repo_lifecycle_before
+        else:
+            where = must_be if where is None else {"*and": [must_be, where]}
 
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await config.foreign_resource.repository.get_all(
             page=1,
             limit=1,
             columns=columns,
             sort=None,
-            where=where,
+            where=context_data[DATA_KEY]["where"],
             _use_own_hooks=False,
-            _lifecycle_before=_lifecycle_before,
+            _lifecycle_before=_repo_lifecycle_before,
         )
 
         # If we get a result, grab the first value. There should only be one in many to one.
         data: dict[str, Any] | None = None
         if len(result.data) != 0:
             row_data: Row = result.data[0]
             table_record: CruddyModel = config.foreign_resource.repository.model(
                 **row_data._mapping
             )
-            if foreign_lifecycle_after != None:
-                await foreign_lifecycle_after(table_record)
+            if foreign_repo_lifecycle_after:
+                await foreign_repo_lifecycle_after(table_record)
             data = table_record.model_dump()
-        else:
-            if foreign_lifecycle_after != None:
-                await foreign_lifecycle_after(None)
+        elif foreign_repo_lifecycle_after:
+            await foreign_repo_lifecycle_after(None)
 
         if data is None:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND, detail="Record not found"
             )
 
+        context_data[DATA_KEY] = data
+
+        # If there is a user space lifecycle hook, run it (allows context mutations)
+        if config.foreign_resource.controller_lifecycles["after_get_one"]:
+            await config.foreign_resource.controller_lifecycles["after_get_one"](
+                request, context_data
+            )
+
         # Invoke the dynamically built model
-        return config.foreign_resource.schemas["single"](**{DATA_KEY: data})
+        return config.foreign_resource.schemas["single"](
+            **{DATA_KEY: context_data[DATA_KEY]}
+        )
 
 
 def _ControllerConfigOneToMany(
     controller: APIRouter,
     repository: "AbstractRepository",
     id_type: possible_id_types,
     relationship_prop: str,
@@ -765,21 +798,22 @@
     # 2. Primary resource policies
     # 3. Related resource policies
     @controller.get(
         f'/{"{id}"}/{relationship_prop}',
         description=f"Get all '{foreign_model_name}' belonging to a '{resource_model_name}'",
         response_model=config.foreign_resource.schemas["many"],
         response_model_exclude_none=True,
-        dependencies=assemblePolicies(
+        dependencies=assemble_policies(
             policies_universal,
             policies_get_one,
             config.foreign_resource.policies["get_many"],
         ),
     )
     async def get_one_to_many(
+        request: Request,
         id: id_type = Path(..., alias="id"),
         page: int = 1,
         limit: int = default_limit,
         columns: list[str] = Query(None, alias="columns"),
         sort: list[str] = Query(None, alias="sort"),
         where: Json = Query(None, alias="where"),
     ):
@@ -791,59 +825,89 @@
                 status_code=status.HTTP_404_NOT_FOUND, detail=f"Record {id} not found"
             )
 
         # Build a query to use foreign resource to find related objects
         additional_where = {
             far_col_name: {"*eq": origin_record.model_dump()[near_col_name]}
         }
-        if where != None:
-            repo_where = {"*and": [additional_where, where]}
-        else:
-            repo_where = additional_where
 
-        _lifecycle_before = None
-        foreign_lifecycle_before = config.foreign_resource.repository.lifecycle[
+        _repo_lifecycle_before = None
+        foreign_repo_lifecycle_before = config.foreign_resource.repository.lifecycle[
             "before_get_all"
         ]
 
+        context_data = {
+            DATA_KEY: {
+                "page": page,
+                "limit": limit,
+                "columns": columns,
+                "sort": sort,
+                "where": where,
+            },
+            META_KEY: None,
+        }
+
+        # If there is a user space lifecycle hook, run it (allows context mutations)
+        if config.foreign_resource.controller_lifecycles["before_get_all"]:
+            await config.foreign_resource.controller_lifecycles["before_get_all"](
+                request, context_data
+            )
+
         # This will shim the lifecycle hook so it does not see the relational portion of the query
         # but can still alter the general search object as if its a single resource query.
         # This is good because a lifecycle hook should only be concerned about its own resource.
-        if foreign_lifecycle_before != None:
+        if foreign_repo_lifecycle_before:
 
-            async def _shimmed_lifecycle_before(query_conf):
-                local_where = query_conf["where"]
-                query_conf["where"] = where
-                await foreign_lifecycle_before(query_conf)
-                query_conf["where"] = local_where
+            async def _shimmed_repo_lifecycle_before(query_conf):
+                await foreign_repo_lifecycle_before(query_conf)
+                shim_where = query_conf["where"]
+                query_conf["where"] = (
+                    additional_where
+                    if shim_where is None
+                    else {"*and": [additional_where, shim_where]}
+                )
                 return
 
-            _lifecycle_before = _shimmed_lifecycle_before
+            _repo_lifecycle_before = _shimmed_repo_lifecycle_before
+        else:
+            context_data[DATA_KEY]["where"] = (
+                additional_where
+                if context_data[DATA_KEY]["where"] is None
+                else {"*and": [additional_where, context_data[DATA_KEY]["where"]]}
+            )
 
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await config.foreign_resource.repository.get_all(
-            page=page,
-            limit=limit,
-            columns=columns,
-            sort=sort,
-            where=repo_where,
-            _lifecycle_before=_lifecycle_before,
+            **context_data[DATA_KEY],
+            _lifecycle_before=_repo_lifecycle_before,
             _lifecycle_after=config.foreign_resource.repository.lifecycle[
                 "after_get_all"
             ],
             _use_own_hooks=False,
         )
-        meta = {
+
+        context_data[DATA_KEY] = result.data
+        context_data[META_KEY] = {
             "page": result.page,
             "limit": result.limit,
             "pages": result.total_pages,
             "records": result.total_records,
         }
+
+        # If there is a user space lifecycle hook, run it (allows context mutations)
+        if config.foreign_resource.controller_lifecycles["after_get_all"]:
+            await config.foreign_resource.controller_lifecycles["after_get_all"](
+                request, context_data
+            )
+
         return config.foreign_resource.schemas["many"](
-            **{META_KEY: meta_schema(**meta), DATA_KEY: result.data}
+            **{
+                META_KEY: meta_schema(**context_data[META_KEY]),
+                DATA_KEY: context_data[DATA_KEY],
+            }
         )
 
 
 def _ControllerConfigManyToMany(
     controller: APIRouter,
     repository: "AbstractRepository",
     id_type: possible_id_types,
@@ -865,60 +929,86 @@
     # 2. Primary resource policies
     # 3. Related resource policies
     @controller.get(
         f'/{"{id}"}/{relationship_prop}',
         description=f"Get all '{foreign_model_name}' related to a '{resource_model_name}'",
         response_model=config.foreign_resource.schemas["many"],
         response_model_exclude_none=True,
-        dependencies=assemblePolicies(
+        dependencies=assemble_policies(
             policies_universal,
             policies_get_one,
             config.foreign_resource.policies["get_many"],
         ),
     )
     async def get_many_to_many(
+        request: Request,
         id: id_type = Path(..., alias="id"),
         page: int = 1,
         limit: int = default_limit,
         columns: list[str] = Query(None, alias="columns"),
         sort: list[str] = Query(None, alias="sort"),
         where: Json = Query(None, alias="where"),
     ):
         # Consider raising 404 here and in get by ID
         if await repository.get_by_id(id=id) == None:
             raise HTTPException(
                 status_code=status.HTTP_404_NOT_FOUND, detail=f"Record {id} not found"
             )
 
+        context_data = {
+            DATA_KEY: {
+                "page": page,
+                "limit": limit,
+                "columns": columns,
+                "sort": sort,
+                "where": where,
+            },
+            META_KEY: None,
+        }
+
+        # If there is a user space lifecycle hook, run it (allows context mutations)
+        if config.foreign_resource.controller_lifecycles["before_get_all"]:
+            await config.foreign_resource.controller_lifecycles["before_get_all"](
+                request, context_data
+            )
+
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await repository.get_all_relations(
             id=id,
             relation=relationship_prop,
             relation_model=far_model,
-            page=page,
-            limit=limit,
-            columns=columns,
-            sort=sort,
-            where=where,
+            **context_data[DATA_KEY],
             # the foreign resource must interact with its own lifecycle
             _lifecycle_before=config.foreign_resource.repository.lifecycle[
                 "before_get_all"
             ],
             _lifecycle_after=config.foreign_resource.repository.lifecycle[
                 "after_get_all"
             ],
         )
-        meta = {
+
+        context_data[DATA_KEY] = result.data
+        context_data[META_KEY] = {
             "page": result.page,
             "limit": result.limit,
             "pages": result.total_pages,
             "records": result.total_records,
         }
+
+        # If there is a user space lifecycle hook, run it (allows context mutations)
+        if config.foreign_resource.controller_lifecycles["after_get_all"]:
+            await config.foreign_resource.controller_lifecycles["after_get_all"](
+                request, context_data
+            )
+
         return config.foreign_resource.schemas["many"](
-            **{META_KEY: meta_schema(**meta), DATA_KEY: result.data}
+            **{
+                META_KEY: meta_schema(**context_data[META_KEY]),
+                DATA_KEY: context_data[DATA_KEY],
+            }
         )
 
 
 # -------------------------------------------------------------------------------------------
 # CONTROLLER CONFIGURATOR
 # Binds routes to controller actions based on application configuration
 # -------------------------------------------------------------------------------------------
@@ -949,51 +1039,51 @@
 ) -> APIRouter:
     if not disable_create:
         controller.post(
             "",
             description=f"Create a single '{single_name}'",
             response_model=single_schema,
             response_model_exclude_none=True,
-            dependencies=assemblePolicies(policies_universal, policies_create),
+            dependencies=assemble_policies(policies_universal, policies_create),
         )(actions.create)
 
     if not disable_update:
         controller.patch(
             "/{id}",
             description=f"Update a single '{single_name}'",
             response_model=single_schema,
             response_model_exclude_none=True,
-            dependencies=assemblePolicies(policies_universal, policies_update),
+            dependencies=assemble_policies(policies_universal, policies_update),
         )(actions.update)
 
     if not disable_delete:
         controller.delete(
             "/{id}",
             description=f"Delete a single '{single_name}'",
             response_model=single_schema,
             response_model_exclude_none=True,
-            dependencies=assemblePolicies(policies_universal, policies_delete),
+            dependencies=assemble_policies(policies_universal, policies_delete),
         )(actions.delete)
 
     if not disable_get_one:
         controller.get(
             "/{id}",
             description=f"Fetch a single '{single_name}'",
             response_model=single_schema,
             response_model_exclude_none=True,
-            dependencies=assemblePolicies(policies_universal, policies_get_one),
+            dependencies=assemble_policies(policies_universal, policies_get_one),
         )(actions.get_by_id)
 
     if not disable_get_many:
         controller.get(
             "",
             description=f"Fetch many '{plural_name}'",
             response_model=many_schema,
             response_model_exclude_none=True,
-            dependencies=assemblePolicies(policies_universal, policies_get_many),
+            dependencies=assemble_policies(policies_universal, policies_get_many),
         )(actions.get_all)
 
     # Add relationship link endpoints starting here...
     # Maybe add way to disable these getters?
     # Maybe add way to wrangle this unknown number of functions into the actions map?
     for key, config in relations.items():
         if config.orm_relationship.direction == ONETOMANY:
```

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/util.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.6/pyproject.toml` & `fastapi_cruddy_framework-1.4.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.6"
+version = "1.4.7"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.6/PKG-INFO` & `fastapi_cruddy_framework-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.6
+Version: 1.4.7
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.6 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.7 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

