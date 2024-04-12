# Comparing `tmp/WangLab-0.0.18.tar.gz` & `tmp/WangLab-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WangLab-0.0.18.tar", last modified: Tue Mar 12 07:08:48 2024, max compression
+gzip compressed data, was "WangLab-0.1.1.tar", last modified: Fri Apr 12 12:59:33 2024, max compression
```

## Comparing `WangLab-0.0.18.tar` & `WangLab-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.718685 WangLab-0.0.18/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1066 2023-12-19 05:56:51.000000 WangLab-0.0.18/LICENSE
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8046 2024-03-12 07:08:48.718685 WangLab-0.0.18/PKG-INFO
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     6941 2024-03-11 11:22:27.000000 WangLab-0.0.18/README.md
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.714684 WangLab-0.0.18/WangLab/
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.714684 WangLab-0.0.18/WangLab/ChIP_seq/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1880 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/ChIP_seq/bowtie_ChIP_Seq.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1501 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1418 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/ChIP_seq/macs.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)       19 2024-03-12 07:08:46.000000 WangLab-0.0.18/WangLab/Constants.py
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.714684 WangLab-0.0.18/WangLab/RNA_seq/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     3284 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/RNA_seq/rna_seq.py
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.714684 WangLab-0.0.18/WangLab/Sequence_operate/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1901 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/calc_content.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     3540 2023-12-19 06:57:22.000000 WangLab-0.0.18/WangLab/Sequence_operate/extract_seqs.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     5745 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/file_merge.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1023 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/ossutil.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     9147 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/primer_blast.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     2803 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/primer_generator.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     4980 2023-12-19 06:00:03.000000 WangLab-0.0.18/WangLab/Sequence_operate/qPCR.py
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.718685 WangLab-0.0.18/WangLab/TIS/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     1342 2023-12-21 04:38:21.000000 WangLab-0.0.18/WangLab/TIS/bowtie.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)      909 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/TIS/combine_reads.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     6293 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/TIS/count_reads.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     2623 2023-12-19 04:36:25.000000 WangLab-0.0.18/WangLab/TIS/cutadapt.py
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)       76 2024-03-12 07:03:56.000000 WangLab-0.0.18/WangLab/__init__.py
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.718685 WangLab-0.0.18/WangLab.egg-info/
--rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8046 2024-03-12 07:08:48.000000 WangLab-0.0.18/WangLab.egg-info/PKG-INFO
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)      753 2024-03-12 07:08:48.000000 WangLab-0.0.18/WangLab.egg-info/SOURCES.txt
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)        1 2024-03-12 07:08:48.000000 WangLab-0.0.18/WangLab.egg-info/dependency_links.txt
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)       62 2024-03-12 07:08:48.000000 WangLab-0.0.18/WangLab.egg-info/requires.txt
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)        8 2024-03-12 07:08:48.000000 WangLab-0.0.18/WangLab.egg-info/top_level.txt
-drwxrwxr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-03-12 07:08:48.718685 WangLab-0.0.18/bin/
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)    19080 2024-03-12 07:08:43.000000 WangLab-0.0.18/bin/wanglab
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)       24 2024-03-12 06:50:33.000000 WangLab-0.0.18/bin/wanglab.bat
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)       38 2024-03-12 07:08:48.718685 WangLab-0.0.18/setup.cfg
--rw-rw-r--   0 byf1999   (1000) byf1999   (1000)     2397 2024-03-12 07:02:28.000000 WangLab-0.0.18/setup.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.940405 WangLab-0.1.1/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1066 2023-12-18 21:56:50.000000 WangLab-0.1.1/LICENSE
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8091 2024-04-12 12:59:33.938410 WangLab-0.1.1/PKG-INFO
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6948 2024-04-11 20:40:10.000000 WangLab-0.1.1/README.md
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.894386 WangLab-0.1.1/WangLab/
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.909405 WangLab-0.1.1/WangLab/ChIP_seq/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1880 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/bowtie_ChIP_Seq.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1501 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1418 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/ChIP_seq/macs.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       18 2024-04-12 12:54:03.000000 WangLab-0.1.1/WangLab/Constants.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.911398 WangLab-0.1.1/WangLab/RNA_seq/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3284 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/RNA_seq/rna_seq.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.925403 WangLab-0.1.1/WangLab/Sequence_operate/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2538 2024-04-12 11:49:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/calc_content.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3978 2024-04-12 12:32:13.000000 WangLab-0.1.1/WangLab/Sequence_operate/calc_usage_deviation.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     3540 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/extract_seqs.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     5745 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/file_merge.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1023 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/ossutil.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     9147 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/primer_blast.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2803 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/primer_generator.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     4980 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/Sequence_operate/qPCR.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.932403 WangLab-0.1.1/WangLab/TIS/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     1342 2024-04-11 20:40:14.000000 WangLab-0.1.1/WangLab/TIS/bowtie.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)      909 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/combine_reads.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     6293 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/count_reads.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2623 2024-04-11 20:40:12.000000 WangLab-0.1.1/WangLab/TIS/cutadapt.py
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       76 2024-04-11 20:40:14.000000 WangLab-0.1.1/WangLab/__init__.py
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.904396 WangLab-0.1.1/WangLab.egg-info/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     8091 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/PKG-INFO
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)      802 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/SOURCES.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)        1 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/dependency_links.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       68 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/requires.txt
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)        8 2024-04-12 12:59:33.000000 WangLab-0.1.1/WangLab.egg-info/top_level.txt
+drwxr-xr-x   0 byf1999   (1000) byf1999   (1000)        0 2024-04-12 12:59:33.936396 WangLab-0.1.1/bin/
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)    21801 2024-04-12 12:29:52.000000 WangLab-0.1.1/bin/wanglab
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       24 2024-04-11 20:40:10.000000 WangLab-0.1.1/bin/wanglab.bat
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)       38 2024-04-12 12:59:33.940405 WangLab-0.1.1/setup.cfg
+-rw-r--r--   0 byf1999   (1000) byf1999   (1000)     2479 2024-04-12 12:59:25.000000 WangLab-0.1.1/setup.py
```

### Comparing `WangLab-0.0.18/LICENSE` & `WangLab-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/PKG-INFO` & `WangLab-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: WangLab
-Version: 0.0.18
+Version: 0.1.1
 Summary: Simple bioinformatic tools
 Home-page: http://github.com/byf1999/WangLab/
 Author: Yifan Bu
 Author-email: y30210580@163.com
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argcomplete
 Requires-Dist: biopython
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: scipy
 Requires-Dist: selenium
 Requires-Dist: cutadapt
 Requires-Dist: openpyxl
 
 # WangLab
 Provide several simple bioinformatic scripts
 
@@ -39,17 +40,17 @@
 This project contains several simple bioinformatic and sequence operating scripts and will
 not update nor provide support when this student is graduated.
 
 The project contains 4 modules: [`Sequence_operate`](#Sequence_operate), [`TIS`](#TIS), [`ChIP_seq`](#ChIP_seq) and [`RNA_seq`](#RNA_seq). For detailed usage, users can refer to [**Usage**](#Usage). 
 
 ## Install
 
-The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./INSTALL.md) document for detail.
+The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./docs/INSTALL.md) document for detail.
 
-In general, you can install through PyPI as `pip install macs3`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
+In general, you can install through PyPI as `pip install WangLab`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
 
 ## Usage
 
 See [Sequence_operate](./docs/Sequence_operate.md), [ChIP_seq](./docs/ChIP_seq.md), [TIS](./docs/TIS.md), [RNA_seq](./docs/RNA_seq.md) in docs
 
 ## Example Usage
```

### Comparing `WangLab-0.0.18/README.md` & `WangLab-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 This project contains several simple bioinformatic and sequence operating scripts and will
 not update nor provide support when this student is graduated.
 
 The project contains 4 modules: [`Sequence_operate`](#Sequence_operate), [`TIS`](#TIS), [`ChIP_seq`](#ChIP_seq) and [`RNA_seq`](#RNA_seq). For detailed usage, users can refer to [**Usage**](#Usage). 
 
 ## Install
 
-The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./INSTALL.md) document for detail.
+The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./docs/INSTALL.md) document for detail.
 
-In general, you can install through PyPI as `pip install macs3`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
+In general, you can install through PyPI as `pip install WangLab`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
 
 ## Usage
 
 See [Sequence_operate](./docs/Sequence_operate.md), [ChIP_seq](./docs/ChIP_seq.md), [TIS](./docs/TIS.md), [RNA_seq](./docs/RNA_seq.md) in docs
 
 ## Example Usage
```

### Comparing `WangLab-0.0.18/WangLab/ChIP_seq/bowtie_ChIP_Seq.py` & `WangLab-0.1.1/WangLab/ChIP_seq/bowtie_ChIP_Seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py` & `WangLab-0.1.1/WangLab/ChIP_seq/cutadapt_ChIP_Seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/ChIP_seq/macs.py` & `WangLab-0.1.1/WangLab/ChIP_seq/macs.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/RNA_seq/rna_seq.py` & `WangLab-0.1.1/WangLab/RNA_seq/rna_seq.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/calc_content.py` & `WangLab-0.1.1/WangLab/Sequence_operate/calc_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,27 +35,41 @@
     n1_count = seq.count(n1)
     n2_count = seq.count(n2)
     content = (n1_count + n2_count) / len(seq)
     return content
 
 
 def calc_content(input_path, seq_path, n1='G', n2='C', fmt='t', output_path=None):
-    seq_list = read_file(input_path, fmt)
-    full_seq = None
-    for record in SeqIO.parse(seq_path, 'fasta'):
-        full_seq = record.seq.upper()
-    if not full_seq:
-        print('No sequence captured!')
-        return
-    if not output_path:
-        for name, start, end in seq_list:
-            print('\t'.join([name, start, end, f'{calc_single_content(full_seq[int(start) - 1:int(end)], n1, n2):.2f}']))
-    else:
-        with open(output_path, 'w') as fo:
+    if input_path:
+        print(input_path+'1 ')
+        seq_list = read_file(input_path, fmt)
+        full_seq = None
+        for record in SeqIO.parse(seq_path, 'fasta'):
+            full_seq = record.seq.upper()
+        if not full_seq:
+            print('No sequence captured!')
+            return
+        if not output_path:
             for name, start, end in seq_list:
-                fo.write('\t'.join(
-                    [name, start, end, f'{calc_single_content(full_seq[int(start) - 1:int(end)], n1, n2):.2f}']) + '\n')
+                print('\t'.join(
+                    [name, start, end, f'{calc_single_content(full_seq[int(start) - 1:int(end)], n1, n2):.2f}']))
+        else:
+            with open(output_path, 'w') as fo:
+                for name, start, end in seq_list:
+                    fo.write('\t'.join(
+                        [name, start, end,
+                         f'{calc_single_content(full_seq[int(start) - 1:int(end)], n1, n2):.2f}']) + '\n')
+    else:
+        if not output_path:
+            for record in SeqIO.parse(seq_path, 'fasta'):
+                print('\t'.join(
+                    [record.id, f'{calc_single_content(str(record.seq), n1, n2):.2f}']))
+        else:
+            with open(output_path, 'w') as fo:
+                for record in SeqIO.parse(seq_path, 'fasta'):
+                    fo.write('\t'.join(
+                        [record.id, f'{calc_single_content(str(record.seq), n1, n2):.2f}']) + '\n')
 
 
 if __name__ == '__main__':
     print(sys.argv, file=sys.stderr)
     calc_content(*sys.argv[1:])
```

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/extract_seqs.py` & `WangLab-0.1.1/WangLab/Sequence_operate/extract_seqs.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/file_merge.py` & `WangLab-0.1.1/WangLab/Sequence_operate/file_merge.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/ossutil.py` & `WangLab-0.1.1/WangLab/Sequence_operate/ossutil.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/primer_blast.py` & `WangLab-0.1.1/WangLab/Sequence_operate/primer_blast.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/primer_generator.py` & `WangLab-0.1.1/WangLab/Sequence_operate/primer_generator.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/Sequence_operate/qPCR.py` & `WangLab-0.1.1/WangLab/Sequence_operate/qPCR.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/TIS/bowtie.py` & `WangLab-0.1.1/WangLab/TIS/bowtie.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/TIS/combine_reads.py` & `WangLab-0.1.1/WangLab/TIS/combine_reads.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/TIS/count_reads.py` & `WangLab-0.1.1/WangLab/TIS/count_reads.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab/TIS/cutadapt.py` & `WangLab-0.1.1/WangLab/TIS/cutadapt.py`

 * *Files identical despite different names*

### Comparing `WangLab-0.0.18/WangLab.egg-info/PKG-INFO` & `WangLab-0.1.1/WangLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: WangLab
-Version: 0.0.18
+Version: 0.1.1
 Summary: Simple bioinformatic tools
 Home-page: http://github.com/byf1999/WangLab/
 Author: Yifan Bu
 Author-email: y30210580@163.com
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argcomplete
 Requires-Dist: biopython
 Requires-Dist: pandas
 Requires-Dist: numpy
+Requires-Dist: scipy
 Requires-Dist: selenium
 Requires-Dist: cutadapt
 Requires-Dist: openpyxl
 
 # WangLab
 Provide several simple bioinformatic scripts
 
@@ -39,17 +40,17 @@
 This project contains several simple bioinformatic and sequence operating scripts and will
 not update nor provide support when this student is graduated.
 
 The project contains 4 modules: [`Sequence_operate`](#Sequence_operate), [`TIS`](#TIS), [`ChIP_seq`](#ChIP_seq) and [`RNA_seq`](#RNA_seq). For detailed usage, users can refer to [**Usage**](#Usage). 
 
 ## Install
 
-The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./INSTALL.md) document for detail.
+The easiest way to install WangLab in through PyPI. Please check the [INSTALL](./docs/INSTALL.md) document for detail.
 
-In general, you can install through PyPI as `pip install macs3`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
+In general, you can install through PyPI as `pip install WangLab`. To use virtual environment is highly recommended. Or you can install after unzipping the released package downloaded from Github, then place scripts into corresponding folders of specific python environment.
 
 ## Usage
 
 See [Sequence_operate](./docs/Sequence_operate.md), [ChIP_seq](./docs/ChIP_seq.md), [TIS](./docs/TIS.md), [RNA_seq](./docs/RNA_seq.md) in docs
 
 ## Example Usage
```

### Comparing `WangLab-0.0.18/WangLab.egg-info/SOURCES.txt` & `WangLab-0.1.1/WangLab.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 WangLab.egg-info/requires.txt
 WangLab.egg-info/top_level.txt
 WangLab/ChIP_seq/bowtie_ChIP_Seq.py
 WangLab/ChIP_seq/cutadapt_ChIP_Seq.py
 WangLab/ChIP_seq/macs.py
 WangLab/RNA_seq/rna_seq.py
 WangLab/Sequence_operate/calc_content.py
+WangLab/Sequence_operate/calc_usage_deviation.py
 WangLab/Sequence_operate/extract_seqs.py
 WangLab/Sequence_operate/file_merge.py
 WangLab/Sequence_operate/ossutil.py
 WangLab/Sequence_operate/primer_blast.py
 WangLab/Sequence_operate/primer_generator.py
 WangLab/Sequence_operate/qPCR.py
 WangLab/TIS/bowtie.py
```

### Comparing `WangLab-0.0.18/bin/wanglab` & `WangLab-0.1.1/bin/wanglab`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import argparse as ap
 import argcomplete
 import sys
 import os
 
 from WangLab.Constants import *
 
+
 def main():
     argparser = prepare_argparser()
     argcomplete.autocomplete(argparser)  # Accomplish the autocomplete function in terminal
     args = argparser.parse_args()
 
     subcommand = args.subcommand
     if subcommand == 'primer_generator':
@@ -69,14 +70,17 @@
         from WangLab.Sequence_operate.primer_blast import primer_blast
         primer_blast(args)
 
     elif subcommand == 'qPCR':
         from WangLab.Sequence_operate.qPCR import calc
         calc(args)
 
+    elif subcommand == 'calc_usage_deviation':
+        from WangLab.Sequence_operate.calc_usage_deviation import main
+        main(args)
     else:
         print(f'Command {subcommand} not recognized!')
         return
 
 
 def prepare_argparser():
     description = f"WangLab main executable. Version: {VERSION}"
@@ -122,14 +126,16 @@
 
     # coommand for 'primer-blast'
     add_primer_blast(subparsers)
 
     # command for 'qPCR'
     add_qPCR(subparsers)
 
+    # command for 'calc_usage_deviation'
+    add_calc_usage_devitation(subparsers)
     return argparser
 
 
 def add_qPCR(subparsers):
     """Add function 'qPCR' argument parsers"""
     name = 'qPCR'
 
@@ -290,16 +296,16 @@
         epilog=f"""Examples:
     $ {os.path.basename(sys.argv[0])} {name} -i input.txt -r eib202.fa -n G C -f t
     $ {os.path.basename(sys.argv[0])} {name} -i input.txt -r eib202.fa -n A T -f , -o output.txt 
     
 The input file should contain 3 columns, each represent the name, start position and 
 end position of regions. The format of input file is specified by -f argument, default is 
 tab-separated.""")
-    argparse_macs.add_argument("-i", '--input', dest='input_path', type=str, required=True, nargs="?",
-                               help='Input file')
+    argparse_macs.add_argument("-i", '--input', dest='input_path', type=str, required=False, nargs="?",
+                               help='Input file', default=None)
     argparse_macs.add_argument("-r", '--reference', dest='ref', type=str, required=True, nargs="?",
                                help='Reference sequence file')
     argparse_macs.add_argument("-n", '--nucl', dest='nucl', type=str, required=False, nargs="+",
                                help='Nucleotides that are counted, default G C', default='GC')
     argparse_macs.add_argument("-f", '--fmt', dest='fmt', type=str, required=False, nargs="?",
                                help='Input file format, default is separated by tab', default='t')
     argparse_macs.add_argument("-o", '--output', dest='output_path', type=str, required=False, nargs="?",
@@ -365,25 +371,58 @@
                               help='Whether to transform sequences, default is No, supported transformation include: '
                                    f'{list(__FLAG_DICT__.keys())}', default=None)
 
 
 def add_rna_seq(subparsers):
     """Add function 'rna_seq' argument parsers"""
     name = 'rna_seq'
-    
+
     from WangLab.RNA_seq.rna_seq import prepare_argparser
     argparser_rna_seq = subparsers.add_parser(name, help='Analysis of RNA-Seq data',
                                               formatter_class=ap.RawDescriptionHelpFormatter, epilog=f"""Examples:
     $ {os.path.basename(sys.argv[0])} {name} -d . -i eib202.fa -p 4
     $ {os.path.basename(sys.argv[0])} {name} -d . -i eib202.fa -p 4 --remove_tmp False
 """)
     prepare_argparser(argparser_rna_seq)
     return
 
 
+def add_calc_usage_devitation(subparsers):
+    """Add function 'calc_usage_deviation' argument parsers"""
+    name = 'calc_usage_deviation'
+
+    # from WangLab.Sequence_operate.calc_usage_deviation import prepare_argparser
+    help_content = 'Calculate the genomic nuleotide usage deviation and person rho of peaks in ChIP-Seq callpeak results'
+    argparser_calc_usage_deviation = subparsers.add_parser(name,
+                                                           help=help_content,
+                                                           formatter_class=ap.RawDescriptionHelpFormatter, epilog=f"""Examples:
+    $ {os.path.basename(sys.argv[0])} {name} -i peak.xlsx -r genome.fa
+    $ {os.path.basename(sys.argv[0])} {name} -i peak.xlsx -r genome.fa -o output_300.xlsx -n 3 -l 300
+""")
+
+    argparser_calc_usage_deviation.add_argument("-i", '--input', dest='input_path', type=str, required=True, nargs="?",
+                                                help='Peak file path')
+    argparser_calc_usage_deviation.add_argument("-r", '--reference', dest='ref', type=str, required=True, nargs="?",
+                                                help='Reference sequence file')
+    argparser_calc_usage_deviation.add_argument("-o", '--output', dest='out', type=str, required=False,
+                                                nargs="?",
+                                                help='Output file path', default=None)
+    argparser_calc_usage_deviation.add_argument("-p", '--p-model', dest='p_model', type=str, required=False, nargs="?",
+                                                help='Model used for calculating usage deviation of peaks',
+                                                default='no-scale')
+    argparser_calc_usage_deviation.add_argument("-g", '--g-model', dest='g_model', type=str, required=False, nargs="?",
+                                                help='Model used for calculating genomic usage deviation',
+                                                default='zero-order')
+    argparser_calc_usage_deviation.add_argument("-n", '--n-max', dest='n', type=str, required=False, nargs="?",
+                                                help='Maximum number of successive  nucleotides', default='3')
+    argparser_calc_usage_deviation.add_argument("-l", '--length', dest='length', type=str, required=False, nargs="?",
+                                                help='Length of peaks selected from summits', default='200')
+    return
+
+
 def run_cutadapt(args):
     if args.data_type.upper() == 'TN-SEQ':
         if not args.plasmid:
             print(f'Please enter transposon plasmid name.')
             return
         from WangLab.TIS.cutadapt import main
         main([args.subcommand, args.dir], args.plasmid.upper())
```

### Comparing `WangLab-0.0.18/setup.py` & `WangLab-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,38 +18,42 @@
 
 # get version
 exec(open("WangLab/Constants.py").read())
 
 # classifiers
 classifiers = [ \
     'Development Status :: 5 - Production/Stable',
-    'Environment :: Console',
+    # 'Environment :: Terminal',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'License :: OSI Approved :: MIT License',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: POSIX',
     'Operating System :: Unix',
+    'Operating System :: Microsoft :: Windows',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
     'Programming Language :: Cython', ]
 
 install_requires = ["argcomplete",
                     "biopython",
                     "pandas",
                     "numpy",
+                    "scipy",
                     "selenium",
                     "cutadapt",
                     "openpyxl",
                     ]
 tests_requires = ['pytest']
 scripts = ['bin/wanglab', 'bin/wanglab.bat']
+
+
 def main():
     if sys.version_info < (3, 9):
         sys.stderr.write("CRITICAL: Python version must >= 3.9!\n")
         sys.exit(1)
 
     # NumPy include dir
     numpy_include_dir = [numpy.get_include()]
```

