# Comparing `tmp/kibo_unibs_fp_lib-1.0.3.tar.gz` & `tmp/kibo_unibs_fp_lib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibo_unibs_fp_lib-1.0.3.tar", last modified: Sun Apr  7 19:54:34 2024, max compression
+gzip compressed data, was "kibo_unibs_fp_lib-1.0.4.tar", last modified: Fri Apr 12 13:05:58 2024, max compression
```

## Comparing `kibo_unibs_fp_lib-1.0.3.tar` & `kibo_unibs_fp_lib-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:54:34.729699 kibo_unibs_fp_lib-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-07 19:54:34.729699 kibo_unibs_fp_lib-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:54:34.729699 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/ansi_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/file_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/input_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/known_problems.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/pretty_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/random_draws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:54:34.729699 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-07 19:54:34.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-07 19:54:34.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:54:34.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 19:54:34.000000 kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:54:34.729699 kibo_unibs_fp_lib-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 19:54:30.000000 kibo_unibs_fp_lib-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/known_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/pretty_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/random_draws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 13:05:58.000000 kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:05:58.345670 kibo_unibs_fp_lib-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 13:05:53.000000 kibo_unibs_fp_lib-1.0.4/setup.py
```

### Comparing `kibo_unibs_fp_lib-1.0.3/LICENSE.txt` & `kibo_unibs_fp_lib-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kibo_unibs_fp_lib-1.0.3/PKG-INFO` & `kibo_unibs_fp_lib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kibo_unibs_fp_lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: UniBSFpLib modified, documented and converted in python.
 Home-page: https://github.com/AlessandroMuscio/kibo_unibs_fp_lib
 Author: Alessandro Muscio
 Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Muscio
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/file_service.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/file_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Module representing the file_service class"""
 
 # Standard Libraries
 import pickle
 
 # Internal Libraries
-from kibo_unibs_fp_lib.ansi_colors import ansi_colors
+from kibo_unibs_fp_lib.ansi_colors import AnsiColors
 
 
 class FileService:
     """
-    This class has useful methods to serialize/deserialize objects and save/load them to/from a 
+    This class has useful methods to serialize/deserialize objects and save/load them to/from a
     file.
     """
 
-    _RED_ATTENTION = f"{ansi_colors["red"]}Attention!{ansi_colors["reset"]}"
+    _RED_ATTENTION = f"{AnsiColors.RED}Attention!{AnsiColors.RESET}"
     _FILE_NOT_FOUND_ERROR = f"{_RED_ATTENTION}\nCan't find the file "
     _READING_ERROR = f"{_RED_ATTENTION}\nProblem reading the file "
     _WRITING_ERROR = f"{_RED_ATTENTION}\nProblem writing the file "
 
     def __init__(self) -> None:
         """Prevents instantiation of this class
 
         Raises:
             NotImplementedError
         """
 
-        raise NotImplementedError()
+        raise NotImplementedError("This class isn't instantiable!")
 
     @staticmethod
     def serialize_object(file_path: str, to_save: object) -> None:
         """Serialize whatever object is given.
 
         Params:
             file_path -> The file path where to save the serialized object.
@@ -42,20 +42,20 @@
                 pickle.dump(to_save, f)
         except IOError as e:
             print(FileService._WRITING_ERROR + file_path)
             print(e)
 
     @staticmethod
     def deserialize_object(file_path: str, object_class: type) -> object:
-        """Deserialize whatever object is saved in the given file. The deserialized file will be 
+        """Deserialize whatever object is saved in the given file. The deserialized file will be
         cast into the given class.
 
         Params:
             file_path -> The file path where to find the serialized object.
-            
+
             object_class -> The class to cast the serialized object into.
 
         Returns:
             An instance of the deserialized object.
         """
 
         try:
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/input_data.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/input_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 """Module for the InputData class"""
 
-from kibo_unibs_fp_lib.ansi_colors import ansi_colors
+# Internal Libraries
+from kibo_unibs_fp_lib.ansi_colors import AnsiColors
 
 
 class InputData:
     """
-    This class can read a specific data type inserted in input by the user, while also allowing to 
+    This class can read a specific data type inserted in input by the user, while also allowing to
     make controls on the data inserted.
     """
 
-    _RED_ATTENTION = f"{ansi_colors["red"]}Attention!{ansi_colors["reset"]}"
-    _ALPHANUMERIC_CHARACTERS_ERROR = f"{_RED_ATTENTION}\nOnly alphanumeric characters are allowed."
+    _RED_ATTENTION = f"{AnsiColors.RED}Attention!{AnsiColors.RESET}"
+    _ALPHANUMERIC_CHARACTERS_ERROR = (
+        f"{_RED_ATTENTION}\nOnly alphanumeric characters are allowed."
+    )
     _EMPTY_STRING_ERROR = f"{_RED_ATTENTION}\nNo characters were inserted."
     _ALLOWED_CHARACTERS_ERROR = f"{_RED_ATTENTION}\nThe only allowed characters are: "
     _YES_ANSWERS = "yY"
     _NO_ANSWERS = "nN"
     _INTEGER_FORMAT_ERROR = f"""
     {_RED_ATTENTION}\nThe inserted data is in an incorrect format.
     An integer is required.
     """
-    _MINIMUM_ERROR = f"{_RED_ATTENTION}\nA value greater than or equal to %.2f is required."
-    _MAXIMUM_ERROR = f"{_RED_ATTENTION}\nA value less than or equal to %.2f is required."
+    _MINIMUM_ERROR = (
+        f"{_RED_ATTENTION}\nA value greater than or equal to %.2f is required."
+    )
+    _MAXIMUM_ERROR = (
+        f"{_RED_ATTENTION}\nA value less than or equal to %.2f is required."
+    )
     _FLOAT_FORMAT_ERROR = f"""
     {_RED_ATTENTION}\nThe inserted data is in an incorrect format.
     A float is required.
     """
 
     def __init__(self) -> None:
         """Prevents instantiation of this class
 
         Raises:
             NotImplementedError
         """
 
-        raise NotImplementedError()
+        raise NotImplementedError("This class isn't instantiable!")
 
     @staticmethod
     def read_string(message: str, alphanumeric: bool) -> str:
-        """Prints message in the terminal and reads the text inserted by the user. If it isn't a 
-        string an error message is printed. It's also possible to select if the inserted text needs 
+        """Prints message in the terminal and reads the text inserted by the user. If it isn't a
+        string an error message is printed. It's also possible to select if the inserted text needs
         to be alphanumeric or not via the alphanumeric input variable.
 
         Params:
             message -> The message to print.
 
             alphanumeric -> If the input needs to be alphanumeric or not.
 
@@ -62,16 +69,16 @@
             if not is_alphanumeric:
                 print(InputData._ALPHANUMERIC_CHARACTERS_ERROR)
 
         return read
 
     @staticmethod
     def read_non_empty_string(message: str, alphanumeric: bool) -> str:
-        """Prints message in the terminal and reads the text inserted by the user, given that it 
-        isn't empty. If it isn't a string an error message is printed. It's also possible to select 
+        """Prints message in the terminal and reads the text inserted by the user, given that it
+        isn't empty. If it isn't a string an error message is printed. It's also possible to select
         if the inserted text needs to be alphanumeric or not via the alphanumeric input variable.
 
         Params:
             message -> The message to print.
 
             alphanumeric -> If the input needs to be alphanumeric or not.
 
@@ -112,15 +119,15 @@
                 is_allowed = True
             else:
                 print(InputData._ALLOWED_CHARACTERS_ERROR, list(allowed))
 
         return read
 
     @staticmethod
-    def read_yer_or_no(question: str) -> bool:
+    def read_yes_or_no(question: str) -> bool:
         """Prompts the user with a question and expects a yes or no response.
 
         Params:
             question -> The question to display the user without question mark.
 
         Returns:
             True if the user reponds with 'y' or 'Y', False otherwise.
@@ -211,15 +218,15 @@
             message -> The message to display the user.
 
             min_value -> The minimum allowed value for the input.
 
             max_value -> The maximum allowed value for the input.
 
         Returns:
-            The integer input by the user that is greater than or equal to min and less than or 
+            The integer input by the user that is greater than or equal to min and less than or
             equal to max.
         """
 
         is_input_valid = False
 
         while not is_input_valid:
             read = InputData.read_integer(message)
@@ -310,15 +317,15 @@
             message -> The message to display the user.
 
             min_value -> The minimum allowed value for the input.
 
             max_value -> The maximum allowed value for the input.
 
         Returns:
-            The float input by the user that is greater than or equal to min and less than or equal 
+            The float input by the user that is greater than or equal to min and less than or equal
             to max.
         """
 
         is_input_valid = False
 
         while not is_input_valid:
             read = InputData.read_float(message)
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/known_problems.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/known_problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def __init__(self) -> None:
         """Prevents instantiation of this class
 
         Raises:
             NotImplementedError
         """
 
-        raise NotImplementedError()
+        raise NotImplementedError("This class isn't instantiable!")
 
     @staticmethod
     def mcd(a: int, b: int) -> int:
         """Finds the MCD (Maximum Common Divider) between two integers.
 
         Params:
             a -> The first number to calculate the MCD.
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/menu.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/menu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for the Menu class"""
 
 # Standard Libraries
 import os
 import time
 
 # Internal Libraries
-from kibo_unibs_fp_lib.ansi_colors import ansi_colors
+from kibo_unibs_fp_lib.ansi_colors import AnsiColors
 from kibo_unibs_fp_lib.input_data import InputData
 from kibo_unibs_fp_lib.known_problems import KnownProblems
 from kibo_unibs_fp_lib.pretty_strings import PrettyStrings
 
 
 class Menu:
     """
@@ -17,26 +17,26 @@
     The class also contains some methods that may be useful for visualizing the menu.
     """
 
     _NEW_LINE = "\n"
     _EXIT_ENTRY = "0. Exit"
     _INSERT_REQUEST = "> "
     _NEGATIVE_MILLIS_ERROR = (
-        f"{ansi_colors["red"]}Attention!{ansi_colors["reset"]}\nYou can't have negative time."
+        f"{AnsiColors.RED}Attention!{AnsiColors.RESET}\nYou can't have negative time."
     )
 
     def __init__(
         self,
         title: str,
         entries: list[str],
         use_exit_entry: bool,
         centred_title: bool,
     ) -> None:
-        """Constructor that creates a Menu object specifying a title, the entries of the menu, if 
-        you want the exit entry or not, if you want the title centred, and the vertical frame will 
+        """Constructor that creates a Menu object specifying a title, the entries of the menu, if
+        you want the exit entry or not, if you want the title centred, and the vertical frame will
         be off by default. It will also automatically calculate the frame length.
 
         Params:
             title -> Represents the title of the menu.
 
             entries -> Represents the entries of the menu.
 
@@ -46,55 +46,54 @@
 
             use_vertical_frame -> If you want to use the vertical frame or not.
         """
 
         self._title = title
         self._entries = entries
         self._use_exit_entry = use_exit_entry
-        self._frame_length = Menu._calculate_frame_length(title, entries)
+        self._frame_length = self._calculate_frame_length()
         self._centred_title = centred_title
         self._use_vertical_frame = False
 
     @property
     def use_vertical_frame(self) -> bool:
         """Getter of attribute use_vertical_frame.
-        
+
         Returns:
             A bool representing the current value of use_vertical_frame.
         """
 
         return self._use_vertical_frame
 
     @use_vertical_frame.setter
     def use_vertical_frame(self, value: bool) -> None:
         """Setter of attribute use_vertical_frame.
-        
+
         Params:
             value -> The new value of use_vertical_frame.
         """
 
         self._use_vertical_frame = value
 
-    @staticmethod
-    def _calculate_frame_length(title: str, entries: list[str]) -> int:
+    def _calculate_frame_length(self) -> int:
         """Calculates the frame length by measuring the length of the title and of all the entries
         of the menu, accounting for their number and the ". " string before the actual entry.
 
         Params:
             title -> The title of the menu.
 
             entries -> The entries of the menu.
 
         Returns:
             An integer representing the length of the frame.
         """
 
-        frame_length = len(title)
+        frame_length = len(self._title)
 
-        for i, entry in enumerate(entries):
+        for i, entry in enumerate(self._entries):
             frame_length = max(
                 frame_length, len(entry) + KnownProblems.count_integer_digits(i + 1) + 2
             )
 
         return frame_length + 10  # Adding a bit of extra space
 
     def _print_menu(self) -> None:
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/pretty_strings.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/pretty_strings.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self) -> None:
         """Prevents instantiation of this class
 
         Raises:
             NotImplementedError
         """
 
-        raise NotImplementedError()
+        raise NotImplementedError("This class isn't instantiable!")
 
     @staticmethod
     def frame(
         to_frame: str, frame_length: int, centered: bool, vertical_frame: bool
     ) -> str:
         """Puts the given string in the center or in the beginning of the line surrounded by the
         horizontal frame above and below and, if needed, also the vertical frame before and after.
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib/random_draws.py` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib/random_draws.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self) -> None:
         """Prevents instantiation of this class
 
         Raises:
             NotImplementedError
         """
 
-        raise NotImplementedError()
+        raise NotImplementedError("This class isn't instantiable!")
 
     @staticmethod
     def draw_integer(minimum: int, maximum: int) -> int:
         """Draws a random integer between given minimum and maximum values.
 
         Params:
             minimum -> The minimum value to draw.
```

### Comparing `kibo_unibs_fp_lib-1.0.3/kibo_unibs_fp_lib.egg-info/PKG-INFO` & `kibo_unibs_fp_lib-1.0.4/kibo_unibs_fp_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kibo_unibs_fp_lib
-Version: 1.0.3
+Version: 1.0.4
 Summary: UniBSFpLib modified, documented and converted in python.
 Home-page: https://github.com/AlessandroMuscio/kibo_unibs_fp_lib
 Author: Alessandro Muscio
 Author-email: Alessandro Muscio <a.muscio001@studenti.unibs.it>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Muscio
```

### Comparing `kibo_unibs_fp_lib-1.0.3/pyproject.toml` & `kibo_unibs_fp_lib-1.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kibo_unibs_fp_lib"
-version = "1.0.3"
+version = "1.0.4"
 license = {file = "LICENSE.txt"}
 
 description = "UniBSFpLib modified, documented and converted in python."
 authors = [{ name="Alessandro Muscio", email="a.muscio001@studenti.unibs.it"}]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
```

