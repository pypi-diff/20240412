# Comparing `tmp/pcffont-0.0.1.tar.gz` & `tmp/pcffont-0.0.2.tar.gz`

## Comparing `pcffont-0.0.1.tar` & `pcffont-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.1/requirements.txt
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/artwiz/anorexia.pcf
--rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/artwiz/kates.pcf
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/dweep/dweep.pcf
--rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/profont-x11/ProFont_r400-29.pcf
--rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/raize/raize-normal-19.pcf
--rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/sgi/rock36.pcf
--rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/trisk/trisk.pcf
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/unifont/OFL.txt
--rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.1/assets/unifont/unifont-15.1.05.pcf
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.1/examples/__init__.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 pcffont-0.0.1/examples/demo.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/__init__.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/error.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/font.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/header.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/metric.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_accelerators.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_bitmaps.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_encodings.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_glyph_names.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_metrics.py
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_properties.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/t_scalable_widths.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/table.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/xlfd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/internal/__init__.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/internal/buffer.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 pcffont-0.0.1/src/pcffont/internal/util.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pcffont-0.0.1/tests/test_dump.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pcffont-0.0.1/tests/test_load_save.py
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 pcffont-0.0.1/tests/test_reload.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.1/LICENSE
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 pcffont-0.0.1/README.md
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 pcffont-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pcffont-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pcffont-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pcffont-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/artwiz/anorexia.pcf
+-rw-r--r--   0        0        0    23368 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/artwiz/kates.pcf
+-rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/dweep/dweep.pcf
+-rw-r--r--   0        0        0    37540 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/profont-x11/ProFont_r400-29.pcf
+-rw-r--r--   0        0        0    17888 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/raize/raize-normal-19.pcf
+-rw-r--r--   0        0        0    22688 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/sgi/rock36.pcf
+-rw-r--r--   0        0        0    13832 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/trisk/trisk.pcf
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/unifont/OFL.txt
+-rw-r--r--   0        0        0  5155808 2020-02-02 00:00:00.000000 pcffont-0.0.2/assets/unifont/unifont-15.1.05.pcf
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pcffont-0.0.2/examples/__init__.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pcffont-0.0.2/examples/demo.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/__init__.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/error.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/font.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/header.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/metric.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_accelerators.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_bitmaps.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_encodings.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_glyph_names.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_metrics.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_properties.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/t_scalable_widths.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/table.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/xlfd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/buffer.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 pcffont-0.0.2/src/pcffont/internal/util.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_dump.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_load_save.py
+-rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 pcffont-0.0.2/tests/test_reload.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 pcffont-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pcffont-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pcffont-0.0.2/README.md
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 pcffont-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 pcffont-0.0.2/PKG-INFO
```

### Comparing `pcffont-0.0.1/.github/workflows/publish.yml` & `pcffont-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/.github/workflows/test.yml` & `pcffont-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/artwiz/anorexia.pcf` & `pcffont-0.0.2/assets/artwiz/anorexia.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/artwiz/kates.pcf` & `pcffont-0.0.2/assets/artwiz/kates.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/dweep/dweep.pcf` & `pcffont-0.0.2/assets/dweep/dweep.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/profont-x11/ProFont_r400-29.pcf` & `pcffont-0.0.2/assets/profont-x11/ProFont_r400-29.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/raize/raize-normal-19.pcf` & `pcffont-0.0.2/assets/raize/raize-normal-19.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/sgi/rock36.pcf` & `pcffont-0.0.2/assets/sgi/rock36.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/trisk/trisk.pcf` & `pcffont-0.0.2/assets/trisk/trisk.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/unifont/OFL.txt` & `pcffont-0.0.2/assets/unifont/OFL.txt`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/assets/unifont/unifont-15.1.05.pcf` & `pcffont-0.0.2/assets/unifont/unifont-15.1.05.pcf`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/examples/demo.py` & `pcffont-0.0.2/examples/demo.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,17 +12,24 @@
     os.makedirs(outputs_dir)
 
     font = PcfFont.load(os.path.join(assets_dir, 'unifont', 'unifont-15.1.05.pcf'))
     print(f'name: {font.properties.font}')
     print(f'size: {font.properties.pixel_size}')
     print(f'ascent: {font.accelerators.font_ascent}')
     print(f'descent: {font.accelerators.font_descent}')
+    print()
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
-        print(f'{code_point:04X} {chr(code_point)} - {font.glyph_names[glyph_index]}')
-        for bitmap_row in font.bitmaps[glyph_index]:
-            print(''.join(map(str, bitmap_row)).replace('0', '__').replace('1', '**'))
+        glyph_name = font.glyph_names[glyph_index]
+        metric = font.metrics[glyph_index]
+        bitmap = font.bitmaps[glyph_index]
+        print(f'char: {chr(code_point)} ({code_point:04X})')
+        print(f'glyph_name: {glyph_name}')
+        print(f'advance_width: {metric.character_width}')
+        print(f'offset: ({-metric.left_sided_bearing}, {-metric.character_descent})')
+        for bitmap_row in bitmap:
+            print(f'{''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
 
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pcffont-0.0.1/src/pcffont/error.py` & `pcffont-0.0.2/src/pcffont/error.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/src/pcffont/font.py` & `pcffont-0.0.2/src/pcffont/font.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,35 @@
 from pcffont.t_properties import PcfProperties
 from pcffont.t_scalable_widths import PcfScalableWidths
 from pcffont.table import PcfTable
 
 
 class PcfFont(UserDict[PcfTableType, PcfTable]):
     @staticmethod
-    def parse(stream: BinaryIO) -> 'PcfFont':
+    def parse(stream: BinaryIO, strict_level: int = 1) -> 'PcfFont':
         buffer = Buffer(stream)
 
         headers = PcfHeader.parse(buffer)
 
         tables = {}
         for header in headers:
-            if header.table_type in tables:
+            if header.table_type in tables and strict_level >= 1:
                 raise PcfError(f"Duplicate table '{header.table_type.name}'")
-            tables[header.table_type] = util.parse_table(buffer, header)
+            table = util.parse_table(buffer, header, strict_level)
+            tables[header.table_type] = table
 
         return PcfFont(tables)
 
     @staticmethod
-    def load(file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> 'PcfFont':
+    def load(
+            file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes],
+            strict_level: int = 1,
+    ) -> 'PcfFont':
         with open(file_path, 'rb') as file:
-            return PcfFont.parse(file)
+            return PcfFont.parse(file, strict_level)
 
     def __init__(self, tables: dict[PcfTableType, PcfTable | None] = None):
         super().__init__(tables)
 
     def __setitem__(self, table_type: PcfTableType, table: PcfTable | None):
         if table is None:
             self.pop(table_type, None)
```

### Comparing `pcffont-0.0.1/src/pcffont/header.py` & `pcffont-0.0.2/src/pcffont/header.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/src/pcffont/metric.py` & `pcffont-0.0.2/src/pcffont/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pcffont.internal.buffer import ByteOrder, Buffer
 
 
 class PcfMetric:
     @staticmethod
     def parse(buffer: Buffer, byte_order: ByteOrder, is_compressed: bool) -> 'PcfMetric':
         if is_compressed:
-            left_sided_bearing = buffer.read_int8(byte_order)
-            right_side_bearing = buffer.read_int8(byte_order)
-            character_width = buffer.read_int8(byte_order)
-            character_ascent = buffer.read_int8(byte_order)
-            character_descent = buffer.read_int8(byte_order)
+            left_sided_bearing = buffer.read_int8(byte_order) - 0x80
+            right_side_bearing = buffer.read_int8(byte_order) - 0x80
+            character_width = buffer.read_int8(byte_order) - 0x80
+            character_ascent = buffer.read_int8(byte_order) - 0x80
+            character_descent = buffer.read_int8(byte_order) - 0x80
             character_attributes = 0
         else:
             left_sided_bearing = buffer.read_int16(byte_order)
             right_side_bearing = buffer.read_int16(byte_order)
             character_width = buffer.read_int16(byte_order)
             character_ascent = buffer.read_int16(byte_order)
             character_descent = buffer.read_int16(byte_order)
@@ -41,19 +41,19 @@
         self.character_width = character_width
         self.character_ascent = character_ascent
         self.character_descent = character_descent
         self.character_attributes = character_attributes
 
     def dump(self, buffer: Buffer, byte_order: ByteOrder, is_compressed: bool):
         if is_compressed:
-            buffer.write_int8(self.left_sided_bearing, byte_order)
-            buffer.write_int8(self.right_side_bearing, byte_order)
-            buffer.write_int8(self.character_width, byte_order)
-            buffer.write_int8(self.character_ascent, byte_order)
-            buffer.write_int8(self.character_descent, byte_order)
+            buffer.write_int8(self.left_sided_bearing + 0x80, byte_order)
+            buffer.write_int8(self.right_side_bearing + 0x80, byte_order)
+            buffer.write_int8(self.character_width + 0x80, byte_order)
+            buffer.write_int8(self.character_ascent + 0x80, byte_order)
+            buffer.write_int8(self.character_descent + 0x80, byte_order)
         else:
             buffer.write_int16(self.left_sided_bearing, byte_order)
             buffer.write_int16(self.right_side_bearing, byte_order)
             buffer.write_int16(self.character_width, byte_order)
             buffer.write_int16(self.character_ascent, byte_order)
             buffer.write_int16(self.character_descent, byte_order)
             buffer.write_int16(self.character_attributes, byte_order)
```

### Comparing `pcffont-0.0.1/src/pcffont/t_accelerators.py` & `pcffont-0.0.2/src/pcffont/t_accelerators.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
 class PcfAccelerators(PcfTable):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfAccelerators':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfAccelerators':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
         is_accel_w_ink_bounds = table_format & PcfTableFormat.ACCEL_W_INKBOUNDS > 0
 
         no_overlap = buffer.read_bool()
         constant_metrics = buffer.read_bool()
         terminal_font = buffer.read_bool()
@@ -23,31 +23,30 @@
         font_ascent = buffer.read_int32(byte_order)
         font_descent = buffer.read_int32(byte_order)
         max_overlap = buffer.read_int32(byte_order)
 
         min_bounds = PcfMetric.parse(buffer, byte_order, False)
         max_bounds = PcfMetric.parse(buffer, byte_order, False)
 
-        _ink_bounds_chunk = None  # TODO
-        _padding_chunk_info = None  # TODO
-
         if is_accel_w_ink_bounds:
             ink_min_bounds = PcfMetric.parse(buffer, byte_order, False)
             ink_max_bounds = PcfMetric.parse(buffer, byte_order, False)
         else:
             ink_min_bounds = None
             ink_max_bounds = None
-            # TODO
-            if header.table_size >= buffer.tell() - header.table_offset + 2 * 6 * 2:
-                _ink_bounds_chunk = buffer.read(2 * 6 * 2)
 
         # TODO
-        _padding = header.table_size - (buffer.tell() - header.table_offset)
-        if _padding > 0:
-            _padding_chunk_info = buffer.read(_padding), _padding
+        if header.table_size > buffer.tell() - header.table_offset:
+            buffer.seek(header.table_offset + 4 + 8 + 4 * 3 + 2 * 6 * 2)
+            _compat_chunk_start = buffer.tell() - header.table_offset
+            _compat_chunk_size = header.table_size - _compat_chunk_start
+            _compat_chunk = buffer.read(_compat_chunk_size)
+            _compat_info = _compat_chunk_start, _compat_chunk_size, _compat_chunk
+        else:
+            _compat_info = None
 
         return PcfAccelerators(
             table_format,
             no_overlap,
             constant_metrics,
             terminal_font,
             constant_width,
@@ -57,16 +56,15 @@
             font_ascent,
             font_descent,
             max_overlap,
             min_bounds,
             max_bounds,
             ink_min_bounds,
             ink_max_bounds,
-            _ink_bounds_chunk,  # TODO
-            _padding_chunk_info,  # TODO
+            _compat_info,
         )
 
     def __init__(
             self,
             table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
             no_overlap: bool = False,
             constant_metrics: bool = False,
@@ -78,16 +76,15 @@
             font_ascent: int = 0,
             font_descent: int = 0,
             max_overlap: int = 0,
             min_bounds: PcfMetric = None,
             max_bounds: PcfMetric = None,
             ink_min_bounds: PcfMetric = None,
             ink_max_bounds: PcfMetric = None,
-            _ink_bounds_chunk: bytes = None,  # TODO
-            _padding_chunk_info: tuple[bytes, int] = None,  # TODO
+            _compat_info: tuple[int, int, bytes] = None,
     ):
         super().__init__(table_format)
         self.no_overlap = no_overlap
         self.constant_metrics = constant_metrics
         self.terminal_font = terminal_font
         self.constant_width = constant_width
         self.ink_inside = ink_inside
@@ -96,16 +93,15 @@
         self.font_ascent = font_ascent
         self.font_descent = font_descent
         self.max_overlap = max_overlap
         self.min_bounds = min_bounds
         self.max_bounds = max_bounds
         self.ink_min_bounds = ink_min_bounds
         self.ink_max_bounds = ink_max_bounds
-        self._ink_bounds_chunk = _ink_bounds_chunk  # TODO
-        self._padding_chunk_info = _padding_chunk_info  # TODO
+        self._compat_info = _compat_info
 
     def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
         byte_order = util.get_table_byte_order(self.table_format)
         is_accel_w_ink_bounds = self.table_format & PcfTableFormat.ACCEL_W_INKBOUNDS > 0
 
         buffer.seek(table_offset)
         buffer.write_int32_le(self.table_format)
@@ -123,21 +119,30 @@
 
         self.min_bounds.dump(buffer, byte_order, False)
         self.max_bounds.dump(buffer, byte_order, False)
 
         if is_accel_w_ink_bounds:
             self.ink_min_bounds.dump(buffer, byte_order, False)
             self.ink_max_bounds.dump(buffer, byte_order, False)
-        else:
-            # TODO
-            if compat_mode and self._ink_bounds_chunk is not None:
-                buffer.write(self._ink_bounds_chunk)
 
         table_size = buffer.tell() - table_offset
 
         # TODO
-        if compat_mode and self._padding_chunk_info is not None:
-            _padding_chunk, _padding = self._padding_chunk_info
-            buffer.write(_padding_chunk)
-            table_size += _padding
+        if compat_mode and self._compat_info is not None:
+            _compat_chunk_start, _compat_chunk_size, _compat_chunk = self._compat_info
+            _compat_chunk = bytearray(_compat_chunk)
+
+            ink_chunk_size = 2 * 6 * 2
+            if table_size == _compat_chunk_start + ink_chunk_size:
+                _compat_chunk_start += ink_chunk_size
+                _compat_chunk_size -= ink_chunk_size
+                for _ in range(ink_chunk_size):
+                    if len(_compat_chunk) == 0:
+                        break
+                    _compat_chunk.pop(0)
+            else:
+                assert table_size == _compat_chunk_start
+
+            buffer.write(_compat_chunk)
+            table_size += _compat_chunk_size
 
         return table_size
```

### Comparing `pcffont-0.0.1/src/pcffont/t_bitmaps.py` & `pcffont-0.0.2/src/pcffont/t_bitmaps.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 new_bitmap_row.append(0)
         new_bitmap.append(new_bitmap_row)
     return new_bitmap
 
 
 class PcfBitmaps(PcfTable, UserList[list[list[int]]]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfBitmaps':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBitmaps':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
 
         # How each row in each glyph's bitmap is padded
         # 0 => byte, 1 => short, 2 => int32, 3 => int64
         bitmap_padded_mode = table_format & 3
         bitmap_row_size = [1, 2, 4, 8][bitmap_padded_mode]
@@ -67,19 +67,19 @@
 
         return PcfBitmaps(table_format, bitmaps, size_configs)
 
     def __init__(
             self,
             table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
             bitmaps: list[list[list[int]]] = None,
-            _old_size_configs: list[int] = None,  # TODO
+            _compat_size_configs: list[int] = None,
     ):
         PcfTable.__init__(self, table_format)
         UserList.__init__(self, bitmaps)
-        self._old_size_configs = _old_size_configs  # TODO
+        self._compat_size_configs = _compat_size_configs
 
     def _dump(self, buffer: Buffer, table_offset: int, compat_mode: bool = False) -> int:
         byte_order = util.get_table_byte_order(self.table_format)
 
         # How each row in each glyph's bitmap is padded
         # 0 => byte, 1 => short, 2 => int32, 3 => int64
         bitmap_padded_mode = self.table_format & 3
@@ -106,16 +106,16 @@
                     if byte_order == 'little':
                         array.reverse()
                     bin_string = ''.join(map(str, array))
                     data = int(bin_string, 2).to_bytes(1, 'big')
                     bitmaps_size += buffer.write(data)
 
         # TODO
-        if compat_mode and self._old_size_configs is not None:
-            size_configs = list(self._old_size_configs)
+        if compat_mode and self._compat_size_configs is not None:
+            size_configs = list(self._compat_size_configs)
             size_configs[bitmap_padded_mode] = bitmaps_size
         else:
             unit_size_config = bitmaps_size // bitmap_row_size
             size_configs = [
                 unit_size_config,
                 unit_size_config * 2,
                 unit_size_config * 4,
```

### Comparing `pcffont-0.0.1/src/pcffont/t_encodings.py` & `pcffont-0.0.2/src/pcffont/t_encodings.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class PcfBdfEncodings(PcfTable, UserDict[int, int]):
     """
     code_point -> glyph_index
     """
 
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfBdfEncodings':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfBdfEncodings':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
 
         min_char_or_byte2 = buffer.read_int16(byte_order)
         max_char_or_byte2 = buffer.read_int16(byte_order)
         min_byte1 = buffer.read_int16(byte_order)
         max_byte1 = buffer.read_int16(byte_order)
```

### Comparing `pcffont-0.0.1/src/pcffont/t_glyph_names.py` & `pcffont-0.0.2/src/pcffont/t_glyph_names.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 
 class PcfGlyphNames(PcfTable, UserList[str]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfGlyphNames':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfGlyphNames':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
 
         glyphs_count = buffer.read_int32(byte_order)
         name_offsets = [buffer.read_int32(byte_order) for _ in range(glyphs_count)]
         buffer.skip_int()  # strings_size
         strings_start = buffer.tell()
```

### Comparing `pcffont-0.0.1/src/pcffont/t_metrics.py` & `pcffont-0.0.2/src/pcffont/t_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pcffont.internal.buffer import Buffer
 from pcffont.metric import PcfMetric
 from pcffont.table import PcfTable
 
 
 class PcfMetrics(PcfTable, UserList[PcfMetric]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfMetrics':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfMetrics':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
         is_compressed = table_format & PcfTableFormat.COMPRESSED_METRICS > 0
 
         if is_compressed:
             metrics_count = buffer.read_int16(byte_order)
         else:
```

### Comparing `pcffont-0.0.1/src/pcffont/t_properties.py` & `pcffont-0.0.2/src/pcffont/t_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         matched = re.search(r'[-?*,"]', value)
         if matched is not None:
             raise PcfPropValueError(key, value, f"contains illegal characters '{matched.group()}'")
 
 
 class PcfProperties(PcfTable, UserDict[str, str | int]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfProperties':
+    def parse(buffer: Buffer, header: PcfHeader, strict_level: int) -> 'PcfProperties':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
 
         props_count = buffer.read_int32(byte_order)
 
         prop_infos = []
         for _ in range(props_count):
@@ -134,15 +134,22 @@
             buffer.seek(strings_start + key_offset)
             key = buffer.read_string()
             if is_string_prop:
                 buffer.seek(strings_start + value)
                 value = buffer.read_string()
             else:
                 value = int(value)
-            properties[key] = value
+
+            try:
+                _check_key(key)
+                _check_value(key, value)
+                properties[key] = value
+            except (PcfPropKeyError, PcfPropValueError) as e:
+                if strict_level >= 1:
+                    raise e
 
         return PcfProperties(table_format, properties)
 
     def __init__(
             self,
             table_format: int = PcfTable.DEFAULT_TABLE_FORMAT,
             properties: dict[str, str | int] = None,
```

### Comparing `pcffont-0.0.1/src/pcffont/t_scalable_widths.py` & `pcffont-0.0.2/src/pcffont/t_scalable_widths.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pcffont.internal import util
 from pcffont.internal.buffer import Buffer
 from pcffont.table import PcfTable
 
 
 class PcfScalableWidths(PcfTable, UserList[int]):
     @staticmethod
-    def parse(buffer: Buffer, header: PcfHeader) -> 'PcfScalableWidths':
+    def parse(buffer: Buffer, header: PcfHeader, _strict_level: int) -> 'PcfScalableWidths':
         table_format = util.read_and_check_table_format(buffer, header)
         byte_order = util.get_table_byte_order(table_format)
 
         glyphs_count = buffer.read_int32(byte_order)
         scalable_widths = [buffer.read_int32(byte_order) for _ in range(glyphs_count)]
 
         return PcfScalableWidths(table_format, scalable_widths)
```

### Comparing `pcffont-0.0.1/src/pcffont/table.py` & `pcffont-0.0.2/src/pcffont/table.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/src/pcffont/xlfd.py` & `pcffont-0.0.2/src/pcffont/xlfd.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/src/pcffont/internal/buffer.py` & `pcffont-0.0.2/src/pcffont/internal/buffer.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/src/pcffont/internal/util.py` & `pcffont-0.0.2/src/pcffont/internal/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     PcfTableType.BDF_ENCODINGS: PcfBdfEncodings,
     PcfTableType.SWIDTHS: PcfScalableWidths,
     PcfTableType.GLYPH_NAMES: PcfGlyphNames,
     PcfTableType.BDF_ACCELERATORS: PcfAccelerators,
 }
 
 
-def parse_table(buffer: Buffer, header: PcfHeader) -> PcfTable | None:
+def parse_table(buffer: Buffer, header: PcfHeader, strict_level: int = 1) -> PcfTable | None:
     clz = TABLE_TYPE_REGISTRY.get(header.table_type, None)
     if clz is not None:
-        return clz.parse(buffer, header)
+        return clz.parse(buffer, header, strict_level)
     return None
 
 
 def read_and_check_table_format(buffer: Buffer, header: PcfHeader) -> int:
     buffer.seek(header.table_offset)
     table_format = buffer.read_int32_le()
     if table_format != header.table_format:
```

### Comparing `pcffont-0.0.1/tests/test_dump.py` & `pcffont-0.0.2/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/tests/test_load_save.py` & `pcffont-0.0.2/tests/test_load_save.py`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/tests/test_reload.py` & `pcffont-0.0.2/tests/test_reload.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,16 @@
     assert font_1.accelerators.min_bounds.character_attributes == font_2.accelerators.min_bounds.character_attributes == 0
 
     assert font_1.accelerators.ink_min_bounds is None
     assert font_1.accelerators.ink_max_bounds is None
     assert font_2.accelerators.ink_min_bounds is None
     assert font_2.accelerators.ink_max_bounds is None
 
-    assert font_1.accelerators._ink_bounds_chunk is not None
-    assert font_1.accelerators._padding_chunk_info is not None
-    assert font_2.accelerators._ink_bounds_chunk is None
-    assert font_2.accelerators._padding_chunk_info is None
+    assert font_1.accelerators._compat_info is not None
+    assert font_2.accelerators._compat_info is None
 
     assert len(font_1.metrics) == len(font_2.metrics)
     for glyph_index, metric_1 in enumerate(font_1.metrics):
         metric_2 = font_2.metrics[glyph_index]
         assert metric_1.left_sided_bearing == metric_2.left_sided_bearing
         assert metric_1.right_side_bearing == metric_2.right_side_bearing
         assert metric_1.character_width == metric_2.character_width
@@ -110,11 +108,9 @@
     assert font_1.bdf_accelerators.min_bounds.character_attributes == font_2.bdf_accelerators.min_bounds.character_attributes == 0
 
     assert font_1.bdf_accelerators.ink_min_bounds is None
     assert font_1.bdf_accelerators.ink_max_bounds is None
     assert font_2.bdf_accelerators.ink_min_bounds is None
     assert font_2.bdf_accelerators.ink_max_bounds is None
 
-    assert font_1.bdf_accelerators._ink_bounds_chunk is not None
-    assert font_1.bdf_accelerators._padding_chunk_info is not None
-    assert font_2.bdf_accelerators._ink_bounds_chunk is None
-    assert font_2.bdf_accelerators._padding_chunk_info is None
+    assert font_1.bdf_accelerators._compat_info is not None
+    assert font_2.bdf_accelerators._compat_info is None
```

### Comparing `pcffont-0.0.1/.gitignore` & `pcffont-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/LICENSE` & `pcffont-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pcffont-0.0.1/README.md` & `pcffont-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,18 +28,25 @@
     os.makedirs(outputs_dir)
 
     font = PcfFont.load(os.path.join(assets_dir, 'unifont', 'unifont-15.1.05.pcf'))
     print(f'name: {font.properties.font}')
     print(f'size: {font.properties.pixel_size}')
     print(f'ascent: {font.accelerators.font_ascent}')
     print(f'descent: {font.accelerators.font_descent}')
+    print()
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
-        print(f'{code_point:04X} {chr(code_point)} - {font.glyph_names[glyph_index]}')
-        for bitmap_row in font.bitmaps[glyph_index]:
-            print(''.join(map(str, bitmap_row)).replace('0', '__').replace('1', '**'))
+        glyph_name = font.glyph_names[glyph_index]
+        metric = font.metrics[glyph_index]
+        bitmap = font.bitmaps[glyph_index]
+        print(f'char: {chr(code_point)} ({code_point:04X})')
+        print(f'glyph_name: {glyph_name}')
+        print(f'advance_width: {metric.character_width}')
+        print(f'offset: ({-metric.left_sided_bearing}, {-metric.character_descent})')
+        for bitmap_row in bitmap:
+            print(f'{''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
 
 
 if __name__ == '__main__':
     main()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pcffont-0.0.1/pyproject.toml` & `pcffont-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pcffont"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library for manipulating Portable Compiled Format (PCF) Fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pcffont-0.0.1/PKG-INFO` & `pcffont-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pcffont
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for manipulating Portable Compiled Format (PCF) Fonts.
 Project-URL: homepage, https://github.com/TakWolf/pcffont
 Project-URL: source, https://github.com/TakWolf/pcffont
 Project-URL: issues, https://github.com/TakWolf/pcffont/issues
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
@@ -46,18 +46,25 @@
     os.makedirs(outputs_dir)
 
     font = PcfFont.load(os.path.join(assets_dir, 'unifont', 'unifont-15.1.05.pcf'))
     print(f'name: {font.properties.font}')
     print(f'size: {font.properties.pixel_size}')
     print(f'ascent: {font.accelerators.font_ascent}')
     print(f'descent: {font.accelerators.font_descent}')
+    print()
     for code_point, glyph_index in sorted(font.bdf_encodings.items()):
-        print(f'{code_point:04X} {chr(code_point)} - {font.glyph_names[glyph_index]}')
-        for bitmap_row in font.bitmaps[glyph_index]:
-            print(''.join(map(str, bitmap_row)).replace('0', '__').replace('1', '**'))
+        glyph_name = font.glyph_names[glyph_index]
+        metric = font.metrics[glyph_index]
+        bitmap = font.bitmaps[glyph_index]
+        print(f'char: {chr(code_point)} ({code_point:04X})')
+        print(f'glyph_name: {glyph_name}')
+        print(f'advance_width: {metric.character_width}')
+        print(f'offset: ({-metric.left_sided_bearing}, {-metric.character_descent})')
+        for bitmap_row in bitmap:
+            print(f'{''.join(map(str, bitmap_row)).replace('0', '  ').replace('1', '██')}*')
         print()
     font.save(os.path.join(outputs_dir, 'unifont-15.1.05.pcf'))
 
 
 if __name__ == '__main__':
     main()
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

