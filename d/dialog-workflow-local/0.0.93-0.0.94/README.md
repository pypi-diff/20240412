# Comparing `tmp/dialog-workflow-local-0.0.93.tar.gz` & `tmp/dialog-workflow-local-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.93.tar", last modified: Sun Apr  7 05:12:40 2024, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.94.tar", last modified: Fri Apr 12 03:57:17 2024, max compression
```

## Comparing `dialog-workflow-local-0.0.93.tar` & `dialog-workflow-local-0.0.94.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 05:12:40.000000 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-07 05:12:40.000000 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 05:12:40.000000 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 05:12:40.000000 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 05:12:40.000000 dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 05:12:40.235331 dialog-workflow-local-0.0.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 05:12:12.000000 dialog-workflow-local-0.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:57:17.564532 dialog-workflow-local-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 03:57:17.564532 dialog-workflow-local-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:57:17.560532 dialog-workflow-local-0.0.94/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:57:17.564532 dialog-workflow-local-0.0.94/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29813 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:57:17.564532 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-12 03:57:17.000000 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 03:57:17.000000 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:57:17.000000 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 03:57:17.000000 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 03:57:17.000000 dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:57:17.564532 dialog-workflow-local-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-12 03:56:48.000000 dialog-workflow-local-0.0.94/setup.py
```

### Comparing `dialog-workflow-local-0.0.93/PKG-INFO` & `dialog-workflow-local-0.0.94/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.93/README.md` & `dialog-workflow-local-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local/src/Constants.py` & `dialog-workflow-local-0.0.94/dialog_workflow_local/src/Constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from enum import Enum
 
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from python_sdk_remote.utilities import our_get_env
 
 
-# TODO Let's use SQL2Code
-
 # TODO Move to a seperate file
 # TODO Use Sql2Code
 class WorkflowActionEnum(Enum):
     PRESENT_AND_CHOOSE_SCRIPT = 0
     LABEL_ACTION = 1
     TEXT_MESSAGE_ACTION = 2
     QUESTION_ACTION = 3
```

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local/src/DialogWorkflow.py` & `dialog-workflow-local-0.0.94/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 import random
 
-from database_mysql_local.connector import Connector
+from database_mysql_local.generic_crud import GenericCRUD
+from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 from message_local.CompoundMessage import CompoundMessage
 from user_context_remote.user_context import UserContext
 from variable_local.variable import VariablesLocal
-from language_remote.lang_code import LangCode
 
 from .Constants import DIALOG_WORKFLOW_CODE_LOGGER_OBJECT
 from .ProfileContext import DialogWorkflowRecord
 from .action import Action
 from .utils import get_curr_state, update_profile_curr_state_in_db
 
 user = UserContext()
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
+generic_crud = GenericCRUD(default_schema_name='dialog_workflow',
+                           default_table_name='dialog_workflow_state',
+                           default_view_table_name='dialog_workflow_state_view')
 
 
 # Get all potential records in a specific state and choose randomly one of them
 # TODO Please use MessagesLocal to store the message(s) recieved and anwers
 # TODO Please use the function defined in avatar similar to get_dialog_workflow_avatar_profile_id( profile_id1, prompt, group_id, profile_id2...) using avatar_table and avtar_group_table
 def get_dialog_workflow_record(profile_curr_state: int, language: LangCode):
     logger.start(
         object={'profile_curr_state': profile_curr_state, 'language': language})
     # TODO Change * to the fields required
-    connection = Connector.connect('dialog_workflow')
-    cursor = connection.cursor(dictionary=True, buffered=True)
-    cursor.execute("""SELECT * FROM dialog_workflow_state_view WHERE state_id = %s AND lang_code = %s""",
-                   (profile_curr_state, language.value))
-    optional_records = cursor.fetchall()
+    optional_records = generic_crud.select_multi_dict_by_where(where="state_id = %s AND lang_code = %s",
+                                                               params=(profile_curr_state, language.value))
     if not optional_records:
         error_message = f"No records found for state_id: {profile_curr_state} and language: {language}"
         logger.error(error_message)
         logger.end()
         raise Exception(error_message)
     random_index = random.randint(0, len(optional_records) - 1)
     dialog_workflow_record = DialogWorkflowRecord(optional_records[random_index])
     logger.end(object={'dialog_workflow_record': str(dialog_workflow_record)})
     return dialog_workflow_record
 
 
-def post_message(profile_id: int, incoming_message: str):
+def post_message(*, incoming_message: str, profile_id: int = None):
     """This function is supposed to serve as a POST request later on using REST API.
     It runs until needing input from the user, which it then sends a json to the user with the message and exits
     PARAMS: 
         1. profile_id: the profile id that sent the request
         2. incoming_message: the message he sent"""
     # TODO: remove profile_id an use user context
-    logger.start(object={'profile_id': profile_id,
-                         'incoming_message': incoming_message})
+    logger.start(object={'profile_id': profile_id, 'incoming_message': incoming_message})
+    profile_id = profile_id or user.get_effective_profile_id()
     # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
     variables = VariablesLocal()
     profile_curr_state = get_curr_state(profile_id)
-    # TODO lang_code =
-    language = user.get_effective_profile_preferred_lang_code()
+    lang_code = user.get_effective_profile_preferred_lang_code()
     got_response = incoming_message.strip() != ""  # This variable indicates if we must act now as we got a response from the user or as if we should send one to him
     init_action = Action(incoming_message, profile_id,
-                         language, profile_curr_state, variables)
+                         lang_code, profile_curr_state, variables)
     while True:
-        dialog_workflow_record = get_dialog_workflow_record(
-            init_action.profile_curr_state, language)
-        is_state_changed, outgoing_message = init_action.act(
-            dialog_workflow_record, got_response)
+        dialog_workflow_record = get_dialog_workflow_record(init_action.profile_curr_state, lang_code)
+        is_state_changed, outgoing_message = init_action.act(dialog_workflow_record, got_response)
         # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
         if outgoing_message is not None:
             if not isinstance(outgoing_message, list):
                 outgoing_compound_message = CompoundMessage(body=outgoing_message).get_message_fields()
             else:
                 outgoing_compound_message = outgoing_message
             logger.end(object={'outgoing_message': str(outgoing_compound_message)})
             return outgoing_compound_message
         init_action.profile_curr_state = dialog_workflow_record.next_state_id if is_state_changed == False else init_action.profile_curr_state
-        update_profile_curr_state_in_db(
-            init_action.profile_curr_state, profile_id)
+        update_profile_curr_state_in_db(init_action.profile_curr_state, profile_id)
         got_response = False
```

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local/src/ProfileContext.py` & `dialog-workflow-local-0.0.94/dialog_workflow_local/src/ProfileContext.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,57 @@
-from database_mysql_local.connector import Connector
+from database_mysql_local.generic_crud import GenericCRUD
 from logger_local.LoggerLocal import Logger
 from variable_local.variable import VariablesLocal
 
 from .Constants import DIALOG_WORKFLOW_CODE_LOGGER_OBJECT
 from .utils import get_curr_state
 
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
 
-class ProfileContext(object):
+class ProfileContext(GenericCRUD, object):
     # TODO We should consider to take ProfileContact to a separate package or merge it with UserContext
     def __init__(self, profile_id):
-        self.dict = {}
+        super().__init__(default_schema_name='logger', default_table_name='logger_table')
         self.profile_id = profile_id
         self.chosen_poll_options = {}
         self.curr_state_id = get_curr_state(self.profile_id)
         self.variables = VariablesLocal()
         self.groups = []
 
-    def get_variable_value_by_variable_id(self, variable_id: int) -> str:
-        logger.start(object={'variable_id': variable_id})
-        variable_value = self.dict[variable_id]
-        logger.end(object={'variable_value': variable_value})
-        return variable_value
-
     def save_chosen_options(self, question_asked: str, variable_id: int, chosen_numbers_list: list,
                             list_of_options: list):
         """Saves the options chosen by the user in the multi_choice_poll action in a dict with the question as the key
             and a list of the options chosen as the value i.e: {<question asked> : [<chosen option 1>, <chosen option 2>, ...]}
             Also saves the chosen options in the database."""
         logger.start(object={'question_asked': question_asked, 'variable_id': variable_id,
                              'chosen_numbers_list': chosen_numbers_list, 'list_of_options': list_of_options})
+        if not list_of_options:
+            logger.error('list_of_options is empty', object={
+                'question_asked': question_asked, 'variable_id': variable_id,
+                'chosen_numbers_list': chosen_numbers_list, 'list_of_options': list_of_options})
+            raise Exception('list_of_options is empty')
         self.chosen_poll_options[question_asked] = [
             list_of_options[chosen_option - 1] for chosen_option in chosen_numbers_list]
         variable_value_to_insert = question_asked + " "
         for chosen_option in self.chosen_poll_options[question_asked]:
-            variable_value_to_insert = variable_value_to_insert + \
-                                       str(chosen_option) + ", "
+            variable_value_to_insert = variable_value_to_insert + str(chosen_option) + ", "
         self.variables.set_variable_value_by_variable_id(
             variable_id, variable_value_to_insert, self.profile_id, self.curr_state_id)
         logger.end()
 
-    def get_variable_value_by_variable_name(self, variable_name: str) -> str:
-        logger.start(object={'variable_name': variable_name})
-        variable_value = self.get_variable_value_by_variable_id(
-            self.variables.get_variable_id_by_variable_name(variable_name))
-        logger.end(object={'variable_value': variable_value})
-        return variable_value
-
-    # TODO Should be moved to variable-value-local-python-package
-    def set(self, variable_id: int, variable_value: str):
-        logger.start(object={'variable_id': variable_id, 'variable_value': variable_value})
-        self.dict[variable_id] = variable_value
-        connection = Connector.connect('logger')
-        cursor = connection.cursor(dictionary=True, buffered=True)
-        # cursor.execute("""USE logger""")
-        # TODO Can we replace it with GenericCRUD
-        cursor.execute("""INSERT INTO logger
-                        (profile_id, state_id, variable_id, variable_value_new) 
-                        VALUES (%s,%s,%s,%s)""",
-                       (self.profile_id, self.curr_state_id, variable_id, variable_value))
-        connection.commit()
-        logger.end()
-
-
-class ProfilesDict(object):
-    def __init__(self):
-        self.profiles_dict = {}
-
-    def add(self, profile: ProfileContext):
-        logger.start(object={'profile': profile})
-        # TODO Should we also keep in the database?
-        self.profiles_dict[profile.profile_id] = profile
-        logger.end()
-
-    def get(self, profile_id: int) -> ProfileContext or None:
-        logger.start(object={'profile_id': profile_id})
-        if profile_id not in self.profiles_dict:
-            logger.end()
-            return None
-        else:
-            profile_dict = self.profiles_dict[profile_id]
-            logger.end(object={'profile_dict': profile_dict})
-            return profile_dict
-        # return None if profile_id not in self.profiles_dict else self.profiles_dict[profile_id]
-
 
-class DialogWorkflowRecord(object):
+class DialogWorkflowRecord:
     def __init__(self, record: dict) -> None:
         self.curr_state_id: int = record.get("state_id")
         self.parent_state_id: int = record.get("parent_state_id")
         self.workflow_action_id: int = record.get("workflow_action_id")
         self.lang_code = record.get("lang_code")
         self.parameter1 = record.get("parameter1")
         self.variable1_id: int = record.get("variable1_id")
         self.result_logical = record.get("result_logical")
         self.result_figure_min: float = record.get("result_figure_min")
         self.result_figure_max: float = record.get("result_figure_max")
         self.next_state_id: int = record.get("next_state_id")
         self.no_feedback_milliseconds: float = record.get("no_feedback_milliseconds")
         self.next_state_id_if_there_is_no_feedback: int = record.get("next_state_id_if_there_is_no_feedback")
+        self.is_test_data: bool = record.get("is_test_data")
```

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local/src/action.py` & `dialog-workflow-local-0.0.94/dialog_workflow_local/src/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from variable_local.template import ReplaceFieldsWithValues
 from variable_local.variable import VariablesLocal
 
 from .Constants import (COMMUNICATION_TYPE, DIALOG_WORKFLOW_CODE_LOGGER_OBJECT,
                         CommunicationTypeEnum, WorkflowActionEnum)
 from .ProfileContext import DialogWorkflowRecord, ProfileContext
 from .utils import (Group, generic_menu, get_child_nodes_of_current_state,
-                    get_curr_state, get_variable_value_by_id, process_message,
+                    get_curr_state, process_message,
                     update_profile_curr_state_in_db)
 
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
 
 class Action(object):
     def __init__(self, incoming_message: str, profile_id: int, language: LangCode, profile_curr_state: int,
@@ -149,78 +149,83 @@
                 return question_act
             else:
                 question_act = False, None
                 logger.end(object={'question_act': question_act})
                 return question_act
         else:
             self.variable.set_variable_value_by_variable_id(
-                self.record.variable1_id, self.incoming_message, str(self.profile_id), self.profile_curr_state)
+                self.record.variable1_id, self.incoming_message, self.profile_id, self.profile_curr_state)
             question_act = False, None
             logger.end(object={'question_act': question_act})
             return question_act
 
     def jump_action(self):
         """Jumps from one state to another."""
         logger.start()
         self.profile_curr_state = int(self.record.parameter1)
-        update_profile_curr_state_in_db(
-            self.profile_id, int(self.record.parameter1))
+        update_profile_curr_state_in_db(self.profile_id, int(self.record.parameter1))
         jump_act = True, None
         logger.end(object={'jump_Act': jump_act})
         return jump_act
 
     def send_rest_api_action(self):
         """Sends a REST API post"""
         # TODO: implament this function
         logger.start()
         # api_url = self.record.parameter1
         # payload_variable_id = self.record.variable1_id
-        # json_payload_string = get_variable_value_by_id(self.language, payload_variable_id)
+        # json_payload_string = self.variables.get_variable_value_by_variable_id(
+        #             payload_variable_id, self.language, self.profile_id)
         # json_payload = json.loads(json_payload_string)
         # incoming_message = requests.post(api_url, json=json_payload)
         # incoming_message_string = json.dumps(incoming_message.json())
         # insert_profile_variable_value(self.profile_id, self.variable.get_variable_id("Post Result"), incoming_message_string, self.profile_curr_state)
         API_post = False, None
         logger.end(object={'API_post': API_post})
         return API_post
 
     def assign_variable_action(self):
         """Assigns a value to a given variable"""
         logger.start()
         parameter_value = self.record.parameter1
         variable_id = self.record.variable1_id
         self.variable.set_variable_value_by_variable_id(
-            variable_id, parameter_value, str(self.profile_id), self.profile_curr_state)
+            variable_id, parameter_value, self.profile_id, self.profile_curr_state)
         assinged_variable_action = self.got_response, None
         logger.end(
             object={'assinged_variable_action': assinged_variable_action})
         return assinged_variable_action
 
     def increment_variable_action(self):
         """Increments a value to a given variable by the amount of the given paramter1"""
         logger.start()
         number_to_add = int(self.record.parameter1)
         variable_id = self.record.variable1_id
-        current_variable_value = get_variable_value_by_id(
-            self.language, variable_id)
+        current_variable_value = self.variables.get_variable_value_by_variable_id(
+            variable_id, self.language, self.profile_id)
         self.variables.set_variable_value_by_variable_id(variable_id, str(
-            int(current_variable_value) + number_to_add), str(self.profile_id), self.profile_curr_state)
+            int(current_variable_value) + number_to_add), self.profile_id, self.profile_curr_state)
         incremented_variable_action = self.got_response, None
         logger.end(
             object={'incremented_variable_action': incremented_variable_action})
         return incremented_variable_action
 
     def decrement_variable_action(self):
         """Increments a value to a given variable by the amount of the given paramter1"""
         logger.start()
+        if isinstance(self.record.parameter1, str) and not self.record.parameter1.isdigit():
+            error = f"Parameter1 must be a number (got {self.record.parameter1})"
+            logger.error(error)
+            raise ValueError(error)
         number_to_add = int(self.record.parameter1)
         variable_id = self.record.variable1_id
-        current_variable_value = get_variable_value_by_id(self.language, variable_id)
+        current_variable_value = self.variables.get_variable_value_by_variable_id(
+            variable_id, self.language, self.profile_id)
         self.variable.set_variable_value_by_variable_id(variable_id, str(int(current_variable_value) - number_to_add),
-                                                        str(self.profile_id), get_curr_state(self.profile_id))
+                                                        self.profile_id, get_curr_state(self.profile_id))
         decremented_variable_action = False, None
         logger.end(
             object={'decremented_variable_action': decremented_variable_action})
         return decremented_variable_action
 
     """I have put this in remark right now because this action need to work with multiple profiles,
     But right now this change makes it difficult to do that. Will work on it later."""
@@ -426,27 +431,31 @@
             self.profile_curr_state = available_scripts_dict[menu[0] -
                                                              1]["start_state_id"]
             present_and_choosed_script = True, None
             logger.end(
                 object={'present_and_choosed_script': present_and_choosed_script})
             return present_and_choosed_script
 
-    def present_form_action(self):
+    def present_form_action(self) -> (bool, list):
         logger.start()
         form_id = self.record.parameter1
+        if not isinstance(form_id, int):
+            if isinstance(form_id, str) and form_id.isdigit():
+                form_id = int(form_id)
+            else:
+                raise ValueError(f"parameter1 must be an integer (got {form_id})")
         connection = Connector.connect("form")
         query = """SELECT DISTINCT question_id,message_template_text_block_id,question_title,variable_name,question_type_id from form_general_view WHERE form_id=%s"""
         cursor = connection.cursor(dictionary=True, buffered=True)
         cursor.execute(query, (form_id,))
         questions = cursor.fetchall()
         forms = []
         for question in questions:
             message_template_id = question["message_template_text_block_id"]
-            form = CompoundMessage(message_template_id=message_template_id).get_compound_message_str()
-            forms.append(form)
+            forms.append(CompoundMessage(message_template_id=message_template_id).get_compound_message_str())
         return True, forms
 
 
 def generic_user_choice_action(record: DialogWorkflowRecord, accumulated_message: str, child_nodes: list,
                                choose_exactly_one_option: bool, got_response: bool, chosen_numbers: str,
                                profile: ProfileContext):
     """Sends the user a question with a couple of answers. This function is generic and can let the user choose either
```

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local/src/utils.py` & `dialog-workflow-local-0.0.94/dialog_workflow_local/src/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 
 from database_mysql_local.connector import Connector
-from language_remote.lang_code import LangCode
 from logger_local.LoggerLocal import Logger
 
 from .Constants import (COMMUNICATION_TYPE, DIALOG_WORKFLOW_CODE_LOGGER_OBJECT,
                         CommunicationTypeEnum, WorkflowActionEnum)
 
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
@@ -14,26 +13,14 @@
 
 # TODO: Please include type to all parameters.
 # TODO: Please include return value.
 # TODO: Please add short documentation per PEP8 standard
 
 # TODO:Let's move to Object Oriented Programming
 
-def get_variable_value_by_id(language: LangCode, variable_id: int) -> str:
-    # TODO: language is not used
-    logger.start(object={'variable_id': variable_id})
-    connection = Connector.connect('logger')
-    cursor = connection.cursor(dictionary=True, buffered=True)
-    cursor.execute(
-        """SELECT variable_value_new FROM logger_dialog_workflow_state_history_view WHERE variable_id= %s ORDER BY timestamp DESC""",
-        (variable_id,))
-    variable_value = (cursor.fetchone())["variable_value_new"]
-    logger.end(object={'variable_value': variable_value})
-    return variable_value
-
 
 def process_message(communication_type: CommunicationTypeEnum, action_type: WorkflowActionEnum, message: str) -> str:
     """Processes message according to which communication_type is used: console or websocket
         If console then we continue the code normally.
         If websocket then we create a json out of the given message and exit(0)"""
     logger.start(object={'communication_type': communication_type, 'action_type': action_type, 'message': message})
     if communication_type == CommunicationTypeEnum.CONSOLE:
@@ -53,15 +40,15 @@
     else:
         json_message["type"] = "text"
     json_dumps = json.dumps(json_message)
     logger.end(object={'json_dumps': json_dumps})
     return json_dumps
 
 
-def update_profile_curr_state_in_db(new_state: int, profile_id):
+def update_profile_curr_state_in_db(new_state: int, profile_id: int):
     """This function updates the last_dialog_workflow_state_id in the profile table to the new state.
        Note that this function UPDATES the field sand doesn't INSERT into the table. """
     logger.start(object={"new_state": new_state, 'profile_id': profile_id})
     connection = Connector.connect('profile')
     cursor = connection.cursor(dictionary=True, buffered=True)
     # cursor.execute("""USE profile""")
     cursor.execute("""UPDATE profile_table SET last_dialog_workflow_state_id = %s WHERE (profile_id= %s)""",
```

### Comparing `dialog-workflow-local-0.0.93/dialog_workflow_local.egg-info/PKG-INFO` & `dialog-workflow-local-0.0.94/dialog_workflow_local.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.93
+Version: 0.0.94
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.93/setup.py` & `dialog-workflow-local-0.0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.93',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.94',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

