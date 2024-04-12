# Comparing `tmp/tb1_parser-1.0.0.tar.gz` & `tmp/tb1_parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-1.0.0.tar", last modified: Sun Apr  7 13:18:03 2024, max compression
+gzip compressed data, was "tb1_parser-1.0.1.tar", last modified: Fri Apr 12 15:43:14 2024, max compression
```

## Comparing `tb1_parser-1.0.0.tar` & `tb1_parser-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 13:18:03.518327 tb1_parser-1.0.0/
--rw-rw-rw-   0        0        0      272 2024-04-07 13:18:03.517327 tb1_parser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 13:18:03.519327 tb1_parser-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-07 13:17:27.000000 tb1_parser-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:18:03.507326 tb1_parser-1.0.0/tb1_parser/
--rw-rw-rw-   0        0        0      585 2024-04-07 12:56:12.000000 tb1_parser-1.0.0/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5785 2024-04-07 12:54:57.000000 tb1_parser-1.0.0/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2106 2024-04-07 12:55:01.000000 tb1_parser-1.0.0/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-1.0.0/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-1.0.0/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1767 2024-04-07 13:05:56.000000 tb1_parser-1.0.0/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-1.0.0/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-1.0.0/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/signal.py
--rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-1.0.0/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1640 2024-04-07 12:55:41.000000 tb1_parser-1.0.0/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 13:18:03.516328 tb1_parser-1.0.0/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      272 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 13:18:03.000000 tb1_parser-1.0.0/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.837742 tb1_parser-1.0.1/
+-rw-rw-rw-   0        0        0      272 2024-04-12 15:43:14.837742 tb1_parser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:43:14.839744 tb1_parser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      393 2024-04-12 15:31:33.000000 tb1_parser-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.826740 tb1_parser-1.0.1/tb1_parser/
+-rw-rw-rw-   0        0        0      157 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5806 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2127 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2213 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     6197 2024-04-12 12:47:47.000000 tb1_parser-1.0.1/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4454 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1767 2024-04-07 14:02:43.000000 tb1_parser-1.0.1/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-1.0.1/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0     1625 2024-04-12 15:31:09.000000 tb1_parser-1.0.1/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:43:14.836743 tb1_parser-1.0.1/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      272 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      531 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 15:43:14.000000 tb1_parser-1.0.1/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-1.0.1/tb1_parser/_ai_sheet_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import logging
 import re
 
 from pandas import DataFrame
 
 from ._regex_lib import TB1
 from ._sheet_parser import SheetParser
-from .ai_signal import AiSignal
-from .signals_collection import SignalsCollection
+from ._types import AiSignal, SignalsCollection
 
 
 config = TB1['Ai']['regex']
 
 
 class AiSheetParser(SheetParser):
 
@@ -97,14 +96,15 @@
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
             try:
                 new = AiSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
+                new.plc_channel = int(row.plc_channel)
                 new.variable = self._parse_variable(row.variable, row.plc_module)
                 new.name = self._clean_name(row.name)
                 new.formated_name = self._format_signal_name(row.name)
                 new.unit = row.unit if row.unit else self.__find_unit(row.range)
                 new.LL, new.HL = self.__parse_range(row.range)
                 new.LW, new.HW = self.__parse_range(row.warning_range)
                 new.LA, new.HA = self.__parse_range(row.alarm_range)
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_di_sheet_parser.py` & `tb1_parser-1.0.1/tb1_parser/_di_sheet_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 from pandas import DataFrame
 
 from ._do_sheet_parser import DoSheetParser
 from ._regex_lib import TB1 as config
-from .di_signal import DiSignal
-from .signals_collection import SignalsCollection
+from ._types import DiSignal, SignalsCollection
 
 
 class DiSheetParser(DoSheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
@@ -28,14 +27,15 @@
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
             try:
                 new = DiSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
+                new.plc_channel = int(row.plc_channel)
                 new.variable = self._parse_variable(row.variable, row.plc_module)
                 new.name = self._clean_name(row.name)
                 new.formated_name = self._format_signal_name(row.name)
                 new.logic_value = self._parse_logic_value(row.logic_value)
                 new.alarm_signal = self.__parse_signal(row.alarm_signal)
                 new.warning_signal = self.__parse_signal(row.warning_signal)
                 new.error_signal = self.__parse_signal(row.error_signal)
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_do_sheet_parser.py` & `tb1_parser-1.0.1/tb1_parser/_do_sheet_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 
 from pandas import DataFrame
 
 from ._regex_lib import TB1 as config
 from ._sheet_parser import SheetParser
-from .do_signal import DoSignal
-from .signals_collection import SignalsCollection
+from ._types import DoSignal, SignalsCollection
 
 
 class DoSheetParser(SheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
@@ -36,14 +35,15 @@
 
         out = []
 
         for row in self._sheet.itertuples(False, 'Signal'):
             try:
                 new = DoSignal()
                 new.plc_module = self._parse_plc_module(row.plc_module)
+                new.plc_channel = int(row.plc_channel)
                 new.variable = self._parse_variable(row.variable, row.plc_module)
                 new.name = self._clean_name(row.name)
                 new.formated_name = self._format_signal_name(row.name)
                 new.logic_value = self._parse_logic_value(row.logic_value)
 
                 out.append(new)
                 logging.info(f'{self._logs_owner}:{row.variable}: значения успешно получены')
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_regex_lib.py` & `tb1_parser-1.0.1/tb1_parser/_regex_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
                         'variable': r'^.*((([Нн]ом([ер]{2}|\.)?)|№)?\s?([Пп]ерем\.?([а-я]+[йян])?)).*$',
                         'name': r'^.*((([Нн]а)?([Ии]м\.?(я|ен\.?(\w+)?))\s?)([Пп]арам(\.|етр(\.|а))|сигнала)).*$',
                         'unit': r'^.*([Ее]диница измерения).*$',
                         'range': r'^.*(([Дд]иап\.?(аз\.?)?(он)?\s)([Ии]зм\.?(ер\.?)?(ен\.?)?(ия)?)?).*$',
                         'warning_range': r'^.*(ПС).*$',
                         'alarm_range': r'^.*(АС).*$',
                         'error_range': r'^.*(НС).*$',
-                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$'
+                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$',
+                        'plc_channel': r'^.*([Кк]анал).*$'
                     }
                 },
                 'replace': {
                     'trash': {
                         'pattern': r'(\(.*?\))|\n|\-',
                         'new_value': ''
                     }
@@ -66,15 +67,16 @@
                         'variable': r'^.*((([Нн]ом([ер]{2}|\.)?)|№)?\s?([Пп]ерем\.?([а-я]+[йян])?)).*$',
                         'name': r'^.*((([Нн]а)?([Ии]м\.?(я|ен\.?(\w+)?))\s?)([Пп]арам(\.|етр(\.|а))|сигнала)).*$',
                         'logic_value': r'^.*[Лл]ог(\w+)?\.?\s?[Зз]нач(\w+)?\.?',
                         'alarm_signal': r'^.*(АС).*$',
                         'warning_signal': r'^.*(ПС).*$',
                         'tele_signal': r'^.*(ТС).*$',
                         'error_signal': r'^.*(НС).*$',
-                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$'
+                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$',
+                        'plc_channel': r'^.*([Кк]анал).*$'
                     }
                 },
                 'replace': {
                     'trash': {
                         'pattern': r'(\(.*?\))|\n|\-',
                         'new_value': ''
                     }
@@ -91,15 +93,16 @@
             },
             'columns': {
                 'validate': {
                     'names': {
                         'variable': r'^.*((([Нн]ом([ер]{2}|\.)?)|№)?\s?([Пп]ерем\.?([а-я]+[йян])?)).*$',
                         'name': r'^.*((([Нн]а)?([Ии]м\.?(я|ен\.?(\w+)?))\s?)([Пп]арам(\.|етр(\.|а))|сигнала)).*$',
                         'logic_value': r'^.*[Лл]ог(\w+)?\.?\s?[Зз]нач(\w+)?\.?',
-                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$'
+                        'plc_module': r'^.*([Мм]одуль\s(\w+)?).*$',
+                        'plc_channel': r'^.*([Кк]анал).*$'
                     }
                 },
                 'replace': {
                     'trash': {
                         'pattern': r'(\(.*?\))|\n|\-',
                         'new_value': ''
                     }
@@ -129,10 +132,11 @@
             'Температура': 'T',
             'Давление': 'P',
             'Перепад давления': 'dP',
             'Ток': 'I',
             'Напряжение': 'U',
             'Уровень': 'L'
         },
-        'find_plc_module': r'^\w{2}\-[a-z0-9-]+\,?\s+?\(?(\w(\d+).?(\d+))\)?$'
+        # 'find_plc_module': r'^\w{2}\-[a-z0-9-]+\,?\s+?\(?(\w(\d+).?(\d+))\)?$'
+        'find_plc_module': r'([IOAD]+.?\d+\D\d+)\s{0,}\(?(\D?\d+\-\d+)\)?'
     }
 }
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_sheet_parser.py` & `tb1_parser-1.0.1/tb1_parser/_sheet_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 
 from pandas import DataFrame
 from transliterate import translit
 
 from ._regex_lib import PARSER as config
-from .signals_collection import SignalsCollection
+from ._types import SignalsCollection
 
 
 class SheetParser:
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
@@ -29,42 +29,47 @@
             return count
         except Exception as exception:
             pass
         finally:
             pass
 
 
-    def _parse_variable(self, raw_variable: str, raw_plc_module: str) -> int | tuple[int]:
-        type_regex = r'^\D{2}'
-        clean_input = lambda x: re.sub(type_regex, '', x)
-        clear_variable = clean_input(raw_variable)
-        try:
-            if 'ai' in raw_variable.lower():
-                out = int(clear_variable)
-            else:
-                out = nums = tuple(map(int, clear_variable.split('-')))
-
-        except ValueError as value_error:
-            logging.warning(f'{self._logs_owner}: некорректный номер переменной "{raw_variable}"')
-            count_plc_channels = self._find_count_plc_channels(raw_plc_module)
-            nums = tuple(map(int, clear_variable.split('-')))
-
-            if len(nums) == 2:
-                logging.info(f'{self._logs_owner}: вычисление порядкового номера "{raw_variable}"')
-                out = count_plc_channels * nums[0] + nums[1]
-                logging.warning(f'{self._logs_owner}: номер переменной "{raw_variable}" принудительно нормализован - "{out}"')
-            else:
-                raise ValueError('попытка вычисления порядкового номера переменной провалена')
+    # def _parse_variable(self, raw_variable: str, raw_plc_module: str) -> int | tuple[int]:
+    #     type_regex = r'^\D{2}'
+    #     clean_input = lambda x: re.sub(type_regex, '', x)
+    #     clear_variable = clean_input(raw_variable)
+    #     try:
+    #         if 'ai' in raw_variable.lower():
+    #             out = int(clear_variable)
+    #         else:
+    #             out = nums = tuple(map(int, clear_variable.split('-')))
+
+    #     except ValueError as value_error:
+    #         logging.warning(f'{self._logs_owner}: некорректный номер переменной "{raw_variable}"')
+    #         count_plc_channels = self._find_count_plc_channels(raw_plc_module)
+    #         nums = tuple(map(int, clear_variable.split('-')))
+
+    #         if len(nums) == 2:
+    #             logging.info(f'{self._logs_owner}: вычисление порядкового номера "{raw_variable}"')
+    #             out = count_plc_channels * nums[0] + nums[1]
+    #             logging.warning(f'{self._logs_owner}: номер переменной "{raw_variable}" принудительно нормализован - "{out}"')
+    #         else:
+    #             raise ValueError('попытка вычисления порядкового номера переменной провалена')
             
-        except Exception as exception:
-            logging.error(f'{self._logs_owner}: ошибка парсинга "{raw_variable}" переменной - {type(exception).__name__}:{exception}')
-            out = None
+    #     except Exception as exception:
+    #         logging.error(f'{self._logs_owner}: ошибка парсинга "{raw_variable}" переменной - {type(exception).__name__}:{exception}')
+    #         out = None
 
-        finally:
-            return out
+    #     finally:
+    #         return out
+
+
+    # FIXME Заглушка метода парсинга переменной сигнала
+    def _parse_variable(self, raw_variable: str, _):
+        return raw_variable
 
     
     # REFACT Переписать метод транслитерациии названия параметра
     def _format_signal_name(self, name: str) -> str:
         replace_data = config['signals']['format_variable_name']
         try:
             for key, value in replace_data.items():
@@ -77,19 +82,17 @@
         except Exception as error:
             logging.error(f'{self._logs_owner}: ошибка транслитерации "{name}" названия параметра - {error}')
             out = None
         finally:
             return out
     
 
-    # REFACT Переписать метод парсинга канала модуля плк
     def _parse_plc_module(self, raw_string: str) -> str:
         try:
-            out = re.findall(config['signals']['find_plc_module'], raw_string)[0][1:]
-            out = tuple(map(int, out))
+            out = re.findall(config['signals']['find_plc_module'], raw_string)[0]
             if not out:
                 raise ValueError('ошибка сопоставления с шаблоном')
         except Exception as error:
             logging.error(f'{self._logs_owner}: ошибка парсинга "{raw_string.replace('\n', '')}" модуля плк - {error}')
             out = None
         finally:
             return out
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_tb1_file_reader.py` & `tb1_parser-1.0.1/tb1_parser/_tb1_file_reader.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import sys
 from typing import Literal
 
 from pandas import DataFrame, ExcelFile
 
 from ._regex_lib import TB1 as config
-from ._tb1_sheet_reader import TB1SheetReader
 from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from ._tb1_sheet_reader import TB1SheetReader
 
 
 all_avaible_sheets = list(config)
 
 
 class TB1FileReader:
```

### Comparing `tb1_parser-1.0.0/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-1.0.1/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-1.0.0/tb1_parser/tb1_parser.py` & `tb1_parser-1.0.1/tb1_parser/tb1_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ._ai_sheet_parser import AiSheetParser
 from ._di_sheet_parser import DiSheetParser
 from ._do_sheet_parser import DoSheetParser
 from ._tb1_file_reader import TB1FileReader
 from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
-from .parsed_tb1_collection import ParsedTB1Collection
+from ._types import ParsedTB1Collection
 
 
 class TB1Parser:
 
     def __init__(self, filepath: str) -> None:
         self.__logs_owner: str = self.__class__.__name__
         self.__filepath: str = filepath
```

### Comparing `tb1_parser-1.0.0/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-1.0.1/tb1_parser.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,20 +6,14 @@
 tb1_parser/_di_sheet_parser.py
 tb1_parser/_do_sheet_parser.py
 tb1_parser/_regex_lib.py
 tb1_parser/_sheet_parser.py
 tb1_parser/_tb1_file_reader.py
 tb1_parser/_tb1_readed_sheets_collection.py
 tb1_parser/_tb1_sheet_reader.py
-tb1_parser/ai_signal.py
-tb1_parser/di_signal.py
-tb1_parser/do_signal.py
-tb1_parser/parsed_tb1_collection.py
-tb1_parser/signal.py
-tb1_parser/signals_collection.py
 tb1_parser/tb1_parser.py
 tb1_parser.egg-info/PKG-INFO
 tb1_parser.egg-info/SOURCES.txt
 tb1_parser.egg-info/dependency_links.txt
 tb1_parser.egg-info/not-zip-safe
 tb1_parser.egg-info/requires.txt
 tb1_parser.egg-info/top_level.txt
```

