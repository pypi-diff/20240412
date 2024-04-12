# Comparing `tmp/archadeptcli-1.2.1.tar.gz` & `tmp/archadeptcli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archadeptcli-1.2.1.tar", max compression
+gzip compressed data, was "archadeptcli-1.2.2.tar", max compression
```

## Comparing `archadeptcli-1.2.1.tar` & `archadeptcli-1.2.2.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-12-28 19:33:27.009392 archadeptcli-1.2.1/LICENSE
--rw-r--r--   0        0        0     9703 2024-02-15 10:16:43.308026 archadeptcli-1.2.1/README.md
--rw-r--r--   0        0        0     1171 2023-12-28 19:33:27.013898 archadeptcli-1.2.1/archadeptcli/__init__.py
--rw-r--r--   0        0        0    18307 2024-02-15 10:16:55.815839 archadeptcli-1.2.1/archadeptcli/__main__.py
--rw-r--r--   0        0        0     3195 2024-02-15 10:16:43.309354 archadeptcli-1.2.1/archadeptcli/console.py
--rw-r--r--   0        0        0    14494 2024-02-15 10:16:43.309808 archadeptcli-1.2.1/archadeptcli/docker.py
--rw-r--r--   0        0        0     6778 2024-02-15 10:16:43.310266 archadeptcli-1.2.1/archadeptcli/exceptions.py
--rw-r--r--   0        0        0      580 2024-02-15 10:16:59.507657 archadeptcli-1.2.1/pyproject.toml
--rw-r--r--   0        0        0    10518 1970-01-01 00:00:00.000000 archadeptcli-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-03-28 08:03:57.778628 archadeptcli-1.2.2/LICENSE
+-rw-r--r--   0        0        0     9773 2024-04-12 08:39:09.559398 archadeptcli-1.2.2/README.md
+-rw-r--r--   0        0        0     1171 2024-03-28 08:03:57.792460 archadeptcli-1.2.2/archadeptcli/__init__.py
+-rw-r--r--   0        0        0    18306 2024-04-12 08:41:11.101159 archadeptcli-1.2.2/archadeptcli/__main__.py
+-rw-r--r--   0        0        0     3195 2024-03-28 08:03:57.792135 archadeptcli-1.2.2/archadeptcli/console.py
+-rw-r--r--   0        0        0    25905 2024-04-03 13:08:03.003000 archadeptcli-1.2.2/archadeptcli/diagram.py
+-rw-r--r--   0        0        0    14494 2024-03-28 08:03:57.795487 archadeptcli-1.2.2/archadeptcli/docker.py
+-rw-r--r--   0        0        0     6784 2024-04-12 08:39:09.560073 archadeptcli-1.2.2/archadeptcli/exceptions.py
+-rw-r--r--   0        0        0  2197404 2023-11-26 15:28:26.000000 archadeptcli-1.2.2/archadeptcli/static/FiraCodeNerdFont-Regular/FiraCodeNerdFont-Regular.ttf
+-rw-r--r--   0        0        0     4389 2023-11-26 15:32:16.000000 archadeptcli-1.2.2/archadeptcli/static/FiraCodeNerdFont-Regular/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-28 08:50:08.970000 archadeptcli-1.2.2/archadeptcli/static/__init__.py
+-rw-r--r--   0        0        0  2827587 2024-04-03 12:59:06.443000 archadeptcli-1.2.2/archadeptcli/static/instructions.json
+-rw-r--r--   0        0        0      580 2024-04-12 08:41:00.181089 archadeptcli-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10588 1970-01-01 00:00:00.000000 archadeptcli-1.2.2/PKG-INFO
```

### Comparing `archadeptcli-1.2.1/LICENSE` & `archadeptcli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archadeptcli-1.2.1/README.md` & `archadeptcli-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,23 +36,17 @@
 | Operating System  | Version                    | x86_64 | arm64 |
 | ----------------- | -------------------------- | ------ | ----- |
 | Mac               | macOS Sonoma 14.1          | TODO   | 🟢    |
 | Windows 10        | Windows 10 Enterprise 22H2 | 🟢     | N/A   |
 | Windows 11        | TODO                       | TODO   | TODO  |
 | Linux             | Ubuntu 22.04 LTS           | 🟢     | TODO  |
 
-Skip to installation instructions for:
- * [macOS](#macos)
- * [Windows](#windows)
- * [Linux](#linux)
-
-Or skip to [usage](#usage).
-
-
-### macOS
+Click to expand for your operating system:
+<details>
+<summary>macOS instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Install Homebrew by following the instructions at: https://brew.sh
 
 3. Install Python 3.8 or newer via Homebrew:
 ```console
@@ -85,18 +79,19 @@
 ```console
 $ pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
+Proceed to [usage](#usage).
+</details>
 
-
-### Windows
+<details>
+<summary>Windows instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Install Python 3.8 or newer from https://www.python.org/downloads/windows/
 
 > [!WARNING]
 > We strongly recommend *not* using the Microsoft Store to install Python 3; please download and install from the official Python website.
@@ -128,18 +123,19 @@
 ```console
 PS> py -3 -m pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
-
+Proceed to [usage](#usage).
+</details>
 
-### Linux
+<details>
+<summary>Linux instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Use your distribution's package manager to check the installed version of
    Python 3, for example on Ubuntu using `apt`:
 ```console
 $ apt show python3 | grep Version
@@ -177,16 +173,16 @@
 ```console
 $ python3 -m pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
-
+Proceed to [usage](#usage).
+</details>
 
 ## Usage
 
 The following commands are available:
 
 | Command | Description                                                                |
 | ------- | -------------------------------------------------------------------------- |
@@ -254,15 +250,15 @@
 
 
 ### `debug`
 
 ```console
 usage: archadept debug [-h] [-v] CONTAINER
 
-Attaches a GDB debug session to a live QEMU simulation started by `archadept run`.
+Attaches an LLDB debug session to a live QEMU simulation started by `archadept run -s`.
 
 options:
   -h, --help  show this help message and exit
   -v          enable logging verbose debug messages
 
 command-specific positional arguments:
   CONTAINER   container in which the QEMU simulation is running, as given by `archadept run`
```

### Comparing `archadeptcli-1.2.1/archadeptcli/__init__.py` & `archadeptcli-1.2.2/archadeptcli/__init__.py`

 * *Files identical despite different names*

### Comparing `archadeptcli-1.2.1/archadeptcli/__main__.py` & `archadeptcli-1.2.2/archadeptcli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Local deps
 import archadeptcli
 from archadeptcli.console import getConsole, RichAlign, RichGroup, RichPanel, Color
 from archadeptcli.docker import DockerCLIWrapper
 from archadeptcli.exceptions import *
 
-ARCHADEPTCLI_BASE_TAG = '1.2.1'
+ARCHADEPTCLI_BASE_TAG = '1.2.2'
 """ Current base tag of the archadeptcli repository. """
 
 class CommandLineArgs():
     """ Class representing the arguments parsed from the command line. """
 
     def __init__(self):
         """ Parse command line arguments. """
@@ -66,15 +66,15 @@
                         'description': 'Runs an ArchAdept example project on a simulated Raspberry Pi 3b.',
                     },
                 },
                 {
                     'command': 'debug',
                     'dict': {
                         'help': 'attach debugger to live simulation',
-                        'description': 'Attaches an LLDB debug session to a live QEMU simulation started by `archadept run`.',
+                        'description': 'Attaches an LLDB debug session to a live QEMU simulation started by `archadept run -s`.',
                     },
                 },
                 {
                     'command': 'pull',
                     'dict': {
                         'help': 'pull the latest Docker image',
                         'description': 'Pulls the latest ArchAdept CLI backend Docker image from DockerHub.',
@@ -461,15 +461,15 @@
         elif args.command == 'pull':
             return main_pull(args.image, args.tag)
         elif args.command == 'prune':
             return main_prune()
         else:
             raise InternalError(f'unimplemented function: main_{args.command}()')
     except ArchAdeptError as e:
+        e.render()
         if args.debug:
             raise e
         else:
-            e.render()
             return 1
     except Exception as e:
         raise UngracefulExit('crashed due to uncaught exception') from e
```

### Comparing `archadeptcli-1.2.1/archadeptcli/console.py` & `archadeptcli-1.2.2/archadeptcli/console.py`

 * *Files identical despite different names*

### Comparing `archadeptcli-1.2.1/archadeptcli/docker.py` & `archadeptcli-1.2.2/archadeptcli/docker.py`

 * *Files identical despite different names*

### Comparing `archadeptcli-1.2.1/archadeptcli/exceptions.py` & `archadeptcli-1.2.2/archadeptcli/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         if self.is_bug:
             renderables += ['This looks like a bug in archadeptcli 😔\n',
                             'Please submit a bug report to support@archadept.com, or raise an issue',
                             'on the GitHub repository at https://github.com/ArchAdept/archadeptcli.']
         else:
             renderables += ['See https://archadept.com/help/errors for more help with this error.']
         console = getConsole()
-        console.print(RichPanel.fit(RichGroup(*renderables), Color.ERROR,
+        console.print(RichPanel.fit(RichGroup(*renderables), style=Color.ERROR,
                                     title=f'!!! ArchAdept error 0x{self.unique_id:04X} !!!'))
         if not console.debug_enabled:
             console.print(RichPanel.fit(f'Note: You can also rerun with `-v` for more verbose debug logging.', style=Color.ERROR))
 
 class UngracefulExit(ArchAdeptError):
     """ Raised when we crash due to any kind of uncaught exception. """
     unique_id = 0xEAA1
```

### Comparing `archadeptcli-1.2.1/pyproject.toml` & `archadeptcli-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archadeptcli"
-version = "1.2.1"
+version = "1.2.2"
 description = "Command line interface for building, running, debugging, and disassembling the ArchAdept training course example projects."
 authors = ["Ash Wilding <ash@archadept.com>"]
 homepage = "https://archadept.com/"
 repository = "https://github.com/archadept/archadeptcli"
 readme = "README.md"
 license = "MIT"
```

### Comparing `archadeptcli-1.2.1/PKG-INFO` & `archadeptcli-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archadeptcli
-Version: 1.2.1
+Version: 1.2.2
 Summary: Command line interface for building, running, debugging, and disassembling the ArchAdept training course example projects.
 Home-page: https://archadept.com/
 License: MIT
 Author: Ash Wilding
 Author-email: ash@archadept.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -56,23 +56,17 @@
 | Operating System  | Version                    | x86_64 | arm64 |
 | ----------------- | -------------------------- | ------ | ----- |
 | Mac               | macOS Sonoma 14.1          | TODO   | 🟢    |
 | Windows 10        | Windows 10 Enterprise 22H2 | 🟢     | N/A   |
 | Windows 11        | TODO                       | TODO   | TODO  |
 | Linux             | Ubuntu 22.04 LTS           | 🟢     | TODO  |
 
-Skip to installation instructions for:
- * [macOS](#macos)
- * [Windows](#windows)
- * [Linux](#linux)
-
-Or skip to [usage](#usage).
-
-
-### macOS
+Click to expand for your operating system:
+<details>
+<summary>macOS instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Install Homebrew by following the instructions at: https://brew.sh
 
 3. Install Python 3.8 or newer via Homebrew:
 ```console
@@ -105,18 +99,19 @@
 ```console
 $ pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
+Proceed to [usage](#usage).
+</details>
 
-
-### Windows
+<details>
+<summary>Windows instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Install Python 3.8 or newer from https://www.python.org/downloads/windows/
 
 > [!WARNING]
 > We strongly recommend *not* using the Microsoft Store to install Python 3; please download and install from the official Python website.
@@ -148,18 +143,19 @@
 ```console
 PS> py -3 -m pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
-
+Proceed to [usage](#usage).
+</details>
 
-### Linux
+<details>
+<summary>Linux instructions</summary>
 
 1. Install Docker Desktop by following the instructions at: https://www.docker.com/products/docker-desktop/
 
 2. Use your distribution's package manager to check the installed version of
    Python 3, for example on Ubuntu using `apt`:
 ```console
 $ apt show python3 | grep Version
@@ -197,16 +193,16 @@
 ```console
 $ python3 -m pipx upgrade archadeptcli
 ```
 
 > [!TIP]
 > Run `archadept pull` now to download the backend Docker image ahead of time; this may take a few minutes to complete.
 
-Skip to [usage](#usage).
-
+Proceed to [usage](#usage).
+</details>
 
 ## Usage
 
 The following commands are available:
 
 | Command | Description                                                                |
 | ------- | -------------------------------------------------------------------------- |
@@ -274,15 +270,15 @@
 
 
 ### `debug`
 
 ```console
 usage: archadept debug [-h] [-v] CONTAINER
 
-Attaches a GDB debug session to a live QEMU simulation started by `archadept run`.
+Attaches an LLDB debug session to a live QEMU simulation started by `archadept run -s`.
 
 options:
   -h, --help  show this help message and exit
   -v          enable logging verbose debug messages
 
 command-specific positional arguments:
   CONTAINER   container in which the QEMU simulation is running, as given by `archadept run`
```

