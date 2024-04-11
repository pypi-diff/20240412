# Comparing `tmp/MethodicConfigurator-0.1.8.tar.gz` & `tmp/MethodicConfigurator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MethodicConfigurator-0.1.8.tar", last modified: Tue Apr  9 13:27:06 2024, max compression
+gzip compressed data, was "MethodicConfigurator-0.1.9.tar", last modified: Tue Apr  9 14:33:37 2024, max compression
```

## Comparing `MethodicConfigurator-0.1.8.tar` & `MethodicConfigurator-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:06.235277 MethodicConfigurator-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:06.231277 MethodicConfigurator-0.1.8/MethodicConfigurator/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27842 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/annotate_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/ardupilot_methodic_configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/backend_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    42536 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/backend_flightcontroller.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/component_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/extract_param_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    60729 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/frontend_tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/param_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/param_pid_adjustment_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/tempcal_IMU.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/MethodicConfigurator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:27:06.231277 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 13:27:06.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:27:03.000000 MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-09 13:27:06.231277 MethodicConfigurator-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 13:27:06.235277 MethodicConfigurator-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-09 13:26:39.000000 MethodicConfigurator-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.173461 MethodicConfigurator-0.1.9/MethodicConfigurator/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27842 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/annotate_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/ardupilot_methodic_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17164 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/backend_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42536 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/backend_flightcontroller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/component_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/extract_param_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60612 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/frontend_tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/param_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9517 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/param_pid_adjustment_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/tempcal_IMU.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/MethodicConfigurator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:33:37.173461 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-09 14:33:37.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:33:34.000000 MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:33:37.177461 MethodicConfigurator-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-09 14:33:16.000000 MethodicConfigurator-0.1.9/setup.py
```

### Comparing `MethodicConfigurator-0.1.8/LICENSE.md` & `MethodicConfigurator-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/annotate_params.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/annotate_params.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/ardupilot_methodic_configurator.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/ardupilot_methodic_configurator.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/backend_filesystem.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/backend_filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from re import compile as re_compile
 # from sys import exit as sys_exit
 # from logging import debug as logging_debug
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 from json import load as json_load
-from typing import Dict, List
+from typing import Dict
+from typing import List
+from typing import Tuple
 from zipfile import ZipFile
 from annotate_params import BASE_URL, PARAM_DEFINITION_XML_FILE, Par
 from annotate_params import get_xml_data
 from annotate_params import create_doc_dict
 from annotate_params import format_columns
 from annotate_params import split_into_lines
 from annotate_params import update_parameter_documentation
@@ -305,58 +307,45 @@
         vehicle_name = self.get_vehicle_directory_name()
         return os_path.join(self.vehicle_dir, f"{vehicle_name}.zip")
 
     def zip_file_exists(self):
         zip_file_path = self.zip_file_path()
         return os_path.exists(zip_file_path) and os_path.isfile(zip_file_path)
 
-    def zip_files(self, wrote_complete, filename_complete, wrote_read_only, filename_read_only,
-                  wrote_calibrations, filename_calibrations, wrote_non_calibrations, filename_non_calibrations):  # pylint: disable=too-many-arguments
+    def zip_files(self, files_to_zip: List[Tuple[bool, str]]):
         """
         Zips the intermediate parameter files that were written to, including specific summary files.
 
         This method creates a zip archive containing all intermediate parameter files, along with
         specific summary files if they were written. The zip file is saved in the same directory as the
         intermediate parameter files. The method checks for the existence of each file before
         attempting to add it to the zip archive.
 
         Parameters:
-        - wrote_complete (bool): Indicates if the complete parameter file was written.
-        - filename_complete (str): The name of the complete parameter file.
-        - wrote_read_only (bool): Indicates if the read-only parameter file was written.
-        - filename_read_only (str): The name of the read-only parameter file.
-        - wrote_calibrations (bool): Indicates if the calibration parameter file was written.
-        - filename_calibrations (str): The name of the calibration parameter file.
-        - wrote_non_calibrations (bool): Indicates if the non-calibration parameter file was written.
-        - filename_non_calibrations (str): The name of the non-calibration parameter file.
-
-        The method does not return any value. Instead, it logs the path of the created zip file upon completion.
+        - files_to_zip (List[Tuple[bool, str]]): A list of tuples, where each tuple contains a boolean
+                                            indicating if the file was written and a string for the filename.
         """
         zip_file_path = self.zip_file_path()
         with ZipFile(zip_file_path, 'w') as zipf:
             # Add all intermediate parameter files
             for file_name in self.file_parameters:
                 zipf.write(os_path.join(self.vehicle_dir, file_name), arcname=file_name)
 
             # Check for and add specific files if they exist
             specific_files = ["00_default.param", "apm.pdef.xml", "file_documentation.json"]
             for file_name in specific_files:
                 file_path = os_path.join(self.vehicle_dir, file_name)
                 if os_path.exists(file_path):
                     zipf.write(file_path, arcname=file_name)
 
-            # Add the newly created summary files
-            if wrote_complete:
-                zipf.write(os_path.join(self.vehicle_dir, filename_complete), arcname=filename_complete)
-            if wrote_read_only:
-                zipf.write(os_path.join(self.vehicle_dir, filename_read_only), arcname=filename_read_only)
-            if wrote_calibrations:
-                zipf.write(os_path.join(self.vehicle_dir, filename_calibrations), arcname=filename_calibrations)
-            if wrote_non_calibrations:
-                zipf.write(os_path.join(self.vehicle_dir, filename_non_calibrations), arcname=filename_non_calibrations)
+            for wrote, filename in files_to_zip:
+                if wrote:
+                    file_path = os_path.join(self.vehicle_dir, filename)
+                    if os_path.exists(file_path):
+                        zipf.write(file_path, arcname=filename)
 
         logging_info("Intermediate parameter files and summary files zipped to %s", zip_file_path)
 
     @staticmethod
     def application_icon_filepath():
         script_dir = os_path.dirname(os_path.abspath(__file__))
         return os_path.join(script_dir, 'ArduPilot_icon.png')
```

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/backend_flightcontroller.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/backend_flightcontroller.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/component_editor.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/component_editor.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/extract_param_defaults.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/extract_param_defaults.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/frontend_tkinter.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/frontend_tkinter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from logging import info as logging_info
 from logging import warning as logging_warning
 from logging import error as logging_error
 from logging import critical as logging_critical
 from PIL import Image
 from PIL import ImageTk
 from platform import system as platform_system
+from typing import List
+from typing import Tuple
 
 from webbrowser import open as webbrowser_open  # to open the blog post documentation
 
 from backend_filesystem import LocalFilesystem
 from backend_filesystem import is_within_tolerance
 from backend_flightcontroller import FlightController
 
@@ -1034,39 +1036,40 @@
                                                  "complete.param", False)
         wrote_read_only = self.write_summary_file(non_default__read_only_params,
                                                   "non-default_read-only.param", False)
         wrote_calibrations = self.write_summary_file(non_default__writable_calibrations,
                                                      "non-default_writable_calibrations.param", False)
         wrote_non_calibrations = self.write_summary_file(non_default__writable_non_calibrations,
                                                          "non-default_writable_non-calibrations.param", False)
-        self.write_zip_file(wrote_complete, wrote_read_only, wrote_calibrations, wrote_non_calibrations)
+        files_to_zip = [
+            (wrote_complete, "complete.param"),
+            (wrote_read_only, "non-default_read-only.param"),
+            (wrote_calibrations, "non-default_writable_calibrations.param"),
+            (wrote_non_calibrations, "non-default_writable_non-calibrations.param")]
+        self.write_zip_file(files_to_zip)
 
     def write_summary_file(self, param_dict: dict, filename: str, annotate_doc: bool):
         should_write_file = True
         if param_dict:
             if self.local_filesystem.intermediate_parameter_file_exists(filename):
                 should_write_file = messagebox.askyesno("Overwrite existing file",
                                                         f"{filename} file already exists.\nDo you want to overwrite it?")
             if should_write_file:
                 self.local_filesystem.export_to_param(param_dict, filename, annotate_doc)
                 logging_info("Summary file %s written", filename)
         return should_write_file
 
-    def write_zip_file(self, file1: bool, file2: bool, file3: bool, file4: bool):
+    def write_zip_file(self, files_to_zip: List[Tuple[bool, str]]):
         should_write_file = True
-        if True or file1 or file2 or file3 or file4:
-            zip_file_path = self.local_filesystem.zip_file_path()
-            if self.local_filesystem.zip_file_exists():
-                should_write_file = messagebox.askyesno("Overwrite existing file",
-                                                        f"{zip_file_path} file already exists.\nDo you want to overwrite it?")
-            if should_write_file:
-                self.local_filesystem.zip_files(file1, "complete.param",
-                                                file2, "non-default_read-only.param",
-                                                file3, "non-default_writable_calibrations.param",
-                                                file4, "non-default_writable_non-calibrations.param")
-                messagebox.showinfo("Parameter files zipped", "All relevant files have been zipped into the \n"
-                                    f"{zip_file_path} file.\n\nYou can now upload this file to the ArduPilot Methodic\n"
-                                    "Configuration Blog post on discuss.ardupilot.org.")
+        zip_file_path = self.local_filesystem.zip_file_path()
+        if self.local_filesystem.zip_file_exists():
+            should_write_file = messagebox.askyesno("Overwrite existing file",
+                                                    f"{zip_file_path} file already exists.\nDo you want to overwrite it?")
+        if should_write_file:
+            self.local_filesystem.zip_files(files_to_zip)
+            messagebox.showinfo("Parameter files zipped", "All relevant files have been zipped into the \n"
+                                f"{zip_file_path} file.\n\nYou can now upload this file to the ArduPilot Methodic\n"
+                                "Configuration Blog post on discuss.ardupilot.org.")
         return should_write_file
 
     def close_connection_and_quit(self):
         self.root.quit() # Then stop the Tkinter event loop
```

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/param_ftp.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/param_ftp.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/param_pid_adjustment_update.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/param_pid_adjustment_update.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator/tempcal_IMU.py` & `MethodicConfigurator-0.1.9/MethodicConfigurator/tempcal_IMU.py`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/MethodicConfigurator.egg-info/SOURCES.txt` & `MethodicConfigurator-0.1.9/MethodicConfigurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MethodicConfigurator-0.1.8/setup.py` & `MethodicConfigurator-0.1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,26 +27,37 @@
                 'pyserial>=3.0']
 
 dev_requirements = [
     'flake8',
     # Add any other development requirements here
 ]
 
+prj_url = "https://github.com/ArduPilot/MethodicConfigurator"
+
 # Read the long description from the README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
+    # Use Absolute links so that the pyPI page renders correctly
+    long_description = long_description.replace("(USERMANUAL.md", f"({prj_url}/blob/master/USERMANUAL.md")
+    long_description = long_description.replace("(CONTRIBUTING.md", f"({prj_url}/blob/master/CONTRIBUTING.md")
+    long_description = long_description.replace("(ARCHITECTURE.md", f"({prj_url}/blob/master/ARCHITECTURE.md")
+    long_description = long_description.replace("(CODE_OF_CONDUCT.md", f"({prj_url}/blob/master/CODE_OF_CONDUCT.md")
+    long_description = long_description.replace("(LICENSE.md", f"({prj_url}/blob/master/LICENSE.md")
+    long_description = long_description.replace("(credits/CREDITS.md", f"({prj_url}/blob/master/credits/CREDITS.md")
+    long_description = long_description.replace("images/App_screenshot1.png",
+                                                f"{prj_url}/raw/master/images/App_screenshot1.png")
 
 setup(
     name='MethodicConfigurator',
     version=VERSION,
     zip_safe=True,
     description='A clear configuration sequence for ArduPilot vehicles',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/ArduPilot/MethodicConfigurator',
+    url=prj_url,
     author='Amilcar do Carmo Lucas',
     author_email='amilcar.lucas@iav.de',
     packages=find_packages(),
     install_requires=[
         'pymavlink',
         'pyserial',
         'pillow',
```

