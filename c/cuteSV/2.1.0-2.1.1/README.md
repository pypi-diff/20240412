# Comparing `tmp/cuteSV-2.1.0.tar.gz` & `tmp/cuteSV-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuteSV-2.1.0.tar", last modified: Fri Nov 17 08:18:49 2023, max compression
+gzip compressed data, was "cuteSV-2.1.1.tar", last modified: Thu Apr 11 12:32:19 2024, max compression
```

## Comparing `cuteSV-2.1.0.tar` & `cuteSV-2.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-11-17 08:18:49.000000 cuteSV-2.1.0/
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     1065 2023-05-17 06:33:50.000000 cuteSV-2.1.0/LICENSE
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    15122 2023-11-17 08:18:49.000000 cuteSV-2.1.0/PKG-INFO
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    14797 2023-11-12 04:40:53.000000 cuteSV-2.1.0/README.md
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       38 2023-11-17 08:18:49.000000 cuteSV-2.1.0/setup.cfg
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)      794 2023-11-17 08:07:57.000000 cuteSV-2.1.0/setup.py
-drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-11-17 08:18:49.000000 cuteSV-2.1.0/src/
-drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-11-17 08:18:49.000000 cuteSV-2.1.0/src/benchmarks/
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-05-17 06:33:35.000000 cuteSV-2.1.0/src/benchmarks/__init__.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     8612 2023-05-17 06:33:34.000000 cuteSV-2.1.0/src/benchmarks/cmp_NA19240.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     4349 2023-05-17 06:33:38.000000 cuteSV-2.1.0/src/benchmarks/eval_BND.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     6507 2023-11-17 08:07:51.000000 cuteSV-2.1.0/src/benchmarks/eval_forcecalling.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    13868 2023-05-17 06:33:35.000000 cuteSV-2.1.0/src/benchmarks/eval_sim.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5834 2023-05-17 06:33:37.000000 cuteSV-2.1.0/src/benchmarks/eval_trio.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5587 2023-05-17 06:33:39.000000 cuteSV-2.1.0/src/benchmarks/multi_platform.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     6919 2023-05-17 06:33:37.000000 cuteSV-2.1.0/src/benchmarks/sta_venn.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     2511 2023-05-17 06:33:38.000000 cuteSV-2.1.0/src/benchmarks/vcf2bedpe.py
-drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-11-17 08:18:49.000000 cuteSV-2.1.0/src/cuteSV/
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5159 2023-05-17 06:33:41.000000 cuteSV-2.1.0/src/cuteSV/CommandRunner.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-05-17 06:33:41.000000 cuteSV-2.1.0/src/cuteSV/__init__.py
--rwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)    54307 2023-11-12 04:40:53.000000 cuteSV-2.1.0/src/cuteSV/cuteSV
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    12219 2023-11-12 04:40:53.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_Description.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    32361 2023-11-12 04:40:54.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_forcecalling.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    26441 2023-11-12 04:40:54.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_genotype.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     8116 2023-11-12 04:40:55.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_resolveDUP.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    20358 2023-11-12 04:40:55.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_resolveINDEL.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    11767 2023-11-12 04:40:55.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_resolveINV.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     9397 2023-11-12 04:40:55.000000 cuteSV-2.1.0/src/cuteSV/cuteSV_resolveTRA.py
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     2991 2023-05-17 06:33:44.000000 cuteSV-2.1.0/src/cuteSV/diploid_calling.py
-drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-11-17 08:18:49.000000 cuteSV-2.1.0/src/cuteSV.egg-info/
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    15122 2023-11-17 08:18:48.000000 cuteSV-2.1.0/src/cuteSV.egg-info/PKG-INFO
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)      817 2023-11-17 08:18:48.000000 cuteSV-2.1.0/src/cuteSV.egg-info/SOURCES.txt
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        1 2023-11-17 08:18:48.000000 cuteSV-2.1.0/src/cuteSV.egg-info/dependency_links.txt
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        1 2023-05-17 06:33:45.000000 cuteSV-2.1.0/src/cuteSV.egg-info/not-zip-safe
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       60 2023-11-17 08:18:48.000000 cuteSV-2.1.0/src/cuteSV.egg-info/requires.txt
--rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       18 2023-11-17 08:18:48.000000 cuteSV-2.1.0/src/cuteSV.egg-info/top_level.txt
+drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2024-04-11 12:32:19.000000 cuteSV-2.1.1/
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     1065 2023-05-17 06:33:50.000000 cuteSV-2.1.1/LICENSE
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    15326 2024-04-11 12:32:19.000000 cuteSV-2.1.1/PKG-INFO
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    15001 2024-04-10 12:58:20.000000 cuteSV-2.1.1/README.md
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       38 2024-04-11 12:32:19.000000 cuteSV-2.1.1/setup.cfg
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)      785 2024-04-04 09:20:20.000000 cuteSV-2.1.1/setup.py
+drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2024-04-11 12:32:18.000000 cuteSV-2.1.1/src/
+drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2024-04-11 12:32:18.000000 cuteSV-2.1.1/src/benchmarks/
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-05-17 06:33:35.000000 cuteSV-2.1.1/src/benchmarks/__init__.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     8612 2023-05-17 06:33:34.000000 cuteSV-2.1.1/src/benchmarks/cmp_NA19240.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     4349 2023-05-17 06:33:38.000000 cuteSV-2.1.1/src/benchmarks/eval_BND.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     6507 2023-11-17 08:07:51.000000 cuteSV-2.1.1/src/benchmarks/eval_forcecalling.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    13868 2023-05-17 06:33:35.000000 cuteSV-2.1.1/src/benchmarks/eval_sim.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5834 2023-05-17 06:33:37.000000 cuteSV-2.1.1/src/benchmarks/eval_trio.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5587 2023-05-17 06:33:39.000000 cuteSV-2.1.1/src/benchmarks/multi_platform.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     6919 2023-05-17 06:33:37.000000 cuteSV-2.1.1/src/benchmarks/sta_venn.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     2511 2023-05-17 06:33:38.000000 cuteSV-2.1.1/src/benchmarks/vcf2bedpe.py
+drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2024-04-11 12:32:19.000000 cuteSV-2.1.1/src/cuteSV/
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     5159 2023-05-17 06:33:41.000000 cuteSV-2.1.1/src/cuteSV/CommandRunner.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        0 2023-05-17 06:33:41.000000 cuteSV-2.1.1/src/cuteSV/__init__.py
+-rwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)    54363 2024-04-04 09:20:09.000000 cuteSV-2.1.1/src/cuteSV/cuteSV
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    12218 2024-04-04 09:19:40.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_Description.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    32433 2024-03-31 09:36:46.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_forcecalling.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    26653 2024-03-31 09:36:46.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_genotype.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     8116 2023-11-12 04:40:55.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_resolveDUP.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    20358 2023-11-12 04:40:55.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_resolveINDEL.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    11767 2023-11-12 04:40:55.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_resolveINV.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     9397 2023-11-12 04:40:55.000000 cuteSV-2.1.1/src/cuteSV/cuteSV_resolveTRA.py
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)     2991 2023-05-17 06:33:44.000000 cuteSV-2.1.1/src/cuteSV/diploid_calling.py
+drwxrwxr-x   0 caoshuqi  (1099) caoshuqi  (1100)        0 2024-04-11 12:32:19.000000 cuteSV-2.1.1/src/cuteSV.egg-info/
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)    15326 2024-04-11 12:32:16.000000 cuteSV-2.1.1/src/cuteSV.egg-info/PKG-INFO
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)      817 2024-04-11 12:32:17.000000 cuteSV-2.1.1/src/cuteSV.egg-info/SOURCES.txt
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        1 2024-04-11 12:32:16.000000 cuteSV-2.1.1/src/cuteSV.egg-info/dependency_links.txt
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)        1 2023-05-17 06:33:45.000000 cuteSV-2.1.1/src/cuteSV.egg-info/not-zip-safe
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       54 2024-04-11 12:32:16.000000 cuteSV-2.1.1/src/cuteSV.egg-info/requires.txt
+-rw-rw-r--   0 caoshuqi  (1099) caoshuqi  (1100)       18 2024-04-11 12:32:16.000000 cuteSV-2.1.1/src/cuteSV.egg-info/top_level.txt
```

### Comparing `cuteSV-2.1.0/LICENSE` & `cuteSV-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/PKG-INFO` & `cuteSV-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuteSV
-Version: 2.1.0
+Version: 2.1.1
 Summary: Long-read-based human genomic structural variation detection with cuteSV
 Home-page: https://github.com/tjiangHIT/cuteSV
 Author: Jiang Tao
 Author-email: tjiang@hit.edu.cn
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -58,19 +58,21 @@
 
 We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
 
 ---
 ### Dependence
 	
 	1. python3
+ 	2. scipy
 	2. pysam
 	3. Biopython
 	4. cigar
 	5. numpy
-	6. pyvcf
+	6. pyvcf3
+ 	7. scikit-learn
 
 ---
 ### Usage
 	cuteSV <sorted.bam> <reference.fa> <output.vcf> <work_dir>
 	
 *Suggestions*
 
@@ -132,15 +134,20 @@
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
 
 Please cite the manuscript of cuteSV before using these callsets.
 
 ---
 ### Changelog
-	cuteSV (v2.1.0)
+	cuteSV (v2.1.1)
+	1. fix bugs in resolving reference genomes
+ 	2. modify several dependencies and remove some useless dependencies
+  	3. update several evaluation scripts
+ 
+ 	cuteSV (v2.1.0)
  	1. Speed up both SV discovery calling and force calling comprehensively.
   	2. Upgrade the force calling module.
    	3. Modify the temporary files. The sigs file are only generated with the "write_old_sigs" parameter.
 	4. Update several regulations in signature extraction.
  
  	cuteSV (v2.0.3):
 	1. Fix the error of missing min_size parameter.
```

### Comparing `cuteSV-2.1.0/README.md` & `cuteSV-2.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,21 @@
 
 We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
 
 ---
 ### Dependence
 	
 	1. python3
+ 	2. scipy
 	2. pysam
 	3. Biopython
 	4. cigar
 	5. numpy
-	6. pyvcf
+	6. pyvcf3
+ 	7. scikit-learn
 
 ---
 ### Usage
 	cuteSV <sorted.bam> <reference.fa> <output.vcf> <work_dir>
 	
 *Suggestions*
 
@@ -120,15 +122,20 @@
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
 
 Please cite the manuscript of cuteSV before using these callsets.
 
 ---
 ### Changelog
-	cuteSV (v2.1.0)
+	cuteSV (v2.1.1)
+	1. fix bugs in resolving reference genomes
+ 	2. modify several dependencies and remove some useless dependencies
+  	3. update several evaluation scripts
+ 
+ 	cuteSV (v2.1.0)
  	1. Speed up both SV discovery calling and force calling comprehensively.
   	2. Upgrade the force calling module.
    	3. Modify the temporary files. The sigs file are only generated with the "write_old_sigs" parameter.
 	4. Update several regulations in signature extraction.
  
  	cuteSV (v2.0.3):
 	1. Fix the error of missing min_size parameter.
```

### Comparing `cuteSV-2.1.0/setup.py` & `cuteSV-2.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name = "cuteSV",
-    version = "2.1.0",
+    version = "2.1.1",
     description = "Long-read-based human genomic structural variation detection with cuteSV",
     author = "Jiang Tao",
     author_email = "tjiang@hit.edu.cn",
     url = "https://github.com/tjiangHIT/cuteSV",
     license = "MIT",
     packages = find_packages("src"),
     package_dir = {"": "src"},
     data_files = [("", ["LICENSE"])],
     scripts=['src/cuteSV/cuteSV'],
     # long_description = LONG_DESCRIPTION,
     long_description = readme,
     long_description_content_type = 'text/markdown',
     zip_safe = False,
-    install_requires = ['scipy', 'Cython', 'pysam', 'Biopython', 'Cigar', 'numpy', 'pyvcf', 'scikit-learn']
+    install_requires = ['scipy', 'pysam', 'Biopython', 'Cigar', 'numpy', 'pyvcf3', 'scikit-learn']
 )
```

### Comparing `cuteSV-2.1.0/src/benchmarks/cmp_NA19240.py` & `cuteSV-2.1.1/src/benchmarks/cmp_NA19240.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/eval_BND.py` & `cuteSV-2.1.1/src/benchmarks/eval_BND.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/eval_forcecalling.py` & `cuteSV-2.1.1/src/benchmarks/eval_forcecalling.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/eval_sim.py` & `cuteSV-2.1.1/src/benchmarks/eval_sim.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/eval_trio.py` & `cuteSV-2.1.1/src/benchmarks/eval_trio.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/multi_platform.py` & `cuteSV-2.1.1/src/benchmarks/multi_platform.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/sta_venn.py` & `cuteSV-2.1.1/src/benchmarks/sta_venn.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/benchmarks/vcf2bedpe.py` & `cuteSV-2.1.1/src/benchmarks/vcf2bedpe.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/CommandRunner.py` & `cuteSV-2.1.1/src/cuteSV/CommandRunner.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV` & `cuteSV-2.1.1/src/cuteSV/cuteSV`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 ''' 
  * All rights Reserved, Designed By HIT-Bioinformatics   
  * @Title: cuteSV 
  * @author: tjiang & sqcao & zdzhang
- * @date: Nov. 29th 2023
- * @version V2.1.0
+ * @date: Apr. 4th 2024
+ * @version V2.1.1
 '''
 
 import pysam
 import cigar
 from cuteSV.cuteSV_Description import parseArgs
 from multiprocessing import Pool,Manager,Queue, current_process
 from cuteSV.CommandRunner import *
@@ -189,14 +189,17 @@
 
 def analysis_split_read(split_read, SV_size, RLength, read_name, candidate, MaxSize, query):
     '''
     read_start	read_end	ref_start	ref_end	chr	strand
     #0			#1			#2			#3		#4	#5
     '''
     SP_list = sorted(split_read, key = lambda x:x[0])
+    # print(read_name)
+    # for i in SP_list:
+    #     print(i)
 
     # detect INS involoved in a translocation
     trigger_INS_TRA = 0	
 
     # Store Strands of INV
 
     if len(SP_list) == 2:
@@ -1017,16 +1020,16 @@
             task_round = int(local_ref_len/batch_size)
             for j in range(task_round):
                 Task_list.append([i[0], pos, pos+batch_size])
                 pos += batch_size
             if pos < local_ref_len:
                 Task_list.append([i[0], pos, local_ref_len])
     bed_regions = load_bed(args.include_bed, Task_list)
-    #'''
     
+    #'''
     candidates={}
     candidates["DEL"]=list()
     candidates["INS"]=list()
     candidates["DUP"]=list()
     candidates["INV"]=list()
     candidates["TRA"]=list()
     reads_info_list=list()
@@ -1049,17 +1052,16 @@
                     args.merge_ins_threshold, 
                     args.max_size,
                     None if bed_regions == None else bed_regions[i])]
         analysis_pools.map_async(multi_run_wrapper, paras)
     pids = [process.pid for process in analysis_pools._pool]
     analysis_pools.close()
     analysis_pools.join()
-    #'''
     logging.info("Rebuilding signatures of structural variants.")
-
+    #'''
     analysis_pools = Pool(processes=int(args.threads))
     paras=[]
     for sv_type in SVTYPES:
         paras.append((sv_type,temporary_dir,pids,args.write_old_sigs))
     paras.append(("reads",temporary_dir,pids,args.write_old_sigs))
     results=analysis_pools.map_async(process_process_sigs_type, paras)
     analysis_pools.close()
@@ -1073,15 +1075,15 @@
     with open("%s/sigindex.pickle"%temporary_dir,"wb") as f:
         pickle.dump(sigs_index,f)
     del reads_info_list
     del results
     del candidates
     gc.collect()
     logging.info("Rebuilding signatures completed.")
-    #'''
+
     result = list()
 
     if args.Ivcf != None:
         # force calling
         max_cluster_bias_dict = dict()
         max_cluster_bias_dict['INS'] = args.max_cluster_bias_INS
         max_cluster_bias_dict['DEL'] = args.max_cluster_bias_DEL
```

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_Description.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_Description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ''' 
  * All rights Reserved, Designed By HIT-Bioinformatics   
  * @Title:  cuteSV_Description.py
  * @author: tjiang & sqcao & zdzhang
- * @date: Nov. 29th 2023
- * @version V2.1.0
+ * @date: Apr. 4th 2024
+ * @version V2.1.1
 '''
 import argparse
 
-VERSION = '2.1.0'
+VERSION = '2.1.1'
 
 class cuteSVdp(object):
 	'''
 	Detailed descriptions of cuteSV version and its parameters.
 	'''
 
 	USAGE="""\
```

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_forcecalling.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_forcecalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -572,16 +572,19 @@
 
 def solve_fc_wrapper(args):
     return solve_fc(*args)
 def solve_fc(chrom_list, svs_dict, temporary_dir, max_cluster_bias_dict, threshold_gloab_dict, gt_round, sigs_index, read_range, svs_multi):
     reads_info = dict() # [10000, 10468, 0, 'm54238_180901_011437/52298335/ccs']
     readsfile = open("%sreads.pickle"%(temporary_dir), 'rb')
     for chrom in chrom_list:
-        readsfile.seek(sigs_index["reads"][chrom])
-        reads_info[chrom]=pickle.load(readsfile)
+        try:
+            readsfile.seek(sigs_index["reads"][chrom])
+            reads_info[chrom]=pickle.load(readsfile)
+        except:
+            reads_info[chrom] = []
     readsfile.close()
     sv_dict = dict()
     for sv_type in ["DEL", "DUP", "INS", "INV", "TRA"]:
         sv_dict[sv_type] = parse_sigs_chrom(sv_type, temporary_dir, chrom_list, sigs_index)
     
     gt_list = {}
     for chrom in svs_dict:
```

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_genotype.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_genotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,22 +242,25 @@
     '''
     Generation of VCF format file.
     VCF version: 4.2
     '''
 
     # genotype_trigger = TriggerGT[args.genotype]
 
+    f=open("%sresults/%s.pickle"%(temporary_dir,chrom), "wb")
     semi_result.sort(key = lambda x:int(x[2]))
     action = args.genotype
     fa_file = pysam.FastaFile(reference)
-    ref_chrom=fa_file.fetch(chrom)
+    try:
+        ref_chrom=fa_file.fetch(chrom)
+    except:
+        raise Exception("No corresponding contig in reference with %s."%(chrom))
     fa_file.close()
     lines=[]
     BATCH_SIZE=1000
-    f=open("%sresults/%s.pickle"%(temporary_dir,chrom), "wb")
     for i in semi_result:
         if i[1] in ["DEL", "INS"]:
             if abs(int(float(i[3]))) > args.max_size and args.max_size != -1:
                 continue
             if abs(int(float(i[3]))) < args.min_size:
                 continue
             if i[1] == "INS":
@@ -418,15 +421,18 @@
     # f.close()
     # return lines
 
 
 # def generate_pvcf(args, result, contigINFO, argv, ref_g):
 def generate_pvcf(args, result, reference, chrom):
     fa_file = pysam.FastaFile(reference)
-    ref_chrom=fa_file.fetch(chrom)
+    try:
+        ref_chrom=fa_file.fetch(chrom)
+    except:
+        raise Exception("No corresponding contig in reference with %s."%(chrom))
     fa_file.close()
     # file = open(args.output, 'w')
     # Generation_VCF_header(file, contigINFO, args.sample, argv)
     # file.write("#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\t%s\n"%(args.sample))
     # [chrom(0), sv_start, genotype(2), sv_type, sv_end(4), CIPOS, CILEN(6), [gt_re, DR, GT(new), GL, GQ, QUAL], rname(8), svid, ref(10), alts, sv_strand(12), seq]
     lines=[]
     for i in result:
```

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_resolveDUP.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_resolveDUP.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_resolveINDEL.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_resolveINDEL.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_resolveINV.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_resolveINV.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/cuteSV_resolveTRA.py` & `cuteSV-2.1.1/src/cuteSV/cuteSV_resolveTRA.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV/diploid_calling.py` & `cuteSV-2.1.1/src/cuteSV/diploid_calling.py`

 * *Files identical despite different names*

### Comparing `cuteSV-2.1.0/src/cuteSV.egg-info/PKG-INFO` & `cuteSV-2.1.1/src/cuteSV.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuteSV
-Version: 2.1.0
+Version: 2.1.1
 Summary: Long-read-based human genomic structural variation detection with cuteSV
 Home-page: https://github.com/tjiangHIT/cuteSV
 Author: Jiang Tao
 Author-email: tjiang@hit.edu.cn
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -58,19 +58,21 @@
 
 We provided a new document for applying **force calling** (or **regenotyping**) benchmark [here](https://github.com/tjiangHIT/cuteSV/tree/master/src/documentation).
 
 ---
 ### Dependence
 	
 	1. python3
+ 	2. scipy
 	2. pysam
 	3. Biopython
 	4. cigar
 	5. numpy
-	6. pyvcf
+	6. pyvcf3
+ 	7. scikit-learn
 
 ---
 ### Usage
 	cuteSV <sorted.bam> <reference.fa> <output.vcf> <work_dir>
 	
 *Suggestions*
 
@@ -132,15 +134,20 @@
 You can download them at: 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3783083.svg)](https://doi.org/10.5281/zenodo.3783083)
 
 Please cite the manuscript of cuteSV before using these callsets.
 
 ---
 ### Changelog
-	cuteSV (v2.1.0)
+	cuteSV (v2.1.1)
+	1. fix bugs in resolving reference genomes
+ 	2. modify several dependencies and remove some useless dependencies
+  	3. update several evaluation scripts
+ 
+ 	cuteSV (v2.1.0)
  	1. Speed up both SV discovery calling and force calling comprehensively.
   	2. Upgrade the force calling module.
    	3. Modify the temporary files. The sigs file are only generated with the "write_old_sigs" parameter.
 	4. Update several regulations in signature extraction.
  
  	cuteSV (v2.0.3):
 	1. Fix the error of missing min_size parameter.
```

### Comparing `cuteSV-2.1.0/src/cuteSV.egg-info/SOURCES.txt` & `cuteSV-2.1.1/src/cuteSV.egg-info/SOURCES.txt`

 * *Files identical despite different names*

