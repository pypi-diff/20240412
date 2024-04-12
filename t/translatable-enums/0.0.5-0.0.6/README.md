# Comparing `tmp/translatable_enums-0.0.5.tar.gz` & `tmp/translatable_enums-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translatable_enums-0.0.5.tar", max compression
+gzip compressed data, was "translatable_enums-0.0.6.tar", max compression
```

## Comparing `translatable_enums-0.0.5.tar` & `translatable_enums-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      485 2024-04-06 13:09:19.657292 translatable_enums-0.0.5/i18n/__init__.py
--rw-r--r--   0        0        0     1916 2024-04-06 13:09:19.835977 translatable_enums-0.0.5/i18n/__main__.py
--rw-r--r--   0        0        0      442 2024-04-06 13:09:19.740810 translatable_enums-0.0.5/i18n/enums.py
--rw-r--r--   0        0        0      215 2024-04-06 13:14:45.304159 translatable_enums-0.0.5/i18n/settings.py
--rw-r--r--   0        0        0      404 2024-04-06 13:09:19.760304 translatable_enums-0.0.5/i18n/tools.py
--rw-r--r--   0        0        0      282 2024-04-06 12:57:01.911526 translatable_enums-0.0.5/i18n/types.py
--rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.5/i18n/utils/__init__.py
--rw-r--r--   0        0        0       94 2024-04-06 13:09:19.874235 translatable_enums-0.0.5/i18n/utils/clsutils/__init__.py
--rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.5/i18n/utils/clsutils/generators.py
--rw-r--r--   0        0        0      248 2024-04-06 13:09:19.948795 translatable_enums-0.0.5/i18n/utils/gettext/__init__.py
--rw-r--r--   0        0        0      277 2024-04-06 13:09:19.982037 translatable_enums-0.0.5/i18n/utils/gettext/contexts.py
--rw-r--r--   0        0        0      495 2024-04-06 13:09:19.698542 translatable_enums-0.0.5/i18n/utils/gettext/shortcuts.py
--rw-r--r--   0        0        0       65 2024-04-06 13:09:19.709541 translatable_enums-0.0.5/i18n/utils/imputils/__init__.py
--rw-r--r--   0        0        0      842 2024-04-06 13:16:05.556430 translatable_enums-0.0.5/i18n/utils/imputils/utils.py
--rw-r--r--   0        0        0      102 2024-04-06 13:09:19.754693 translatable_enums-0.0.5/i18n/utils/potfile/__init__.py
--rw-r--r--   0        0        0      353 2024-04-06 13:09:19.769710 translatable_enums-0.0.5/i18n/utils/potfile/constants.py
--rw-r--r--   0        0        0     2021 2024-04-06 13:09:19.864235 translatable_enums-0.0.5/i18n/utils/potfile/potfile.py
--rw-r--r--   0        0        0      103 2024-04-06 13:09:19.778730 translatable_enums-0.0.5/i18n/utils/potfile/types.py
--rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.5/LICENSE
--rw-r--r--   0        0        0      800 2024-04-06 13:08:10.690546 translatable_enums-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2795 2024-04-06 13:19:21.424481 translatable_enums-0.0.5/README.md
--rw-r--r--   0        0        0     3478 1970-01-01 00:00:00.000000 translatable_enums-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      485 2024-04-06 13:09:19.657292 translatable_enums-0.0.6/i18n/__init__.py
+-rw-r--r--   0        0        0     1960 2024-04-12 08:36:35.103945 translatable_enums-0.0.6/i18n/__main__.py
+-rw-r--r--   0        0        0      442 2024-04-06 13:09:19.740810 translatable_enums-0.0.6/i18n/enums.py
+-rw-r--r--   0        0        0      215 2024-04-12 07:58:21.181143 translatable_enums-0.0.6/i18n/settings.py
+-rw-r--r--   0        0        0     1074 2024-04-12 08:18:54.386248 translatable_enums-0.0.6/i18n/tools.py
+-rw-r--r--   0        0        0      331 2024-04-12 07:58:21.152141 translatable_enums-0.0.6/i18n/types.py
+-rw-r--r--   0        0        0        0 2024-02-10 10:52:36.822551 translatable_enums-0.0.6/i18n/utils/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-06 13:09:19.874235 translatable_enums-0.0.6/i18n/utils/clsutils/__init__.py
+-rw-r--r--   0        0        0      391 2024-02-11 10:25:57.917138 translatable_enums-0.0.6/i18n/utils/clsutils/generators.py
+-rw-r--r--   0        0        0      248 2024-04-06 13:09:19.948795 translatable_enums-0.0.6/i18n/utils/gettext/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-06 13:09:19.982037 translatable_enums-0.0.6/i18n/utils/gettext/contexts.py
+-rw-r--r--   0        0        0      495 2024-04-06 13:09:19.698542 translatable_enums-0.0.6/i18n/utils/gettext/shortcuts.py
+-rw-r--r--   0        0        0       65 2024-04-06 13:09:19.709541 translatable_enums-0.0.6/i18n/utils/imputils/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-06 13:16:05.556430 translatable_enums-0.0.6/i18n/utils/imputils/utils.py
+-rw-r--r--   0        0        0      102 2024-04-06 13:09:19.754693 translatable_enums-0.0.6/i18n/utils/potfile/__init__.py
+-rw-r--r--   0        0        0      353 2024-04-06 13:09:19.769710 translatable_enums-0.0.6/i18n/utils/potfile/constants.py
+-rw-r--r--   0        0        0     2021 2024-04-06 13:09:19.864235 translatable_enums-0.0.6/i18n/utils/potfile/potfile.py
+-rw-r--r--   0        0        0      103 2024-04-06 13:09:19.778730 translatable_enums-0.0.6/i18n/utils/potfile/types.py
+-rw-r--r--   0        0        0     1090 2024-02-10 10:48:35.222832 translatable_enums-0.0.6/LICENSE
+-rw-r--r--   0        0        0      800 2024-04-12 07:58:21.204143 translatable_enums-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3496 2024-04-12 08:36:35.108951 translatable_enums-0.0.6/README.md
+-rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 translatable_enums-0.0.6/PKG-INFO
```

### Comparing `translatable_enums-0.0.5/i18n/__main__.py` & `translatable_enums-0.0.6/i18n/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import argparse
 import sys
-from typing import Iterable
 
 from i18n.settings import APP, DESCRIPTION, VERSION
-from i18n.types import BaseTranslatableEnum, Key
-from i18n.tools import extract_keys
+from i18n.types import BaseTranslatableEnum
+from i18n.tools import extract_keys, save_pot
 from i18n.utils.gettext import set_language
-from i18n.utils.potfile import POTFile, TEMPLATES
+from i18n.utils.potfile import TEMPLATES
 from i18n.utils.imputils import import_module
 
 
 def setup_argparse() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(prog=APP, description=DESCRIPTION)
 
     parser.add_argument(
@@ -37,27 +36,29 @@
         "--template",
         required=False,
         default="common",
         help=".pot file template",
         choices=set(TEMPLATES.keys()),
     )
 
+    parser.add_argument(
+        "-k",
+        "--key-format",
+        required=False,
+        default="{value}",
+        help='key format (name - attribute name, value - attribute value, enum - enum name). Default: "{value}"',
+    )
+
     return parser
 
 
 def show_version():
     print(VERSION)
 
 
-def save_pot(file: str, keys: Iterable[Key], template: str = None) -> None:
-    with POTFile(file=file, mode="w", template=template) as potfile:
-        for key in keys:
-            potfile.write(key=key.key, comment=key.comment)
-
-
 def main():
     parser = setup_argparse()
     args = parser.parse_args()
 
     if args.version:
         show_version()
         sys.exit(0)
@@ -67,12 +68,17 @@
         import_module(source)
     except ImportError:
         raise
 
     set_language("en")
 
     keys = extract_keys(base_enum=BaseTranslatableEnum)
-    save_pot(file=args.destination, keys=keys, template=TEMPLATES[args.template])
+    save_pot(
+        file=args.destination,
+        keys=keys,
+        template=TEMPLATES[args.template],
+        key_format=args.key_format,
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `translatable_enums-0.0.5/i18n/utils/imputils/utils.py` & `translatable_enums-0.0.6/i18n/utils/imputils/utils.py`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.5/i18n/utils/potfile/potfile.py` & `translatable_enums-0.0.6/i18n/utils/potfile/potfile.py`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.5/LICENSE` & `translatable_enums-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `translatable_enums-0.0.5/pyproject.toml` & `translatable_enums-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "translatable-enums"
-version = "0.0.5"
+version = "0.0.6"
 description = "Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "i18n" },
 ]
```

### Comparing `translatable_enums-0.0.5/README.md` & `translatable_enums-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 
 ## Getting-Started
 
 ```python
 from i18n import (
     TranslatableEnum,
     set_domain,
-    set_language
+    set_language,
+    language
 )
 
 
 class Messages(TranslatableEnum):
     HELLO = 'Hello,'
     WORLD = 'World!'
 
@@ -59,14 +60,19 @@
 print(Messages.HELLO, Messages.WORLD)  # Привіт, Світ!
 
 set_language('fr_FR')
 
 print(Messages.HELLO, Messages.WORLD)  # Bonjour le monde!
 
 print(Messages.HELLO.language('uk'), Messages.WORLD.language('en'))  # Привіт, World!
+
+with language('uk_UA'):
+    print(Messages.HELLO, Messages.WORLD)  # Привіт, Світ!
+
+print(Messages.HELLO, Messages.WORLD)  # Bonjour le monde!
 ```
 
 ### Extraction-Tools
 
 To extract the translation-keys from application:
 
 ```shell
@@ -83,26 +89,65 @@
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: \n"
 "MIME-Version: \n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
+# Messages.WORLD
+msgid "World!"
+msgstr ""
+
+# Messages.HELLO
 msgid "Hello,"
 msgstr ""
+```
+
+#### Key-Format
+
+```shell
+python -m i18n main.py application.pot --key-format "{enum}.{name}.{value}"
+```
+
+Default: ```"{value}"```
+
+- enum - enum name
+- name - attribute name
+- value - attribute value
 
+Examples:
+
+```{enum}.{name}.{value}```
+```
+# Messages.WORLD
+msgid "Messages.WORLD.World!"
+msgstr ""
+```
+
+```{enum}.{name}```
+```
+# Messages.WORLD
+msgid "Messages.WORLD"
+msgstr ""
+```
+
+
+```{value}```
+```
+# Messages.WORLD
 msgid "World!"
 msgstr ""
 ```
 
+
 ### Examples
 
 See [/examples](examples/) for more examples.
 
 ## Status
 
-```0.0.5``` - **RELEASED**
+```0.0.6``` - **RELEASED**
 
 ## Licence
 
 Translatable-Enums is released under the MIT License. See the
 bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```

#### html2text {}

```diff
@@ -4,25 +4,33 @@
                                     _S_t_y_l_e_]
 Translatable-Enums is an i18n tool which uses built-in Enums as a convenient
 way to store translation keys. ## Key-Features - No dependencies except the
 Python's standard library. Based on built-in enums & gettext - Powerful utility
 for extracting translation-keys - Easy-to-Use ## Installation You can use PIP:
 ```shell pip install translatable-enums ``` Or Poetry: ```shell poetry add
 translatable-enums ``` ## Getting-Started ```python from i18n import
-( TranslatableEnum, set_domain, set_language ) class Messages
+( TranslatableEnum, set_domain, set_language, language ) class Messages
 (TranslatableEnum): HELLO = 'Hello,' WORLD = 'World!' set_domain('app', './
 resources/languages') set_language('en_US') print(Messages.HELLO,
 Messages.WORLD) # Hello, World! set_language('uk_UA') print(Messages.HELLO,
 Messages.WORLD) # ÐÑÐ¸Ð²ÑÑ, Ð¡Ð²ÑÑ! set_language('fr_FR') print
 (Messages.HELLO, Messages.WORLD) # Bonjour le monde! print
 (Messages.HELLO.language('uk'), Messages.WORLD.language('en')) # ÐÑÐ¸Ð²ÑÑ,
-World! ``` ### Extraction-Tools To extract the translation-keys from
+World! with language('uk_UA'): print(Messages.HELLO, Messages.WORLD) #
+ÐÑÐ¸Ð²ÑÑ, Ð¡Ð²ÑÑ! print(Messages.HELLO, Messages.WORLD) # Bonjour le
+monde! ``` ### Extraction-Tools To extract the translation-keys from
 application: ```shell python -m i18n main.py application.pot ``` You will
 obtain a [.pot](https://pofile.net/) file like this: ```potfile msgid "" msgstr
 "" "Project-Id-Version: \n" "POT-Creation-Date: \n" "Last-Translator: \n"
 "Language-Team: \n" "Language: \n" "MIME-Version: \n" "Content-Type: text/
-plain; charset=utf-8\n" "Content-Transfer-Encoding: 8bit\n" msgid "Hello,"
-msgstr "" msgid "World!" msgstr "" ``` ### Examples See [/examples](examples/
-) for more examples. ## Status ```0.0.5``` - **RELEASED** ## Licence
-Translatable-Enums is released under the MIT License. See the bundled [LICENSE]
-(https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file
-for details.
+plain; charset=utf-8\n" "Content-Transfer-Encoding: 8bit\n" # Messages.WORLD
+msgid "World!" msgstr "" # Messages.HELLO msgid "Hello," msgstr "" ``` ####
+Key-Format ```shell python -m i18n main.py application.pot --key-format "
+{enum}.{name}.{value}" ``` Default: ```"{value}"``` - enum - enum name - name -
+attribute name - value - attribute value Examples: ```{enum}.{name}.{value}```
+``` # Messages.WORLD msgid "Messages.WORLD.World!" msgstr "" ``` ```{enum}.
+{name}``` ``` # Messages.WORLD msgid "Messages.WORLD" msgstr "" ``` ```
+{value}``` ``` # Messages.WORLD msgid "World!" msgstr "" ``` ### Examples See
+[/examples](examples/) for more examples. ## Status ```0.0.6``` - **RELEASED**
+## Licence Translatable-Enums is released under the MIT License. See the
+bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/
+master/LICENSE) file for details.
```

### Comparing `translatable_enums-0.0.5/PKG-INFO` & `translatable_enums-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translatable-enums
-Version: 0.0.5
+Version: 0.0.6
 Summary: Translatable-Enums is a i18n tool which uses built-in Enums as an convenient way to store translation keys.
 Home-page: https://github.com/CrazyProger1/Translatable-Enums
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -54,15 +54,16 @@
 
 ## Getting-Started
 
 ```python
 from i18n import (
     TranslatableEnum,
     set_domain,
-    set_language
+    set_language,
+    language
 )
 
 
 class Messages(TranslatableEnum):
     HELLO = 'Hello,'
     WORLD = 'World!'
 
@@ -77,14 +78,19 @@
 print(Messages.HELLO, Messages.WORLD)  # Привіт, Світ!
 
 set_language('fr_FR')
 
 print(Messages.HELLO, Messages.WORLD)  # Bonjour le monde!
 
 print(Messages.HELLO.language('uk'), Messages.WORLD.language('en'))  # Привіт, World!
+
+with language('uk_UA'):
+    print(Messages.HELLO, Messages.WORLD)  # Привіт, Світ!
+
+print(Messages.HELLO, Messages.WORLD)  # Bonjour le monde!
 ```
 
 ### Extraction-Tools
 
 To extract the translation-keys from application:
 
 ```shell
@@ -101,26 +107,65 @@
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: \n"
 "MIME-Version: \n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
+# Messages.WORLD
+msgid "World!"
+msgstr ""
+
+# Messages.HELLO
 msgid "Hello,"
 msgstr ""
+```
+
+#### Key-Format
+
+```shell
+python -m i18n main.py application.pot --key-format "{enum}.{name}.{value}"
+```
+
+Default: ```"{value}"```
+
+- enum - enum name
+- name - attribute name
+- value - attribute value
 
+Examples:
+
+```{enum}.{name}.{value}```
+```
+# Messages.WORLD
+msgid "Messages.WORLD.World!"
+msgstr ""
+```
+
+```{enum}.{name}```
+```
+# Messages.WORLD
+msgid "Messages.WORLD"
+msgstr ""
+```
+
+
+```{value}```
+```
+# Messages.WORLD
 msgid "World!"
 msgstr ""
 ```
 
+
 ### Examples
 
 See [/examples](examples/) for more examples.
 
 ## Status
 
-```0.0.5``` - **RELEASED**
+```0.0.6``` - **RELEASED**
 
 ## Licence
 
 Translatable-Enums is released under the MIT License. See the
 bundled [LICENSE](https://github.com/CrazyProger1/Translatable-Enums/blob/master/LICENSE) file for details.
```

