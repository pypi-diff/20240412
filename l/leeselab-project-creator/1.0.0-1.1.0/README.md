# Comparing `tmp/leeselab-project-creator-1.0.0.tar.gz` & `tmp/leeselab-project-creator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeselab-project-creator-1.0.0.tar", last modified: Wed Apr  3 06:31:08 2024, max compression
+gzip compressed data, was "leeselab-project-creator-1.1.0.tar", last modified: Fri Apr 12 06:15:57 2024, max compression
```

## Comparing `leeselab-project-creator-1.0.0.tar` & `leeselab-project-creator-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 06:31:08.202943 leeselab-project-creator-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-03-21 12:48:51.000000 leeselab-project-creator-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2744 2024-04-03 06:31:08.202943 leeselab-project-creator-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2089 2024-04-03 06:21:45.000000 leeselab-project-creator-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 06:31:08.192241 leeselab-project-creator-1.0.0/leeselab_project_creator/
--rw-rw-rw-   0        0        0        0 2024-03-19 04:55:35.000000 leeselab-project-creator-1.0.0/leeselab_project_creator/__init__.py
--rw-rw-rw-   0        0        0     6518 2024-04-02 13:26:33.000000 leeselab-project-creator-1.0.0/leeselab_project_creator/__main__.py
--rw-rw-rw-   0        0        0     6449 2024-04-03 05:55:55.000000 leeselab-project-creator-1.0.0/leeselab_project_creator/generate_plate_layout.py
--rw-rw-rw-   0        0        0     8664 2024-04-03 05:55:41.000000 leeselab-project-creator-1.0.0/leeselab_project_creator/generate_worklist.py
-drwxrwxrwx   0        0        0        0 2024-04-03 06:31:08.202943 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/
--rw-rw-rw-   0        0        0     2744 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 06:31:08.000000 leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 06:31:08.202943 leeselab-project-creator-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1002 2024-04-03 06:29:58.000000 leeselab-project-creator-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.124321 leeselab-project-creator-1.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2753 2024-04-12 06:15:57.123324 leeselab-project-creator-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2140 2024-04-12 06:06:43.000000 leeselab-project-creator-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.115331 leeselab-project-creator-1.1.0/leeselab_project_creator/
+-rw-rw-rw-   0        0        0        0 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/__init__.py
+-rw-rw-rw-   0        0        0     6518 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/__main__.py
+-rw-rw-rw-   0        0        0     6447 2024-04-12 06:10:40.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/generate_plate_layout.py
+-rw-rw-rw-   0        0        0     8707 2024-04-12 06:10:07.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/generate_worklist.py
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.123324 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/
+-rw-rw-rw-   0        0        0     2753 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 06:15:57.124321 leeselab-project-creator-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2024-04-12 06:15:30.000000 leeselab-project-creator-1.1.0/setup.py
```

### Comparing `leeselab-project-creator-1.0.0/LICENSE` & `leeselab-project-creator-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `leeselab-project-creator-1.0.0/PKG-INFO` & `leeselab-project-creator-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: leeselab-project-creator
-Version: 1.0.0
+Version: 1.1.0
 Summary: The leeselab project creator.
 Home-page: https://github.com/DominikBuchner/BOLDigger-commandline
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openpyxl>=3.1.1
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: PySimpleGUI<=4.60.5
+Requires-Dist: PySimpleGUI<=4.60.5,>=4.60.0
 
 # leeselab_project_creator
  Python script to generate plate layout lists as well as worklist for laboratory projects in the Aquatic Ecosystem Research Group.
  Automatically suggests a pooling strategy as well as optimal primer order for library generation.
 
 ## How to install and run
 Installation via pip:
 
-`pip install leeselab_project_creator`
+`pip install leeselab-project-creator`
 
 How to update:
 
-`pip install --upgrade leeselab_project_creator`
+`pip install --upgrade leeselab-project-creator`
 
 How to run:
 
-`leeselab_project_creator` or `python -m leeselab_project_creator`
+`leeselab-project-creator` or `python -m leeselab-project-creator`
 
 ## How to use
 After starting the GUI will look like this:  
 ![alt text](image-1.png)
 
 The project creator needs an Excel list with sample names as input. 
 You can set the Path to the sample list, the sheet in which it can be found as well as the cell of the first sample.
```

### Comparing `leeselab-project-creator-1.0.0/README.md` & `leeselab-project-creator-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# leeselab_project_creator
- Python script to generate plate layout lists as well as worklist for laboratory projects in the Aquatic Ecosystem Research Group.
- Automatically suggests a pooling strategy as well as optimal primer order for library generation.
-
-## How to install and run
-Installation via pip:
-
-`pip install leeselab_project_creator`
-
-How to update:
-
-`pip install --upgrade leeselab_project_creator`
-
-How to run:
-
-`leeselab_project_creator` or `python -m leeselab_project_creator`
-
-## How to use
-After starting the GUI will look like this:  
-![alt text](image-1.png)
-
-The project creator needs an Excel list with sample names as input. 
-You can set the Path to the sample list, the sheet in which it can be found as well as the cell of the first sample.
-Select between 1 and 500 extraction replicates.
-Select between 1 and 500 PCR replicates.
-Select what primers to use, seperated by comma (e.g. fwh2, rbcl, 16S).
-Select which 1st step primer tags are available for the primer sets, seperated by comma (e.g. 1,2,3,4,5,6,7,8).
-Enter a project name and select a folder where to save the plate layout.
-Hit "Generate sample list".
-
-## Example
-As an example sample list a list with 12 samples was selected:  
-![alt text](image.png)  
-
-The example setup looks like this when it is completly filled:  
-![alt text](image-2.png)  
-
-The project creator will generate a plate layout according to the settings.
-This will include the technical replicates to control for cross-contamination as well as the selected amount of extraction replicates (indicated by _1, _2 ...)
-
-![alt text](image-3.png)
-
-Two more sheet will be generated, the extraction worklist and the PCR worklist:
-![alt text](image-4.png)
-
-In the PCR worklist a pooling strategy for the librarys will be calculated as well as an optimal use of primers to maximize library diversity.
-The selected PCR replicates will be generated as seperate plates in the PCR worklist.
-![alt text](image-5.png)
-
-All sheets can be printed and taken into the lab to document all required data to sufficiently describe the analysis in the end.
-
+# leeselab_project_creator
+ Python script to generate plate layout lists as well as worklist for laboratory projects in the Aquatic Ecosystem Research Group.
+ Automatically suggests a pooling strategy as well as optimal primer order for library generation.
+
+## How to install and run
+Installation via pip:
+
+`pip install leeselab-project-creator`
+
+How to update:
+
+`pip install --upgrade leeselab-project-creator`
+
+How to run:
+
+`leeselab-project-creator` or `python -m leeselab-project-creator`
+
+## How to use
+After starting the GUI will look like this:  
+![alt text](image-1.png)
+
+The project creator needs an Excel list with sample names as input. 
+You can set the Path to the sample list, the sheet in which it can be found as well as the cell of the first sample.
+Select between 1 and 500 extraction replicates.
+Select between 1 and 500 PCR replicates.
+Select what primers to use, seperated by comma (e.g. fwh2, rbcl, 16S).
+Select which 1st step primer tags are available for the primer sets, seperated by comma (e.g. 1,2,3,4,5,6,7,8).
+Enter a project name and select a folder where to save the plate layout.
+Hit "Generate sample list".
+
+## Example
+As an example sample list a list with 12 samples was selected:  
+![alt text](image.png)  
+
+The example setup looks like this when it is completly filled:  
+![alt text](image-2.png)  
+
+The project creator will generate a plate layout according to the settings.
+This will include the technical replicates to control for cross-contamination as well as the selected amount of extraction replicates (indicated by _1, _2 ...)
+
+![alt text](image-3.png)
+
+Two more sheet will be generated, the extraction worklist and the PCR worklist:
+![alt text](image-4.png)
+
+In the PCR worklist a pooling strategy for the librarys will be calculated as well as an optimal use of primers to maximize library diversity.
+The selected PCR replicates will be generated as seperate plates in the PCR worklist.
+![alt text](image-5.png)
+
+All sheets can be printed and taken into the lab to document all required data to sufficiently describe the analysis in the end.
+
```

### Comparing `leeselab-project-creator-1.0.0/leeselab_project_creator/__main__.py` & `leeselab-project-creator-1.1.0/leeselab_project_creator/__main__.py`

 * *Files identical despite different names*

### Comparing `leeselab-project-creator-1.0.0/leeselab_project_creator/generate_plate_layout.py` & `leeselab-project-creator-1.1.0/leeselab_project_creator/generate_plate_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     # add tube order
     tube_order = dict(zip(alpha, tube_order + tube_order))
     out_df["Lysis\ntube"] = out_df["Lysis,\nExtraction,\nPCR Well"].map(tube_order)
 
     # add tagging primers
     alpha = dict(zip(alpha, range(1, 97)))
-    out_df["Aliquotiert"] = ""
+    out_df["aliquoted"] = ""
     out_df["Primer\n2nd PCR"] = out_df["Lysis,\nExtraction,\nPCR Well"].map(alpha)
     out_df["Notes"] = ""
     out_df = out_df.reset_index(names="#")
     out_df["#"] = out_df["#"] + 1
 
     # create a temporary save before doing some styling
     savename = "{}_plate_layout.xlsx".format(project_name)
```

### Comparing `leeselab-project-creator-1.0.0/leeselab_project_creator/generate_worklist.py` & `leeselab-project-creator-1.1.0/leeselab_project_creator/generate_worklist.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         "{} - {}".format(primer_name, primer_number) for primer_number in primers
     ]
 
     output_worklist["tagging primer"] = primers
     output_worklist["1st pcr"] = ""
     output_worklist["clean up"] = ""
     output_worklist["2nd pcr"] = ""
+    output_worklist["gel 2nd pcr"] = ""
     output_worklist["normalization"] = ""
     output_worklist["pooling"] = ""
 
     return (
         output_worklist,
         starting_library_number,
         plates_per_library,
@@ -257,21 +258,21 @@
         top=Side(style="thin"),
         bottom=Side(style="thin"),
     )
 
     fill = PatternFill(start_color="00C0C0C0", end_color="00C0C0C0", fill_type="solid")
 
     for row in range(2, ws.max_row + 1):
-        for col in range(1, 9):
+        for col in range(1, 10):
             ws.cell(row=row, column=col).border = thin_border
             if row % 2 == 0:
                 ws.cell(row=row, column=col).fill = fill
 
     # merge cells where steps are executed together
-    for col in range(7, 9):
+    for col in range(8, 10):
         for row in range(3, ws.max_row + 1, plates_per_library):
             ws.merge_cells(
                 start_row=row,
                 end_row=row + plates_per_library - 1,
                 start_column=col,
                 end_column=col,
             )
```

### Comparing `leeselab-project-creator-1.0.0/leeselab_project_creator.egg-info/PKG-INFO` & `leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: leeselab-project-creator
-Version: 1.0.0
+Version: 1.1.0
 Summary: The leeselab project creator.
 Home-page: https://github.com/DominikBuchner/BOLDigger-commandline
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openpyxl>=3.1.1
 Requires-Dist: pandas>=1.5.3
-Requires-Dist: PySimpleGUI<=4.60.5
+Requires-Dist: PySimpleGUI<=4.60.5,>=4.60.0
 
 # leeselab_project_creator
  Python script to generate plate layout lists as well as worklist for laboratory projects in the Aquatic Ecosystem Research Group.
  Automatically suggests a pooling strategy as well as optimal primer order for library generation.
 
 ## How to install and run
 Installation via pip:
 
-`pip install leeselab_project_creator`
+`pip install leeselab-project-creator`
 
 How to update:
 
-`pip install --upgrade leeselab_project_creator`
+`pip install --upgrade leeselab-project-creator`
 
 How to run:
 
-`leeselab_project_creator` or `python -m leeselab_project_creator`
+`leeselab-project-creator` or `python -m leeselab-project-creator`
 
 ## How to use
 After starting the GUI will look like this:  
 ![alt text](image-1.png)
 
 The project creator needs an Excel list with sample names as input. 
 You can set the Path to the sample list, the sheet in which it can be found as well as the cell of the first sample.
```

### Comparing `leeselab-project-creator-1.0.0/setup.py` & `leeselab-project-creator-1.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leeselab-project-creator",
-    version="1.0.0",
+    version="1.1.0",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="The leeselab project creator.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/BOLDigger-commandline",
     packages=setuptools.find_packages(),
     license="MIT",
-    install_requires=["openpyxl>=3.1.1", "pandas>=1.5.3", "PySimpleGUI<=4.60.5"],
+    install_requires=[
+        "openpyxl>=3.1.1",
+        "pandas>=1.5.3",
+        "PySimpleGUI >= 4.60.0, <=4.60.5",
+    ],
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

