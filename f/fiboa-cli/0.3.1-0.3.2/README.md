# Comparing `tmp/fiboa-cli-0.3.1.tar.gz` & `tmp/fiboa-cli-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiboa-cli-0.3.1.tar", last modified: Thu Apr 11 15:17:38 2024, max compression
+gzip compressed data, was "fiboa-cli-0.3.2.tar", last modified: Fri Apr 12 11:00:29 2024, max compression
```

## Comparing `fiboa-cli-0.3.1.tar` & `fiboa-cli-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/fiboa_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/create_geoparquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/describe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/jsonschema_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/validate_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/fiboa_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/fiboa_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 15:17:38.000000 fiboa-cli-0.3.1/fiboa_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 15:17:38.638429 fiboa-cli-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-11 15:17:34.000000 fiboa-cli-0.3.1/tests/test_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:00:29.703561 fiboa-cli-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-12 11:00:29.703561 fiboa-cli-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:00:29.699561 fiboa-cli-0.3.2/fiboa_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    10916 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/create_geoparquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/describe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9648 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/jsonschema_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/rename_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/validate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/validate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/fiboa_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:00:29.703561 fiboa-cli-0.3.2/fiboa_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 11:00:29.000000 fiboa-cli-0.3.2/fiboa_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:00:29.703561 fiboa-cli-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:00:29.703561 fiboa-cli-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 11:00:23.000000 fiboa-cli-0.3.2/tests/test_jsonschema.py
```

### Comparing `fiboa-cli-0.3.1/LICENSE` & `fiboa-cli-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/PKG-INFO` & `fiboa-cli-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -95,14 +95,31 @@
 
 To validate a fiboa Schema YAML file, you can for example run:
 
 - `fiboa validate-schema schema/schema.yaml`
 
 Check `fiboa validate-schema --help` for more details.
 
+## Update an extension template with new names
+
+Once you've created and git cloned a new extension, you can use the CLI
+to update all template placeholders with proper names.
+
+For example, if your extension is meant to have
+- the title "Timestamps Extension", 
+- the prefix `ts` (e.g. field `ts:created` or `ts:updated`),
+- is hosted at `https://github.io/fiboa/timestamps-extension`
+  (organization: `fiboa`, repository `timestamps-extension`),
+- and you run fiboa in the folder of the extension.
+
+Then the following command could be used:
+- `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
+
+Check `fiboa rename-extension --help` for more details.
+
 ## Converter for existing datasets
 
 To convert an existing dataset to fiboa using the pre-defined converters:
 
 - `fiboa convert de_nrw`
 
 Available converters:
```

### Comparing `fiboa-cli-0.3.1/README.md` & `fiboa-cli-0.3.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -73,14 +73,31 @@
 
 To validate a fiboa Schema YAML file, you can for example run:
 
 - `fiboa validate-schema schema/schema.yaml`
 
 Check `fiboa validate-schema --help` for more details.
 
+## Update an extension template with new names
+
+Once you've created and git cloned a new extension, you can use the CLI
+to update all template placeholders with proper names.
+
+For example, if your extension is meant to have
+- the title "Timestamps Extension", 
+- the prefix `ts` (e.g. field `ts:created` or `ts:updated`),
+- is hosted at `https://github.io/fiboa/timestamps-extension`
+  (organization: `fiboa`, repository `timestamps-extension`),
+- and you run fiboa in the folder of the extension.
+
+Then the following command could be used:
+- `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
+
+Check `fiboa rename-extension --help` for more details.
+
 ## Converter for existing datasets
 
 To convert an existing dataset to fiboa using the pre-defined converters:
 
 - `fiboa convert de_nrw`
 
 Available converters:
```

### Comparing `fiboa-cli-0.3.1/fiboa_cli/__init__.py` & `fiboa-cli-0.3.2/fiboa_cli/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 import os
 
 from .convert import convert as convert_
 from .create_geoparquet import create_geoparquet as create_geoparquet_
 from .create_geojson import create_geojson as create_geojson_
 from .describe import describe as describe_
 from .jsonschema import jsonschema as jsonschema_
+from .rename_extension import rename_extension as rename_extension_
 from .validate import validate as validate_
 from .validate_schema import validate_schema as validate_schema_
 from .version import __version__, fiboa_version as fiboa_version_
-from .util import log, check_ext_schema_for_cli, valid_file_for_cli, valid_file_for_cli_with_ext, valid_files_folders_for_cli
+from .util import log, check_ext_schema_for_cli, valid_file_for_cli, valid_file_for_cli_with_ext, valid_files_folders_for_cli, valid_folder_for_cli
 
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     """
     The fiboa CLI.
     """
@@ -300,17 +301,57 @@
     try:
         convert_(dataset, out, cache, source_coop, collection)
     except Exception as e:
         log(e, "error")
         sys.exit(1)
 
 
+## RENAME EXTENSION
+@click.command()
+@click.argument('folder', nargs=1, callback=valid_folder_for_cli)
+@click.option(
+    '--title', '-t',
+    type=click.STRING,
+    help='Title of the extension, e.g. `Timestamps`',
+    required=True
+)
+@click.option(
+    '--slug', '-s',
+    type=click.STRING,
+    help='Slug of the repository, e.g. for `https://github.com/fiboa/timestamps-extension` it would be `timestamps-extension`',
+    required=True
+)
+@click.option(
+    '--org', '-o',
+    type=click.STRING,
+    help='Slug of the GitHub Organization. Defaults to `fiboa`',
+    default="fiboa"
+)
+@click.option(
+    '--prefix', '-p',
+    type=click.STRING,
+    help='Prefix for the field, e.g. `time` if the fields should be `time:created` or `time:updated`. An empty string removed the prefix, not providing a prefix leaves it as is.',
+    default=None
+)
+def rename_extension(folder, title, slug, org = "fiboa", prefix = None):
+    """
+    Updates placeholders in an extension folder to the new name.
+    """
+    log(f"fiboa CLI {__version__} - Rename placeholders in extensions\n", "success")
+    try:
+        rename_extension_(folder, title, slug, gh_org=org, prefix=prefix)
+    except Exception as e:
+        log(e, "error")
+        sys.exit(1)
+
+
 cli.add_command(describe)
 cli.add_command(validate)
 cli.add_command(validate_schema)
 cli.add_command(create_geoparquet)
 cli.add_command(create_geojson)
 cli.add_command(jsonschema)
 cli.add_command(convert)
+cli.add_command(rename_extension)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `fiboa-cli-0.3.1/fiboa_cli/convert.py` & `fiboa-cli-0.3.2/fiboa_cli/convert.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/convert_utils.py` & `fiboa-cli-0.3.2/fiboa_cli/convert_utils.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/create_geojson.py` & `fiboa-cli-0.3.2/fiboa_cli/create_geojson.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/create_geoparquet.py` & `fiboa-cli-0.3.2/fiboa_cli/create_geoparquet.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/describe.py` & `fiboa-cli-0.3.2/fiboa_cli/describe.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/geopandas.py` & `fiboa-cli-0.3.2/fiboa_cli/geopandas.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/jsonschema.py` & `fiboa-cli-0.3.2/fiboa_cli/jsonschema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/jsonschema_template.py` & `fiboa-cli-0.3.2/fiboa_cli/jsonschema_template.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/parquet.py` & `fiboa-cli-0.3.2/fiboa_cli/parquet.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/types.py` & `fiboa-cli-0.3.2/fiboa_cli/types.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/util.py` & `fiboa-cli-0.3.2/fiboa_cli/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,14 +188,22 @@
     return is_valid_file_uri(value)
 
 
 def valid_file_for_cli_with_ext(value, extensions):
     return is_valid_file_uri(value, extensions)
 
 
+def valid_folder_for_cli(ctx, param, value):
+    """Determine if the input is a folder."""
+    if os.path.exists(value) and os.path.isdir(value):
+        return value
+    else:
+        raise click.BadParameter('Input must be an existing local folder')
+
+
 def get_collection(data, collection_path = None, basepath = None):
     # If the user provided a collection, enforce using it
     if collection_path is not None:
         return load_file(collection_path)
 
     # Look if the data contains a fiboa property
     if "fiboa" in data:
```

### Comparing `fiboa-cli-0.3.1/fiboa_cli/validate.py` & `fiboa-cli-0.3.2/fiboa_cli/validate.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/validate_data.py` & `fiboa-cli-0.3.2/fiboa_cli/validate_data.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli/validate_schema.py` & `fiboa-cli-0.3.2/fiboa_cli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `fiboa-cli-0.3.1/fiboa_cli.egg-info/PKG-INFO` & `fiboa-cli-0.3.2/fiboa_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiboa-cli
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI tools such as validation and file format conversion for fiboa.
 Home-page: https://github.com/fiboa/cli
 Author: Matthias Mohr
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -95,14 +95,31 @@
 
 To validate a fiboa Schema YAML file, you can for example run:
 
 - `fiboa validate-schema schema/schema.yaml`
 
 Check `fiboa validate-schema --help` for more details.
 
+## Update an extension template with new names
+
+Once you've created and git cloned a new extension, you can use the CLI
+to update all template placeholders with proper names.
+
+For example, if your extension is meant to have
+- the title "Timestamps Extension", 
+- the prefix `ts` (e.g. field `ts:created` or `ts:updated`),
+- is hosted at `https://github.io/fiboa/timestamps-extension`
+  (organization: `fiboa`, repository `timestamps-extension`),
+- and you run fiboa in the folder of the extension.
+
+Then the following command could be used:
+- `fiboa rename-extension . -t Timestamps -p ts -s timestamps-extension -o fiboa`
+
+Check `fiboa rename-extension --help` for more details.
+
 ## Converter for existing datasets
 
 To convert an existing dataset to fiboa using the pre-defined converters:
 
 - `fiboa convert de_nrw`
 
 Available converters:
```

### Comparing `fiboa-cli-0.3.1/fiboa_cli.egg-info/SOURCES.txt` & `fiboa-cli-0.3.2/fiboa_cli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 fiboa_cli/create_geojson.py
 fiboa_cli/create_geoparquet.py
 fiboa_cli/describe.py
 fiboa_cli/geopandas.py
 fiboa_cli/jsonschema.py
 fiboa_cli/jsonschema_template.py
 fiboa_cli/parquet.py
+fiboa_cli/rename_extension.py
 fiboa_cli/types.py
 fiboa_cli/util.py
 fiboa_cli/validate.py
 fiboa_cli/validate_data.py
 fiboa_cli/validate_schema.py
 fiboa_cli/version.py
 fiboa_cli.egg-info/PKG-INFO
```

### Comparing `fiboa-cli-0.3.1/setup.py` & `fiboa-cli-0.3.2/setup.py`

 * *Files identical despite different names*

