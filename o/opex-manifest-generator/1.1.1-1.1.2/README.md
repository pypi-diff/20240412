# Comparing `tmp/opex_manifest_generator-1.1.1.tar.gz` & `tmp/opex_manifest_generator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.1.tar", last modified: Fri Apr  5 13:57:01 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.2.tar", last modified: Fri Apr 12 13:12:32 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.1.tar` & `opex_manifest_generator-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.595410 opex_manifest_generator-1.1.1/opex_manifest_generator/
--rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6190 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/hash.py
--rw-rw-rw-   0        0        0    25427 2024-04-05 13:55:47.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest.py
--rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest_reference.py
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-05 08:23:42.000000 opex_manifest_generator-1.1.1/opex_manifest_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-05 13:57:01.000000 opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      819 2024-04-05 08:25:10.000000 opex_manifest_generator-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 13:57:01.642300 opex_manifest_generator-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.138027 opex_manifest_generator-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.2/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-04-12 13:12:32.135662 opex_manifest_generator-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.092160 opex_manifest_generator-1.1.2/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6050 2024-04-12 13:08:38.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/hash.py
+-rw-rw-rw-   0        0        0    27307 2024-04-12 13:07:29.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0    20008 2024-03-26 21:35:58.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest_reference.py
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/test_cli.py
+-rw-rw-rw-   0        0        0       21 2024-04-12 13:09:20.000000 opex_manifest_generator-1.1.2/opex_manifest_generator/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:12:32.133647 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-12 13:12:31.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 13:12:32.000000 opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      864 2024-04-12 13:09:27.000000 opex_manifest_generator-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:12:32.139025 opex_manifest_generator-1.1.2/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.1/LICENSE.md` & `opex_manifest_generator-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.1/PKG-INFO` & `opex_manifest_generator-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.1/README.md` & `opex_manifest_generator-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.2/opex_manifest_generator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 def parse_args():
     parser = argparse.ArgumentParser(description="OPEX Manifest Generator for Preservica Uploads")
     parser.add_argument('root',default=os.getcwd())
     parser.add_argument("-c","--autoclass",required=False,choices=['catalog','c','accession','a','both','b','generic','g','catalog-generic','cg',"accession-generic","ag","both-generic","bg"],type=str.lower)
     parser.add_argument("-p","--prefix",required=False, nargs='+')
     parser.add_argument("-fx","--fixity",required=False,const="SHA-1",default=None, nargs='?', choices=['NONE','SHA-1','MD5','SHA-256','SHA-512'],type=str.upper)
     parser.add_argument("-rme","--remove-empty",required=False,action='store_true',default=False)
-    parser.add_argument("-f","--force",required=False,action='store_true',default=False)
     parser.add_argument("-o","--output",required=False,nargs=1)
     parser.add_argument("-clr","--clear-opex",required=False,action='store_true',default=False)
     parser.add_argument("-s","--start-ref",required=False,nargs='?',default=1)
     parser.add_argument("-m","--metadata",required=False,const='e',default='none',nargs='?',choices=['none','n','exact','e','flat','f'],type=str.lower)
     parser.add_argument("-dmd", "--disable-meta-dir",required=False,action='store_false')
     parser.add_argument("-ex","--export",required=False,action='store_true',default=False)
     parser.add_argument("-i","--input",required=False)
@@ -99,15 +98,14 @@
         if not i.lower() == "y": print("Closing program..."); time.sleep(3); raise SystemExit()
     time.sleep(3)
     OpexManifestGenerator(root=args.root,
                           output_path=args.output,
                           autoclass_flag=args.autoclass,
                           prefix=args.prefix,
                           acc_prefix=acc_prefix,
-                          force_flag=args.force,
                           empty_flag=args.remove_empty,
                           remove_flag=args.remove,
                           clear_opex_flag=args.clear_opex,
                           algorithm = args.fixity,
                           startref=args.start_ref,
                           export_flag=args.export,
                           meta_dir_flag=args.disable_meta_dir,
```

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.2/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.2/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.2/opex_manifest_generator/opex_manifest_reference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 """
 Opex Manifest Generator tool
 
 This tool is utilised to recusrively generate Opex files for files / directories for use in uploading to Preservica and other OPEX conformin systems.
 
 author: Christopher Prince
 license: Apache License 2.0"
@@ -14,234 +15,160 @@
 from datetime import datetime
 import time
 import pandas as pd
 from pandas.api.types import is_datetime64_any_dtype
 from opex_manifest_generator.hash import HashGenerator
 from opex_manifest_generator.common import *
 import stat
-import shutil
 
 class OpexManifestGenerator():
     def __init__(self,
                  root,
                  output_path=os.getcwd(),
                  meta_dir_flag=True,
                  metadata_dir=os.path.join(os.path.dirname(os.path.realpath(__file__)), "metadata"),
                  metadata_flag='none',
                  autoclass_flag=False,
-                 prefix=None,
-                 acc_prefix=None,
+                 prefix=False,
                  startref=1,
-                 algorithm=None,
+                 fixity_flag=False,
+                 algorithm=False,
                  empty_flag=False,
                  force_flag=False,
-                 remove_flag=False,
                  clear_opex_flag=False,
                  export_flag=False,
                  input=False,
                  zip_flag=False,
-                 hidden_flag=False,
                  output_format="xlsx"):
         
         self.root = os.path.abspath(root)
         self.opexns = "http://www.openpreservationexchange.org/opex/v1.2"        
         self.list_path = []
         self.list_fixity = []
         self.start_time = datetime.now()
-        self.algorithm = algorithm
+        self.fixity_flag = fixity_flag
         self.empty_flag = empty_flag
-        self.remove_flag = remove_flag
         self.export_flag = export_flag
         self.startref = startref
         self.autoclass_flag = autoclass_flag
         self.force_flag = force_flag
         self.output_path = output_path
         self.clear_opex_flag = clear_opex_flag
         self.meta_dir_flag = meta_dir_flag
         self.prefix = prefix
-        self.acc_prefix = acc_prefix
+        self.algorithm = algorithm
         self.input = input
         self.title_flag = False
         self.description_flag = False
         self.security_flag = False
-        self.ignore_flag = False
-        self.sourceid_flag = False
-        self.hash_from_spread = False        
-        self.hidden_flag = hidden_flag
         self.zip_flag = zip_flag
         self.output_format = output_format
         self.metadata_flag = metadata_flag
         self.metadata_dir = metadata_dir
         
     def print_running_time(self):
         print(f'Running time: {datetime.now() - self.start_time}')
         time.sleep(1)
     
     def meta_df_lookup(self,file_path: str):
         idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty:
+        try:
+            if self.title_flag:
+                title = self.df.loc[idx].Title.item()
+                if str(title) == "nan": title = None
+            else: title = None
+            if self.description_flag: 
+                description = self.df.loc[idx].Description.item()
+                if str(description) == "nan": description = None
+            else: description = None
+            if self.security_flag: 
+                security = self.df.loc[idx].Security.item()
+                if str(security) == "nan": security = None
+            else: security = None
+        except Exception as e:
+            print(e)
             title = None
             description = None
             security = None
-        else:
-            try:
-                if self.title_flag:
-                    title = self.df['Title'].loc[idx].item()
-                    if str(title).lower() in {"nan","nat"}: title = None
-                else: title = None
-                if self.description_flag: 
-                    description = self.df['Description'].loc[idx].item()
-                    if str(description).lower() in {"nan","nat"}: description = None
-                else: description = None
-                if self.security_flag: 
-                    security = self.df['Security'].loc[idx].item()
-                    if str(security).lower() in {"nan","nat"}: security = None
-                else: security = None
-            except Exception as e:
-                print(e)
-                raise SystemError()
         return title,description,security
     
-    def remove_df_lookup(self,file_path: str):
-        idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: return False
-        else:
-            remove = self.df['Removals'].loc[idx].item()
-            if str(remove).lower() in {"nan","nat"}: return False
-            elif bool(remove):
-                print(f"Removing: {file_path}")
-                # Not functioning correctly
-                if os.path.isdir(file_path): shutil.rmtree(dir)
-                else: os.remove(file_path)
-                return True
-            else: return False
-                
-    def ignore_df_lookup(self,file_path: str):
-        idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: return False
-        else: ignore = self.df['Ignore'].loc[idx].item()
-        if str(ignore).lower() in {"nan","nat"}: return False
-        elif str(ignore).lower() in {"true"}: return True
-        else: return False
+    def ignore_remove_df_lookup(self,file_path):
+        pass
 
-    def sourceid_df_lookup(self,xml_element,file_path):
+    def ident_df_lookup(self,file_path,code_name="code",accession_flag=None):
         idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: pass
+        if idx.empty: reference = "ERROR"
+        else: 
+            if accession_flag:
+                reference = self.df.loc[idx].Accession_Reference.item()
+            else: 
+                reference = self.df.loc[idx].Archive_Reference.item()
+        if isinstance(reference,float): pass
         else:
-            sourceid = self.df['SourceID'].loc[idx].item()
-            if str(sourceid) in {"nan","nat"}: pass
-            else:
-                source_xml = ET.SubElement(xml_element,f"{{{self.opexns}}}SourceID")
-                source_xml.text = str(sourceid)
+            self.identifier.text = reference
+            self.identifier.set("type",code_name)
 
-    def hash_df_lookup(self,file_path,xml_fixities):
-        idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: pass
-        else:
-            if "Hash" in self.column_headers and "Algorithm" in self.column_headers:
-                self.fixity = ET.SubElement(xml_fixities,f"{{{self.opexns}}}Fixity")        
-                self.hash = self.df["Hash"].loc[idx].item()
-                self.algorithm = self.df["Algorithm"].loc[idx].item()
-                self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
-                self.fixity.set("type", self.algorithm)
-                self.fixity.set("value",self.hash)
-            else: pass
+        column_headers = self.df.columns.values.tolist()
+        for header in column_headers:
+            if 'Identifier' in header:
+                #self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
+                #reference = self.df[header].loc[idx].item()
+                #print(reference)
+                #code_name = str(header).rsplit[':'][-1]        
+                #print(header)
+                pass
 
-    def ident_df_lookup(self,file_path):
-        idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty:
-            ident = "ERROR"
-            self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
-            self.identifier.set("type","code")
-            self.identifier.text = ident
-        else:
-            for header in self.column_headers:
-                if any(s in header for s in {'Identifier','Archive_Reference','Accession_Reference'}):
-                    ident = self.df[header].loc[idx].item()
-                    if 'Identifier:' in header: code_name = str(header).rsplit(':')[-1]
-                    elif 'Archive_Reference' in header: code_name = "code"
-                    elif 'Accession_Reference' in header: code_name = "accref"
-                else: ident = None
-                if str(ident).lower() in {"nan","nat"} or not ident: pass
-                else:
-                    self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
-                    self.identifier.set("type",code_name)
-                    self.identifier.text = str(ident)
-        
     def write_opex(self,file_path,opexxml):
         opex_path = str(file_path) + ".opex"
-        if os.path.exists(opex_path):
-            print(f"Opex exists: {opex_path}: Avoiding override")
+        if os.path.exists(opex_path) and not self.force_flag:
+            print(f"Opex exists: {opex_path}, but force option is not set: Avoiding override")
             pass
         else:
             opex = ET.indent(opexxml,"  ")
             opex = ET.tostring(opexxml,pretty_print=True,xml_declaration=True,encoding="UTF-8",standalone=True)
             with open(f'{opex_path}','w',encoding="UTF-8") as writer:
                 writer.write(opex.decode('UTF-8'))
-                #if self.force_flag and os.path.exists(opex_path): print(f"Force Option Set. Forcing Override to: {opex_path}")
-                print('Saved Opex File to: ' + opex_path)
+                if self.force_flag and os.path.exists(opex_path): print(f"Force Option Set. Forcing Override to: {opex_path}")
+                else: print('Saved Opex File to: ' + opex_path)
         return opex_path
 
     def init_df(self):
         if self.autoclass_flag:
             if self.autoclass_flag in {"catalog","c","catalog-generic","cg"}:
                 ac = ClassificationGenerator(self.root,output_path=self.output_path,prefix=self.prefix,start_ref=self.startref,empty_flag=self.empty_flag,accession_flag=False)
+                self.df = ac.init_dataframe()
             elif self.autoclass_flag in {"accession","a","accession-generic","ag","both","b","both-generic","bg"}:
-                ac = ClassificationGenerator(self.root,output_path=self.output_path,prefix=self.prefix,accprefix=self.acc_prefix,start_ref=self.startref,empty_flag=self.empty_flag,accession_flag="File")
-            self.df = ac.init_dataframe()
-            if self.autoclass_flag in {"accession","a","accesion-generic","ag"}:
-                self.df = self.df.drop('Archive_Reference',axis=1)
-            self.column_headers = self.df.columns.values.tolist()
+                ac = ClassificationGenerator(self.root,output_path=self.output_path,prefix=self.prefix,accprefix=prefix_acc,start_ref=self.startref,empty_flag=self.empty_flag,accession_flag="File")
+                self.df = ac.init_dataframe()
             if self.export_flag:
                 output_path = define_output_file(self.output_path,self.root,meta_dir_flag=self.meta_dir_flag,output_format=self.output_format)                
                 if self.output_format == "xlsx": export_xl(self.df,output_path)
                 elif self.output_format == "csv": export_csv(self.df,output_path)
         elif self.input:
             if self.input.endswith('xlsx'): self.df = pd.read_excel(self.input)
             elif self.input.endswith('csv'): self.df = pd.read_csv(self.input)
-            self.column_headers = self.df.columns.values.tolist()
-            self.set_flags()
+            self.parse_input_df()
         else:
             self.df = None
-            self.column_headers = None
                 
     def clear_opex(self):
         walk = list(os.walk(self.root))
         for dir,_,files in walk[::-1]:
             for file in files:
                 file_path = win_256_check(os.path.join(dir,file))   
                 if str(file_path).endswith('.opex'):
                     os.remove(file_path)
-                    print(f'Cleared Opex: {file_path}')
+                    print(f'Removed: {file_path}') #fileprint(os.path.join(d,sd,f))
     
-    def set_flags(self):
+    def parse_input_df(self):
         if 'Title' in self.df: self.title_flag = True
         if 'Description' in self.df: self.description_flag = True
         if 'Security' in self.df: self.security_flag = True
-        if 'SourceID' in self.df: self.sourceid_flag = True
-        if 'Ignore' in self.df: self.ignore_flag = True
-        if 'Hash' in self.df and 'Algorithm' in self.df:
-            self.hash_from_spread = True
-            print("Hash detected in Spreadsheet; taking hashes from spreadsheet");time.sleep(3)
-
-    def print_descriptive_xmls(self):
-        for file in os.listdir(self.metadata_dir):
-            path = os.path.join(self.metadata_dir,file)
-            print(path)
-            xml_file = ET.parse(path)
-            root_element = ET.QName(xml_file.find('.'))
-            root_element_ln = root_element.localname
-            for elem in xml_file.findall(".//"):
-                elem_path = xml_file.getelementpath(elem)
-                elem = ET.QName(elem)
-                elem_lnpath = elem_path.replace(f"{{{elem.namespace}}}",root_element_ln + ":")
-                print(elem_lnpath)
-
-    def init_generate_descriptive_metadata(self):
-        self.xml_files = []
+        
+    def generate_descriptive_metadata(self,xml_descmeta,file_path):
         for file in os.listdir(self.metadata_dir):
             if file.endswith('xml'):
                 """
                 Generates info on the elements of the XML Files placed in the Metadata directory.
                 Composed as a list of dictionaries.
                 """
                 path = os.path.join(self.metadata_dir,file)
@@ -253,226 +180,194 @@
                 for elem in xml_file.findall('.//'):
                     elem_path = xml_file.getelementpath(elem)
                     elem = ET.QName(elem)
                     elem_ln = elem.localname
                     elem_ns = elem.namespace
                     elem_lnpath = elem_path.replace(f"{{{elem_ns}}}",root_element_ln + ":")
                     elements_list.append({"Name":root_element_ln + ":" + elem_ln,"Namespace":elem_ns,"Path":elem_lnpath})
+                list_xml = []
 
                 """
                 Compares the column headers in the Spreadsheet against the headers. Filters out non-matching data.
                 """
-                list_xml = []
+                column_headers = self.df.columns.values.tolist()
                 for elem_dict in elements_list:
-                    if elem_dict.get('Name') in self.column_headers or elem_dict.get('Path') in self.column_headers:
+                    if elem_dict.get('Name') in column_headers or elem_dict.get('Path') in column_headers:
                         list_xml.append({"Name":elem_dict.get('Name'),"Namespace":elem_dict.get('Namespace'),"Path":elem_dict.get('Path')})
-            if len(list_xml) > 0:
-                self.xml_files.append({'data':list_xml, 'localname':root_element_ln, 'xmlfile': path})
-
-    def generate_descriptive_metadata(self,xml_desc,file_path):
-        for xml_file in self.xml_files:
-            list_xml = xml_file.get('data')
-            localname = xml_file.get('localname')
-            """
-            Composes the data into an xml file.
-            """
-            if len(list_xml):
-                idx = self.df.index[self.df['FullName'] == file_path]
-                if not idx.empty:
-                    xml_new = ET.parse(xml_file.get('xmlfile'))
+                """
+                Composes the data into an xml file.
+                """
+                if len(list_xml):
+                    idx = self.df.index[self.df['FullName'] == file_path]
+                    xml_new = xml_file
                     for elem_dict in list_xml:
                         name = elem_dict.get('Name')
                         path = elem_dict.get('Path')
                         ns = elem_dict.get('Namespace')
-                        try:
-                            if self.metadata_flag in {'e','exact'}: val = self.df.loc[idx,path].values[0]
-                            elif self.metadata_flag in {'f','flat'}: val = self.df.loc[idx,name].values[0]
-                            if pd.isnull(val): continue
+                        if self.metadata_flag in {'e','exact'}:
+                            try: 
+                                print(file_path)
+                                val = self.df.loc[idx,path].values[0]
+                            except KeyError as e:
+                                print('Key Error: please ensure column header\'s are an exact match...')
+                                print(f'Missing Column: {e}')
+                                print('Alternatively use flat mode...')
+                                time.sleep(5)
+                                raise SystemError()
+                            if str(val) == "nan": val = ""
+                            n = path.replace(root_element_ln + ":", f"{{{ns}}}")
+                            elem = xml_new.find(f'/{n}')
+                            elem.text = str(val)
+                        elif self.metadata_flag in {'f','flat'}:
+                            val = self.df.loc[idx,name].values[0]
+                            if pd.isnull(val): val = ""
                             else:
                                 if is_datetime64_any_dtype(val):
                                     val = pd.to_datetime(val)
                                     val = datetime.strftime(val,"%Y-%m-%dT%H-%M-%S.00Z")
-                        except KeyError as e:
-                            print('Key Error: please ensure column header\'s are an exact match...')
-                            print(f'Missing Column: {e}')
-                            print('Alternatively use flat mode...')
-                            time.sleep(5)
-                            raise SystemError()
-                        except IndexError as e:
-                            print("""Index Error; it is likely you have removed or added a file/folder to the directory \
-                                after generating the spreadsheet. An opex will still be generated but with no xml metadata. \
-                                To ensure metadata match up please regenerate the spreadsheet...""")
-                            print(f'Error: {e}')
-                            time.sleep(1)
-                            break
-                        if str(val).lower() in {"nan","nat"}: continue
-                        if self.metadata_flag in {'e','exact'}:
-                            n = path.replace(localname + ":", f"{{{ns}}}")
-                            elem = xml_new.find(f'/{n}')
-                        elif self.metadata_flag in {'f','flat'}:
+                            if str(val) == "nan": val = ""
                             n = name.split(':')[-1]
                             elem = xml_new.find(f'//{{{ns}}}{n}')
-                        elem.text = str(val)    
-                    xml_desc.append(xml_new.find('.'))
-                else: pass
-            else: pass
-
-    def generate_opex_properties(self,xmlroot,file_path,title=None,description=None,security=None):
-        self.properties = ET.SubElement(xmlroot,f"{{{self.opexns}}}Properties")
-        self.identifiers = ET.SubElement(self.properties,f"{{{self.opexns}}}Identifiers")
-        if title:
-            self.titlexml = ET.SubElement(self.properties,f"{{{self.opexns}}}Title")
-            self.titlexml.text = str(title)
-        if description:
-            self.descriptionxml = ET.SubElement(self.properties,f"{{{self.opexns}}}Description")
-            self.descriptionxml.text = str(description)      
-        if security:
-            self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
-            self.securityxml.text = str(security)
-        if self.autoclass_flag in {"generic","g"}:
-            self.properties.remove(self.identifiers)
-        elif self.autoclass_flag or self.input:
-            self.ident_df_lookup(file_path)
-        if self.identifiers is None: self.properties.remove(self.identifiers)
-        if self.properties is None: xmlroot.remove(self.properties)
+                            elem.text = str(val)
+                    xml_descmeta.append(xml_new.find('.'))
 
+    def generate_opex_properties(self,xmlroot,file_path,title=None,description=None,security=None,code="code"):
+            self.properties = ET.SubElement(xmlroot,f"{{{self.opexns}}}Properties")
+            self.identifiers = ET.SubElement(self.properties,f"{{{self.opexns}}}Identifiers")
+            self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier")           
+            if title:
+                self.titlexml = ET.SubElement(self.properties,f"{{{self.opexns}}}Title")
+                self.titlexml.text = str(title)
+            if description:
+                self.descriptionxml = ET.SubElement(self.properties,f"{{{self.opexns}}}Description")
+                self.descriptionxml.text = str(description)      
+            if security:
+                self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
+                self.securityxml.text = str(security)
+            if self.autoclass_flag in {"catalog","c","catalog-generic","cg"}:
+                self.ident_df_lookup(file_path,code_name=code)
+            elif self.autoclass_flag in {"accession","a","accession-generic","ag"}:
+                self.ident_df_lookup(file_path,accession_flag=True)
+            elif self.autoclass_flag in {"both","b","both-generic","bg"}:
+                self.ident_df_lookup(file_path,code_name=code)
+                self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier")           
+                self.ident_df_lookup(file_path,code_name="accref",accession_flag=True)
+            elif self.autoclass_flag in {"generic","g"}:
+                self.properties.remove(self.identifiers)
+            elif self.input:
+                self.ident_df_lookup(file_path)                
 
-    def genererate_opex_fixity(self,file_path):
+    def genererate_opex_fixity(self):
         self.fixity = ET.SubElement(self.fixities,f"{{{self.opexns}}}Fixity")        
-        self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
+        self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(self.file_path) # Double Check...
         self.fixity.set("type", self.algorithm)
         self.fixity.set("value",self.hash)
-        self.OMG.list_fixity.append([self.algorithm,self.hash,file_path])
-        self.OMG.list_path.append(file_path)
+        self.OMG.list_fixity.append([self.algorithm,self.hash,self.file_path])
+        self.OMG.list_path.append(self.file_path)        
 
     def main(self):
         print(f"Start time: {self.start_time}")        
         if self.clear_opex_flag:
             self.clear_opex()
-            if self.autoclass_flag or self.algorithm or self.input: pass
+            if self.autoclass_flag or self.fixity_flag or self.force_flag or self.input: pass
             else: 
                 self.print_running_time()
                 print('Cleared OPEXES. No additional arguments passed, so ending program.'); time.sleep(3)
                 raise SystemExit()
         if self.empty_flag:
             ClassificationGenerator(self.root,self.output_path,meta_dir_flag=self.meta_dir_flag).remove_empty_directories()
         self.init_df()
         self.count = 1
-        if not self.metadata_flag in {'none','n'}: self.init_generate_descriptive_metadata()
         OpexDir(self,self.root).generate_opex_dirs(self.root)
-        if self.algorithm:
+        if self.fixity_flag:
             output_path = define_output_file(self.output_path,self.root,self.meta_dir_flag,output_suffix="_Fixities",output_format="txt")
             export_list_txt(self.list_fixity,output_path)
         self.print_running_time()
 
+
 class OpexDir(OpexManifestGenerator):
     def __init__(self,OMG,folder_path,title=None,description=None,security=None):
         self.OMG = OMG
         self.root = self.OMG.root
-        self.opexns = self.OMG.opexns
-        if folder_path.startswith(u'\\\\?\\'): self.folder_path = folder_path.replace(u'\\\\?\\',"")
-        else: self.folder_path = folder_path
-        if self.OMG.ignore_flag: 
-            self.ignore = self.OMG.ignore_df_lookup(folder_path)
-            if self.ignore: return
-        else: self.ignore = False
+        self.opexns = self.OMG.opexns        
+        self.folder_path = win_256_check(folder_path)
         self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
         self.transfer = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}Transfer")
-        if self.OMG.sourceid_flag:
-            self.OMG.sourceid_df_lookup(self.transfer,self.folder_path)
         self.manifest = ET.SubElement(self.transfer,f"{{{self.opexns}}}Manifest")
         self.folders = ET.SubElement(self.manifest,f"{{{self.opexns}}}Folders")
         self.files = ET.SubElement(self.manifest,f"{{{self.opexns}}}Files")
         if self.OMG.autoclass_flag in {"generic","g","catalog-generic","cg","accession-generic","ag","both-generic","bg"}:
             self.title = os.path.basename(self.folder_path)
             self.description = os.path.basename(self.folder_path)
             self.security = "open"
         else:
             self.title = title
             self.description = description
             self.security = security
         if self.OMG.autoclass_flag or self.OMG.input:
-            if self.OMG.remove_flag:
-                removal = self.OMG.remove_df_lookup(self.folder_path)
-                if removal: return
             self.OMG.generate_opex_properties(self.xmlroot,self.folder_path,title=self.title,description=self.description,security=self.security)
             if not self.OMG.metadata_flag in {'none','n'}:
                 self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
-                self.OMG.generate_descriptive_metadata(self.xmlroot,self.folder_path)
-
+                self.OMG.generate_descriptive_metadata(self.xml_descmeta,self.folder_path)
+    
     def filter_directories(self,directory):    #Sorts the list Alphabetically and Ignores: 1. Hidden Directories starting with '.', 2. '.opex' files, 3. Folders titled 'meta', 4. Script file 5. Output file. 
-        if not self.OMG.hidden_flag:
-            list_directories = sorted([os.path.join(directory,f) for f in os.listdir(directory) \
-                if not f.startswith('.') \
-                and not bool(os.stat(os.path.join(directory,f)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN) \
-                and f != 'meta'\
-                and f != os.path.basename(__file__)],key=str.casefold)
-        else:
-            list_directories = sorted([os.path.join(directory,f) for f in os.listdir(directory) \
-                if f != 'meta' \
-                and f != os.path.basename(__file__)],key=str.casefold)
+        list_directories = sorted([win_256_check(os.path.join(directory,f)) for f in os.listdir(directory) \
+        if not f.startswith('.') \
+        and f != 'meta'\
+        and f != os.path.basename(__file__) \
+        and not f.endswith('_AutoClass.xlsx') and not f.endswith('_autoclass.xlsx')\
+        and not f.endswith('_EmptyDirectoriesRemoved.txt')],key=str.casefold)
         return list_directories
         
     def generate_opex_dirs(self,file_path):
+        os.chdir(file_path)
         if self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag: self.title,self.description,self.security = self.OMG.meta_df_lookup(file_path) 
         self = OpexDir(self.OMG,file_path,title=self.title,description=self.description,security=self.security)
         for f in self.filter_directories(file_path):
             if f.endswith('.opex'):
                 pass
             elif os.path.isdir(f):
-                if not self.ignore:
-                    self.folder = ET.SubElement(self.folders,f"{{{self.opexns}}}Folder")
-                    self.folder.text = str(os.path.basename(f))
+                self.folder = ET.SubElement(self.folders,f"{{{self.opexns}}}Folder")
+                self.folder.text = str(os.path.basename(f))
                 self.generate_opex_dirs(f)
             else:
                 OpexFile(self.OMG,f,self.OMG.algorithm)
-        if not self.ignore:
-            for f in self.filter_directories(file_path):                         # Creates the files element of the Opex Manifest.
+        
+        for f in self.filter_directories(file_path):                         # Creates the files element of the Opex Manifest.
                 if os.path.isfile(f):
                     file = ET.SubElement(self.files,f"{{{self.opexns}}}File")
                     if f.endswith('.opex'): file.set("type","metadata")
                     else:
                         file.set("type","content")
                         file.set("size",str(os.path.getsize(f)))
                     file.text = str(os.path.basename(f))
-            opex_path = os.path.join(os.path.abspath(self.folder_path),os.path.basename(self.folder_path))
-            self.OMG.write_opex(opex_path,self.xmlroot)
+                #self.count += 1
+        opex_path = os.path.join(os.path.abspath(self.folder_path),os.path.basename(self.folder_path))
+        self.OMG.write_opex(opex_path,self.xmlroot)
 
 class OpexFile(OpexManifestGenerator):
     def __init__(self,OMG,file_path,algorithm="SHA-1",title=None,description=None,security=None):
         self.OMG = OMG
         self.opexns = self.OMG.opexns  
-        if file_path.startswith(u'\\\\?\\'): self.file_path = file_path.replace(u'\\\\?\\',"")
-        else: self.file_path = file_path
-        if self.OMG.ignore_flag: 
-            self.ignore = self.OMG.ignore_df_lookup(file_path)
-            if self.ignore: return
-        else: self.ignore = False
+        self.file_path = win_256_check(file_path)
         self.algorithm = algorithm
         if self.OMG.autoclass_flag in {"generic","g","catalog-generic","cg","accession-generic","ag","both-generic","bg"}:
             self.title = os.path.splitext(os.path.basename(self.file_path))[0]
             self.description = os.path.splitext(os.path.basename(self.file_path))[0]
             self.security = "open"
         else:
             self.title = title
             self.description = description
             self.security = security
-        if self.OMG.algorithm or self.OMG.autoclass_flag or self.OMG.input:
-            if self.OMG.remove_flag:
-                removal = self.OMG.remove_df_lookup(self.file_path)
-                if removal: return
+        if self.OMG.fixity_flag or self.OMG.autoclass_flag or self.OMG.input:
             self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
-            if self.OMG.algorithm or self.OMG.sourceid_flag:
+            if self.OMG.fixity_flag:
                 self.transfer = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}Transfer")
-                if self.OMG.sourceid_flag:
-                    self.OMG.sourceid_df_lookup(self.transfer,self.file_path)
-                if self.OMG.algorithm:
-                    self.fixities = ET.SubElement(self.transfer,f"{{{self.opexns}}}Fixities")
-                    if self.OMG.hash_from_spread: self.OMG.hash_df_lookup(self.file_path,self.fixities)  
-                    else: self.genererate_opex_fixity(self.file_path)            
+                self.fixities = ET.SubElement(self.transfer,f"{{{self.opexns}}}Fixities")
+                self.genererate_opex_fixity()            
             if self.OMG.autoclass_flag or self.OMG.input:
                 if self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag: self.title,self.description,self.security = self.OMG.meta_df_lookup(file_path) 
                 self.OMG.generate_opex_properties(self.xmlroot,self.file_path,title=self.title,description=self.description,security=self.security)
                 if not self.OMG.metadata_flag in {'none','n'}:
                     self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
                     self.OMG.generate_descriptive_metadata(self.xml_descmeta,self.file_path)
             opex_path = self.OMG.write_opex(self.file_path,self.xmlroot)
```

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.1
+Version: 1.1.2
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.1/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.2/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.1/pyproject.toml` & `opex_manifest_generator-1.1.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 226f 7065 785f 6d61  .name = "opex_ma
 00000070: 6e69 6665 7374 5f67 656e 6572 6174 6f72  nifest_generator
 00000080: 220d 0a76 6572 7369 6f6e 203d 2022 312e  "..version = "1.
-00000090: 312e 3122 0d0a 6175 7468 6f72 7320 3d20  1.1"..authors = 
+00000090: 312e 3222 0d0a 6175 7468 6f72 7320 3d20  1.2"..authors = 
 000000a0: 5b0d 0a20 2020 207b 6e61 6d65 3d22 4368  [..    {name="Ch
 000000b0: 7269 7374 6f70 6865 7220 5072 696e 6365  ristopher Prince
 000000c0: 222c 2065 6d61 696c 3d22 632e 706a 2e70  ", email="c.pj.p
 000000d0: 7269 6e63 6540 676d 6169 6c2e 636f 6d22  rince@gmail.com"
 000000e0: 7d0d 0a20 2020 205d 0d0a 6465 7363 7269  }..    ]..descri
 000000f0: 7074 696f 6e20 3d20 224f 7065 7820 4d61  ption = "Opex Ma
 00000100: 6e69 6665 7374 2047 656e 6572 6174 6f72  nifest Generator
@@ -45,8 +45,10 @@
 000002c0: 4350 4a50 5249 4e43 452f 6f70 6578 5f6d  CPJPRINCE/opex_m
 000002d0: 616e 6966 6573 745f 6765 6e65 7261 746f  anifest_generato
 000002e0: 722f 6973 7375 6573 220d 0a5b 7072 6f6a  r/issues"..[proj
 000002f0: 6563 742e 7363 7269 7074 735d 0d0a 6f70  ect.scripts]..op
 00000300: 6578 5f67 656e 6572 6174 6520 3d20 226f  ex_generate = "o
 00000310: 7065 785f 6d61 6e69 6665 7374 5f67 656e  pex_manifest_gen
 00000320: 6572 6174 6f72 2e63 6c69 3a72 756e 5f63  erator.cli:run_c
-00000330: 6c69 22                                  li"
+00000330: 6c69 220d 0a0d 0a5b 746f 6f6c 2e68 6174  li"....[tool.hat
+00000340: 6368 2e62 756c 645d 0d0a 696e 636c 7564  ch.buld]..includ
+00000350: 6520 3d20 5b27 6d65 7461 6461 7461 275d  e = ['metadata']
```

