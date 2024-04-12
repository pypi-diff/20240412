# Comparing `tmp/ultra_logger-0.1.1.tar.gz` & `tmp/ultra_logger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultra_logger-0.1.1.tar", last modified: Thu Apr 11 16:10:58 2024, max compression
+gzip compressed data, was "ultra_logger-0.1.2.tar", last modified: Fri Apr 12 05:43:16 2024, max compression
```

## Comparing `ultra_logger-0.1.1.tar` & `ultra_logger-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/
--rw-rw-rw-   0        0        0     5306 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2024-04-11 13:48:05.000000 ultra_logger-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1550 2024-04-11 16:10:47.000000 ultra_logger-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.946976 ultra_logger-0.1.1/ultra_logger/
--rw-rw-rw-   0        0        0       28 2024-04-11 15:24:41.000000 ultra_logger-0.1.1/ultra_logger/__init__.py
--rw-rw-rw-   0        0        0     8077 2024-03-27 15:30:50.000000 ultra_logger-0.1.1/ultra_logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.960422 ultra_logger-0.1.1/ultra_logger.egg-info/
--rw-rw-rw-   0        0        0     5306 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 05:43:16.548176 ultra_logger-0.1.2/
+-rw-rw-rw-   0        0        0     5362 2024-04-12 05:43:16.547138 ultra_logger-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3960 2024-04-12 05:42:42.000000 ultra_logger-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 05:43:16.548176 ultra_logger-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1550 2024-04-12 05:42:50.000000 ultra_logger-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:43:16.506520 ultra_logger-0.1.2/ultra_logger/
+-rw-rw-rw-   0        0        0       28 2024-04-11 15:24:41.000000 ultra_logger-0.1.2/ultra_logger/__init__.py
+-rw-rw-rw-   0        0        0     8077 2024-03-27 15:30:50.000000 ultra_logger-0.1.2/ultra_logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-12 05:43:16.546110 ultra_logger-0.1.2/ultra_logger.egg-info/
+-rw-rw-rw-   0        0        0     5362 2024-04-12 05:43:16.000000 ultra_logger-0.1.2/ultra_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-12 05:43:16.000000 ultra_logger-0.1.2/ultra_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 05:43:16.000000 ultra_logger-0.1.2/ultra_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2024-04-12 05:43:16.000000 ultra_logger-0.1.2/ultra_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 05:43:16.000000 ultra_logger-0.1.2/ultra_logger.egg-info/top_level.txt
```

### Comparing `ultra_logger-0.1.1/PKG-INFO` & `ultra_logger-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultra_logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python package provides a robust and customizable logger that simplifies the process of recording messages and events in your applications. It leverages the power of the `colorlog` library to enhance readability and debugging capabilities.
 Author: Om Sing Chandel
 Author-email: omchandel1703@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
@@ -52,26 +52,28 @@
 * **Default Loggers:** Provides convenient wrappers for standard logging methods (`debug`, `info`, `warning`, `error`, `critical`, and `exception`).
 * **Session Logging:** Decorator function `log_session` to enclose a block of code with logging messages for session tracking.
 * **Log File Reading:** Utility function `read_log_file` to conveniently read and display the contents of the log file.
 * **Log File Clearing:** Optional `clear_log_file` method to clear existing log data.
 
 **Installation**
 
-To install the `custom_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
+From [pypi.org](https://pypi.org/project/ultra-logger/)
+
+To install the `ultra_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
 
 ```bash
-pip install custom_logger
+pip install ultra_logger
 ```
 
 **Usage**
 
 1. **Import the Logger Class:**
 
    ```python
-   from custom_logger import Logger
+   from ultra_logger import Logger
    ```
 
 2. **Create a Logger Instance:**
 
    ```python
    logger = Logger(log_name='my_logger', log_file='app.log', log_to_console=True)
    ```
```

### Comparing `ultra_logger-0.1.1/README.md` & `ultra_logger-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,26 +15,28 @@
 * **Default Loggers:** Provides convenient wrappers for standard logging methods (`debug`, `info`, `warning`, `error`, `critical`, and `exception`).
 * **Session Logging:** Decorator function `log_session` to enclose a block of code with logging messages for session tracking.
 * **Log File Reading:** Utility function `read_log_file` to conveniently read and display the contents of the log file.
 * **Log File Clearing:** Optional `clear_log_file` method to clear existing log data.
 
 **Installation**
 
-To install the `custom_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
+From [pypi.org](https://pypi.org/project/ultra-logger/)
+
+To install the `ultra_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
 
 ```bash
-pip install custom_logger
+pip install ultra_logger
 ```
 
 **Usage**
 
 1. **Import the Logger Class:**
 
    ```python
-   from custom_logger import Logger
+   from ultra_logger import Logger
    ```
 
 2. **Create a Logger Instance:**
 
    ```python
    logger = Logger(log_name='my_logger', log_file='app.log', log_to_console=True)
    ```
```

### Comparing `ultra_logger-0.1.1/setup.py` & `ultra_logger-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
     
 setup(
     name='ultra_logger',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     author="Om Sing Chandel",
     author_email="omchandel1703@gmail.com",
     description="This Python package provides a robust and customizable logger that simplifies the process of recording messages and events in your applications. It leverages the power of the `colorlog` library to enhance readability and debugging capabilities.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
```

### Comparing `ultra_logger-0.1.1/ultra_logger/logger.py` & `ultra_logger-0.1.2/ultra_logger/logger.py`

 * *Files identical despite different names*

### Comparing `ultra_logger-0.1.1/ultra_logger.egg-info/PKG-INFO` & `ultra_logger-0.1.2/ultra_logger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultra_logger
-Version: 0.1.1
+Version: 0.1.2
 Summary: This Python package provides a robust and customizable logger that simplifies the process of recording messages and events in your applications. It leverages the power of the `colorlog` library to enhance readability and debugging capabilities.
 Author: Om Sing Chandel
 Author-email: omchandel1703@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: colorama==0.4.6
@@ -52,26 +52,28 @@
 * **Default Loggers:** Provides convenient wrappers for standard logging methods (`debug`, `info`, `warning`, `error`, `critical`, and `exception`).
 * **Session Logging:** Decorator function `log_session` to enclose a block of code with logging messages for session tracking.
 * **Log File Reading:** Utility function `read_log_file` to conveniently read and display the contents of the log file.
 * **Log File Clearing:** Optional `clear_log_file` method to clear existing log data.
 
 **Installation**
 
-To install the `custom_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
+From [pypi.org](https://pypi.org/project/ultra-logger/)
+
+To install the `ultra_logger` package from PyPI (the Python Package Index), use the following command in your terminal:
 
 ```bash
-pip install custom_logger
+pip install ultra_logger
 ```
 
 **Usage**
 
 1. **Import the Logger Class:**
 
    ```python
-   from custom_logger import Logger
+   from ultra_logger import Logger
    ```
 
 2. **Create a Logger Instance:**
 
    ```python
    logger = Logger(log_name='my_logger', log_file='app.log', log_to_console=True)
    ```
```

### Comparing `ultra_logger-0.1.1/ultra_logger.egg-info/requires.txt` & `ultra_logger-0.1.2/ultra_logger.egg-info/requires.txt`

 * *Files identical despite different names*

