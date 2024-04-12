# Comparing `tmp/context_menu-1.4.0.tar.gz` & `tmp/context_menu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "context_menu-1.4.0.tar", last modified: Thu Apr 11 06:25:12 2024, max compression
+gzip compressed data, was "context_menu-1.4.1.tar", last modified: Fri Apr 12 19:36:28 2024, max compression
```

## Comparing `context_menu-1.4.0.tar` & `context_menu-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.277140 context_menu-1.4.0/
--rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.4.0/LICENSE
--rw-rw-rw-   0        0        0    15187 2024-04-11 06:25:12.275141 context_menu-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    14571 2024-04-11 06:18:32.000000 context_menu-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.239817 context_menu-1.4.0/context_menu/
--rw-rw-rw-   0        0        0        0 2024-04-11 05:58:22.000000 context_menu-1.4.0/context_menu/__init__.py
--rw-rw-rw-   0        0        0    12780 2024-04-11 05:58:22.000000 context_menu-1.4.0/context_menu/linux_menus.py
--rw-rw-rw-   0        0        0     6325 2024-04-11 06:18:29.000000 context_menu-1.4.0/context_menu/menus.py
--rw-rw-rw-   0        0        0     6319 2024-04-11 06:18:29.000000 context_menu-1.4.0/context_menu/pytest_plugin.py
--rw-rw-rw-   0        0        0    15441 2024-04-11 06:18:32.000000 context_menu-1.4.0/context_menu/windows_menus.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.265329 context_menu-1.4.0/context_menu.egg-info/
--rw-rw-rw-   0        0        0    15187 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 06:25:12.000000 context_menu-1.4.0/context_menu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 06:25:12.278142 context_menu-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      989 2024-04-11 06:18:58.000000 context_menu-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:25:12.273128 context_menu-1.4.0/tests/
--rw-rw-rw-   0        0        0      157 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_imports.py
--rw-rw-rw-   0        0        0     1493 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_linux.py
--rw-rw-rw-   0        0        0      520 2024-04-11 05:58:22.000000 context_menu-1.4.0/tests/test_menus.py
--rw-rw-rw-   0        0        0     5470 2024-04-11 06:18:32.000000 context_menu-1.4.0/tests/test_windows.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:36:28.806711 context_menu-1.4.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 19:45:36.000000 context_menu-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0    15255 2024-04-12 19:36:28.805711 context_menu-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14639 2024-04-12 19:34:43.000000 context_menu-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 19:36:28.773163 context_menu-1.4.1/context_menu/
+-rw-rw-rw-   0        0        0        0 2024-04-11 05:58:22.000000 context_menu-1.4.1/context_menu/__init__.py
+-rw-rw-rw-   0        0        0    12780 2024-04-11 05:58:22.000000 context_menu-1.4.1/context_menu/linux_menus.py
+-rw-rw-rw-   0        0        0     6494 2024-04-12 19:34:43.000000 context_menu-1.4.1/context_menu/menus.py
+-rw-rw-rw-   0        0        0     7824 2024-04-12 19:34:43.000000 context_menu-1.4.1/context_menu/pytest_plugin.py
+-rw-rw-rw-   0        0        0    15776 2024-04-12 19:34:43.000000 context_menu-1.4.1/context_menu/windows_menus.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:36:28.799415 context_menu-1.4.1/context_menu.egg-info/
+-rw-rw-rw-   0        0        0    15255 2024-04-12 19:36:28.000000 context_menu-1.4.1/context_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-04-12 19:36:28.000000 context_menu-1.4.1/context_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 19:36:28.000000 context_menu-1.4.1/context_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-12 19:36:28.000000 context_menu-1.4.1/context_menu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 19:36:28.000000 context_menu-1.4.1/context_menu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 19:36:28.806711 context_menu-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      989 2024-04-12 19:36:23.000000 context_menu-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:36:28.803420 context_menu-1.4.1/tests/
+-rw-rw-rw-   0        0        0      157 2024-04-11 05:58:22.000000 context_menu-1.4.1/tests/test_imports.py
+-rw-rw-rw-   0        0        0     1493 2024-04-11 05:58:22.000000 context_menu-1.4.1/tests/test_linux.py
+-rw-rw-rw-   0        0        0      520 2024-04-11 05:58:22.000000 context_menu-1.4.1/tests/test_menus.py
+-rw-rw-rw-   0        0        0     6684 2024-04-12 19:34:43.000000 context_menu-1.4.1/tests/test_windows.py
```

### Comparing `context_menu-1.4.0/LICENSE` & `context_menu-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `context_menu-1.4.0/PKG-INFO` & `context_menu-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context_menu
-Version: 1.4.0
+Version: 1.4.1
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -216,15 +216,15 @@
 ## The `ContextCommand` Class
 
 The [ContextCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextCommand)
 class creates the selectable part of the menu (you can click it). It requires a name, and either a Python function or a
 command **(but NOT both)** and has various other options
 
 ```Python
-ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None)
+ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None, icon_path: str = None)
 ```
 
 Python functions can be passed to this method, regardless of their location. **However, the function must accept only
 two parameters `filenames`, which is a list of paths\*, and `params`, the parameters passed to the function**. and if
 the function is in the same file as the menu, you have to surround it with `if __name__ == '__main__':`
 
 ```python
@@ -248,19 +248,19 @@
 
 Any command passed (as a string) will be directly ran from the shell.
 
 ## The `FastCommand` Class
 
 The [FastCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.FastCommand) class
 is an extension of the ContextMenu class and allows you to quickly create a single entry menu. It expects a name, type,
-and command/function.
+command/function and an optional icon path.
 
 ```python
 FastCommand(
-    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None)
+    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None, icon_path: str = None)
 ```
 
 ```python
 def foo1(filenames, params):
     print(filenames)
     input()
```

### Comparing `context_menu-1.4.0/README.md` & `context_menu-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 ## The `ContextCommand` Class
 
 The [ContextCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextCommand)
 class creates the selectable part of the menu (you can click it). It requires a name, and either a Python function or a
 command **(but NOT both)** and has various other options
 
 ```Python
-ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None)
+ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None, icon_path: str = None)
 ```
 
 Python functions can be passed to this method, regardless of their location. **However, the function must accept only
 two parameters `filenames`, which is a list of paths\*, and `params`, the parameters passed to the function**. and if
 the function is in the same file as the menu, you have to surround it with `if __name__ == '__main__':`
 
 ```python
@@ -230,19 +230,19 @@
 
 Any command passed (as a string) will be directly ran from the shell.
 
 ## The `FastCommand` Class
 
 The [FastCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.FastCommand) class
 is an extension of the ContextMenu class and allows you to quickly create a single entry menu. It expects a name, type,
-and command/function.
+command/function and an optional icon path.
 
 ```python
 FastCommand(
-    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None)
+    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None, icon_path: str = None)
 ```
 
 ```python
 def foo1(filenames, params):
     print(filenames)
     input()
```

### Comparing `context_menu-1.4.0/context_menu/linux_menus.py` & `context_menu-1.4.1/context_menu/linux_menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.4.0/context_menu/menus.py` & `context_menu-1.4.1/context_menu/menus.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,24 +69,26 @@
     def __init__(
         self,
         name: str,
         command: str | None = None,
         python: FunctionType | None = None,
         params: str = "",
         command_vars: list[CommandVar] | None = None,
+        icon_path: str = None,
     ) -> None:
         """
         Do not specify both 'python' and 'command', either pass a python function or a command but not both.
         """
         self.name = name
         self.command = command
         self.isMenu = False
         self.python = python
         self.params = params
         self.command_vars = command_vars
+        self.icon_path = icon_path
 
         if command != None and python != None:
             raise ValueError("both command and python cannot be defined")
 
     def get_platform_command(self):
         """
         Will be used in future changes.
@@ -122,21 +124,23 @@
         self,
         name: str,
         type: ActivationType | str,
         command: str | None = None,
         python: FunctionType | None = None,
         params: str = "",
         command_vars: list[CommandVar] | None = None,
+        icon_path: str = None,
     ) -> None:
         self.name = name
         self.type = type
         self.command = command
         self.python = python
         self.params = params
         self.command_vars = command_vars
+        self.icon_path = icon_path
 
         if command != None and python != None:
             raise ValueError("both command and python cannot be defined")
 
     def get_method_info(self) -> MethodInfo:
         assert self.python is not None
         func_file_path = os.path.abspath(inspect.getfile(self.python))
@@ -166,14 +170,15 @@
             windows_menus.FastRegistryCommand(
                 self.name,
                 self.type,
                 self.command,
                 self.python,
                 self.params,
                 self.command_vars,
+                self.icon_path,
             ).compile()
 
 
 try:
 
     def removeMenu(name: str, type: ActivationType | str) -> None:
         """
```

### Comparing `context_menu-1.4.0/context_menu/pytest_plugin.py` & `context_menu-1.4.1/context_menu/pytest_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -113,14 +113,31 @@
             # Checks the key parent\\name
             ("", name),
             # Checks the key parent\\name\\command
             ("\\command", command),
         ):
             assert self.get_key_value(f"{parent}\\{name}{k}", "") == v
 
+    def assert_context_command_with_icon(self, parent: str, name: str, command: str, icon_path: str) -> None:
+        """Asserts that keys for a ContextCommand are correctly set.
+
+        :param parent: parent \\shell key
+        :param name: name of the key for the command
+        :param command: expected command set in \\command
+        """
+        for k, v in (
+            # Checks the key parent\\name
+            ("", name),
+            # Checks the key parent\\name\\command
+            ("\\command", command),
+        ):
+            assert self.get_key_value(f"{parent}\\{name}{k}", "") == v
+
+        assert self.get_key_value(f"{parent}\\{name}", "Icon") == icon_path
+
     def assert_fast_command(self, parent: str, name: str, command: str) -> None:
         """Asserts that keys for a FastCommand are correctly set.
 
         For some reasons, the name is no set when using FastCommand,
         while it is set for a ContextCommand.
 
         :param parent: parent \\shell key
@@ -131,14 +148,34 @@
             # Checks the key parent\\name
             ("", ""),
             # Checks the key parent\\name\\command
             ("\\command", command),
         ):
             assert self.get_key_value(f"{parent}\\{name}{k}", "") == v
 
+    def assert_fast_command_with_icon(self, parent: str, name: str, command: str, icon_path: str) -> None:
+        """Asserts that keys for a FastCommand are correctly set.
+
+        For some reasons, the name is no set when using FastCommand,
+        while it is set for a ContextCommand.
+
+        :param parent: parent \\shell key
+        :param name: name of the key for the command
+        :param command: expected command set in \\command
+        """
+        for k, v in (
+            # Checks the key parent\\name
+            ("", ""),
+            # Checks the key parent\\name\\command
+            ("\\command", command),
+        ):
+            assert self.get_key_value(f"{parent}\\{name}{k}", "") == v
+
+        assert self.get_key_value(f"{parent}\\{name}", "Icon") == icon_path
+
 
 @pytest.fixture
 def mocked_winreg() -> Iterable[MockedWinReg]:
     """Mocks the calls to winreg in windows_menus."""
     with MockedWinReg() as winreg:
         yield winreg
```

### Comparing `context_menu-1.4.0/context_menu/windows_menus.py` & `context_menu-1.4.1/context_menu/windows_menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,26 +306,29 @@
             set_key_value(key_path, 'Icon', icon_path)
 
         key_shell_path = join_keys(key_path, "shell")
         create_key(key_shell_path)
 
         return key_shell_path
 
-    def create_command(self, name: str, path: str, command: str) -> None:
+    def create_command(self, name: str, path: str, command: str, icon_path: str = None) -> None:
         """
         Creates a key with a command subkey with the 'name' and 'command', at path 'path'.
         """
         key_path = join_keys(path, name)
         create_key(key_path)
         set_key_value(key_path, "", name)
 
         command_path = join_keys(key_path, "command")
         create_key(command_path)
         set_key_value(command_path, "", command)
 
+        if icon_path is not None:
+            set_key_value(key_path, 'Icon', icon_path)
+
     def compile(
         self, items: list[ItemType] | None = None, path: str | None = None
     ) -> None:
         """
         Used to create the menu. Recursively iterates through each element in the top level menu.
         """
         if items == None:
@@ -353,25 +356,25 @@
                         func_name, func_file_name, func_dir_path, item.params
                     )
                 else:
                     # If it requires a file command
                     new_command = create_file_select_command(
                         func_name, func_file_name, func_dir_path, item.params
                     )
-                self.create_command(item.name, path, new_command)
+                self.create_command(item.name, path, new_command, item.icon_path)
             elif item.command_vars != None:
                 # If the item has to be ran from os.system
                 assert item.command is not None
                 assert item.command_vars is not None
                 new_command = create_shell_command(item.command, item.command_vars)
-                self.create_command(item.name, path, new_command)
+                self.create_command(item.name, path, new_command, item.icon_path)
             else:
                 # The item is just a plain old command
                 assert item.command is not None
-                self.create_command(item.name, path, item.command)
+                self.create_command(item.name, path, item.command, item.icon_path)
 
 
 # Fast command class
 # Everything is identical to either the RegistryMenu class or code in the menus file
 class FastRegistryCommand:
     """
     Fast command class.
@@ -383,22 +386,24 @@
         self,
         name: str,
         type: ActivationType | str,
         command: str,
         python: FunctionType,
         params: str,
         command_vars: list[CommandVar],
+        icon_path: str = None,
     ) -> None:
         self.name = name
         self.type = type
         self.path = context_registry_format(type)
         self.command = command
         self.python = python
         self.params = params
         self.command_vars = command_vars
+        self.icon_path = icon_path
 
     def get_method_info(self) -> MethodInfo:
         import inspect
 
         func_file_path = os.path.abspath(inspect.getfile(self.python))
 
         func_dir_path = os.path.dirname(func_file_path)
@@ -433,14 +438,17 @@
                 )
         elif self.command_vars != None:
             # If it has command_vars
             new_command = create_shell_command(self.command, self.command_vars)
 
         set_key_value(command_path, "", new_command)
 
+        if self.icon_path is not None:
+            set_key_value(key_path, 'Icon', self.icon_path)
+
 
 # Testing section...
 
 try:
 
     def remove_windows_menu(name: str, type: ActivationType | str) -> None:
         """
```

### Comparing `context_menu-1.4.0/context_menu.egg-info/PKG-INFO` & `context_menu-1.4.1/context_menu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: context-menu
-Version: 1.4.0
+Version: 1.4.1
 Summary: Library to create cross-platform native context menus.
 Home-page: https://github.com/saleguas/context_menu
 Author: Salvador Aleguas
 Author-email: salvador@aleguas.dev
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -216,15 +216,15 @@
 ## The `ContextCommand` Class
 
 The [ContextCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.ContextCommand)
 class creates the selectable part of the menu (you can click it). It requires a name, and either a Python function or a
 command **(but NOT both)** and has various other options
 
 ```Python
-ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None)
+ContextCommand(name: str, command: str = None, python: 'function' = None, params: str = None, command_vars: list = None, icon_path: str = None)
 ```
 
 Python functions can be passed to this method, regardless of their location. **However, the function must accept only
 two parameters `filenames`, which is a list of paths\*, and `params`, the parameters passed to the function**. and if
 the function is in the same file as the menu, you have to surround it with `if __name__ == '__main__':`
 
 ```python
@@ -248,19 +248,19 @@
 
 Any command passed (as a string) will be directly ran from the shell.
 
 ## The `FastCommand` Class
 
 The [FastCommand](https://context-menu.readthedocs.io/en/latest/context_menu.html#context_menu.menus.FastCommand) class
 is an extension of the ContextMenu class and allows you to quickly create a single entry menu. It expects a name, type,
-and command/function.
+command/function and an optional icon path.
 
 ```python
 FastCommand(
-    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None)
+    name: str, type: str, command: str = None, python: 'function' = None, params: str = '', command_vars: list = None, icon_path: str = None)
 ```
 
 ```python
 def foo1(filenames, params):
     print(filenames)
     input()
```

### Comparing `context_menu-1.4.0/setup.py` & `context_menu-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 # This call to setup() does all the work
 setuptools.setup(
     name="context_menu",
-    version="1.4.0",
+    version="1.4.1",
     description="Library to create cross-platform native context menus.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/saleguas/context_menu",
     author="Salvador Aleguas",
     author_email="salvador@aleguas.dev",
     license="MIT",
```

### Comparing `context_menu-1.4.0/tests/test_linux.py` & `context_menu-1.4.1/tests/test_linux.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.4.0/tests/test_menus.py` & `context_menu-1.4.1/tests/test_menus.py`

 * *Files identical despite different names*

### Comparing `context_menu-1.4.0/tests/test_windows.py` & `context_menu-1.4.1/tests/test_windows.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,131 +25,169 @@
 
     # Corrected the assertion to match the expected call with the .ico extension
     mocked_winreg.assert_context_menu_with_icon("Software\\Classes\\*\\shell", "Test", "\\this\\is\\a\\placeholder.ico")
 
 
 
 @pytest.mark.parametrize(
-    "activation_type,params,expected_parent,expected_command",
+    "activation_type,params,expected_parent,expected_command,expected_icon",
     (
         # Test with a simple command
         (
             "FILES",
             {"command": "echo hello"},
             "Software\\Classes\\*\\shell",
             "echo hello",
+            None,
+        ),
+        # Test with an icon
+        (
+            "FILES",
+            {"command": "echo hello", "icon_path": "\\this\\is\\a\\placeholder.ico"},
+            "Software\\Classes\\*\\shell",
+            "echo hello",
+            "\\this\\is\\a\\placeholder.ico"
         ),
         # Test with command variables
         (
             "FILES",
             {"command": "echo ?", "command_vars": ["FILENAME"]},
             "Software\\Classes\\*\\shell",
             '''"{}" -c "import os; import sys; os.system('echo ' + ' '.join(sys.argv[1:])  + '')" "%1"'''.format(
                 sys.executable
             ),
+            None,
         ),
         # Test with a python function
         (
             "FILES",
             {"python": foo},
             "Software\\Classes\\*\\shell",
             '''"{}" -c "import sys; sys.path.insert(0, '{}'); import test_windows; test_windows.foo([' '.join(sys.argv[1:]) ],'')" "%1"'''.format(
                 sys.executable, Path(__file__).parent.as_posix()
             ),
+            None,
         ),
         # Test with DIRECTORY_BACKGROUND
         (
             "DIRECTORY_BACKGROUND",
             {"python": foo},
             "Software\\Classes\\Directory\\Background\\shell",
             '''"{}" -c "import sys; import os; sys.path.insert(0, '{}'); import test_windows; test_windows.foo([os.getcwd()],'')"'''.format(
                 sys.executable, Path(__file__).parent.as_posix()
             ),
+            None,
         ),
         # Test with DESKTOP
         (
             "DESKTOP",
             {"python": foo},
             "Software\\Classes\\DesktopBackground\\shell",
             '''"{}" -c "import sys; sys.path.insert(0, '{}'); import test_windows; test_windows.foo([' '.join(sys.argv[1:]) ],'')" "%1"'''.format(
                 sys.executable, Path(__file__).parent.as_posix()
             ),
+            None,
         ),
     ),
 )
 def test_context_command(
     activation_type: ActivationType,
     params: dict[str, Any],
     expected_parent: str,
     expected_command: str,
+    expected_icon: str,
     windows_platform: None,
     mocked_winreg: MockedWinReg,
 ) -> None:
     """Tests ContextCommand with various options."""
     cm = menus.ContextMenu("Test", activation_type)
     cm.add_items([menus.ContextCommand("Command", **params)])
     cm.compile()
 
     mocked_winreg.assert_context_menu(expected_parent, "Test")
-    mocked_winreg.assert_context_command(
-        f"{expected_parent}\\Test\\shell", "Command", expected_command
-    )
+
+    if expected_icon is not None:
+        mocked_winreg.assert_context_command_with_icon(
+            f"{expected_parent}\\Test\\shell", "Command", expected_command, expected_icon
+        )
+    else:
+        mocked_winreg.assert_context_command(
+            f"{expected_parent}\\Test\\shell", "Command", expected_command
+        )
 
 
 @pytest.mark.parametrize(
-    "activation_type,params,expected_parent,expected_command",
+    "activation_type,params,expected_parent,expected_command,expected_icon",
     (
         # Test with a simple command
         (
             "FILES",
             {"command": "echo hello"},
             "Software\\Classes\\*\\shell",
             "echo hello",
+            None,
+        ),
+        # Test with an icon
+        (
+            "FILES",
+            {"command": "echo hello", "icon_path": "\\this\\is\\a\\placeholder.ico"},
+            "Software\\Classes\\*\\shell",
+            "echo hello",
+            "\\this\\is\\a\\placeholder.ico",
         ),
         # Test with command variables
         (
             "FILES",
             {"command": "echo ?", "command_vars": ["FILENAME"]},
             "Software\\Classes\\*\\shell",
             '''"{}" -c "import os; import sys; os.system('echo ' + ' '.join(sys.argv[1:])  + '')" "%1"'''.format(
                 sys.executable
             ),
+            None,
         ),
         # Test with a python function
         (
             "FILES",
             {"python": foo},
             "Software\\Classes\\*\\shell",
             '''"{}" -c "import sys; sys.path.insert(0, '{}'); import test_windows; test_windows.foo([' '.join(sys.argv[1:]) ],'')" "%1"'''.format(
                 sys.executable, Path(__file__).parent.as_posix()
             ),
+            None,
         ),
         # Test with DIRECTORY_BACKGROUND
         (
             "DIRECTORY_BACKGROUND",
             {"python": foo},
             "Software\\Classes\\Directory\\Background\\shell",
             '''"{}" -c "import sys; import os; sys.path.insert(0, '{}'); import test_windows; test_windows.foo([os.getcwd()],'')"'''.format(
                 sys.executable, Path(__file__).parent.as_posix()
             ),
+            None,
         ),
         # Test with file extension
         (
             ".txt",
             {"command": "echo hello"},
             "Software\\Classes\\SystemFileAssociations\\.txt\\shell",
             "echo hello",
+            None,
         ),
     ),
 )
 def test_fast_command(
     activation_type: ActivationType,
     params: dict[str, Any],
     expected_parent: str,
     expected_command: str,
+    expected_icon: str | None,
     windows_platform: None,
     mocked_winreg: MockedWinReg,
 ) -> None:
     """Tests FastCommand with various options."""
     menus.FastCommand("Test", activation_type, **params).compile()
 
-    mocked_winreg.assert_fast_command(expected_parent, "Test", expected_command)
+    if expected_icon is not None:
+        mocked_winreg.assert_fast_command_with_icon(expected_parent, "Test", expected_command, expected_icon)
+    else:
+        mocked_winreg.assert_fast_command(expected_parent, "Test", expected_command)
+
```

