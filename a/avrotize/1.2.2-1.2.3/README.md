# Comparing `tmp/avrotize-1.2.2.tar.gz` & `tmp/avrotize-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avrotize-1.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "avrotize-1.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `avrotize-1.2.2.tar` & `avrotize-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    25996 2024-04-11 14:43:14.781846 avrotize-1.2.2/README.md
--rw-r--r--   0        0        0     1673 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/__init__.py
--rw-r--r--   0        0        0       88 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/__main__.py
--rw-r--r--   0        0        0      411 2024-04-11 14:43:19.905905 avrotize-1.2.2/avrotize/_version.py
--rw-r--r--   0        0        0     8386 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/asn1toavro.py
--rw-r--r--   0        0        0    15558 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotize.py
--rw-r--r--   0        0        0    31485 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotocsharp.py
--rw-r--r--   0        0        0    18518 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojava.py
--rw-r--r--   0        0        0    12102 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojs.py
--rw-r--r--   0        0        0    18100 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotojsons.py
--rw-r--r--   0        0        0     5155 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotokusto.py
--rw-r--r--   0        0        0     5481 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoparquet.py
--rw-r--r--   0        0        0    22185 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoproto.py
--rw-r--r--   0        0        0    13086 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotopython.py
--rw-r--r--   0        0        0    10151 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotots.py
--rw-r--r--   0        0        0     9514 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrototsql.py
--rw-r--r--   0        0        0    16313 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/avrotoxsd.py
--rw-r--r--   0        0        0    12889 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/common.py
--rw-r--r--   0        0        0    19374 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/dependency_resolver.py
--rw-r--r--   0        0        0     1272 2024-04-11 14:43:14.781846 avrotize-1.2.2/avrotize/generic/generic.avsc
--rw-r--r--   0        0        0    91408 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/jsonstoavro.py
--rw-r--r--   0        0        0     2112 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/kconnect.json
--rw-r--r--   0        0        0     2537 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/kstructtoavro.py
--rw-r--r--   0        0        0    19742 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/proto2parser.py
--rw-r--r--   0        0        0    15536 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/proto3parser.py
--rw-r--r--   0        0        0     8722 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototoavro.py
--rw-r--r--   0        0        0     3390 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/any.avsc
--rw-r--r--   0        0        0     6521 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/api.avsc
--rw-r--r--   0        0        0     1629 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/duration.avsc
--rw-r--r--   0        0        0     3558 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/field_mask.avsc
--rw-r--r--   0        0        0     2394 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/struct.avsc
--rw-r--r--   0        0        0      792 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/timestamp.avsc
--rw-r--r--   0        0        0     6296 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/type.avsc
--rw-r--r--   0        0        0     2571 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/prototypes/wrappers.avsc
--rw-r--r--   0        0        0    15752 2024-04-11 14:43:14.785846 avrotize-1.2.2/avrotize/xsdtoavro.py
--rw-r--r--   0        0        0     1019 2024-04-11 14:43:14.785846 avrotize-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    25996 2024-04-11 18:17:04.090406 avrotize-1.2.3/README.md
+-rw-r--r--   0        0        0     1673 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/__main__.py
+-rw-r--r--   0        0        0      411 2024-04-11 18:17:16.478458 avrotize-1.2.3/avrotize/_version.py
+-rw-r--r--   0        0        0     8386 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/asn1toavro.py
+-rw-r--r--   0        0        0    15558 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotize.py
+-rw-r--r--   0        0        0    36250 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotocsharp.py
+-rw-r--r--   0        0        0    18518 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotojava.py
+-rw-r--r--   0        0        0    12102 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotojs.py
+-rw-r--r--   0        0        0    18100 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotojsons.py
+-rw-r--r--   0        0        0     5155 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotokusto.py
+-rw-r--r--   0        0        0     5481 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotoparquet.py
+-rw-r--r--   0        0        0    22185 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotoproto.py
+-rw-r--r--   0        0        0    13086 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotopython.py
+-rw-r--r--   0        0        0    10151 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotots.py
+-rw-r--r--   0        0        0     9514 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrototsql.py
+-rw-r--r--   0        0        0    16313 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/avrotoxsd.py
+-rw-r--r--   0        0        0    12889 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/common.py
+-rw-r--r--   0        0        0    19374 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/dependency_resolver.py
+-rw-r--r--   0        0        0     1272 2024-04-11 18:17:04.090406 avrotize-1.2.3/avrotize/generic/generic.avsc
+-rw-r--r--   0        0        0    91408 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/jsonstoavro.py
+-rw-r--r--   0        0        0     2112 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/kconnect.json
+-rw-r--r--   0        0        0     2537 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/kstructtoavro.py
+-rw-r--r--   0        0        0    19742 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/proto2parser.py
+-rw-r--r--   0        0        0    15536 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/proto3parser.py
+-rw-r--r--   0        0        0     8722 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototoavro.py
+-rw-r--r--   0        0        0     3390 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/any.avsc
+-rw-r--r--   0        0        0     6521 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/api.avsc
+-rw-r--r--   0        0        0     1629 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/duration.avsc
+-rw-r--r--   0        0        0     3558 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/field_mask.avsc
+-rw-r--r--   0        0        0     2394 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/struct.avsc
+-rw-r--r--   0        0        0      792 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/timestamp.avsc
+-rw-r--r--   0        0        0     6296 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/type.avsc
+-rw-r--r--   0        0        0     2571 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/prototypes/wrappers.avsc
+-rw-r--r--   0        0        0    15752 2024-04-11 18:17:04.094406 avrotize-1.2.3/avrotize/xsdtoavro.py
+-rw-r--r--   0        0        0     1019 2024-04-11 18:17:04.094406 avrotize-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    26663 1970-01-01 00:00:00.000000 avrotize-1.2.3/PKG-INFO
```

### Comparing `avrotize-1.2.2/README.md` & `avrotize-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/__init__.py` & `avrotize-1.2.3/avrotize/__init__.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/asn1toavro.py` & `avrotize-1.2.3/avrotize/asn1toavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotize.py` & `avrotize-1.2.3/avrotize/avrotize.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotocsharp.py` & `avrotize-1.2.3/avrotize/avrotocsharp.py`

 * *Files 6% similar despite different names*

```diff
@@ -294,56 +294,109 @@
         if self.newtonsoft_json_annotation:
             class_definition += f'\n{INDENT*2}'+f'\n{INDENT*2}'.join(
                 NEWTONSOFT_JSON_FROMDATA.strip().replace("{type_name}", class_name).split("\n"))
         class_definition += f"\n{INDENT*2}throw new System.NotImplementedException($\"Unsupported content type {{contentType}}\");\n{INDENT}}}"
 
         # emit IsJsonMatch method for System.Text.Json
         if self.system_text_json_annotation:
-            class_definition += f"\n\n{INDENT}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT}{{"
-            class_definition += f"\n{INDENT*2}return "
-            field_count = 0
-            for field in avro_schema.get('fields', []):
-                if field_count > 0:
-                    class_definition += f" && \n{INDENT*3}"
-                field_count += 1
-                field_name = field['name']
-                if self.is_csharp_reserved_word(field_name):
-                    field_name = f"@{field_name}"
-                if field_name == class_name:
-                    field_name += "_"
-                field_type = self.convert_avro_type_to_csharp(
-                    class_name, field_name, field['type'], namespace)
-                is_optional = field_type[-1] == '?'
-                field_type = field_type[:-1] if is_optional else field_type
-                if field_type == 'byte[]':
-                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.String){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
-                elif field_type == 'string':
-                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.String){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
-                elif field_type in ['int', 'long', 'float', 'double', 'decimal', 'short', 'sbyte', 'ushort', 'uint', 'ulong']:
-                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.Number){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
-                elif field_type == 'bool':
-                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.True || {field_name}.ValueKind == System.Text.Json.JsonValueKind.False){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
-                elif field_type.startswith("global::"):
-                    type_kind = self.generated_types[field_type] if field_type in self.generated_types else "class"
-                    if type_kind == "class":
-                        class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({f'{field_name}.ValueKind == System.Text.Json.JsonValueKind.Null || ' if is_optional else ''}{field_type}.IsJsonMatch({field_name})))"
-                    elif type_kind == "enum":
-                        class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({f'{field_name}.ValueKind == System.Text.Json.JsonValueKind.Null ||' if is_optional else ''}({field_name}.ValueKind == System.Text.Json.JsonValueKind.String && Enum.TryParse<{field_type}>({field_name}.GetString(), true, out _ ))))"
-                else:
-                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} true )"
-            class_definition += f";\n{INDENT}}}"
-
+            class_definition += self.create_is_json_match_method(avro_schema, namespace, class_name)
         class_definition += "\n"+"}"
 
         if write_file:
             self.write_to_file(namespace, class_name, class_definition)
         ref = 'global::'+self.concat_namespace(namespace, class_name)
         self.generated_types[ref] = "class"
         return ref
 
+    def create_is_json_match_method(self, avro_schema, namespace, class_name) -> str:
+        """ Generates the IsJsonMatch method for System.Text.Json """
+        class_definition = ''
+        class_definition += f"\n\n{INDENT}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT}{{"
+        class_definition += f"\n{INDENT*2}return "
+        field_count = 0
+        for field in avro_schema.get('fields', []):
+            if field_count > 0:
+                class_definition += f" && \n{INDENT*3}"
+            field_count += 1
+            field_name = field['name']
+            if self.is_csharp_reserved_word(field_name):
+                field_name = f"@{field_name}"
+            if field_name == class_name:
+                field_name += "_"
+            field_type = self.convert_avro_type_to_csharp(
+                    class_name, field_name, field['type'], namespace)
+            class_definition += self.get_is_json_match_clause(class_name, field_name, field_type)
+        class_definition += f";\n{INDENT}}}"
+        return class_definition
+
+    def get_is_json_match_clause(self, class_name, field_name, field_type) -> str:
+        """ Generates the IsJsonMatch clause for a field """
+        class_definition = ''
+        field_name_js = field_name[1:] if field_name[0] == '@' else field_name
+        is_optional = field_type[-1] == '?'
+        field_type = field_type[:-1] if is_optional else field_type
+        if field_type == 'byte[]':
+            class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.String){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type == 'string':
+            class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.String){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type in ['int', 'long', 'float', 'double', 'decimal', 'short', 'sbyte', 'ushort', 'uint', 'ulong']:
+            class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.Number){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type == 'bool':
+            class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({field_name}.ValueKind == System.Text.Json.JsonValueKind.True || {field_name}.ValueKind == System.Text.Json.JsonValueKind.False){f' || {field_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type.startswith("global::"):
+            type_kind = self.generated_types[field_type] if field_type in self.generated_types else "class"
+            if type_kind == "class":
+                class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({f'{field_name}.ValueKind == System.Text.Json.JsonValueKind.Null || ' if is_optional else ''}{field_type}.IsJsonMatch({field_name})))"
+            elif type_kind == "enum":
+                class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({f'{field_name}.ValueKind == System.Text.Json.JsonValueKind.Null ||' if is_optional else ''}({field_name}.ValueKind == System.Text.Json.JsonValueKind.String && Enum.TryParse<{field_type}>({field_name}.GetString(), true, out _ ))))"
+        else:
+            is_union = False
+            field_union = pascal(field_name)+'Union'
+            if field_type == field_union:
+                field_union = class_name+"."+pascal(field_name)+'Union'
+                type_kind = self.generated_types[field_union] if field_union in self.generated_types else "class"
+                if type_kind == "union":
+                    is_union = True
+                    class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} ({f'{field_name}.ValueKind == System.Text.Json.JsonValueKind.Null || ' if is_optional else ''}{field_type}.IsJsonMatch({field_name})))"
+            if not is_union:
+                class_definition += f"({'!' if is_optional else ''}element.TryGetProperty(\"{field_name_js}\", out System.Text.Json.JsonElement {field_name}) {'||' if is_optional else '&&'} true )"
+        return class_definition
+    
+    def get_is_json_match_clause_type(self, element_name, class_name, field_type) -> str:
+        """ Generates the IsJsonMatch clause for a field """
+        class_definition = ''
+        is_optional = field_type[-1] == '?'
+        field_type = field_type[:-1] if is_optional else field_type
+        if field_type == 'byte[]':
+            class_definition += f"({element_name}.ValueKind == System.Text.Json.JsonValueKind.String{f' || {element_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type == 'string':
+            class_definition += f"({element_name}.ValueKind == System.Text.Json.JsonValueKind.String{f' || {element_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type in ['int', 'long', 'float', 'double', 'decimal', 'short', 'sbyte', 'ushort', 'uint', 'ulong']:
+            class_definition += f"({element_name}.ValueKind == System.Text.Json.JsonValueKind.Number{f' || {element_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type == 'bool':
+            class_definition += f"({element_name}.ValueKind == System.Text.Json.JsonValueKind.True || {element_name}.ValueKind == System.Text.Json.JsonValueKind.False{f' || {element_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        elif field_type.startswith("global::"):
+            type_kind = self.generated_types[field_type] if field_type in self.generated_types else "class"
+            if type_kind == "class":
+                class_definition += f"({f'{element_name}.ValueKind == System.Text.Json.JsonValueKind.Null || ' if is_optional else ''}{field_type}.IsJsonMatch({element_name}))"
+            elif type_kind == "enum":
+                class_definition += f"({f'{element_name}.ValueKind == System.Text.Json.JsonValueKind.Null ||' if is_optional else ''}({element_name}.ValueKind == System.Text.Json.JsonValueKind.String && Enum.TryParse<{field_type}>({element_name}.GetString(), true, out _ ))))"
+        else:
+            is_union = False
+            field_union = pascal(element_name)+'Union'
+            if field_type == field_union:
+                field_union = class_name+"."+pascal(element_name)+'Union'
+                type_kind = self.generated_types[field_union] if field_union in self.generated_types else "class"
+                if type_kind == "union":
+                    is_union = True
+                    class_definition += f"({f'{element_name}.ValueKind == System.Text.Json.JsonValueKind.Null || ' if is_optional else ''}{field_type}.IsJsonMatch({element_name})))"
+            if not is_union:
+                class_definition += f"({element_name}.ValueKind == System.Text.Json.JsonValueKind.Object{f' || {element_name}.ValueKind == System.Text.Json.JsonValueKind.Null' if is_optional else ''})"
+        return class_definition
+
     def generate_enum(self, avro_schema: Dict, parent_namespace: str, write_file: bool) -> str:
         """ Generates an Enum """
         enum_definition = ''
         namespace = pascal(self.concat_namespace(
             self.base_namespace, avro_schema.get('namespace', parent_namespace)))
         if 'doc' in avro_schema:
             enum_definition += f"/// <summary>\n/// {avro_schema['doc']}\n/// </summary>\n"
@@ -358,14 +411,15 @@
         ref = 'global::'+self.concat_namespace(namespace, enum_name)
         self.generated_types[ref] = "enum"
         return ref
 
     def generate_embedded_union_class_system_json_text(self, class_name: str, field_name: str, avro_type: List, parent_namespace: str, write_file: bool) -> str:
         """ Generates an embedded Union Class """
         class_definition_ctors = class_definition_decls = class_definition_read = class_definition_write = class_definition = ''
+        list_is_json_match: List [str] = []
         union_class_name = pascal(field_name)+'Union'
         union_types = [self.convert_avro_type_to_csharp(class_name, field_name+"Option"+str(i), t, parent_namespace) for i,t in enumerate(avro_type)]
         for i, union_type in enumerate(union_types):
             is_dict = is_list = False
             if union_type.startswith("Dictionary<"):
                 # get the type information from the dictionary
                 is_dict = True
@@ -406,30 +460,36 @@
                 elif union_type == "DateTime":
                     class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.String)\n{INDENT*3}{{\n{INDENT*4}return new {union_class_name}(System.DateTime.Parse(element.GetString()));\n{INDENT*3}}}\n"
                 elif union_type == "DateTimeOffset":
                     class_definition_read += f"{INDENT*3}if (element.ValueKind == JsonValueKind.String)\n{INDENT*3}{{\n{INDENT*4}return new {union_class_name}(System.DateTimeOffset.Parse(element.GetString()));\n{INDENT*3}}}\n"
             else:
                 class_definition_read += f"{INDENT*3}if ({union_type}.IsJsonMatch(element))\n{INDENT*3}{{\n{INDENT*4}return new {union_class_name}({union_type}.FromData(element, System.Net.Mime.MediaTypeNames.Application.Json));\n{INDENT*3}}}\n"
             class_definition_write += f"{INDENT*3}{'else ' if i>0 else ''}if (value.{union_type_name} != null)\n{INDENT*3}{{\n{INDENT*4}System.Text.Json.JsonSerializer.Serialize(writer, value.{union_type_name}, options);\n{INDENT*3}}}\n"
+            gij = self.get_is_json_match_clause_type("element", class_name, union_type)
+            if gij:
+                list_is_json_match.append(gij)
 
         class_definition = \
             f"public partial class {class_name}\n{{\n{INDENT}[System.Text.Json.Serialization.JsonConverter(typeof({union_class_name}))]\n{INDENT}public sealed class {union_class_name} : System.Text.Json.Serialization.JsonConverter<{union_class_name}>\n{INDENT}{{\n" + \
             f"{INDENT*2}public {union_class_name}() {{ }}\n" + \
             class_definition_ctors + \
             class_definition_decls + \
             f"\n{INDENT*2}public override {union_class_name}? Read(ref Utf8JsonReader reader, Type typeToConvert, JsonSerializerOptions options)\n{INDENT*2}{{\n{INDENT*3}var element = JsonElement.ParseValue(ref reader);\n" + \
             class_definition_read + \
             f"{INDENT*3}throw new NotSupportedException(\"No record type matched the JSON data\");\n{INDENT*2}}}\n" + \
             f"\n{INDENT*2}public override void Write(Utf8JsonWriter writer, {union_class_name} value, JsonSerializerOptions options)\n{INDENT*2}{{\n" + \
             class_definition_write + \
             f"{INDENT*3}else\n{INDENT*3}{{\n{INDENT*4}throw new NotSupportedException(\"No record type is set in the union\");\n{INDENT*3}}}\n{INDENT*2}}}\n" + \
-            f"{INDENT}}}\n}}\n"
+            f"\n{INDENT*2}public static bool IsJsonMatch(System.Text.Json.JsonElement element)\n{INDENT*2}{{" + \
+            f"\n{INDENT*3}return "+f"\n{INDENT*3} || ".join(list_is_json_match)+f";\n{INDENT*2}}}\n" + \
+            f"{INDENT*1}}}\n}}\n"
 
         if write_file:
             self.write_to_file(parent_namespace, class_name +"."+union_class_name, class_definition)
+        self.generated_types[class_name+'.'+union_class_name] = "union" # it doesn't matter if the names clash, we just need to know whether it's a union
         return union_class_name
 
     def generate_property(self, field: Dict, class_name: str, parent_namespace: str) -> str:
         """ Generates a property """
         field_type = self.convert_avro_type_to_csharp(
             class_name, field['name'], field['type'], parent_namespace)
         annotation_name = field_name = field['name']
```

### Comparing `avrotize-1.2.2/avrotize/avrotojava.py` & `avrotize-1.2.3/avrotize/avrotojava.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotojs.py` & `avrotize-1.2.3/avrotize/avrotojs.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotojsons.py` & `avrotize-1.2.3/avrotize/avrotojsons.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotokusto.py` & `avrotize-1.2.3/avrotize/avrotokusto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotoparquet.py` & `avrotize-1.2.3/avrotize/avrotoparquet.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotoproto.py` & `avrotize-1.2.3/avrotize/avrotoproto.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotopython.py` & `avrotize-1.2.3/avrotize/avrotopython.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotots.py` & `avrotize-1.2.3/avrotize/avrotots.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrototsql.py` & `avrotize-1.2.3/avrotize/avrototsql.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/avrotoxsd.py` & `avrotize-1.2.3/avrotize/avrotoxsd.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/common.py` & `avrotize-1.2.3/avrotize/common.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/dependency_resolver.py` & `avrotize-1.2.3/avrotize/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/generic/generic.avsc` & `avrotize-1.2.3/avrotize/generic/generic.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/jsonstoavro.py` & `avrotize-1.2.3/avrotize/jsonstoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/kconnect.json` & `avrotize-1.2.3/avrotize/kconnect.json`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/kstructtoavro.py` & `avrotize-1.2.3/avrotize/kstructtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/proto2parser.py` & `avrotize-1.2.3/avrotize/proto2parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/proto3parser.py` & `avrotize-1.2.3/avrotize/proto3parser.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototoavro.py` & `avrotize-1.2.3/avrotize/prototoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/any.avsc` & `avrotize-1.2.3/avrotize/prototypes/any.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/api.avsc` & `avrotize-1.2.3/avrotize/prototypes/api.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/duration.avsc` & `avrotize-1.2.3/avrotize/prototypes/duration.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/field_mask.avsc` & `avrotize-1.2.3/avrotize/prototypes/field_mask.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/struct.avsc` & `avrotize-1.2.3/avrotize/prototypes/struct.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/timestamp.avsc` & `avrotize-1.2.3/avrotize/prototypes/timestamp.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/type.avsc` & `avrotize-1.2.3/avrotize/prototypes/type.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/prototypes/wrappers.avsc` & `avrotize-1.2.3/avrotize/prototypes/wrappers.avsc`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/avrotize/xsdtoavro.py` & `avrotize-1.2.3/avrotize/xsdtoavro.py`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/pyproject.toml` & `avrotize-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avrotize-1.2.2/PKG-INFO` & `avrotize-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avrotize
-Version: 1.2.2
+Version: 1.2.3
 Summary: Tools to convert from and to Avro Schema from various other schema languages.
 Author-email: Clemens Vasters <clemensv@microsoft.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

