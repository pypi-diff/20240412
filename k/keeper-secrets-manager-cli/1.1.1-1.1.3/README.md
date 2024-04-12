# Comparing `tmp/keeper-secrets-manager-cli-1.1.1.tar.gz` & `tmp/keeper_secrets_manager_cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keeper-secrets-manager-cli-1.1.1.tar", last modified: Sat Sep 16 00:02:00 2023, max compression
+gzip compressed data, was "keeper_secrets_manager_cli-1.1.3.tar", last modified: Fri Apr 12 21:20:01 2024, max compression
```

## Comparing `keeper-secrets-manager-cli-1.1.1.tar` & `keeper_secrets_manager_cli-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 00:02:00.885181 keeper-secrets-manager-cli-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-09-16 00:02:00.881181 keeper-secrets-manager-cli-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 00:02:00.881181 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45190 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/exec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/init.py
--rw-r--r--   0 runner    (1001) docker     (127)    19719 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    30918 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    54547 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-16 00:02:00.881181 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-16 00:02:00.000000 keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-16 00:02:00.885181 keeper-secrets-manager-cli-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-09-16 00:01:33.000000 keeper-secrets-manager-cli-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:01.042687 keeper_secrets_manager_cli-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-12 21:20:01.042687 keeper_secrets_manager_cli-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:01.042687 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47563 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/exec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37930 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54547 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:20:01.042687 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-12 21:20:01.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 21:20:00.000000 keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:20:01.042687 keeper_secrets_manager_cli-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-12 21:19:46.000000 keeper_secrets_manager_cli-1.1.3/setup.py
```

### Comparing `keeper-secrets-manager-cli-1.1.1/PKG-INFO` & `keeper_secrets_manager_cli-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-cli
-Version: 1.1.1
+Version: 1.1.3
 Summary: Command line tool for Keeper Secrets Manager
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/secrets-manager-command-line-interface
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: keeper-secrets-manager-core>=16.5.4
+Requires-Dist: keeper-secrets-manager-core>=16.6.4
 Requires-Dist: keeper-secrets-manager-helper
-Requires-Dist: keeper-secrets-manager-storage>=1.0.1
+Requires-Dist: keeper-secrets-manager-storage>=1.0.2
 Requires-Dist: prompt-toolkit~=2.0
 Requires-Dist: jsonpath-rw-ext
 Requires-Dist: colorama
 Requires-Dist: importlib_metadata
 Requires-Dist: click
 Requires-Dist: click_help_colors
 Requires-Dist: click-repl
@@ -44,14 +44,23 @@
 
 The Keeper Secrets Manager command line interface
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/secrets-manager-command-line-interface
 
 # Change History
 
+## 1.1.3
+
+- KSM-496: Added upload file option
+- KSM-495: Added query option to ksm secret list command
+- KSM-494: Added folder support to secret list command
+- KSM-493: Added CLI options to update title and notes
+- KSM-492: Added clone option
+- KSM-485: Added sub-folder support to ksm secret add command
+
 ## 1.1.1
 
 * KSM-429 - Add `--profile-name` to `ksm profile import` command
 
 ## 1.1.0
 * KSM-395 - New feature to load configurations from AWS Secrets Manager
```

### Comparing `keeper-secrets-manager-cli-1.1.1/README.md` & `keeper_secrets_manager_cli-1.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 
 The Keeper Secrets Manager command line interface
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/secrets-manager-command-line-interface
 
 # Change History
 
+## 1.1.3
+
+- KSM-496: Added upload file option
+- KSM-495: Added query option to ksm secret list command
+- KSM-494: Added folder support to secret list command
+- KSM-493: Added CLI options to update title and notes
+- KSM-492: Added clone option
+- KSM-485: Added sub-folder support to ksm secret add command
+
 ## 1.1.1
 
 * KSM-429 - Add `--profile-name` to `ksm profile import` command
 
 ## 1.1.0
 * KSM-395 - New feature to load configurations from AWS Secrets Manager
```

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/__init__.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/__main__.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,26 @@
         "import",
         "init",
         "setup",
         "sync",
         "secret",
         "totp",
         "download",
+        "upload",
         "get",
         "list",
         "notation",
         "update",
         "version",
         "password",
         "template",
         "add",
         "editor",
         "field",
+        "clone",
         "record",
         "file",
         "cache",
         "record-type-dir"
     ]
 
     alias_commands = {
@@ -244,15 +246,16 @@
     def handle_parse_result(self, ctx, opts, args):
         # ('option','value') - option present with the specified value assigned
         # ('option',) - option present with or without any value
         current_opt:bool = self.name in opts
         for mutex_opt in self.not_required_if:
             if mutex_opt and mutex_opt[0] in opts and (len(mutex_opt) == 1 or opts.get(mutex_opt[0], str(mutex_opt[1])+'_') == mutex_opt[1]):
                 if current_opt:
-                    raise click.UsageError("Illegal usage: '" + str(self.name) + "' is mutually exclusive with " + str(mutex_opt) + ".")
+                    opt = str(mutex_opt) if len(mutex_opt) > 1 else f"'{str(mutex_opt[0])}'"
+                    raise click.UsageError("Illegal usage: '" + str(self.name) + "' is mutually exclusive with " + opt + ".")
                 else:
                     self.prompt = None
         for mutex_opt in self.required_if:
             if mutex_opt and mutex_opt[0] in opts and (len(mutex_opt) == 1 or opts.get(mutex_opt[0], str(mutex_opt[1])+'_') == mutex_opt[1]):
                 if not current_opt:
                     raise click.UsageError("Illegal usage: '" + str(self.name) + "' is required with " + str(mutex_opt) + ".")
                 else:
@@ -525,26 +528,34 @@
 
 
 @click.command(
     name='list',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
-@click.option('--uid', "-u", type=str, multiple=True)
+@click.option('--uid', '-u', type=str, multiple=True, help='List specific records by Record UID', cls=Mutex, not_required_if=[('folder',)])
+@click.option('--folder', '-f', type=str, help='List only records in specified folder UID')
+@click.option('--recursive', '-r', is_flag=True, help='List recursively all records including subfolders of the folder UID')
+@click.option('--query', '-q', type=str, help='List records matching the JSONPath query')
+@click.option('--show-value', '-v', is_flag=True, help='Print matching value instead of record title')
 @click.option('--json', is_flag=True, help='Return secret as JSON')
 @click.pass_context
-def secret_list_command(ctx, uid, json):
+def secret_list_command(ctx, uid, folder, recursive, query, show_value, json):
     """List all secrets"""
 
     output = "text"
     if json is True:
         output = "json"
 
     ctx.obj["secret"].secret_list(
         uids=uid,
+        folder=folder,
+        recursive=recursive,
+        query=query,
+        show_value=show_value,
         output_format=output,
         use_color=ctx.obj["cli"].use_color
     )
 
 
 @click.command(
     name='get',
@@ -619,27 +630,45 @@
 )
 @click.option('--uid', '-u', required=True, type=str, help="Unique identifier of record.")
 @click.option('--field', type=str, multiple=True, help="Update value in field section of vault")
 @click.option('--custom-field', type=str, multiple=True, help="Update value in custom field section of vault")
 @click.option('--field-json', type=str, multiple=True, help="Update value in field section of vault using JSON")
 @click.option('--custom-field-json', type=str, multiple=True,
               help="Update value in custom field section of vault using JSON")
+@click.option('--title', '-t', type=str, help="Update record title.")
+@click.option('--notes', '-n', type=str, help="Update record notes.")
 @click.pass_context
-def secret_update_command(ctx, uid, field, custom_field, field_json, custom_field_json):
+def secret_update_command(ctx, uid, field, custom_field, field_json, custom_field_json, title, notes):
     """Update an existing record"""
     ctx.obj["secret"].update(
         uid=uid,
         fields=field,
         custom_fields=custom_field,
         fields_json=field_json,
-        custom_fields_json=custom_field_json
+        custom_fields_json=custom_field_json,
+        title=title,
+        notes=notes
     )
 
 
 @click.command(
+    name='upload',
+    cls=HelpColorsCommand,
+    help_options_color='blue'
+)
+@click.option('--uid', '-u', required=True, type=str, help='UID of the secret.')
+@click.option('--file', '-f', required=True, type=str, help='Path to the file to upload.')
+@click.option('--title', '-t', type=str, help='File title (defaults to the filename if none provided).')
+@click.pass_context
+def secret_upload_command(ctx, uid, file, title):
+    """Upload a file to a secret record"""
+    ctx.obj["secret"].upload(uid=uid, file=file, title=title)
+
+
+@click.command(
     name='download',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.option('--uid', '-u', required=True, type=str, help="UID of the secret.")
 @click.option('--name', type=str, help='Name of the file to download.')
 @click.option('--file-uid', type=str, help='Unique id of the file to download.')
@@ -808,30 +837,30 @@
 
 @click.command(
     name='editor',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.pass_context
-@click.option('--shared-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
+@click.option('--storage-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
 @click.option('--record-type', '--rt', required=True, type=str, help="Record type")
 @click.option('--password-generate', '-p', is_flag=True, help='Generate passwords for empty password fields.')
 @click.option('--title', '-t', type=str, help="Record title")
 @click.option('--notes', '-n', type=str, help="Record simple note")
 @click.option('--output-format', '-o', type=click.Choice(['yaml', 'json'], case_sensitive=False), default='json',
               help='File format to display in editor.')
 @click.option('--editor', '-e', type=str, help='Application to use to edit record data.')
 @click.option('--version', type=click.Choice(['v3'], case_sensitive=False), default='v3', help='Record version.')
-def secret_add_editor_command(ctx, shared_folder_uid, record_type, password_generate, title, notes,
+def secret_add_editor_command(ctx, storage_folder_uid, record_type, password_generate, title, notes,
                               output_format, editor, version):
     """Add a secret record via a text editor"""
 
     ctx.obj["secret"].add_record_interactive(
         version=version,
-        folder_uid=shared_folder_uid,
+        folder_uid=storage_folder_uid,
         record_type=record_type,
         output_format=output_format,
         password_generate_flag=password_generate,
         title=title,
         notes=notes,
         editor=editor
     )
@@ -840,67 +869,94 @@
 
 @click.command(
     name='file',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.pass_context
-@click.option('--shared-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
+@click.option('--storage-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
 @click.option('--file', '-f', required=True, type=str, help='Add records from record script file.')
 @click.option('--password-generate', '-p', is_flag=True, help='Generate passwords for empty password fields.')
-def secret_add_file_command(ctx, shared_folder_uid, file, password_generate):
+def secret_add_file_command(ctx, storage_folder_uid, file, password_generate):
     """Add a secret record(s) from a file"""
 
     ctx.obj["secret"].add_record_from_file(
-        folder_uid=shared_folder_uid,
+        folder_uid=storage_folder_uid,
         file=file,
         password_generate_flag=password_generate,
     )
     print("", file=sys.stderr)
 
 
 @click.command(
     name='field',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.pass_context
-@click.option('--shared-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
+@click.option('--storage-folder-uid', '--sf', required=True, type=str, help="Place record in folder with UID.")
 @click.option('--record-type', '--rt', required=True, type=str, help="Record type")
 @click.option('--title', '-t', required=True, type=str, help="Record title")
 @click.option('--password-generate', '-p', is_flag=True, help='Generate passwords for empty password fields.')
 @click.option('--notes', '-n', type=str, help="Record simple note")
 @click.option('--version', type=click.Choice(['v3'], case_sensitive=False), default='v3', help='Record version.')
 @click.argument('field_args', type=str, nargs=-1)
-def secret_add_field_command(ctx, shared_folder_uid, record_type, title, password_generate, notes, version,
+def secret_add_field_command(ctx, storage_folder_uid, record_type, title, password_generate, notes, version,
                              field_args):
     """Add a secret record from a command line field arguments"""
 
     ctx.obj["secret"].add_record_from_field_args(
         version=version,
-        folder_uid=shared_folder_uid,
+        folder_uid=storage_folder_uid,
         password_generate_flag=password_generate,
         record_type=record_type,
         title=title,
         notes=notes,
         field_args=list(field_args)
     )
     print("", file=sys.stderr)
 
 
+def validate_non_empty(ctx, param, value):
+    """Validate that parameter's value is not an empty string"""
+    if isinstance(value, str) and value != "":
+        return value
+    raise click.BadParameter("Empty strings are not allowed")
+
+
+@click.command(
+    name='clone',
+    cls=HelpColorsCommand,
+    help_options_color='blue'
+)
+@click.pass_context
+@click.option('--uid', '-u', required=True, type=str, callback=validate_non_empty, help="Record UID to clone")
+@click.option('--title', '-t', type=str, help="New record title")
+def secret_add_clone_command(ctx, uid, title):
+    """Add new record by duplicating existing record"""
+
+    ctx.obj["secret"].add_record_from_clone(
+        uid=uid,
+        title=title
+    )
+    print("", file=sys.stderr)
+
+
+secret_add_command.add_command(secret_add_clone_command)
 secret_add_command.add_command(secret_add_field_command)
 secret_add_command.add_command(secret_add_file_command)
 secret_add_command.add_command(secret_add_editor_command)
 
 
 secret_command.add_command(secret_list_command)
 secret_command.add_command(secret_get_command)
 secret_command.add_command(secret_notation_command)
 secret_command.add_command(secret_update_command)
 secret_command.add_command(secret_add_command)
+secret_command.add_command(secret_upload_command)
 secret_command.add_command(secret_download_command)
 secret_command.add_command(secret_totp_command)
 secret_command.add_command(secret_password_command)
 secret_command.add_command(secret_template_command)
 
 
 # EXEC COMMAND
@@ -1166,15 +1222,15 @@
     name='sync',
     cls=HelpColorsCommand,
     help_options_color='blue'
 )
 @click.option('--credentials', '-c', type=str, metavar="UID", help="Keeper record with credentials to access destination key/value store.",
     cls=Mutex,
     # not_required_if=[('type','json')],
-    required_if=[('type','azure'), ('type','aws'), ('type','gcp')]
+    required_if=[('type', 'azure'), ('type', 'aws'), ('type', 'gcp')]
 )
 @click.option('--type', '-t', type=click.Choice(['aws', 'azure', 'gcp', 'json']), default='json', help="Type of the target key/value storage (aws, azure, gcp, json).", show_default=True)
 @click.option('--dry-run', '-n', is_flag=True, help='Perform a trial run with no changes made.')
 @click.option('--preserve-missing', '-p', is_flag=True, help='Preserve destination value when source value is deleted.')
 @click.option('--map', '-m', nargs=2, type=(str, str), multiple=True, required=True, metavar="<KEY NOTATION>...", help='Map destination key names to values using notation URI.')
 @click.pass_context
 def sync_command(ctx, credentials, type, dry_run, preserve_missing, map):
```

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/common.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/common.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/config.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/config.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/exception.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/exception.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/exec.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/exec.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/export.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/export.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/init.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/init.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/profile.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/profile.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/secret.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/secret.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,25 +10,28 @@
 # Contact: ops@keepersecurity.com
 #
 
 import json
 import yaml
 import os
 import re
-from jsonpath_rw_ext import parse
 import sys
 from colorama import Fore, Style
+from pathlib import Path
+from jsonpath_rw_ext import parse
 from keeper_secrets_manager_cli.exception import KsmCliException
 from keeper_secrets_manager_cli.common import launch_editor
-from keeper_secrets_manager_core.core import SecretsManager
+from keeper_secrets_manager_core.core import SecretsManager, CreateOptions, KeeperFolder, KeeperFileUpload
 from keeper_secrets_manager_core.utils import get_totp_code, generate_password as sdk_generate_password
 from keeper_secrets_manager_helper.record import Record
+from keeper_secrets_manager_helper.v3.record import Record as RecordV3
 from keeper_secrets_manager_helper.field_type import FieldType
 from keeper_secrets_manager_helper.exception import FileSyntaxException
 from .table import Table, ColumnAlign
+from typing import List, Tuple
 import uuid
 import tempfile
 
 
 class Secret:
     # Maps the type in a field to what it should pull in from the real record. There
     # might be multiple field that need to be pulled in.
@@ -146,14 +149,15 @@
         if len(raw_custom_fields) > 0 and load_references is True:
             custom_fields = self._get_custom_fields(raw_custom_fields, unmask, use_color, inflate)
 
         ret = {
             "uid": record.uid,
             "title": record.title,
             "type": record.type,
+            "notes": record.dict.get("notes", ""),
             "fields": standard_fields,
             "custom_fields": custom_fields,
             "files": [{
                 "file_uid": x.f.get("fileUid"),
                 "name": x.name,
                 "title": x.title,
                 "type": x.type,
@@ -355,17 +359,31 @@
                     output.endswith('"') is True:
                 output = results
 
             self.cli.output(output)
         except Exception as err:
             raise KsmCliException("JSONPath failed: {}".format(err))
 
-    def query(self, uids=None, titles=None, field=None, output_format='json', jsonpath_query=None,
-              force_array=False, load_references=False, unmask=False, use_color=None, inflate=True,
-              raw=False):
+    def _query_jsonpath_list(self, jsonpath_query, records):
+        record_list = Secret._adjust_records(records, True)
+        try:
+            results = []
+            jpe = parse(jsonpath_query)
+            for rec in record_list:
+                val = jpe.find(rec)
+                if val and val[0].value:
+                    rec["query_result"] = val[0].value[0] if isinstance(val[0].value, list) else val[0].value
+                    results.append(rec)
+            return results
+        except Exception as err:
+            raise KsmCliException(f"JSONPath failed: {err}") from err
+
+    def query(self, uids=None, folder=None, recursive=False, titles=None, field=None,
+              output_format='json', jsonpath_query=None, force_array=False,
+              load_references=False, unmask=False, use_color=None, inflate=True, raw=False):
 
         if use_color is None:
             use_color = self.cli.use_color
 
         if uids is None:
             uids = []
         if titles is None:
@@ -386,24 +404,37 @@
         if len(titles) == 0:
             fetch_uids = uids
 
         secrets = self.cli.client.get_secrets(uids=fetch_uids)
         if len(secrets) == 0 and fetch_uids is not None:
             raise KsmCliException("Cannot find requested record(s).")
 
+        folders = self.cli.client.get_folders() if folder and recursive else []
+
         for record in secrets:
             add_record = False
 
-            # If we are searching by title, the fetch_uids was None, we have all the records. We need to filter
-            # them by the title or uids.
-            if len(titles) > 0:
-                if record.title in titles or record.uid in uids:
+            if folder:
+                if record.inner_folder_uid == folder or (not record.inner_folder_uid and record.folder_uid == folder):
                     add_record = True
+                elif recursive and (record.inner_folder_uid or record.folder_uid):
+                    fldr = record.inner_folder_uid or record.folder_uid
+                    fldr = str(fldr) if fldr else ''
+                    while fldr and fldr != folder:
+                        fldr = next((x.parent_uid for x in folders if x.folder_uid == fldr), '')
+                    if fldr == folder:
+                        add_record = True
             else:
-                add_record = True
+                # If we are searching by title, the fetch_uids was None, we have all the records. We need to filter
+                # them by the title or uids.
+                if len(titles) > 0:
+                    if record.title in titles or record.uid in uids:
+                        add_record = True
+                else:
+                    add_record = True
 
             if add_record is True:
                 records.append(self._record_to_dict(record,
                                                     load_references=load_references,
                                                     unmask=unmask,
                                                     inflate=inflate))
 
@@ -422,35 +453,77 @@
                 raw=raw
             )
         else:
             return self.output_results(records=records, output_format=output_format, force_array=force_array,
                                        use_color=use_color)
 
     @staticmethod
-    def _format_list(record_dict, use_color=True):
+    def _format_list(record_dict, use_color=True, columns=None):
         table = Table(use_color=use_color)
-        table.add_column("UID", data_color=Fore.GREEN)
-        table.add_column("Record Type")
-        table.add_column("Title", data_color=Fore.YELLOW)
-        for record in record_dict:
-            table.add_row([record["uid"], record["type"], record["title"]])
+        if columns:
+            for col in columns:
+                table.add_column(col[1], data_color=col[2])
+            for record in record_dict:
+                table.add_row([record.get(x[0], "") for x in columns])
+        else:
+            table.add_column("UID", data_color=Fore.GREEN)
+            table.add_column("Record Type")
+            table.add_column("Title", data_color=Fore.YELLOW)
+            for record in record_dict:
+                table.add_row([record["uid"], record["type"], record["title"]])
         return "\n" + table.get_string() + "\n"
 
-    def secret_list(self, uids=None, output_format='json', use_color=None):
+    def secret_list(self, uids=None, folder=None, recursive=False, query=None, show_value=False, output_format='json', use_color=None):
 
         if use_color is None:
             use_color = self.cli.user_color
 
-        record_dict = self.query(uids=uids, output_format='dict', unmask=True, use_color=use_color)
-        if output_format == 'text':
-            self.cli.output(self._format_list(record_dict, use_color=use_color))
-        elif output_format == 'json':
-            records = [{"uid": x.get("uid"), "title": x.get("title"), "record_type": x.get("type")}
-                       for x in record_dict]
-            self.cli.output(json.dumps(records, indent=4))
+        loadrefs = True if query else False  # to load fields[] and custom[]
+        record_dict = self.query(uids=uids, folder=folder, recursive=recursive, output_format='dict', load_references=loadrefs, unmask=True, use_color=use_color)
+        if query:
+            items = self._query_jsonpath_list(query, record_dict)
+            if output_format == 'text':
+                columns = [("uid", "UID", Fore.GREEN), ("type", "Record Type", Style.RESET_ALL), ("query_result", "Value", Fore.YELLOW)] if show_value else []
+                self.cli.output(self._format_list(items, use_color=use_color, columns=columns))
+            elif output_format == 'json':
+                records = [{
+                    "uid": x.get("uid", ""),
+                    "record_type": x.get("type", ""),
+                    "title": x.get("title", ""),
+                    "value": x.get("query_result", "")}
+                           for x in items]
+                if not show_value:
+                    records = [{k: v for k, v in x.items() if k != "value"} for x in records]
+                self.cli.output(json.dumps(records, indent=4))
+        else:
+            if output_format == 'text':
+                self.cli.output(self._format_list(record_dict, use_color=use_color))
+            elif output_format == 'json':
+                records = [{"uid": x.get("uid"), "title": x.get("title"), "record_type": x.get("type")}
+                        for x in record_dict]
+                self.cli.output(json.dumps(records, indent=4))
+
+    def upload(self, uid, file, title):
+
+        # check if file exists and is readable by current user
+        if not (os.path.isfile(file) and os.access(file, os.R_OK)):
+            raise KsmCliException(f"File {file} doesn't exist or isn't readable.")
+
+        records = self.cli.client.get_secrets(uids=[uid])
+        if len(records) == 0:
+            raise KsmCliException(f"Cannot find a record for UID {uid}. Cannot upload {file}")
+
+        record = records[0]
+        fname = Path(file).name
+        title = title if title else fname
+        ksm_file = KeeperFileUpload.from_file(file, fname, title)
+        file_uid = self.cli.client.upload_file(record, file=ksm_file)
+
+        print("The following is the new file UID ...", file=sys.stderr)
+        return self.cli.output(file_uid)
 
     def download(self, uid, name, file_uid, file_output, create_folders=False):
 
         record = self.cli.client.get_secrets(uids=[uid])
         if len(record) == 0:
             raise KsmCliException("Cannot find a record for UID {}. Cannot download {}".format(uid, name))
 
@@ -462,15 +535,15 @@
                     break
         else:
             file = record[0].find_file_by_title(name)
         if file is None:
             raise KsmCliException("Cannot find a file named {} for UID {}. Cannot download file".format(name, uid))
 
         if file_output == 'stdout':
-            sys.stderr.buffer.write(file.get_file_data())
+            sys.stdout.buffer.write(file.get_file_data())
         elif file_output == 'stderr':
             sys.stderr.buffer.write(file.get_file_data())
         elif type(file_output) is str:
             file.save_file(file_output, create_folders)
         else:
             raise KsmCliException("The file output {} is not supported. Cannot download and save the file.".format(
                 file_output))
@@ -550,26 +623,35 @@
                 if type(value) is not list:
                     value = [value]
             except json.JSONDecodeError:
                 raise KsmCliException("The value is not valid JSON for {}".format(text))
 
         return key, value
 
-    def update(self, uid, fields=None, custom_fields=None, fields_json=None, custom_fields_json=None):
+    def update(self, uid, fields=None, custom_fields=None, fields_json=None, custom_fields_json=None, title=None, notes=None):
 
         record = self.cli.client.get_secrets(uids=[uid])
         if len(record) == 0:
             raise KsmCliException("Cannot find a record for UID {}.".format(uid))
 
         def _get_label(x):
             label = x.get("label")
             if label is None or label == "":
                 label = x.get("type")
             return label
 
+        if title is not None:
+            record[0].title = str(title)
+
+        if notes is not None:
+            record[0].dict["notes"] = str(notes)
+
+        if title is not None or notes is not None:
+            record[0]._update()
+
         # Get a list of all labels/type allowed.
         labels = {
             "field": [_get_label(x) for x in record[0].dict.get("fields", [])],
             "custom_field": [_get_label(x) for x in record[0].dict.get("custom", [])]
         }
 
         data = [
@@ -701,19 +783,21 @@
                 os.unlink(temp_filename)
 
     def add_record_from_file(self, folder_uid, file, password_generate_flag):
 
         self._check_if_can_add_records()
 
         try:
+            folders = self.cli.client.get_folders()
             records = Record.create_from_file(file, password_generate=password_generate_flag)
             record_uids = []
             for record in records:
                 record_create_obj = record.get_record_create_obj()
-                record_uid = self.cli.client.create_secret(folder_uid, record_create_obj)
+                folder_options, folders = self.build_folder_options(folder_uid, folders)
+                record_uid = self.cli.client.create_secret_with_options(folder_options, record_create_obj, folders)
                 record_uids.append(record_uid)
         except FileSyntaxException as err:
             raise KsmCliException(str(err))
         except Exception as err:
             raise KsmCliException(f"Could not load records from file {file}: {err}")
 
         print("The following is the new record UIDs in JSON ...", file=sys.stderr)
@@ -730,21 +814,80 @@
                 title=title,
                 notes=notes,
                 field_args=field_args,
                 password_generate=password_generate_flag
             )
             record = records[0]
             record_create_obj = record.get_record_create_obj()
-            record_uid = self.cli.client.create_secret(folder_uid, record_create_obj)
+
+            folder_options, folders = self.build_folder_options(folder_uid)
+            record_uid = self.cli.client.create_secret_with_options(folder_options, record_create_obj, folders)
         except Exception as err:
             raise KsmCliException(f"{err}")
 
         print("The following is the new record UID ...", file=sys.stderr)
         return self.cli.output(record_uid)
 
+    def add_record_from_clone(self, uid: str, title: str):
+
+        record_uid = ''  # new record UID
+        self._check_if_can_add_records()
+
+        try:
+            recs = self.cli.client.get_secrets([uid]) or []
+            if recs:
+                rec = recs[0]
+                if rec.folder_uid:
+                    folder_options = CreateOptions(rec.folder_uid, rec.inner_folder_uid)
+                    record_data = {
+                        "version": "v3",
+                        "kind": "KeeperRecord",
+                        "data": [{
+                            "recordType": rec.type,
+                            "title": title if title else rec.title,
+                            "notes": rec.dict.get("notes", ""),
+                            "fields": rec.dict.get("fields", []),
+                            "customFields": rec.dict.get("custom", [])
+                        }]
+                    }
+                    records = RecordV3.create_from_data(record_data)
+                    record = records[0]
+                    record_create_obj = record.get_record_create_obj()
+                    record_uid = self.cli.client.create_secret_with_options(folder_options, record_create_obj)
+                else:
+                    print(f"Unable to find the parent shared folder for record {uid} - individually shared records cannot be cloned.", file=sys.stderr)
+            else:
+                print(f"Record UID not found {uid}", file=sys.stderr)
+        except Exception as err:
+            raise KsmCliException(f"{err}")
+
+        if record_uid:
+            print("The following is the new record UID ...", file=sys.stderr)
+        return self.cli.output(record_uid)
+
+    def build_folder_options(self, folder_uid: str, folders: List[KeeperFolder] = []) -> Tuple[CreateOptions, List[KeeperFolder]]:
+        """ Build and return folder create options and folders list """
+
+        # find closest shared folder parent
+        if not folders:
+            folders = self.cli.client.get_folders() or []
+
+        shared_folder = next((x for x in folders if x.folder_uid == folder_uid), None)
+        while shared_folder and shared_folder.parent_uid:
+            shared_folder = next((x for x in folders if x.folder_uid == shared_folder.parent_uid), shared_folder)
+
+        if shared_folder is None:
+            raise KsmCliException(f'Unable to find the shared folder for {folder_uid}')
+        if not shared_folder.folder_key:
+            raise KsmCliException(f'Unable to find folder key for folder {shared_folder.folder_uid}')
+
+        # create folder options
+        create_options = CreateOptions(shared_folder.folder_uid, folder_uid)
+        return create_options, folders
+
     def generate_password(self, length, lowercase, uppercase, digits, special_characters):
 
         new_password = sdk_generate_password(
             length=length,
             lowercase=lowercase,
             uppercase=uppercase,
             digits=digits,
```

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/sync.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/sync.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli/table.py` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli/table.py`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/PKG-INFO` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keeper-secrets-manager-cli
-Version: 1.1.1
+Version: 1.1.3
 Summary: Command line tool for Keeper Secrets Manager
 Home-page: https://github.com/Keeper-Security/secrets-manager
 Author: Keeper Security
 Author-email: sm@keepersecurity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Keeper-Security/secrets-manager/issues
 Project-URL: Documentation, https://app.gitbook.com/@keeper-security/s/secrets-manager/secrets-manager/secrets-manager-command-line-interface
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: keeper-secrets-manager-core>=16.5.4
+Requires-Dist: keeper-secrets-manager-core>=16.6.4
 Requires-Dist: keeper-secrets-manager-helper
-Requires-Dist: keeper-secrets-manager-storage>=1.0.1
+Requires-Dist: keeper-secrets-manager-storage>=1.0.2
 Requires-Dist: prompt-toolkit~=2.0
 Requires-Dist: jsonpath-rw-ext
 Requires-Dist: colorama
 Requires-Dist: importlib_metadata
 Requires-Dist: click
 Requires-Dist: click_help_colors
 Requires-Dist: click-repl
@@ -44,14 +44,23 @@
 
 The Keeper Secrets Manager command line interface
 
 For more information see our official documentation page https://docs.keeper.io/secrets-manager/secrets-manager/secrets-manager-command-line-interface
 
 # Change History
 
+## 1.1.3
+
+- KSM-496: Added upload file option
+- KSM-495: Added query option to ksm secret list command
+- KSM-494: Added folder support to secret list command
+- KSM-493: Added CLI options to update title and notes
+- KSM-492: Added clone option
+- KSM-485: Added sub-folder support to ksm secret add command
+
 ## 1.1.1
 
 * KSM-429 - Add `--profile-name` to `ksm profile import` command
 
 ## 1.1.0
 * KSM-395 - New feature to load configurations from AWS Secrets Manager
```

### Comparing `keeper-secrets-manager-cli-1.1.1/keeper_secrets_manager_cli.egg-info/SOURCES.txt` & `keeper_secrets_manager_cli-1.1.3/keeper_secrets_manager_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keeper-secrets-manager-cli-1.1.1/setup.py` & `keeper_secrets_manager_cli-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the README.md file
 with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 install_requires = [
-    'keeper-secrets-manager-core>=16.5.4',
+    'keeper-secrets-manager-core>=16.6.4',
     'keeper-secrets-manager-helper',
-    'keeper-secrets-manager-storage>=1.0.1',
+    'keeper-secrets-manager-storage>=1.0.2',
     'prompt-toolkit~=2.0',
     'jsonpath-rw-ext',
     'colorama',
     'importlib_metadata',
     'click',
     'click_help_colors',
     'click-repl',
@@ -23,15 +23,15 @@
     'psutil',
     'boto3'
 ]
 
 # Version set in the keeper_secrets_manager_cli.version file.
 setup(
     name="keeper-secrets-manager-cli",
-    version="1.1.1",
+    version="1.1.3",
     description="Command line tool for Keeper Secrets Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Keeper Security",
     author_email="sm@keepersecurity.com",
     url="https://github.com/Keeper-Security/secrets-manager",
     license="MIT",
```

